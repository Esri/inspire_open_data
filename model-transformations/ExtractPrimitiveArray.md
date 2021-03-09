## Extract Primitive Array

<table>
<tr>
<td>Category</td>
<td>...</td>
</tr>
<tr>
<td>Description</td>
<td><p>In some cases, direct flattening of high-cardinality properties will lead to data usability issues further downstream in processes. At the same time, at least some software such as QGIS supports arrays of simple properties. This method can be used to extract the salient property of a complex property and then create an array of those simple values. An example where this can be applied is to store relationships between objects:</p>
<ul>
    <li>lowerLevelUnits: LinktoToUnit_01, LinktoToUnit_02, LinktoToUnit_03, ... </li>
</ul>
</td>
</tr>
<tr>
<td>Original instance in default encoding:</td>
<td>

```xml
<au:AdministrativeUnit gml:id="MIG20172_example_AdministrativeUnit">
    <!-- ... -->
    <au:lowerLevelUnit xlink:href="#MIG20172_example_AdministrativeUnit_low1"/>
    <au:lowerLevelUnit xlink:href="#MIG20172_example_AdministrativeUnit_low2"/>
    <au:lowerLevelUnit xlink:href="#MIG20172_example_AdministrativeUnit_low3"/>
    <!-- ... -->
</AdministrativeUnit>
```
   
</td>
</tr>
<tr>
<td>Transformed instance in alternate (GeoJSON) encoding:</td>
<td>

```json
{
    "lowerLevelUnit": ["MIG20172_example_AdministrativeUnit_low1", "MIG20172_example_AdministrativeUnit_low2", "MIG20172_example_AdministrativeUnit_low3"]
}
``` 

</td>
</tr>
<tr>
<td>Model transformation rule: </td>
<td>
    <ul>
        <li>`valueProperty`: The name of the property from which to take the values to be copied to the array in the transformed instance.</li>
    </ul>
    <p>The property name is left unchanged. Its implementation type is transformed from its current type to either an array of the original type if that type was simple, or to an array of the type of the valueProperty. Note that when appied to the Default GML encoding, this rule by itself makes no difference to the encoding when not combined with a concatenation/aggregation instance transformation.</p>
</td>
</tr>
<tr>
<td>Instance transformation rule:</td>
<td><p>Parameters:</p> 
    <ul>
        <li><code>valueProperty</code>: The name of the property from which to take the values to be copied to the array in the transformed instance.</li>
    </ul>
    <p>For each instance of the <code>valueProperty</code>, push its value to the array in the target property. The order of values that are copied from the source properties should be kept.</p>
</td>
</tr>
<tr>
<td>Solves usability issues:</td>
<td>This rule reduces overhead and makes it possible to have workable transformed data structures that are not polluted by hundreds or even thousands of properties. It also provides a good base for further simplification in case the target environment does not support arrays.</td>
</tr>
<tr>
<td>Known usability issues:</td>
<td>Some software cannot process arrays.</td>
</tr>
<tr>
<td>INSPIRE Compliance:</td>
<td>The transformed model is fully compliant to INSPIRE as long as no mandatory properties other than the valueProperty have been left out.</td>
</tr>
</table>

Notes: No notes.
