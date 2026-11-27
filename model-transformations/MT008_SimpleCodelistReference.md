# MT008: Simplified Codelist Reference

> **Implementation note.** As applied in the theme encodings, the rule
> takes **`codelistAttributes`** — a list of
> selectors (bare name = all occurrences, `/`-path = one location) of the reference
> properties to treat as codelists. Each marked reference is flattened by MT001 into
> two Text fields, `<prop>_href` (the `xlink:href`) followed by `<prop>` (the
> `xlink:title`), in that order.

## Category

Alternate Structures for specific types or type hierarchies

## Description

References to codelists are one of the ubiquitous characteristics of the INSPIRE data specifications. They are usually encoded using a `ReferenceType`, which is derived from an `xlink`. In the conceptual model, they are represented using property types that point to classes with a `<<Codelist>>` stereotype.

The main usability issue with ReferenceTypes is that they encode all relevant information in the xlink attributes of the element. In particular, the actual external link is encoded in the `xlink:href` attribute, while additional information may be encoded in attributes such as `xlink:title`. An additional issue is that the actual, full codelist URLs are unwieldy to use for styling and filtering in most GIS. It would be much preferable to use the local codelist values. There is a recommendation to encode these using the mentioned `xlink:title`, but no strict requirement.

This simplified codelist reference takes the property name and uses it to encode the title directly, while all other properties are modelled as "subproperties":

- `reference`
- `reference.href`

Both of these properties are mandatory in the `SimpleCodelistReference`, while extra properties such as `arcRole`, `owns` and `type` are optional.

## Original instance (example)

```xml
<ad:Address gml:id="MIG20172_example_Address">
  <!-- ... -->
  <ad:status
    xlink:href="http://inspire.ec.europa.eu/codelist/StatusValue/current"
    xlink:title="current" />
  <!-- ... -->
</ad:Address>
```

## Transformed instance (example)

```xml
<ads:Address gml:id="MIG20172_example_Address">
  <!-- ... -->
  <simple:status>current</simple:status>
  <simple:status.href>http://inspire.ec.europa.eu/codelist/StatusValue/current</simple:status.href>
  <!-- ... -->
</ads:Address>
```

## Model transformation rule

**Parameters:**

- `type`: The property for which the ReferenceType is to be substituted, e.g. `status`.

Substitute existing `ReferenceType` on the `type` property with this SimpleReference type.

## Instance transformation rule

- Copy the value of the `xlink:title` attribute to the property with the name of the `type` parameter.
- Copy the value of the `xlink:href` attribute to the property with the name of the `type.href` parameter.

## Solves usability issues

The transformed data structure can easily be edited, filtered and symbolized in desktop GIS and web GIS software.

## Known usability issues

None.

## INSPIRE compliance

Fully compliant.

## Notes

 * None.
