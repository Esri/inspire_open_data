## General Flattening

<table>
<tr>
<td>Category</td>
<td>General model simplification rules</td>
</tr>
<tr>
<td>Description</td>
<td><p>The complex structure of model elements can be reduced by applying a flattening method. The principle of the flattening is to derive a flat model structure by moving the nested child elements to its parent. The elements can be renamed to represent the former element path in the name of the resulting element and to avoid naming conflicts. The cardinality of the derived elements should be calculated from the cardinalities of the former element path. When applied recursively, this method flattens the structure of multiple levels.</p> 
<p>When applied recursively, this method flattens the structure of multiple levels and will result in properties such as these:</p>
<ul>
    <li>inspireId_namespace</li>
    <li>name_spelling_text</li>
</ul>
<p>This model transformation rule does not handle cardinalities greater than 1; it thus does not introduce any numeric elements into the new property name to account for multiple occurences. It also does not make use of the element names as they would be encoded in XML to keep the resulting proeprty names shorter. In most cases outside the use of substitution groups, this does not lead to issues. These should be resolved using any of the three Transformation Rules that can deal with that ([Primitive Array](./ExtractPrimitiveArray.md), [Associations to Soft Typed properties](./AssociatedComponentsSoftType.md), [Associations to Hard Typed properties](./AssociatedComponentsHardType.md)).</p>
</td>
</tr>
<tr>
<td>Original instance in default encoding:</td>
<td>

```xml
<am:ManagementRestrictionOrRegulationZone>
  <!-- ... -->
  <am:legalBasis>
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
<ams:ManagementRestrictionOrRegulationZone>
  <!-- ... -->
  <ams:legalBasis.name>Bekendtgørelse af lov om skove</ams:legalBasis.name>
  <ams:legalBasis.shortName>LBK nr 122 af 26/01/2017</ams:legalBasis.shortName>
  <ams:legalBasis.date.date>2017-01-26</ams:legalBasis.date.date>
  <ams:legalBasis.date.dateType.codeListValue>creation</ams:legalBasis.date.dateType.codeListValue>
  <ams:legalBasis.date.dateType.codeList>http://standards.iso.org/ittf/PubliclyAvailableStandards/ISO_19139_Schemas/resources/codelist/ML_gmxCodelists.xml#CI_DateTypeCode</ams:legalBasis.date.dateType.codeList>
  <ams:legalBasis.link>http://www.retsinformation.dk/eli/lta/2017/122</ams:legalBasis.link>
  <ams:legalBasis.linklevel>national</ams:legalBasis.linklevel>
  <ams:legalBasis.linklevel.href>http://inspire.ec.europa.eu/codelist/LegislationLevelValue/national</ams:legalBasis.linklevel.href>
  <!-- ... -->
</ams:ManagementRestrictionOrRegulationZone>
``` 

</td>
</tr>
<tr>
<td>Model transformation rule: </td>
<td>
    <p>Parameters:</p> 
    <ul>
        <li><code>separator</code>: The character to use to separate the original property name from the type name of the components.</li>
    </ul>
    <p>Recursively go down through the complex structure of the property and concatenate the local name of the property, using the <code>separator</code> character in between each local name. This rule will drop inherited properties that have the same local name as a property declared on the feature type or property type itself, e.g. <code>gml:name</code> vs. <code>gn:name</code>. Note that Geometry properties are excluded from this rule!</p>
</td>
</tr>
<tr>
<td>Instance transformation rule:</td>
<td><p>Parameters: None</p>
    <p>As described above, this rule does not handle property occurences greater than 1; if more than one instance of a property occur, only the first instance will be kept.</p>
    </td>
</tr>
<tr>
<td>Solves usability issues:</td>
<td>This rule deals with most nested property structures and flattens them, so that the data can be used easily in analysis and visualisation.</td>
</tr>
<tr>
<td>Known usability issues:</td>
<td>This rule has no fixed limit in the character length of the resulting property names. Some of these names can get very long. The rule should thus be combined with others that reduce the likelyhood of that happening, such as [SimpleGeographicName](./SimpleGeographicName.html).</td>
</tr>
<tr>
<td>INSPIRE Compliance:</td>
<td>Data transformed using this rule is INSPIRE compliant as long as the cardinality of the source data was 0..1 for all affected properties.</td>
</tr>
</table>

Notes: No notes.
