## European Legislation Identifier

<table>
<tr>
<td>Category</td>
<td>Alternative structures for specific types or type hierarchies</td>
</tr>
<tr>
<td>Description</td>
<td>
<p>This model transformation replaces the LegislationCitation class from the Base Types 2 application schema by a class having the semantics of the LegalResource class as defined in the [European Legislation Identifier ontology](https://publications.europa.eu/en/web/eu-vocabularies/model/-/resource/dataset/eli).</p>
<p>This model transformation is intended to be used together with (TODO link to "Restriction of property encoding options to only by-reference") and followed by an encoding defined by the [European Legislation Identifier specification](https://publications.europa.eu/en/web/eu-vocabularies/model/-/resource/dataset/eli).</p>
</td>
</tr>
<tr>
<td>Original instance in default encoding:</td>
<td>

```xml
<base2:LegislationCitation>
  <base2:name>Bekendtgørelse af lov om skove</base2:name>
  <base2:shortName>LBK nr 315 af 28/03/2019</base2:shortName>
  <base2:date>
	<gmd:CI_Date>
	  <gmd:date>
		<gco:Date>2019-03-30</gco:Date>
	  </gmd:date>
	  <gmd:dateType>
		<gmd:CI_DateTypeCode
		  codeListValue="publication"
		  codeList="http://standards.iso.org/ittf/PubliclyAvailableStandards/ISO_19139_Schemas/resources/codelist/ML_gmxCodelists.xml#CI_DateTypeCode" />
	  </gmd:dateType>
	</gmd:CI_Date>
  </base2:date>
  <base2:link>http://www.retsinformation.dk/eli/lta/2019/315/dan/pdf</base2:link>
  <base2:level
	xlink:href="http://inspire.ec.europa.eu/codelist/LegislationLevelValue/national"
	xlink:title="national" />
</base2:LegislationCitation>
```

</td>
</tr>
<tr>
<td>Transformed instance in default encoding:</td>
<td>
<p>Not applicable: this model transformation must be used together with another encoding rule including a conversion rule that uses an existing schema for encoding the LegalResource class.</p>
</td>
</tr>
<tr>
<td>Transformed instance in RDF encoding:</td>
<td>

```xml
<eli:LegalResource rdf:about="https://www.retsinformation.dk/eli/lta/2019/315">
    <eli:date_publication rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2019-03-30</eli:date_publication>
    <eli:is_realized_by rdf:resource="http://example.dk/path/to/specific/law/dan" />
</eli:LegalResource>
<eli:LegalExpression rdf:about="https://www.retsinformation.dk/eli/lta/2019/315/dan">
    <eli:realizes rdf:resource="https://www.retsinformation.dk/eli/lta/2019/315" />
    <eli:title rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Bekendtgørelse af lov om skove</eli:title>
    <eli:title_short rdf:datatype="http://www.w3.org/2001/XMLSchema#string">LBK nr 315 af 28/03/2019</eli:title_short>
</eli:LegalExpression>
<eli:Format rdf:about="http://www.retsinformation.dk/eli/lta/2019/315/dan/pdf">
    <eli:embodies rdf:resource="http://www.retsinformation.dk/eli/lta/2019/315/dan" />
</eli:Format>
```

</td>
</tr>
<tr>
<td>Model transformation rule: </td>
<td>
    <p>Parameters:</p>
    <ul>
        <li>`separator`: The character to use to separate the original property name from the type name of the components.</li>
    </ul>
    <p>...</p>
</td>
</tr>
<tr>
<td>Instance transformation rule:</td>
<td><p>Parameters:</p>
    <ul>
        <li><code>valueProperty</code>: The name of the property from which to take the value to be copied to the transformed instance.</li>
    </ul>
    <p>...</p>
    </td>
</tr>
<tr>
<td>Solves usability issues:</td>
<td>...</td>
</tr>
<tr>
<td>Known usability issues:</td>
<td>...</td>
</tr>
<tr>
<td>INSPIRE Compliance:</td>
<td>...</td>
</tr>
</table>

Notes: No notes.
