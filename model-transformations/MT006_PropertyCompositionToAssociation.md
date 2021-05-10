## MT006: Restriction of property encoding options to only by-reference

<table>
<tr>
<td>Category</td>
<td>General model simplification rules</td>
</tr>
<tr>
<td>Description</td>
<td><p>Information regarding certain types of resources is typically accessible through an external register or non-INSPIRE online application. Those resources should be referred to "by reference".</p>
</td>
</tr>
<tr>
<td>Original instance in default encoding:</td>
<td>
<p>Possibility 1: inline</p>

```xml
<am:ManagementRestrictionOrRegulationZone>
  <!-- ... -->
  <am:legalBasis>
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
  </am:legalBasis>
  <!-- ... -->
</am:ManagementRestrictionOrRegulationZone>
```

<p>Possibility 2: by reference</p>

```xml
<am:ManagementRestrictionOrRegulationZone>
  <!-- ... -->
  <am:legalBasis
    xlink:href="http://example.dk/path/to/specific/law/resource"
    xlink:title="Bekendtgørelse af lov om skove" />
  <!-- ... -->
</am:ManagementRestrictionOrRegulationZone>
```

<p>Possibility 3: by reference and inline. From the GML standard:</p>

<blockquote>If both a link and content are present in an instance of a property element, then the object found by traversing the xlink:href link shall be the normative value of the property. The object included as content shall be used by the data recipient only if the remote instance cannot be resolved; this may be considered to be a "cached" version of the object.</blockquote>

```xml
<am:ManagementRestrictionOrRegulationZone>
  <!-- ... -->
  <am:legalBasis
    xlink:href="http://example.dk/path/to/specific/law/resource"
    xlink:title="Bekendtgørelse af lov om skove">
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
  <ams:legalBasis
    xlink:href="http://example.dk/path/to/specific/law/resource"
    xlink:title="Bekendtgørelse af lov om skove"
  />
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
        <li><code>referenceProperty</code>: The name of the property which to change to a reference.</li>
    </ul>
    <p>On the model level, this changes the tagged value <code>inlineOrByReference</code> to have the value <code>byReference</code> on the property.</p>
</td>
</tr>
<tr>
<td>Instance transformation rule:</td>
<td><p>Parameters: None</p>
    <p>It is only possible to convert an instance using the "inline" pattern when a URL to the related resource is present in the original data or can be added upon transformation from the original data to the INSPIRE data. This URL must be inserted in <code>@xlink:href</code>.</p>
    <p>A name or title (e.g. "Bekendtgørelse af lov om skove"), or even a full-blown bibliographic reference in the case of objects that are information resources (e.g. "Bekendtgørelse af lov om skove. 28 marts 2019. LBK nr 315."), if present, may be inserted in <code>@xlink:title</code>.</p>
    </td>
</tr>
<tr>
<td>Solves usability issues:</td>
<td>This rule reduces nested structures (inline referencing causes nested structures with many levels). It also reduces implementation effort of and duplication of data by data providers, if the value of the property is a resource managed by another data provider.</td>
</tr>
<tr>
<td>Known usability issues:</td>
<td>Display of <code>@xlink:href</code> and <code>@xlink:title</code> may not be supported in all clients. However, this is the same problem as for code lists, which are widely used in INSPIRE.</td>
</tr>
<tr>
<td>INSPIRE Compliance:</td>
<td>Fully compliant if the referenced resource is stored in an external register or non-INSPIRE online application.</td>
</tr>
</table>

Notes: No notes.
