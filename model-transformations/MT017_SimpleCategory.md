# MT017: Simplified Category

## Category

Alternate Structures for specific types or type hierarchies

## Description

A `swe:Category` (OGC SWE Common) encodes a classified term — a value drawn from
a controlled vocabulary, identified by a code space. In the default encoding it
explodes into the full SWE Common machinery (`referenceFrame`, `axisID`,
`updatable`, `optional`, `definition`, `extension`, `identifier`, `label`,
`description`, nested `quality`/`Quantity`, `constraint`, `nilValues`, …) — dozens
of housekeeping fields per occurrence.

This rule keeps only the classification itself, as two Text fields:

* `<property>_codespace` — the code space (the dictionary / scheme the term is from),
* `<property>_value` — the category value (the term).

## Original instance (example, default encoding)

```xml
<mr-core:expression>
  <swe:Category codeSpace="http://.../ExpressionDictionary">
    <swe:value>vein</swe:value>
    <!-- + referenceFrame, axisID, quality, constraint, ... -->
  </swe:Category>
</mr-core:expression>
```

## Transformed instance (example)

```xml
<mr-cores:MineralOccurrence>
  <!-- ... -->
  <mr-cores:expression_codespace>http://.../ExpressionDictionary</mr-cores:expression_codespace>
  <mr-cores:expression_value>vein</mr-cores:expression_value>
  <!-- ... -->
</mr-cores:MineralOccurrence>
```

## Model transformation rule

**Parameters:**

- `properties` (optional): selectors (bare name = all occurrences) of the
  `Category`-typed properties to collapse. Omitted = every property whose data
  type is `Category`.

For each selected property, keep exactly `codespace` (Text) and `value` (Text),
and drop the rest of the SWE Common structure (and the spurious reference flag).

## Instance transformation rule

Copy the `swe:Category` `codeSpace` to `<property>_codespace` and `swe:value` to
`<property>_value`.

## Solves usability issues

- Removes dozens of SWE Common housekeeping fields per category occurrence.
- Yields a compact, directly usable code-space + value pair.

## Known usability issues

- None of note; the classification (scheme + term) is preserved.

## INSPIRE compliance

Compliant: the kept fields carry the classification value and its code space — the
INSPIRE domain content. The dropped members are SWE Common encoding scaffolding
(`referenceFrame`, `axisID`, `quality`, `constraint`, …), not domain information, so
the classification is preserved and the encoding is effectively lossless.

## Notes

- Used by MineralResources for `expression`/`form`/`shape`.
- Not part of the original INSPIRE MIF 2017.2 catalogue (MT001–MT009); added in this project.
