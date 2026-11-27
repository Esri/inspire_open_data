# MT024: Simplified Dimension

## Category

Alternate Structures for specific types or type hierarchies

## Description

`EarthResourceDimension` (INSPIRE Mineral Resources) describes the physical
extent of a deposit/occurrence through up to four members — `area`, `length`,
`width`, `depth` — each modelled as an OGC **SWE Common `QuantityRange`** (a
value range *low … high* with a unit of measure). In the default encoding every
member explodes into the full SWE Common structure (`referenceFrame`, `axisID`,
`updatable`, `optional`, `definition`, `extension`, `identifier`, `label`,
`description`, nested `quality/Quantity`, …) — hundreds of housekeeping fields
per feature.

This rule keeps, **per member**, only what the simplified encoding needs:

* `<member>_uom` (Text) — the unit of measure,
* `<member>_value_low` (Float) — the lower bound,
* `<member>_value_high` (Float) — the upper bound,

and drops the rest of the SWE Common machinery.

## Original instance (example, default encoding)

```xml
<mr-core:dimension>
  <mr-core:EarthResourceDimension>
    <mr-core:area>
      <swe:QuantityRange>
        <swe:uom code="km2"/>
        <swe:value>1.5 2.0</swe:value>
        <!-- + referenceFrame, axisID, quality/Quantity, ... -->
      </swe:QuantityRange>
    </mr-core:area>
    <!-- length, width, depth analogous -->
  </mr-core:EarthResourceDimension>
</mr-core:dimension>
```

## Transformed instance (example)

```xml
<mr-cores:MineralOccurrence>
  <!-- ... -->
  <mr-cores:dimension_area_uom>km2</mr-cores:dimension_area_uom>
  <mr-cores:dimension_area_value_low>1.5</mr-cores:dimension_area_value_low>
  <mr-cores:dimension_area_value_high>2.0</mr-cores:dimension_area_value_high>
  <!-- dimension_length_*, dimension_width_*, dimension_depth_* analogous -->
</mr-cores:MineralOccurrence>
```

## Model transformation rule

**Parameters:**

- `properties` (required in practice): selectors (bare name = all occurrences) of
  the `EarthResourceDimension`-typed properties to collapse.

For each selected property, for each member, replace the SWE `QuantityRange`
sub-tree with exactly `uom` (Text) + `value_low` (Float) + `value_high` (Float);
members are ordered `area, length, width, depth`.

## Instance transformation rule

Copy the `QuantityRange` `uom/@code` to `<member>_uom` and the two tokens of the
`QuantityRange` `value` (the range) to `<member>_value_low` / `<member>_value_high`.

## Solves usability issues

- Removes hundreds of SWE Common housekeeping fields per feature.
- Yields a compact, directly usable per-member value range.

## Known usability issues

- Assumes the member is a `QuantityRange` (low/high). A single-valued `Quantity`
  member would need a `<member>_value` variant.

## INSPIRE compliance

Compliant: the kept fields carry the dimension values (low/high) and unit — the
INSPIRE domain content. The dropped members are SWE Common encoding scaffolding, not
domain information, so the dimension is preserved and the encoding is effectively
lossless (assuming the member is a `QuantityRange` with low/high bounds).

## Notes

- Used by MineralResources for `dimension` (MineralOccurrence).
- Not part of the original INSPIRE MIF 2017.2 catalogue; added to make the
  per-theme Geodatabase encoding rules executable.
