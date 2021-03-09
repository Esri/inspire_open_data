## Flatten aggregated or associated components using codelist values

<table>
<tr>
<td>Category</td>
<td>General model simplification rules</td>
</tr>
<tr>
<td>Description</td>
<td><p>Several INSPIRE themes, such as Addresses, use a soft type pattern to add a set of properties to a feature. An example for this is the <code>locator</code> in <code>Address</code> in the Addresses theme. This property has a set of 1..n <code>AddressLocators</code> that together provides a human readable designator or name of the actual address within the scope of the other <code>AddressComponents</code>. Inside the <code>AddressLocators</code>, there are 0..n <code>LocatorDesignator</code> objects. In a simplified model, we want to replace this construct with a set of inlined properties. The individual <code>LocatorDesignator</code> objects have a property that make them unique - the value of the <code>type` of each <code>LocatorDesignator</code>, which comes from the [Locator Designator Type codelist](http://inspire.ec.europa.eu/codelist/LocatorDesignatorTypeValue). We can thus use those codelist values (n.b. without the codelist namespace) to create a new set of properties from the original structures, like so:</p>
<ul>
    <li><code>locator.designator.addressNumber</code></li>
    <li><code>locator.designator.addressNumberExtension</code></li>
    <li><code>locator.designator.entranceDoorIdentifier</code></li>
</ul>
<p>Note that this rule only describes how to deal with components that have a type property or other identifying property. In the example above, the outer structure (the locator property) is also flattened. Furthermore, the instance transformation rule needs to receive a parameter to indicate which (simple) property of the property to use as a value (in the running example, that would be the <code>designator</code> property).</p>
</td>
</tr>
<tr>
<td>Original instance in default encoding:</td>
<td>

```xml
<ad:Address gml:id="MIG20172_example_Address">
	<ad:inspireId>...</ad:inspireId>
	<ad:position>...</ad:position>
	<ad:locator>
		<ad:AddressLocator>
			<ad:designator>
				<ad:LocatorDesignator>
					<ad:designator>99</ad:designator>
					<ad:type xlink:href="http://inspire.ec.europa.eu/codelist/LocatorDesignatorTypeValue/addressNumber">addressNumber</ad:type>
				</ad:LocatorDesignator>
			</ad:designator>
			<ad:level>unitLevel</ad:level>
		</ad:AddressLocator>
	</ad:locator>
	<!-- ... -->
</ad:Address>
```
   
</td>
</tr>
<tr>
<td>Transformed instance in default encoding:</td>
<td>

```xml
<ad:Address gml:id="MIG20172_example_Address">
	<ad:inspireId>...</ad:inspireId>
	<ad:position>...</ad:position>
	<ads:locator_designator_addressNumber>99</ad:locator_designator_addressNumber>
	<!-- ... -->
</ad:Address>
``` 

</td>
</tr>
<tr>
<td>Model transformation rule: </td>
<td>
    <p>Parameters:</p> 
    <ul>
        <li><code>separator</code>: The character to use to separate the original property name from the type name of the components.</li>
		<li><code>keyProperty</code>: The name of the property from whose allowed values (Enumeration or Codelist) to take the new property names.
    </ul>
    <p>Create a new property for every value in an associated code list, using the original property name, the separator, and the name of the element (i.e. without a ...type suffix) to build the new property name.</p>
</td>
</tr>
<tr>
<td>Instance transformation rule:</td>
<td><p>Parameters:</p> 
    <ul>
        <li><code>valueProperty</code>: The name of the property from which to take the value to be copied to the transformed instance.</li>
    </ul>
    <p>Copy the value of the <code>valueProperty</code> to the newly created property. If the <code>valueProperty</code> is still a complex property, it might have to be transformed using a different rule in addition.</p>
    </td>
</tr>
<tr>
<td>Solves usability issues:</td>
<td>The flattened data can be filtered and symbolized easily in desktop GIS and web GIS software. The flattened data can be processed much easier by many tools, e.g. it can be converted to excel easily.</td>
</tr>
<tr>
<td>Known usability issues:</td>
<td>Flattening of large arrays will lead to a very large number of properties on the first level. Some software and formats can only work with a limited number of properties on a layer (ArcMap has 65.534, shapefile is limited to 250), so this can limit usability in extreme cases. Some software also has limits on the length of property names (File Geodatabase = 64 characters, Shapefile = 11 characters).</td>
</tr>
<tr>
<td>INSPIRE Compliance:</td>
<td>This rule can only be applied if there is at maximum one occurence of each codelist value for the type property in a set of properties.</td>
</tr>
</table>
