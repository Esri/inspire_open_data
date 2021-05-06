## MT007: Simplified Citation

<table>
<tr>
<td>Category</td>
<td>Alternate Structures for specific types or type hierarchies</td>
</tr>
<tr>
<td>Description</td>
<td><p>Citations are another element type that is used in many different places throughout the INSPIRE data specifications. ISO 19115 defines <code>CI_Citation</code>, which has a very deep structure that tend to bury key information, creating a lot of overhead. INSPIRE introduced two base types to simplify citations, <code>LegislationCitation</code> and <code>DocumentCitation</code>. However, in many places, <code>CI_Citation</code> is in use. This rule proposes a simplified alternative representation for <code>CI_Citation</code>. For consistency, it can also be used as a substitute to <code>LegislationCitation</code> and <code>DocumentCitation</code> when no external register is available.</p> 
<p>The simplified citation is based on a link to an external publication and adds minimal information with four properties:</p>
<ul>
    <li>citationDate</li>
    <li>citationLink</li>
    <li>citationName</li>
    <li>citationLevel</li>
    <li>citationType</li>
</ul>
<p>Each of these properties maps directly to an existing property of the original citation types. The <code>citationType</code> property can be used to indicate what kind of citation is represented by this object; its values can be taken from the original type name, or can be based on a codelist.</p>
</td>
</tr>
<tr>
<td>Original instance in default encoding:</td>
<td>

```xml
<am:ManagementRestrictionOrRegulationZone>
  <!-- ... -->
  <am:legalBasis
    xlink:href="http://www.retsinformation.dk/eli/lta/2017/122"
    xlink:title="Bekendtgørelse af lov om skove">
    <base2:LegislationCitation>
      <base2:name>Bekendtgørelse af lov om skove</base2:name>
      <base2:shortName>LBK nr 122 af 26/01/2017</base2:shortName>
      <base2:date>
        <gmd:CI_Date>
          <gmd:date>
            <gco:Date>2017-01-26</gco:Date>
          </gmd:date>
          <gmd:dateType>
            <gmd:CI_DateTypeCode
              codeListValue="creation"
              codeList="http://standards.iso.org/ittf/PubliclyAvailableStandards/ISO_19139_Schemas/resources/codelist/ML_gmxCodelists.xml#CI_DateTypeCode" />
          </gmd:dateType>
        </gmd:CI_Date>
      </base2:date>
      <base2:link>http://www.retsinformation.dk/eli/lta/2017/122</base2:link>
      <base2:level xlink:href="http://inspire.ec.europa.eu/codelist/LegislationLevelValue/national" xlink:title="national" />
    </base2:LegislationCitation>
  </am:legalBasis>
  <!-- ... -->
</am:ManagementRestrictionOrRegulationZone>
```
   
</td>
</tr>
<tr>
<td>Transformed instance in default encoding:</td>
<td>

```xml
<ems:EnvironmentalMonitoringFacility>
  <!-- ... -->
  <ems:legalBackground>
    <simple:SimpleCitiation>
      <simple:name>Bekendtgørelse af lov om skove</simple:name>
      <simple:type>LegislationCitation</simple:type>
      <simple:date>2017-01-26</simple:date>
      <simple:link>http://www.retsinformation.dk/eli/lta/2017/122</simple:link>
      <simple:level xlink:href="http://inspire.ec.europa.eu/codelist/LegislationLevelValue/national" xlink:title="national" />
    </simple:SimpleCitation>
  </ems:legalBackground>
  <!-- ... -->
</ems:EnvironmentalMonitoringFacility>
``` 

</td>
</tr>
<tr>
<td>Model transformation rule: </td>
<td>
    <p>Substitute existing <code>LegislationCitation</code> and <code>CI_Citation</code> types with this SimpleCitation type.</p>
</td>
</tr>
<tr>
<td>Instance transformation rule:</td>
<td>
	<ul>
		<li>Copy the value of <code>base2:dateEnteredIntoForce</code> to the property <code>simple:date</code>.</li>
		<li>Copy the value of <code>base2:name</code> to the property <code>simple:name</code>.</li>
		<li>Copy the value of <code>base2:dateEnteredIntoForce</code> to the property <code>simple:date</code>.</li>
		<li>Copy the value(s) of <code>base2:level</code> to the property <code>simple:level</code>. Note that only one link may be present in the data.</li>
		<li>Insert the element name <code>LegislationCitation</code> to the property <code>simple:type</code>.</li>
	</ul>
</td>
</tr>
<tr>
<td>Solves usability issues:</td>
<td>The transformed data structure can easily be edited, filtered and symbolized in desktop GIS and web GIS software. This transformation also reduces data volume.</td>
</tr>
<tr>
<td>Known usability issues:</td>
<td>None.</td>
</tr>
<tr>
<td>INSPIRE Compliance:</td>
<td>This rule works only with one external link, and it removed finer grained information about dates. It can be combined with the [Property Composition to Association](./PropertyCompositiontoAssociation.md) rule to add more information from an external register.</td>
</tr>
</table>

Notes:

 * None.
