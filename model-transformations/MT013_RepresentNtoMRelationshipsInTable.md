# MT013: Represent n:m Relationships in Table

## Category

Alternate Structures for specific types or type hierarchies

## Description

Relationships between Features can be represented in a Table structure by providing the IDs of corresponding objects in a table. Each Table row represents a Relationship in both directions. If the relationship is only one-directional this rule should not be used

## Original instance (example)

```xml
<au:AdministrativeUnit gml:id="AdminUnit_1">
 <!--... -->
  <au:boundary xlink:href="#AdminBoundary_1"/>
  <au:boundary xlink:href="#AdminBoundary_2"/>
  <au:boundary xlink:href="#AdminBoundary_3"/>
<!--... -->
</au:AdministrativeUnit>

<au:AdministrativeBoundary gml:id="AdminBoundary_1">
<!--... -->
  <au:admUnit xlink:href="#AdminUnit_1"/>
  <au:admUnit xlink:href="#AdminUnit_2"/>
  <au:admUnit xlink:href="#AdminUnit_3"/>
<!--... -->
</au:AdministrativeBoundary>
```

## Transformed instance (example, database table)

Table: AdministrativeUnit
|featureId|...|
|------|------|
|1|...|

Table: AdministrativeBoundary
|featureId|...|
|------|------|
|1|...|

Table: AdministrativeUnit_AdministrativeBoundary
|AdminUnit_ID|AdminBoundary_ID|
|------|------|
|1|1|
|1|2|
|1|3|
|2|1|
|3|1|

## Model transformation rule

Represent all existing References by Rows in the Reference table.

## Instance transformation rule

Copy the value of the ID of the source of the relationship to ID1 in the Relationship table and the ID of the target of the relationship to ID2 in the relationship table.

## Solves usability issues

The transformed data structure can easily be read and edited in desktop GIS and web GIS software and allows direct joins of related objects in RDBMS.  This transformation also reduces the number of necessary tables as both directions are stored in one table.

## Known usability issues

Neither feature class carries the related IDs inline: navigating the relationship (in either direction) requires a join through the junction table. A consumer that expects a foreign key on the feature itself will not find one.

## INSPIRE compliance

Compliant — no information is lost. Every relationship instance is stored once as an ID pair and remains navigable in both directions; only the representation changes (a shared table instead of two inline association ends).

## Notes

- Implementation: applied after MT001. Parameters: `tableName`; `left`/`right` each `{featureType, path, column?}`
  (`column` = the Long featureId FK column name, default `<path>Id`). On the `left`
  feature type the junction table is created (two Long FK columns) and the association
  field is dropped; on the `right` feature type only the association field is dropped (the
  table is created once, from the left side). Both columns carry the logical `id` type →
  GDB `Long` / GeoJSON `integer`.
- Used by: AdministrativeUnits (`AdministrativeUnit.boundary` ↔ `AdministrativeBoundary.admUnit`
  → `Relation_Unit_Boundary` with columns `boundaryId`, `unitId`).
- Not part of the original INSPIRE MIF 2017.2 catalogue (MT001–MT009); added in this project.
