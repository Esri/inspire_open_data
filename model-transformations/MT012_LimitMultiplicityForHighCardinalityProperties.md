## MT012: Limit number of High Cardinality Objects

<table>
<tr>
<td>Category</td>
<td>Alternate Structures for specific types or type hierarchies</td>
</tr>
<tr>
<td>Description</td>
<td><p>Providing a data structure for high cardinality objects can be solved by creating extra tables. However these extra tables make it sometimes harder to access the information and in almost all cases the multiplicity required to store real data is much lower. In these cases we limit the maximum of a multiplicity to a fixed value. This increases the usability of the data and reduces the number of tables necessary to store the information, while still supporting most real world scenarios.</p> 
</p>
</td>
</tr>
<tr>
<td>Original instance in default encoding:</td>
<td>

```xml
<au:AdministrativeUnit>
<!-- ... -->
  <au:nationalLevelName>
    <gmd:LocalisedCharacterString>Name 1</gmd:LocalisedCharacterString>
  </au:nationalLevelName>
  <au:nationalLevelName>
    <gmd:LocalisedCharacterString>Name 2</gmd:LocalisedCharacterString>
  </au:nationalLevelName>
  <au:nationalLevelName>
    <gmd:LocalisedCharacterString>Name 3</gmd:LocalisedCharacterString>
  </au:nationalLevelName>
<!-- ... -->
</au:AdministrativeUnit>
  
```
   
</td>
</tr>
<tr>
<td>Transformed instance in default encoding:</td>
<td>

```xml
<aus:AdministrativeUnit>
<!-- ... -->
  <au:nationalLevelName_1>
    <gmd:LocalisedCharacterString>Name 1</gmd:LocalisedCharacterString>
  </au:nationalLevelName_1>
  <au:nationalLevelName_2>
    <gmd:LocalisedCharacterString>Name 2</gmd:LocalisedCharacterString>
  </au:nationalLevelName_2>
  <au:nationalLevelName_3>
    <gmd:LocalisedCharacterString>Name 3</gmd:LocalisedCharacterString>
  </au:nationalLevelName_3>
<!-- ... -->
</aus:AdministrativeUnit>


``` 

</td>
</tr>
<tr>
<td>Model transformation rule: </td>
<td>
<p>Parameters:</p> 
    <ul>
        <li><code>number</code>: The number to which this cardinality is limited by the rule</li>
    </ul>
    <p>Depending on the value of number limit a selected property occurence.</p>
</td>
</tr>
<tr>
<td>Instance transformation rule:</td>
<td>
	<ul>
		<li>Copy the value of <code>property</code> to the same property with a number according to its position in the source data.</li>
	</ul>
</td>
</tr>
<tr>
<td>Solves usability issues:</td>
<td>The transformed data structure can easily be read and edited in desktop GIS and web GIS software. This transformation also reduces data volume.</td>
</tr>
<tr>
<td>Known usability issues:</td>
<td>Depending on the number of fields chosen there might be too many or not enough fields in the database.</td>
</tr>
<tr>
<td>INSPIRE Compliance:</td>
<td>If the cardinality of a property in the source data is higher than the number selected for this rule ther might be information loss.</td>
</tr>
</table>

Notes:

 * None.
