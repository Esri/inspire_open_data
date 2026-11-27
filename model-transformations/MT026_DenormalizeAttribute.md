# MT026: Denormalize Attribute From Related Feature

## Category

Relationships / denormalization

## Description

Some published field lists carry an attribute that, in the INSPIRE model, lives on
a **related** feature but is **denormalized** onto the feature it describes — so a
single record is self-contained and gives a usable map result without a join at
read time.

The archetype is **`mappingFrame`**: in INSPIRE Geology it is a property of
`MappedFeature`, not of the described `GeologicFeature` (`GeologicUnit` /
`ShearDisplacementStructure`). The published field lists fold it onto the described
feature (`MappedFeature.mappingFrame` via the `MappedFeature.specification`
association). A per-feature-type source does not carry that reverse join, so
the attribute is otherwise absent.

This rule **injects the declared attribute** onto the target feature type (appended
after its real properties). It is a *schema-level* denormalization: the field is
declared here; populating its value from the related feature is a data-preparation
(service / ingest) concern, out of scope for the encoding rule.

## Original instance (example, default encoding)

`GeologicUnit` has no `mappingFrame` of its own — it is on the `MappedFeature` that
points at the unit:

```xml
<ge:MappedFeature>
  <ge:mappingFrame xlink:href="…/MappingFrameValue/surfaceGeology"/>
  <ge:specification xlink:href="#GeologicUnit_42"/>
</ge:MappedFeature>
```

Default encoding of `GeologicUnit`: no `mappingFrame` field.

## Transformed instance (example)

`GeologicUnit` gains the denormalized codelist attribute (value + `_href`):

```xml
<ges:GeologicUnit>
  <!-- ... -->
  <ges:mappingFrame>surfaceGeology</ges:mappingFrame>
  <ges:mappingFrame_href>http://.../MappingFrameValue/surfaceGeology</ges:mappingFrame_href>
</ges:GeologicUnit>
```

## Model transformation rule

**Parameters:**

- `attributes`: the attributes to inject — each `{ name, codelist? }` (`codelist`
  default true → value + `_href`; else a plain Text value).
- `from` (provenance): the related feature type the attribute is denormalized from.
- `via` (provenance): the association used for the join.

For each target feature type, append the declared attribute(s) after the real
properties.

## Instance transformation rule

Resolve the join (`<target>` ← `<from>.<via>`) and copy the related feature's
attribute value into the injected field. (Performed during data preparation, not by
the schema-level encoding.)

## Solves usability issues

- Produces a self-contained, map-ready record: the map-relevant attribute of the
  related feature is available directly, without a runtime join.

## Known usability issues

- Purely additive at schema level; the actual value join is a data-preparation
  concern and not verified by the encoding.
- 1:n relations (several related features per target) need a data-prep policy
  (e.g. first / representative); not expressed by the rule.

## INSPIRE compliance

Compliant in spirit: no information is invented — the attribute exists in the model
on the related feature and is surfaced on the feature it characterises. It is a
denormalization, not a new semantic.

## Notes

- Implementation: applied before MT001.
- Used by: GeologyCore (`mappingFrame` on `GeologicUnit` / `ShearDisplacementStructure`,
  denormalized from `MappedFeature` via `specification`).
- Not part of the original INSPIRE MIF 2017.2 catalogue; added to make the
  per-theme Geodatabase encoding rules executable.
