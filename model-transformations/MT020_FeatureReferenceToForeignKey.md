# MT020: Feature Reference To Foreign Key

## Category

Relationships

## Description

A feature association is an `xlink:href` reference from one feature to another
(e.g. `RoadLink.startNode → RoadNode`). The **base rule keeps association roles as
they are**: the default encoding emits a single Text field holding the reference
itself (the `xlink:href` URI / URN) — verbatim, lossless, and correct for external
or URN references.

For a **resolvable intra-dataset** reference, a raw URI is awkward to use in a
Geodatabase; a numeric key that joins to the target feature class is far more
usable. This rule marks such a reference to be encoded instead as a **Long
`featureId` foreign key** — the `featureId` of the referenced feature.

**Reference-style choice (href vs. Long FK):** it is decided **per reference**, by
whether the reference is listed in this rule:

- **not listed → Text** (the `xlink:href`, base-rule default) — right for external /
  URN / not-locally-resolvable references;
- **listed in MT020 → Long FK** (`featureId`) — right for resolvable intra-dataset
  references that should join within the dataset.

There is no dataset-wide toggle; the two styles coexist, chosen reference by
reference.

## Original instance (example, default encoding)

```xml
<tn-ro:RoadLink>
  <tn:startNode xlink:href="#RoadNode_17"/>
</tn-ro:RoadLink>
```

Default encoding: `startNode` (Text) = `"#RoadNode_17"`.

## Transformed instance (example)

```xml
<tn-ros:RoadLink>
  <tn-ros:startNode>17</tn-ros:startNode>
</tn-ros:RoadLink>
```

`startNode` (Long) = `17` — the `featureId` of the referenced `RoadNode`, joinable
to the `RoadNode` feature class.

## Model transformation rule

**Parameters:**

- `references`: the references to encode as Long FKs — each
  `{ path, targetFeatureType? }`. `path` is a selector (bare name or `/`-path);
  `targetFeatureType` (optional) names the target feature class (informative — the
  join target).

Mark each selected reference so it is emitted as a Long `featureId` foreign key
instead of the default Text href.

## Instance transformation rule

Resolve the reference to the target feature and write its `featureId` (the target's
assigned Long id) into the field. Unresolvable references remain empty.

## Solves usability issues

- Turns an opaque href string into a numeric key that joins to the target feature
  class within the Geodatabase — the usable form for intra-dataset relations
  (`startNode`/`endNode`, `inNetwork`, `upperLevelUnit`, `zoning`, …).

## Known usability issues

- Only meaningful for references resolvable within the dataset; external / URN
  references must stay Text (do not list them here).
- Relies on the target feature having a stable `featureId` (the base convention).

## INSPIRE compliance

Compliant: the association is retained; only its encoding changes from the href
string to the equivalent intra-dataset key. No information is lost for resolvable
references.

## Notes

- Used widely for network / hierarchy references (RoadTransportNetwork,
  EnvironmentalMonitoringFacilities `setUpFor`, MineralResources `relatedMine`, …).
- Not part of the original INSPIRE MIF 2017.2 catalogue; added to make the
  per-theme Geodatabase encoding rules executable.
