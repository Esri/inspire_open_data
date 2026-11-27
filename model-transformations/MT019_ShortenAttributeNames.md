# MT019: Shorten Attribute Names

## Category

General model simplification rules

## Description

After flattening (`MT001`), nested INSPIRE properties produce long, repetitive
attribute names (e.g. `habitat_localHabitatName_localScheme`). Several target
formats restrict attribute-name length — a File Geodatabase limits field names to
**64 characters** — and long names are hard to read in GIS clients.

This rule shortens the already-flattened attribute names by applying an **ordered
list of string replacements**. Each replacement maps a name prefix/substring to a
shorter abbreviation. The replacements are applied **in the given order**, and the
order matters: more specific prefixes must come before more general ones so that a
general rule does not consume a substring that a later, more specific rule needs.

This is a pure name-rewriting rule; it changes neither the value types nor the
structure of the model, only the attribute names. It is therefore reversible only
if the replacement map is bijective on the actual set of names.

## Original instance (example, after MT001)

```
habitat_referenceHabitatTypeId
habitat_referenceHabitatTypeId_href
habitat_localHabitatName_localScheme
habitat_areaCovered
habitat_areaCovered_uom
habitatVegetation_localVegetationName_localScheme
```

## Transformed instance (example)

Applying the replacements (in order)
`habitatVegetation_localVegetationName_`→`hVeg_`,
`habitat_reference`→`h_r`,
`habitat_localHabitatName_`→`h_l_`,
`habitat_`→`h_`:

```
h_rHabitatTypeId
h_rHabitatTypeId_href
h_l_localScheme
h_areaCovered
h_areaCovered_uom
hVeg_localScheme
```

## Model transformation rule

**Parameters:**

- `replacements` (required): an **ordered** list of objects, each with:
  - `from` (required): the substring to search for in an attribute name.
  - `to` (required): the replacement string.
  - `exact` (optional, default false): when true, the replacement applies only if the
    whole attribute name equals `from` (anchored), so a general substring is not
    rewritten inside a longer name (e.g. `building` → `building_href` without also
    hitting `ld_buildingIdentifier`).

For each attribute name, apply every replacement in list order: replace the first
occurrence of `from` with `to` (a prefix-style replacement is the typical use).
Process all attributes of the feature type with the same ordered list.

**Ordering requirement:** list more specific `from` strings before more general
ones (e.g. `habitat_localHabitatName_` before `habitat_`), otherwise the general
rule rewrites the prefix first and the specific rule no longer matches.

## Instance transformation rule

None at the attribute-value level — only attribute (field) names change. Values are
copied unchanged from the source attribute to the renamed target attribute.

## Solves usability issues

- Keeps field names within target-format length limits (e.g. 64 chars for File Geodatabase).
- Produces shorter, more readable field names in desktop and web GIS clients.

## Known usability issues

- Abbreviations reduce self-descriptiveness; the mapping should be documented in the
  encoding rule / dataset metadata.
- Carelessly ordered or overlapping replacements can produce collisions (two source
  names mapping to the same target name); the encoding rule author must ensure the
  resulting names stay unique.

## INSPIRE compliance

Fully compliant: the rule only renames attributes and does not remove or alter any
content. Compliance is preserved as long as the renaming stays unambiguous (no two
distinct properties collapse to the same name).

## Notes

- This rule is not part of the original INSPIRE MIF 2017.2 catalogue; it was added
  to make the per-theme Geodatabase encoding rules (which rely on attribute
  shortening, e.g. Habitats And Biotopes) fully executable.
