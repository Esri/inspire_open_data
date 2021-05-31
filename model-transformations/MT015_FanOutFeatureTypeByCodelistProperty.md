## MT015: FanOutFeatureTypeByCodelistProperty

<table>
<tr>
<td>Category</td>
<td>Alternate Structures for specific types or type hierarchies</td>
</tr>
<tr>
<td>Description</td>
<td><p>This rule is used to Fan-Out Features by the value of a codelist property. </p> 
</p>
</td>
</tr>
<tr>
<td>Original instance in default encoding:</td>
<td>

```xml
	<gml:featureMember>
		<au:AdministrativeUnit>
			<au:nationalLevel xlink:href="http://inspire.ec.europa.eu/codelist/AdministrativeHierarchyLevel/1stOrder"/>
			<!-- ... -->
		</au:AdministrativeUnit>
	</gml:featureMember>
	<gml:featureMember>
		<au:AdministrativeUnit>
			<au:nationalLevel xlink:href="http://inspire.ec.europa.eu/codelist/AdministrativeHierarchyLevel/2ndOrder"/>
			<!-- ... -->
			<au:boundary xsi:nil="true"/>
		</au:AdministrativeUnit>
	</gml:featureMember>
	<gml:featureMember>
		<au:AdministrativeUnit>
			<au:nationalLevel xlink:href="http://inspire.ec.europa.eu/codelist/AdministrativeHierarchyLevel/3rdOrder"/>
			<!-- ... -->
		</au:AdministrativeUnit>
	</gml:featureMember>
```
   
</td>
</tr>
<tr>
<td>Transformed instance in default encoding:</td>
<td>

```xml
	<gml:featureMember>
		<au:AdministrativeUnit_1stOrder>
			<au:nationalLevel xlink:href="http://inspire.ec.europa.eu/codelist/AdministrativeHierarchyLevel/1stOrder"/>
			<!-- ... -->
		</au:AdministrativeUnit_1stOrder>
	</gml:featureMember>
	<gml:featureMember>
		<au:AdministrativeUnit_2ndOrder>
			<au:nationalLevel xlink:href="http://inspire.ec.europa.eu/codelist/AdministrativeHierarchyLevel/2ndOrder"/>
			<!-- ... -->
		</au:AdministrativeUnit_2ndOrder>
	</gml:featureMember>
	<gml:featureMember>
		<au:AdministrativeUnit_3rdOrder>
			<au:nationalLevel xlink:href="http://inspire.ec.europa.eu/codelist/AdministrativeHierarchyLevel/3rdOrder"/>
			<!-- ... -->
		</au:AdministrativeUnit_3rdOrder>
	</gml:featureMember>


``` 

</td>
</tr>
<tr>
<td>Model transformation rule: </td>
<td>
    <p>Create a copy of the original feature class for each codelist value. Add the value CodelistValue as a Suffix.</p>
</td>
</tr>
<tr>
<td>Instance transformation rule:</td>
<td>
	<ul>
		<li>Copy the features to a feature class depending on the property that was used for the fan-out.</li>
		</ul>
</td>
</tr>
<tr>
<td>Solves usability issues:</td>
<td>None</td>
</tr>
<tr>
<td>Known usability issues:</td>
<td>Long Codelists can resolve in a big number of extra Feature Classes.</td>
</tr>
<tr>
<td>INSPIRE Compliance:</td>
<td>No issues.</td>
</tr>
</table>

Notes:

 * None.
