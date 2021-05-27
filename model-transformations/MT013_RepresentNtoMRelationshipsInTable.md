## MT015: Represent n:m Relationships in Table

<table>
<tr>
<td>Category</td>
<td>Alternate Structures for specific types or type hierarchies</td>
</tr>
<tr>
<td>Description</td>
<td><p>Relationships between Features can be represented in a Table structur by providing the IDs of corresponding objects in a table. Each Table row represents a Relationship in both directions. If the relationship is only onedirectional this rule should not be used</p> 
</p>
</td>
</tr>
<tr>
<td>Original instance in default encoding:</td>
<td>

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
   
</td>
</tr>
<tr>
<td>Transformed instance encoded in a table:</td>
<td>

|AdmminUnit_ID|AdminBoundary_ID|
|------|------|------|------|
|1|1|
|1|2|
|1|3|
|2|1|
|3|1|


</td>
</tr>
<tr>
<td>Model transformation rule: </td>
<td>
    <p>Represent all existing References with by Rows in the Reference table.</p>
</td>
</tr>
<tr>
<td>Instance transformation rule:</td>
<td>
	Copy the value of the ID of the source of the relationship to ID1 in the Relationship table and the ID of the target of the relationship to ID2 in the relationship table.
</td>
</tr>
<tr>
<td>Solves usability issues:</td>
<td>The transformed data structure can easily be read and edited in desktop GIS and web GIS software and allows direct joins of related objects in RDBMS.  This transformation also reduces the number of necessary tables as both directions are stored in one table.</td>
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
