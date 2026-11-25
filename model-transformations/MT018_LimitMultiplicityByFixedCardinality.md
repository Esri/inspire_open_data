# MT018: Limit Multiplicity by Fixed Cardinality (No Arrays)

> **Not applied as a separate rule.** The fixed-cardinality indexing described here
> is performed by [MT012](./MT012_LimitMultiplicityForHighCardinalityProperties.md)
> (`number > 1` → `<name>_1 … <name>_N`). MT018 documents the pattern for catalogue
> completeness; in the MT012 implementation the index starts at `1` with separator `_`
> (the `startIndex` / `separator` parameters below are not configurable there).

## Category

Multiplicity / Cardinality Handling

## Description

Some target database formats do not support arrays, and at the same time directly
flattening a high-cardinality property (e.g. `0..*`) into hundreds or thousands of
columns is not usable.

This rule limits the multiplicity of a property to a fixed upper bound `N` (parameter)
by replacing the original repeating property with `N` indexed occurrences of the same
property, each with multiplicity `0..1`.

The rule can be applied to primitive properties, complex properties, and associations.
It does not change the value type. Subsequent transformation rules (e.g. flattening or
association handling) may be applied afterwards.

## Original instance (example)

```xml
<au:AdministrativeUnit>
  <au:lowerLevelUnit xlink:href="#low1"/>
  <au:lowerLevelUnit xlink:href="#low2"/>
  <au:lowerLevelUnit xlink:href="#low3"/>
  <au:lowerLevelUnit xlink:href="#low4"/>
</au:AdministrativeUnit>
```

## Transformed instance (example, N = 3)

```xml
<aus:AdministrativeUnit>
  <aus:lowerLevelUnit_1 xlink:href="#low1"/>
  <aus:lowerLevelUnit_2 xlink:href="#low2"/>
  <aus:lowerLevelUnit_3 xlink:href="#low3"/>
</aus:AdministrativeUnit>
```

## Model transformation rule

**Parameters:**

- `number` (required): maximum number of occurrences (`N`).
- `separator` (optional, default `_`): separator between property name and index.
- `startIndex` (optional, default `1`): start value for the index.

For a selected property `P` with multiplicity `0..*` or `1..*`, replace it by `N` new
properties `P_1, P_2, …, P_N`. Each new property has multiplicity `0..1` and the same
value type as `P`.

## Instance transformation rule

Let `P` be the source property and let its occurrences be ordered as in the source
instance.

- For `i = 0 … min(count(P), N) - 1`, copy the (i+1)-th occurrence of `P` into
  `P_{startIndex + i}`.
- If `count(P) > N`, all remaining occurrences are ignored (truncated).

The order of copied values shall be preserved.

## Solves usability issues

- No array usage in the target schema.
- Predictable, fixed schema width.
- Usable for relational databases.

## Known usability issues

- Possible information loss if `count(P) > N`.
- Choosing `N` too small may omit relevant data.
- Choosing `N` too large may lead to very wide tables.

## INSPIRE compliance

The resulting model can remain INSPIRE-compliant if mandatory content is not removed.
Truncation may omit optional occurrences; if full preservation is required, alternative
modelling approaches (e.g. extra tables, see `MT011`) should be used.

## Notes

- This rule is not part of the original INSPIRE MIF 2017.2 catalogue; it was added in
  this project as a catalogue reference for the fixed-cardinality indexing pattern used
  when flattening repeating properties.
