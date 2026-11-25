# MT011: High Cardinality Properties to Extra Tables

> **Implementation note.** As applied in the theme encodings, the rule
> takes **`paths`** — selectors of the high-cardinality properties to extract — and
> optional **`tableNames`** — a `{selector: name}` override (default table name
> `<FeatureType>_<property>`). Each extracted property becomes a separate table with
> an `RID` Long foreign key plus the property's flattened columns.

## Category

Alternate Structures for specific types or type hierarchies

## Description

Direct flattening of high-cardinality properties is not possible for storage in a database, especially when dealing with complex properties. GIS software as ArcGIS supports this through joining the extra information from a related table.

## Original instance (example)

```xml
<bu:Building gml:id="Building_1">
 <!--... -->
  <bu:part xlink:href="#BuildingPart_1"/>
  <bu:part xlink:href="#BuildingPart_2"/>
  <bu:part xlink:href="#BuildingPart_3"/>
<!--... -->
</bu:Building>
```

## Transformed instance (example, database table)

Table: Building
|featureId|...|
|------|------|
|1|...|
|2|...|
|3|...|

Table: Building_part
|RID|BuildingPart|
|------|------|
|1|BuildingPart_1|
|1|BuildingPart_2|
|1|BuildingPart_3|

## Model transformation rule

Move a property of a feature with a multiplicity > 1 to a separate table and link back to the original feature using its featureId. Attach the name of the property to the new table separated by an '_'

## Instance transformation rule

Copy the value of the ID of the source of the relationship to RID field in the Relationship table and all components of the property into the new table.

## Solves usability issues

The transformed data structure can easily be read and edited in desktop GIS and web GIS software and allows direct joins of related objects in RDBMS.

## Known usability issues

The multi-valued property is no longer inline on the feature: reading its values requires a join from the extra table back to the feature via the `RID` foreign key. A flat consumer (e.g. a simple CSV export or a viewer that only reads the feature class) will not see these values without following the relationship.

## INSPIRE compliance

Compliant — no information is lost. All values are retained in the extra table and linked to the feature by `RID`; only the physical layout changes (the repeated property is normalized into a child table), not the semantics.

## Notes

- Not part of the original INSPIRE MIF 2017.2 catalogue (MT001–MT009); added in this project.
