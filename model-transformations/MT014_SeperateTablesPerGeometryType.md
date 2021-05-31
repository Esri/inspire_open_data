## MT014: Separate Tables Per Geometry Type

<table>
<tr>
<td>Category</td>
<td>Alternate Structures for specific types or type hierarchies</td>
</tr>
<tr>
<td>Description</td>
<td><p>The encoding in GML allows mixing geometrie properties with diferent data types in the same file/structure. This is not possible in some GIS Databases. Therefore with this rule the one Feature Class per geometry type is used to seperate heterogenious geometry types into tables. A prefix is used to indicate wicht type of Geometry is stored in each table. P for Point geometries, L for Line and S for Area geeometries.</p> 
</p>
</td>
</tr>
<tr>
<td>Original instance in default encoding:</td>
<td>

```xml
	<gml:featureMember>
		<am:ManagementRestrictionOrRegulationZone>
			<am:geometry>
				<gml:Point ...>
					<!-- ... -->
				</gml:Point>
			</am:geometry>
			<!-- ... -->
		</am:ManagementRestrictionOrRegulationZone>
	</gml:featureMember>
	<gml:featureMember>
		<am:ManagementRestrictionOrRegulationZone>
			<am:geometry>
				<gml:LineString ...>
					<!-- ... -->
				</gml:LineString>
			</am:geometry>
			<!-- ... -->
		</am:ManagementRestrictionOrRegulationZone>
	</gml:featureMember>
	<gml:featureMember>
		<am:ManagementRestrictionOrRegulationZone >
			<gml:MultiSurface>
				<!-- ... -->
			</gml:MultiSurface>
		</am:ManagementRestrictionOrRegulationZone>
		<!-- ... -->
	</gml:featureMember>
```
   
</td>
</tr>
<tr>
<td>Transformed instance in default encoding:</td>
<td>

```xml
<gml:featureMember>
		<ams:ManagementRestrictionOrRegulationZoneP>
			<ams:geometry>
				<gml:Point ...>
					<!-- ... -->
				</gml:Point>
			</ams:geometry>
			<!-- ... -->
		</ams:ManagementRestrictionOrRegulationZoneP>
	</gml:featureMember>
	<gml:featureMember>
		<ams:ManagementRestrictionOrRegulationZoneL>
			<ams:geometry>
				<gml:LineString ...>
					<!-- ... -->
				</gml:LineString>
			</ams:geometry>
			<!-- ... -->
		</ams:ManagementRestrictionOrRegulationZoneL>
	</gml:featureMember>
	<gml:featureMember>
		<ams:ManagementRestrictionOrRegulationZoneS>
			<gml:MultiSurface>
				<!-- ... -->
			</gml:MultiSurface>
		</ams:ManagementRestrictionOrRegulationZoneS>
		<!-- ... -->
	</gml:featureMember>


``` 

</td>
</tr>
<tr>
<td>Model transformation rule: </td>
<td>
    <p>Store each object in table according to its geometry type.</p>
</td>
</tr>
<tr>
<td>Instance transformation rule:</td>
<td>
	<ul>
		<li>If the geometry is a point geometry copy th object into the FeatureClass ending with P</li>
		<li>If the geometry is a line geometry copy th object into the FeatureClass ending with L.</li>
        <li>If the geometry is a area geometry copy th object into the FeatureClass ending with S.</li>
		</ul>
</td>
</tr>
<tr>
<td>Solves usability issues:</td>
<td>The transformed data structure can easily be read and edited in desktop GIS and web GIS software.</td>
</tr>
<tr>
<td>Known usability issues:</td>
<td>There are at maximum 3 instead of one table in the target structure.</td>
</tr>
<tr>
<td>INSPIRE Compliance:</td>
<td>No issues.</td>
</tr>
</table>

Notes:

 * None.
