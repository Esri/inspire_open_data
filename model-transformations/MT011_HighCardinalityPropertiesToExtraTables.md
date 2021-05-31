## MT011: High Cardinality Properties to Extra Tables

<table>
<tr>
<td>Category</td>
<td>Alternate Structures for specific types or type hierarchies</td>
</tr>
<tr>
<td>Description</td>
<td><p>Direct flattening of high-cardinality properties is not possible for storage in a database, especially when dealing with complex properties. GIS software as ArcGIS supports this through joining the extra information from a related table.</p> 
</p>
</td>
</tr>
<tr>
<td>Original instance in default encoding:</td>
<td>

```xml
<bu:Building gml:id="Building_1">
 <!--... -->
  <bu:part xlink:href="#BuildingPart_1"/>
  <au:part xlink:href="#BuildingPart_2"/>
  <au:part xlink:href="#BuildingPart_3"/>
<!--... -->
</bu:Building>
```
   
</td>
</tr>
<tr>
<td>Transformed instance in database table encoding:</td>
<td>
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


</td>
</tr>
<tr>
<td>Model transformation rule: </td>
<td>
    <p>Move a property of a feature with a multiplicity > 1 to a seperate table and link back to the original feature using its featureId. Attach the name of the property to the new table seperated by an '_'</p>
</td>
</tr>
<tr>
<td>Instance transformation rule:</td>
<td>
	Copy the value of the ID of the source of the relationship to RID field in the Relationship table and and all components of the property into the new table.
</td>
</tr>
<tr>
<td>Solves usability issues:</td>
<td>The transformed data structure can easily be read and edited in desktop GIS and web GIS software and allows direct joins of related objects in RDBMS.</td>
</tr>
<tr>
<td>Known usability issues:</td>
<td></td>
</tr>
<tr>
<td>INSPIRE Compliance:</td>
<td></td>
</tr>
</table>

Notes:

 * None.
