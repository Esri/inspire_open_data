## MT010: Simplified PT_FreeText

<table>
<tr>
<td>Category</td>
<td>Alternate Structures for specific types or type hierarchies</td>
</tr>
<tr>
<td>Description</td>
<td><p><code>PT_FreeText</code> is used to provide textual information in different locales using textGroups. These text groups use LocalisedCharacterString to provide information in different languages. The number of text groups is not limited by the data model. This creates a complex structure that is in many cases not necessary making it harder to create and to process.</p> 
<p>This ruel proposes a simplified alternative representation:</p>
</td>
</tr>
<tr>
<td>Original instance in default encoding:</td>
<td>

```xml
<us-emf:EnvironmentalManagementFacility gml:id="id153d54f4-076e-4166-a30c-78e29f2f23ec">
			<!-- ... -->
      <us-emf:facilityDescription>
        <gmd:PT_FreeText>
					<gmd:textGroup>
						  <gmd:LocalisedCharacterString locale="de_DE">Beschreibung der Aktivität</gmd:LocalisedCharacterString>
					</gmd:textGroup>
					<gmd:textGroup>
						  <gmd:LocalisedCharacterString locale="en_EN">Desccription of activity</gmd:LocalisedCharacterString>
					</gmd:textGroup>
				</gmd:PT_FreeText>
      </us-emf:facilityDescription>
		<!-- ... -->
</us-emf:EnvironmentalManagementFacility>

```
   
</td>
</tr>
<tr>
<td>Transformed instance in default encoding:</td>
<td>

```xml
<us-emfs:EnvironmentalManagementFacility gml:id="id153d54f4-076e-4166-a30c-78e29f2f23ec">
			<!-- ... -->
      <us-emfs:facilityDescription>
      	  <gmd:LocalisedCharacterString locale="de_DE">Beschreibung der Aktivität</gmd:LocalisedCharacterString>
				  <gmd:LocalisedCharacterString locale="en_EN">Desccription of activity</gmd:LocalisedCharacterString>
      </us-emfs:facilityDescription>
		<!-- ... -->
</us-emfs:EnvironmentalManagementFacility>
``` 

</td>
</tr>
<tr>
<td>Model transformation rule: </td>
<td>
    <p>Substitute existing <code>PT_FreeText</code> types with this SimplePT_FreeText type.</p>
</td>
</tr>
<tr>
<td>Instance transformation rule:</td>
<td>
	<ul>
		<li>Copy the value of <code>gmd:LocalisedCharacterString</code> to the property <code>gmd:LocalisedCharacterString</code>.</li>
		<li>Copy the value of <code>gmd:LocalisedCharacterString.locale</code> to the property <code>gmd:LocalisedCharacterString.locale</code>.</li>
	</ul>
</td>
</tr>
<tr>
<td>Solves usability issues:</td>
<td>The transformed data structure can easily be edited, filtered and symbolized in desktop GIS and web GIS software.</td>
</tr>
<tr>
<td>Known usability issues:</td>
<td>None.</td>
</tr>
<tr>
<td>INSPIRE Compliance:</td>
<td>Fully compliant.</td>
</tr>
</table>

Notes:

 * None.
