# MT021: Simplified Contact

> **Implementation note.** As applied in the theme encodings, the rule
> flattens a contact to the seven leaves below (`<prop>_address` … `<prop>_website`;
> MT019 may shorten the prefix). Parameters: **`properties`** — property names to treat
> as a contact (needed where the source carries the property, e.g. `pointOfContact`,
> without an inline `Contact` type, so it is matched by name); **`types`** — extra data-type names treated
> as a contact. `telephoneFacsimile` / `telephoneVoice` stay repeatable (limit with MT012).

## Category

Alternate Structures for specific types or type hierarchies

## Description

The INSPIRE base type `base2:Contact` bundles a person's or
organisation's communication channels. Its nested structure (free-text fields,
an embedded address, multi-valued telephone numbers) buries the few values that
matter for most use cases and is awkward to edit, filter and symbolize in a
GIS. This rule proposes a flat alternative representation for
`Contact`, analogous to the [Simple Citation](./MT007_SimpleCitation.md) rule.

The simplified contact keeps the seven properties of `base2:Contact`
as flat text attributes:

- address
- contactInstructions
- electronicMailAddress
- hoursOfService
- telephoneFacsimile
- telephoneVoice
- website

The embedded `address` (an `AddressRepresentation`) is
reduced to a single free-text line. `telephoneFacsimile` and
`telephoneVoice` are multi-valued in the model; they remain
repeatable after this rule and are typically limited to one occurrence with
[MT012](./MT012_LimitMultiplicityForHighCardinalityProperties.md).

## Original instance (example)

```xml
<us-govserv:GovernmentalService>
  <!-- ... -->
  <us-govserv:pointOfContact>
    <base2:Contact>
      <base2:electronicMailAddress>info@example.org</base2:electronicMailAddress>
      <base2:telephoneVoice>+49 30 000000</base2:telephoneVoice>
      <base2:website>https://example.org</base2:website>
    </base2:Contact>
  </us-govserv:pointOfContact>
  <!-- ... -->
</us-govserv:GovernmentalService>
```

## Transformed instance (example)

```xml
<us-govserv:GovernmentalService>
  <!-- ... -->
  <us-govserv:pointOfContact>
    <simple:SimpleContact>
      <simple:electronicMailAddress>info@example.org</simple:electronicMailAddress>
      <simple:telephoneVoice>+49 30 000000</simple:telephoneVoice>
      <simple:website>https://example.org</simple:website>
    </simple:SimpleContact>
  </us-govserv:pointOfContact>
  <!-- ... -->
</us-govserv:GovernmentalService>
```

## Model transformation rule

Substitute the `base2:Contact` type with this SimpleContact type.
Each property maps directly to the property of the same name on
`base2:Contact`.

## Instance transformation rule

- Reduce the embedded `base2:address`
  (`AddressRepresentation`) to a single free-text value and copy
  it to `simple:address`.
- Copy the value of each remaining `base2:*` property to the
  `simple:*` property of the same name.
- For the multi-valued `telephoneFacsimile` and
  `telephoneVoice`, apply MT012 to limit the number of values
  retained where a single value is sufficient.

## Solves usability issues

The transformed data structure can easily be edited, filtered and symbolized in desktop GIS and web GIS software. This transformation also reduces data volume.

## Known usability issues

The structured address and the distinction between multiple telephone/fax numbers are lost. Where these are needed, use the default encoding instead.

## INSPIRE compliance

This rule removes finer-grained address structure and additional telephone/fax values. It is a conformant INSPIRE encoding *on its own* only where those are void, or homogeneous and documented in the dataset metadata; where the source populates a structured address or multiple numbers, it is conformant only as an *additional* encoding alongside the default GML.

## Notes

- Not part of the original INSPIRE MIF 2017.2 catalogue (MT001–MT009); added in this project.
