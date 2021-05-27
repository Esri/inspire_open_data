## MT007: Simplified AddressRepresentation

<table>
<tr>
<td>Category</td>
<td>Alternate Structures for specific types or type hierarchies</td>
</tr>
<tr>
<td>Description</td>
<td><p>AddressRepresnetation is used in Contacts are which are an element type that is used in many different places throughout the INSPIRE data specifications. This rule proposes a simplified alternative representation for <code>AddressRepresentation</code>. AddressRepresentation uses a complex and nested structure to provide Address information. In many cases this information is repeaded redundantly many times for a dataset and is very often also present in the metadata. We propose to provide the AddressInformation as a simple string, as this limits overhead and still allows to transport the core information</p> 
</p>
</td>
</tr>
<tr>
<td>Original instance in default encoding:</td>
<td>

```xml
<ad:AddressRepresentation>
  <ad:adminUnit>
    <gn:GeographicalName>
      <gn:language>deu</gn:language>
      <gn:spelling>
        <gn:SpellingOfName>
          <gn:text>Münster</gn:text>
          <gn:script>latn</gn:script>
        </gn:SpellingOfName>
      </gn:spelling>
    </gn:GeographicalName>
  </ad:adminUnit>
  <ad:locatorDesignator>20</ad:locatorDesignator>
  <ad:locatorName>
    <gn:GeographicalName>
      <gn:language>deu</gn:language>
      <gn:spelling>
        <gn:SpellingOfName>
          <gn:text>Hausnummer</gn:text>
        </gn:SpellingOfName>
      </gn:spelling>
    </gn:GeographicalName>
  </ad:locatorName>
  <ad:postCode>48151</ad:postCode>
  <ad:thoroughfare>
    <gn:GeographicalName>
      <gn:language>deu</gn:language>
      <gn:spelling>
        <gn:SpellingOfName>
          <gn:text>Martin-Luther-King-Weg</gn:text>
          <gn:script>latn</gn:script>
        </gn:SpellingOfName>
      </gn:spelling>
    </gn:GeographicalName>
  </ad:thoroughfare>
</ad:AddressRepresentation>
```
   
</td>
</tr>
<tr>
<td>Transformed instance in default encoding:</td>
<td>

```xml
<ads:AddressRepresentation>
  <ad:adminUnit>Münster</ad:adminUnit>
  <ad:locatorDesignator>20</ad:locatorDesignator>
  <ad:locatorName>Hausnummer</ad:locatorName>
  <ad:postCode>48151</ad:postCode>
  <ad:thoroughfare>Martin-Luther-King-Weg</ad:thoroughfare>
</ad:AddressRepresentation>


``` 

</td>
</tr>
<tr>
<td>Model transformation rule: </td>
<td>
    <p>Substitute all existing <code>AddressRepresentation</code> types with this SimpleAddressRepresentation type.</p>
</td>
</tr>
<tr>
<td>Instance transformation rule:</td>
<td>
	<ul>
		<li>Copy the value of <code>ad:thoroughfare.spelling.text</code> to the property <code>simple:AddressRepresentation</code>.</li>
		<li>Concatenate a whitespace and the value of <code>ad:locatorDesignator</code> to the property <code>simple:AddressRepresentation</code>.</li>
        <li>Concatenate a whitespace and the value of <code>ad:postCode</code> to the property <code>simple:AddressRepresentation</code>.</li>
		<li>Concatenate a whitespace and the value of <code>ad:adminUnitName.spelling.text</code> to the property <code>simple:AddressRepresentation</code>.</li>
	</ul>
</td>
</tr>
<tr>
<td>Solves usability issues:</td>
<td>The transformed data structure can easily be read and edited in desktop GIS and web GIS software. This transformation also reduces data volume.</td>
</tr>
<tr>
<td>Known usability issues:</td>
<td>There might be regions where the instance transformation rules need to be adjusted to adopt the natural Address representation in that region.</td>
</tr>
<tr>
<td>INSPIRE Compliance:</td>
<td>This rule discards individual metadata about geographical names, such as the name status and its nativeness. The nature of the transformation which merges information from multiple properties results in a loss of information.</td>
</tr>
</table>

Notes:

 * None.
