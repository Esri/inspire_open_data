# MT022: Restrict Union Members

## Category

Alternate Structures for specific types or type hierarchies

## Description

INSPIRE models several "by-X" alternatives as a *union* — a type
where exactly one of several members carries the value. In GML these are
encoded as an XSD `<choice>`. Examples are
`ServiceLocationType` (`serviceLocationByAddress` |
`serviceLocationByBuilding` | `serviceLocationByGeometry` |
`serviceLocationByActivityComplex` |
`serviceLocationByUtilityNode`) and
`AreaOfResponsibilityType` (by administrative unit | by named place |
by network | by polygon).

An alternative encoding frequently offers only a subset of the union members —
typically the geometry member, so that the union becomes a plain feature
geometry. This rule lets an encoding declare, per union property, which members
to **keep** (all others are dropped) or which members to
**remove** (the rest are kept). It is general: the retained members
need not be geometry.

## Original instance (example)

```xml
<us-govserv:GovernmentalService>
  <!-- ... -->
  <us-govserv:serviceLocation>
    <us-govserv:ServiceLocationType>
      <us-govserv:serviceLocationByGeometry>
        <gml:Point gml:id="p1"><gml:pos>...</gml:pos></gml:Point>
      </us-govserv:serviceLocationByGeometry>
    </us-govserv:ServiceLocationType>
  </us-govserv:serviceLocation>
  <!-- the choice also permits serviceLocationByAddress / ...ByBuilding /
       ...ByActivityComplex / ...ByUtilityNode -->
</us-govserv:GovernmentalService>
```

## Transformed instance (example, keep serviceLocationByGeometry)

```xml
<us-govservs:GovernmentalService>
  <!-- ... -->
  <us-govservs:serviceLocation>
    <gml:Point gml:id="p1"><gml:pos>...</gml:pos></gml:Point>
  </us-govservs:serviceLocation>
  <!-- only the retained geometry member remains; the union wrapper is dropped -->
</us-govservs:GovernmentalService>
```

## Model transformation rule

For each named union property, retain only the members listed under
`keep` (and drop every other member), or drop only the members
listed under `remove` (and retain the rest). Exactly one of
`keep` / `remove` is given per union.

When the only retained member(s) carry a geometry, the property reduces to
a plain geometry: it becomes the feature class geometry (or, inside an
extracted relationship table, the geometry is not stored — the table keeps
only its `RID`).

## Instance transformation rule

- Discard the instances of every union member that is not retained.
- If a single geometry member is retained, lift its geometry to the
  enclosing feature (the union wrapper element is removed).

## Solves usability issues

Removes alternative reference structures that a given encoding does not
support, so the remaining data is simple to store, edit and symbolize. A
geometry-only union becomes an ordinary spatial column.

## Known usability issues

The dropped union members cannot be represented; data that uses them is not
encodable and must be provided through a member that is retained.

## INSPIRE compliance

Restricting a union to a subset of its members narrows what the encoding can
express. It is intended for alternative encodings with an explicit precondition
(e.g. "the service location is provided by geometry").

## Notes

- A `keep` / `remove` name that is not an actual member of the union is reported
  as a warning, so a typo or an upstream rename never passes unnoticed.
- Not part of the original INSPIRE MIF 2017.2 catalogue (MT001–MT009); added in this project.
