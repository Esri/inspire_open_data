# MT027: Extract Secondary Geometry To Feature Class

## Category

Geometry / relationships

## Description

A feature type may carry **more than one geometry property**. A File Geodatabase
feature class holds exactly **one** geometry column, so only the primary geometry
can live on the main feature class. This rule moves a **secondary** geometry into
its **own spatial child feature class**, linked back to the parent by an `RID`
foreign key (a relationship class in the target GDB).

The archetype is **`CadastralParcel.referencePoint`**: a cadastral parcel has a
surface geometry (its boundary polygon) *and* a `GM_Point` reference point (e.g.
the label / centroid position). The parcel surface stays on `CadastralParcel`;
the reference point becomes a separate Point feature class
`CadastralParcel_referencePoint` (`RID` + geometry), exactly as in the published
GDB. Without this rule the secondary geometry is either dropped by MT001 (which
keeps a single geometry per feature class) or — if forced through MT011 —
mis-encoded as a text column.

The `<FeatureType>_<property>` naming mirrors MT011 relationship tables; the
difference is that the child here is **spatial** (carries geometry) rather than a
plain attribute table.

## Original instance (example, default encoding)

`CadastralParcel` has two geometries — the surface and the reference point:

```xml
<cp:CadastralParcel>
  <cp:geometry>       <gml:Surface>…</gml:Surface></cp:geometry>
  <cp:referencePoint> <gml:Point>…</gml:Point>    </cp:referencePoint>
</cp:CadastralParcel>
```

Default flattening keeps only one geometry per feature class; the reference point
would be lost.

## Transformed instance (example)

Two feature classes, linked by `RID`:

```
CadastralParcel                 (Surface)  … , featureId, …
CadastralParcel_referencePoint  (Point)    RID
```

## Model transformation rule

**Parameters:**

- `geometries`: a list of `{ path, type? }`:
  - `path` — the secondary geometry property (selector; a bare name matches all
    occurrences, a `/`-path matches one location).
  - `type` — the abstract geometry kind `Point` | `Line` | `Surface`. Omitted →
    the abstract `Geometry` (any).

For each entry: remove the named geometry property from the parent's property tree
and register a spatial child feature class `<FeatureType>_<property>` with an `RID`
Long foreign key and the given geometry. Runs **before** MT001, so the
parent's remaining (primary) geometry is picked normally.

## Instance transformation rule

Each parent feature emits one child feature per secondary geometry, carrying the
parent's `RID`. (Populating the child is a data-preparation concern.)

## Solves usability issues

- Preserves a second, map-relevant geometry that a single-geometry feature class
  cannot hold — instead of silently dropping it or degrading it to text.
- Produces the same shape a consumer expects from the published GDB: a small
  spatial child feature class keyed by `RID`.

## Known usability issues

- Reading both geometries together needs the `RID` relationship (a join), as with
  any extracted child.

## INSPIRE compliance

Compliant: no information is invented or lost — the secondary geometry is retained
verbatim, relocated to a linked feature class because the target format allows one
geometry per feature class.

## Notes

- Implementation: applied before MT001; the child feature class is appended to the
  feature classes of the theme.
- Used by: CadastralParcels (`CadastralParcel.referencePoint` → Point feature class
  `CadastralParcel_referencePoint`).
- Not part of the original INSPIRE MIF 2017.2 catalogue; added to make the
  per-theme Geodatabase encoding rules executable.
