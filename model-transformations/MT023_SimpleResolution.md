# MT023: Simplified Resolution

## Category

Alternate Structures for specific types or type hierarchies

## Description

`MD_Resolution` (ISO 19115) models a level of detail / spatial resolution as a
**choice** of two members:

* `equivalentScale` — an `MD_RepresentativeFraction` whose `denominator` is the
  *N* of a map scale 1:*N* (an integer), or
* `distance` — a ground sample distance (a length value with a unit of measure).

In the default encoding this produces a deeply nested, two-branch structure
(`levelOfDetail.MD_Resolution.equivalentScale.MD_RepresentativeFraction.denominator`
and `levelOfDetail.MD_Resolution.distance.Distance` + `uom`), and because the
property carries an `owns`/reference marker it is otherwise mis-encoded as a
feature association (a `Long` foreign key).

This rule collapses the property to **a single value field** — the
`equivalentScale` **denominator** (the 1:*N* scale), encoded as `Long`. The
alternative `distance` member is not represented in the simplified encoding.

## Original instance (example, default encoding)

```xml
<hy-p:Watercourse>
  <hy-p:levelOfDetail>
    <gmd:MD_Resolution>
      <gmd:equivalentScale>
        <gmd:MD_RepresentativeFraction>
          <gmd:denominator><gco:Integer>25000</gco:Integer></gmd:denominator>
        </gmd:MD_RepresentativeFraction>
      </gmd:equivalentScale>
    </gmd:MD_Resolution>
  </hy-p:levelOfDetail>
</hy-p:Watercourse>
```

## Transformed instance (example)

```xml
<hy-ps:Watercourse>
  <!-- ... -->
  <hy-ps:levelOfDetail>25000</hy-ps:levelOfDetail>   <!-- Long: the 1:N scale denominator -->
  <!-- ... -->
</hy-ps:Watercourse>
```

## Model transformation rule

**Parameters:**

- `properties` (optional): selectors (bare property name = all occurrences, or a
  `/`-path) of the `MD_Resolution`-typed properties to collapse. Omitted = every
  property that carries an `equivalentScale`/`distance` member.

For each selected property: keep a single value field (the `equivalentScale`
denominator, `Long`), drop the `distance` branch and the nested
`MD_Resolution`/`MD_RepresentativeFraction` machinery, and clear the spurious
reference flag.

## Instance transformation rule

Copy the value of `equivalentScale/MD_RepresentativeFraction/denominator` to the
property. Where only `distance` is present it is not carried over (deliberate
simplification — most datasets express level of detail as a map scale).

## Solves usability issues

- Removes a deeply nested two-branch choice that is hard to read and edit.
- Yields a single, directly usable scale value per feature.

## Known usability issues

- The `distance` alternative is dropped; datasets that express resolution only as
  a ground distance lose that value. A future variant could keep `distance`
  (+ uom) instead, selected per theme.

## INSPIRE compliance

Compliant where level of detail is expressed as `equivalentScale` (the common
case). Where it is expressed as `distance`, that value is dropped, so the simplified
form is then conformant only as an *additional* encoding alongside the default GML.

## Notes

- Used by HydroPhysicalWaters for `levelOfDetail`.
- Not part of the original INSPIRE MIF 2017.2 catalogue; added to make the
  per-theme Geodatabase encoding rules executable.
