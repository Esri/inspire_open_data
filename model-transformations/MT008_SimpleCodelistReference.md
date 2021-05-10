## MT008: Simplified Codelist Reference

<table>
<tr>
<td>Category</td>
<td>Alternate Structures for specific types or type hierarchies</td>
</tr>
<tr>
<td>Description</td>
<td><p>References to codelists are one of the ubiquitous characteristics of the INSPIRE data specifications. They are usually encoded using a <code>ReferenceType, which is derived from an <code>xlink</code>. In the conceptual model, they are represented using property types that point to classes with a <code>&lt;&lt;Codelist&gt;&gt;</code> stereotype.</p> 
<p>The main usability issue with ReferenceTypes is that they encode all relevant information in the xlink attributes of the element. In particular, the actual external link is encoded in the <code>xlink:href</code> attribute, while additional informaiton may be encoded in attributes such as <code>xlink:title</code>. An additional issue is that the actual, full codelist URLs are unwieldy to use for styling and filtering in most GIS. It would be much preferable to use the local codelist values. There is a recommendation to encode these using the mentioned <code>xlink:title</code>, but no strict requirement.</p>
<p>This simplified codelist reference takes the property name and uses it to encode the title directly, while all othe properties are modelled as "subproperties":</p>
<ul>
    <li><code>reference</code></li>
	  <li><code>reference.href</code></li>
</ul>
<p>Both of these properties are mandatory in the <code>SimpleCitation</code>, while extra properties such as <code>arcRole</code>, <code>owns</code> and <code>type</code> are optional..</p>
</td>
</tr>
<tr>
<td>Original instance in default encoding:</td>
<td>

```xml
<ad:Address gml:id="MIG20172_example_Address">
  <!-- ... -->
  <ad:status
    xlink:href="http://inspire.ec.europa.eu/codelist/StatusValue/current"
    xlink:title="current" />
  <!-- ... -->
</ad:Address>
```
   
</td>
</tr>
<tr>
<td>Transformed instance in default encoding:</td>
<td>

```xml
<ads:Address gml:id="MIG20172_example_Address">
  <!-- ... -->
  <simple:status>current</ads:status>
  <simple:status.href>http://inspire.ec.europa.eu/codelist/StatusValue/current</ads:status.href>
  <!-- ... -->
</ads:Address>
``` 

</td>
</tr>
<tr>
<td>Model transformation rule: </td>
<td>
    <p>Parameters:</p> 
    <ul>
      <li><code>type</code>: The property for which the ReferenceType is to be substituted, e.g. <code>status</code>.</li>
    </ul>
    <p>Substitute existing <code>ReferenceType</code> on the <code>type</code> property with this SimpleReference type.</p>
</td>
</tr>
<tr>
<td>Instance transformation rule:</td>
<td>
	<ul>
		<li>Copy the value of the <code>xlink:title</code> attribute to the property with the name of the <code>type</code> parameter.</li>
		<li>Copy the value of the <code>xlink:href</code> attribute to the property with the name of the <code>type.href</code> parameter.</li>
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
