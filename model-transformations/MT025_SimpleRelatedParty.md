# MT025: Simplified RelatedParty

## Category

Alternate Structures for specific types or type hierarchies

## Description

`base2:RelatedParty` (INSPIRE Base Types 2) names a party related to a feature —
e.g. the `competentAuthority` of a management/restriction zone. It carries the
party's name parts (`individualName` / `organisationName` / `positionName`, all
localised `PT_FreeText`), an embedded `base2:Contact`, and a `role`
(`PartyRoleValue` codelist). Without a dedicated rule, this nested structure would be
carried as a single opaque XML value, which is unusable as a field.

This rule replaces it with the flat **SimpleRelatedParty** leaves the
published field lists use — the three name parts, the seven SimpleContact leaves
of the embedded `Contact` (see MT021), and the `role` — each as Text:

```
individualName, organisationName, positionName,
address, contactInstructions, electronicMailAddress, hoursOfService,
telephoneFacsimile, telephoneVoice, website,
role
```

## Original instance (example, default encoding)

```xml
<am:competentAuthority>
  <base2:RelatedParty>
    <base2:individualName>…</base2:individualName>
    <base2:organisationName>…</base2:organisationName>
    <base2:contact><base2:Contact>…</base2:Contact></base2:contact>
    <base2:role xlink:href="…/PartyRoleValue/authority"/>
  </base2:RelatedParty>
</am:competentAuthority>
```

## Transformed instance (example, prefix `related_`)

```xml
<ams:ManagementRestrictionOrRegulationZone>
  <!-- ... -->
  <ams:related_organisationName>Danish Nature Agency</ams:related_organisationName>
  <ams:related_electronicMailAddress>info@example.org</ams:related_electronicMailAddress>
  <ams:related_role>authority</ams:related_role>
  <!-- + related_individualName, related_positionName, related_address,
       related_contactInstructions, related_hoursOfService,
       related_telephoneFacsimile, related_telephoneVoice, related_website -->
</ams:ManagementRestrictionOrRegulationZone>
```

## Model transformation rule

**Parameters:**

- `properties`: selectors (bare name) of the RelatedParty-typed properties to
  flatten. Needed because the source carries them without an inline
  `RelatedParty` data type, so they can only be matched by name.
- `types` (optional): extra data-type names treated as RelatedParty.
- `prefix` (optional): prepended to every leaf name. The published field lists
  prefix the RelatedParty relation-table columns (e.g. `related_`), which MT011
  would otherwise strip together with the property name.
- `leaves` (optional): a subset of the SimpleRelatedParty leaves to keep (in their
  canonical order), for field lists that retain only part of the party (e.g. just
  `organisationName`). Default = the full set.

For each selected property, replace its content with the flat leaves above (in
the listed order), each Text.

## Instance transformation rule

Copy the RelatedParty name parts and role, and the embedded `Contact` leaves
(per MT021 SimpleContact), into the corresponding `<prefix><leaf>` fields.

## Solves usability issues

- Turns an opaque XML blob into directly usable, flat party + contact fields.

## Known usability issues

- The party `role` is kept as a single Text value (not a value + `_href`
  codelist pair); sufficient for the published field lists.

## INSPIRE compliance

Compliant: the kept fields carry the party's name, contact details and role. Dropped
are the name localisation (the `PT_FreeText` language of the name parts and the
embedded address structure) and the `role` codelist URI (the role is kept as a plain
label). It is a conformant INSPIRE encoding *on its own* only where those are void, or
homogeneous and documented in metadata; otherwise it is conformant only as an
*additional* encoding alongside the default GML.

## Notes

- Embeds the same leaves as MT021 (SimpleContact). Used by
  AreaManagementRestrictionAndRegulationZones for `competentAuthority`.
- Not part of the original INSPIRE MIF 2017.2 catalogue; added to make the
  per-theme Geodatabase encoding rules executable.
