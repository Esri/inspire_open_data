
#ProtectedSites


<br/>
<strong>Geodatabase Documentation</strong>
<hr/>
<strong>Date: </strong>20241127102131.6134996<br/>
<hr/>
<p><strong>Summary Information and Links</strong><br/><br/><a href="#FeatureDatasets">0 Feature Datasets and 3
Feature Classes</a><br/>No Topology Datasets<br/>No Geometric Networks<br/>No Rasters<br/><a href="#ObjectClasses">0 Tables (Object Classes)</a><br/><a href="#RelationshipClasses">0 Relationship
Classes</a><br/><a href="#Domains">6 Domains</a><br/></p>
<hr/>
<p><a name="FeatureDatasets"/><strong>Feature Datasets and Child Classes</strong></p><a name="Raster"/>
<p><strong>Rasters</strong></p><br/>
<hr/><a name="ObjectClasses"/>
<p><strong>Workspace-Level Tables and Feature Classes</strong></p>
    <a href="#FeatureClassProtectedSiteL">ProtectedSiteL - FeatureClass</a><br/><a href="#FeatureClassProtectedSiteP">ProtectedSiteP - FeatureClass</a><br/><a href="#FeatureClassProtectedSiteS">ProtectedSiteS - FeatureClass</a><br/>
<p/><br/>
<hr/><a name="RelationshipClasses"/>
<p><strong>Relationship Classes</strong></p><p/>
<hr/><br/><a name="Domains"/>
<p><strong>Domains</strong></p>
   <a href="#DomainDesignationSchemeValue">DesignationSchemeValue</a><br/><a href="#DomainDesignationSchemeValue_value">DesignationSchemeValue_value</a><br/><a href="#DomainDesignationValue">DesignationValue</a><br/><a href="#DomainDesignationValue_value">DesignationValue_value</a><br/><a href="#DomainProtectionClassificationValue">ProtectionClassificationValue</a><br/><a href="#DomainProtectionClassificationValue_value">ProtectionClassificationValue_value</a><br/>
    <p><hr/><br/><a name="FeatureClassProtectedSiteL"/>
<p><strong>ProtectedSiteL - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">ProtectedSiteL</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>ShapeType</strong></td>
<td width="*" style="border-color: white">Polyline</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FeatureType</strong></td>
<td width="*" style="border-color: white">Simple</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">ProtectedSiteL</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>HasM</strong></td>
<td width="*" style="border-color: white">false</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>HasZ</strong></td>
<td width="*" style="border-color: white">false</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>HasAttachments</strong></td>
<td width="*" style="border-color: white">false</td>
</tr>
</tbody>
</table>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Description</strong></td>
<td width="*" style="border-color: white">ProtectedSiteL</td>
</tr>
</tbody>
</table><br/>
<table width="100%">
<tbody>
<tr style="border:0px">
<td width="8%" style="border:0px"><strong>Field</strong></td>
<td width="8%" style="border:0px"><strong>DataType</strong></td>
<td width="5%" style="border:0px"><strong>Length</strong></td>
<td width="8%" style="border:0px"><strong>AliasName</strong></td>
<td width="8%" style="border:0px"><strong>Description</strong></td>
<td width="8%" style="border:0px"><strong>Domain</strong></td>
<td width="8%" style="border:0px"><strong>DefaultValue</strong></td>
<td width="8%" style="border:0px"><strong>IsNullable</strong></td>
<td width="5%" style="border:0px"><strong>Precision</strong></td>
<td width="5%" style="border:0px"><strong>Scale</strong></td>
</tr>
<tr>
<td width="8%">OBJECTID</td>
<td width="8%">OID</td>
<td width="3%">4</td>
<td width="8%">OBJECTID</td>
<td width="8%"/>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">SHAPE</td>
<td width="8%">Geometry</td>
<td width="3%">0</td>
<td width="8%">SHAPE</td>
<td width="8%"/>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_designation</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_designation</td>
<td width="8%">The actual Site designation.</td>
<td width="8%"><a href="#DomainDesignationValue_value">DesignationValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_designation_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_designation_href</td>
<td width="8%">URI from the INSPIRE code list register - DesignationValue <a href="https://inspire.ec.europa.eu/codelist/DesignationValue">https://inspire.ec.europa.eu/codelist/DesignationValue</a></td>
<td width="8%"><a href="#DomainDesignationValue">DesignationValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_designationScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_designationScheme</td>
<td width="8%">The scheme from which the designation code comes.</td>
<td width="8%"><a href="#DomainDesignationSchemeValue_value">DesignationSchemeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_designationScheme_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_designationScheme_href</td>
<td width="8%">URI from the INSPIRE code list register - DesignationSchemeValue <a href="https://inspire.ec.europa.eu/codelist/DesignationSchemeValue">https://inspire.ec.europa.eu/codelist/DesignationSchemeValue</a></td>
<td width="8%"><a href="#DomainDesignationSchemeValue">DesignationSchemeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_legalDoc_citationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">d_1_legalDoc_citationDate</td>
<td width="8%">The date that the protected site was legally created. This is the date that the real world object was created, not the date that its representation in an information system was created.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_legalDoc_citationLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_legalDoc_citationLevel</td>
<td width="8%">Level of the the cited document. Can be a value from https://inspire.ec.europa.eu/codelist/LegislationLevelValue</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_legalDoc_citationLink</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_legalDoc_citationLink</td>
<td width="8%">A URL or text citation referencing the legal act that created the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_legalDoc_citationName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_legalDoc_citationName</td>
<td width="8%">Name of the cited Legal Document</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_legalDoc_citationType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_legalDoc_citationType</td>
<td width="8%">Either DocumentCitation, CI_Citation, or LegislationCitation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_legalFoundationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">d_1_legalFoundationDate</td>
<td width="8%">The date that the protected site was legally created. This is the date that the real world object was created, not the date that its representation in an information system was created.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_percentageUnderDesignation</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_percentageUnderDesignation</td>
<td width="8%">The percentage of the site that falls under the designation. This is used in particular for the IUCN categorisation. If a value is not provided for this attribute, it is assumed to be 100%</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_designation</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_designation</td>
<td width="8%">The actual Site designation.</td>
<td width="8%"><a href="#DomainDesignationValue_value">DesignationValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_designation_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_designation_href</td>
<td width="8%">URI from the INSPIRE code list register - DesignationValue <a href="https://inspire.ec.europa.eu/codelist/DesignationValue">https://inspire.ec.europa.eu/codelist/DesignationValue</a></td>
<td width="8%"><a href="#DomainDesignationValue">DesignationValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_designationScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_designationScheme</td>
<td width="8%">The scheme from which the designation code comes.</td>
<td width="8%"><a href="#DomainDesignationSchemeValue_value">DesignationSchemeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_designationScheme_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_designationScheme_href</td>
<td width="8%">URI from the INSPIRE code list register - DesignationSchemeValue <a href="https://inspire.ec.europa.eu/codelist/DesignationSchemeValue">https://inspire.ec.europa.eu/codelist/DesignationSchemeValue</a></td>
<td width="8%"><a href="#DomainDesignationSchemeValue">DesignationSchemeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_legalDoc_citationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">d_2_legalDoc_citationDate</td>
<td width="8%">Date of the citation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_legalDoc_citationLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_legalDoc_citationLevel</td>
<td width="8%">Level of the the cited document. Can be a value from https://inspire.ec.europa.eu/codelist/LegislationLevelValue</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_legalDoc_citationLink</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_legalDoc_citationLink</td>
<td width="8%">A URL or text citation referencing the legal act that created the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_legalDoc_citationName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_legalDoc_citationName</td>
<td width="8%">Name of the cited Legal Document</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_legalDoc_citationType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_legalDoc_citationType</td>
<td width="8%">Either DocumentCitation, CI_Citation, or LegislationCitation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_legalFoundationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">d_2_legalFoundationDate</td>
<td width="8%">The date that the protected site was legally created. This is the date that the real world object was created, not the date that its representation in an information system was created.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_percentageUnderDesignation</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_percentageUnderDesignation</td>
<td width="8%">The percentage of the site that falls under the designation. This is used in particular for the IUCN categorisation. If a value is not provided for this attribute, it is assumed to be 100%</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">featureId</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">featureId</td>
<td width="8%">Identifier, used in references to this object</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inspireId_localId</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">inspireId_localId</td>
<td width="8%">A local identifier, assigned by the data provider. The local identifier is unique within the namespace, that is no other spatial object carries the same unique identifier.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inspireId_namespace</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">inspireId_namespace</td>
<td width="8%">Namespace uniquely identifying the data source of the spatial object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inspireId_versionId</td>
<td width="8%">String</td>
<td width="3%">25</td>
<td width="8%">inspireId_versionId</td>
<td width="8%">The identifier of the particular version of the spatial object, with a maximum length of 25 characters. If the specification of a spatial object type with an external object identifier includes life-cycle information, the version identifier is used to distinguish between the different versions of a spatial object. Within the set of all versions of a spatial object, the version identifier is unique</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">protectionClass_1</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">protectionClass_1</td>
<td width="8%">The classification of the protected site based on the purpose for protection.</td>
<td width="8%"><a href="#DomainProtectionClassificationValue_value">ProtectionClassificationValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">protectionClass_1_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">protectionClass_1_href</td>
<td width="8%">URI from the INSPIRE code list register - ProtectionClassificationValue <a href="https://inspire.ec.europa.eu/codelist/ProtectionClassificationValue">https://inspire.ec.europa.eu/codelist/ProtectionClassificationValue</a></td>
<td width="8%"><a href="#DomainProtectionClassificationValue">ProtectionClassificationValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">protectionClass_2</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">protectionClass_2</td>
<td width="8%">The classification of the protected site based on the purpose for protection.</td>
<td width="8%"><a href="#DomainProtectionClassificationValue_value">ProtectionClassificationValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">protectionClass_2_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">protectionClass_2_href</td>
<td width="8%">URI from the INSPIRE code list register - ProtectionClassificationValue <a href="https://inspire.ec.europa.eu/codelist/ProtectionClassificationValue">https://inspire.ec.europa.eu/codelist/ProtectionClassificationValue</a></td>
<td width="8%"><a href="#DomainProtectionClassificationValue">ProtectionClassificationValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">protectionClass_3</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">protectionClass_3</td>
<td width="8%">The classification of the protected site based on the purpose for protection.</td>
<td width="8%"><a href="#DomainProtectionClassificationValue_value">ProtectionClassificationValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">protectionClass_3_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">protectionClass_3_href</td>
<td width="8%">URI from the INSPIRE code list register - ProtectionClassificationValue <a href="https://inspire.ec.europa.eu/codelist/ProtectionClassificationValue">https://inspire.ec.europa.eu/codelist/ProtectionClassificationValue</a></td>
<td width="8%"><a href="#DomainProtectionClassificationValue">ProtectionClassificationValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">siteName_name_1</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">siteName_name_1</td>
<td width="8%">The name of the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">siteName_name_1_lang</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">siteName_name_1_lang</td>
<td width="8%">Language of the Name.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">siteName_name_2</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">siteName_name_2</td>
<td width="8%">The name of the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">siteName_name_2_lang</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">siteName_name_2_lang</td>
<td width="8%">Language of the Name.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">siteName_name_3</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">siteName_name_3</td>
<td width="8%">The name of the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">siteName_name_3_lang</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">siteName_name_3_lang</td>
<td width="8%">Language of the Name.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">thematicId_identifier</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">thematicId_identifier</td>
<td width="8%">External object identifier of the spatial object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">thematicId_identifierScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">thematicId_identifierScheme</td>
<td width="8%">Identifier defining the scheme used to assign the identifier.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">SHAPE_Length</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">SHAPE_Length</td>
<td width="8%"/>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p></p><p><hr/><br/><a name="FeatureClassProtectedSiteP"/>
<p><strong>ProtectedSiteP - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">ProtectedSiteP</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>ShapeType</strong></td>
<td width="*" style="border-color: white">Polyline</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FeatureType</strong></td>
<td width="*" style="border-color: white">Simple</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">ProtectedSiteP</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>HasM</strong></td>
<td width="*" style="border-color: white">false</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>HasZ</strong></td>
<td width="*" style="border-color: white">false</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>HasAttachments</strong></td>
<td width="*" style="border-color: white">false</td>
</tr>
</tbody>
</table>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Description</strong></td>
<td width="*" style="border-color: white">ProtectedSiteP</td>
</tr>
</tbody>
</table><br/>
<table width="100%">
<tbody>
<tr style="border:0px">
<td width="8%" style="border:0px"><strong>Field</strong></td>
<td width="8%" style="border:0px"><strong>DataType</strong></td>
<td width="5%" style="border:0px"><strong>Length</strong></td>
<td width="8%" style="border:0px"><strong>AliasName</strong></td>
<td width="8%" style="border:0px"><strong>Description</strong></td>
<td width="8%" style="border:0px"><strong>Domain</strong></td>
<td width="8%" style="border:0px"><strong>DefaultValue</strong></td>
<td width="8%" style="border:0px"><strong>IsNullable</strong></td>
<td width="5%" style="border:0px"><strong>Precision</strong></td>
<td width="5%" style="border:0px"><strong>Scale</strong></td>
</tr>
<tr>
<td width="8%">OBJECTID</td>
<td width="8%">OID</td>
<td width="3%">4</td>
<td width="8%">OBJECTID</td>
<td width="8%"/>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">SHAPE</td>
<td width="8%">Geometry</td>
<td width="3%">0</td>
<td width="8%">SHAPE</td>
<td width="8%"/>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_designation</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_designation</td>
<td width="8%">The actual Site designation.</td>
<td width="8%"><a href="#DomainDesignationValue_value">DesignationValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_designation_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_designation_href</td>
<td width="8%">URI from the INSPIRE code list register - DesignationValue <a href="https://inspire.ec.europa.eu/codelist/DesignationValue">https://inspire.ec.europa.eu/codelist/DesignationValue</a></td>
<td width="8%"><a href="#DomainDesignationValue">DesignationValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_designationScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_designationScheme</td>
<td width="8%">The scheme from which the designation code comes.</td>
<td width="8%"><a href="#DomainDesignationSchemeValue_value">DesignationSchemeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_designationScheme_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_designationScheme_href</td>
<td width="8%">URI from the INSPIRE code list register - DesignationSchemeValue <a href="https://inspire.ec.europa.eu/codelist/DesignationSchemeValue">https://inspire.ec.europa.eu/codelist/DesignationSchemeValue</a></td>
<td width="8%"><a href="#DomainDesignationSchemeValue">DesignationSchemeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_legalDoc_citationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">d_1_legalDoc_citationDate</td>
<td width="8%">The date that the protected site was legally created. This is the date that the real world object was created, not the date that its representation in an information system was created.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_legalDoc_citationLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_legalDoc_citationLevel</td>
<td width="8%">Level of the the cited document. Can be a value from https://inspire.ec.europa.eu/codelist/LegislationLevelValue</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_legalDoc_citationLink</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_legalDoc_citationLink</td>
<td width="8%">A URL or text citation referencing the legal act that created the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_legalDoc_citationName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_legalDoc_citationName</td>
<td width="8%">Name of the cited Legal Document</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_legalDoc_citationType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_legalDoc_citationType</td>
<td width="8%">Either DocumentCitation, CI_Citation, or LegislationCitation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_legalFoundationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">d_1_legalFoundationDate</td>
<td width="8%">The date that the protected site was legally created. This is the date that the real world object was created, not the date that its representation in an information system was created.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_percentageUnderDesignation</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_percentageUnderDesignation</td>
<td width="8%">The percentage of the site that falls under the designation. This is used in particular for the IUCN categorisation. If a value is not provided for this attribute, it is assumed to be 100%</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_designation</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_designation</td>
<td width="8%">The actual Site designation.</td>
<td width="8%"><a href="#DomainDesignationValue_value">DesignationValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_designation_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_designation_href</td>
<td width="8%">URI from the INSPIRE code list register - DesignationValue <a href="https://inspire.ec.europa.eu/codelist/DesignationValue">https://inspire.ec.europa.eu/codelist/DesignationValue</a></td>
<td width="8%"><a href="#DomainDesignationValue">DesignationValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_designationScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_designationScheme</td>
<td width="8%">The scheme from which the designation code comes.</td>
<td width="8%"><a href="#DomainDesignationSchemeValue_value">DesignationSchemeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_designationScheme_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_designationScheme_href</td>
<td width="8%">URI from the INSPIRE code list register - DesignationSchemeValue <a href="https://inspire.ec.europa.eu/codelist/DesignationSchemeValue">https://inspire.ec.europa.eu/codelist/DesignationSchemeValue</a></td>
<td width="8%"><a href="#DomainDesignationSchemeValue">DesignationSchemeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_legalDoc_citationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">d_2_legalDoc_citationDate</td>
<td width="8%">Date of the citation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_legalDoc_citationLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_legalDoc_citationLevel</td>
<td width="8%">Level of the the cited document. Can be a value from https://inspire.ec.europa.eu/codelist/LegislationLevelValue</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_legalDoc_citationLink</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_legalDoc_citationLink</td>
<td width="8%">A URL or text citation referencing the legal act that created the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_legalDoc_citationName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_legalDoc_citationName</td>
<td width="8%">Name of the cited Legal Document</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_legalDoc_citationType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_legalDoc_citationType</td>
<td width="8%">Either DocumentCitation, CI_Citation, or LegislationCitation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_legalFoundationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">d_2_legalFoundationDate</td>
<td width="8%">The date that the protected site was legally created. This is the date that the real world object was created, not the date that its representation in an information system was created.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_percentageUnderDesignation</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_percentageUnderDesignation</td>
<td width="8%">The percentage of the site that falls under the designation. This is used in particular for the IUCN categorisation. If a value is not provided for this attribute, it is assumed to be 100%</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">featureId</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">featureId</td>
<td width="8%">Identifier, used in references to this object</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inspireId_localId</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">inspireId_localId</td>
<td width="8%">A local identifier, assigned by the data provider. The local identifier is unique within the namespace, that is no other spatial object carries the same unique identifier.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inspireId_namespace</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">inspireId_namespace</td>
<td width="8%">Namespace uniquely identifying the data source of the spatial object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inspireId_versionId</td>
<td width="8%">String</td>
<td width="3%">25</td>
<td width="8%">inspireId_versionId</td>
<td width="8%">The identifier of the particular version of the spatial object, with a maximum length of 25 characters. If the specification of a spatial object type with an external object identifier includes life-cycle information, the version identifier is used to distinguish between the different versions of a spatial object. Within the set of all versions of a spatial object, the version identifier is unique</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">protectionClass_1</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">protectionClass_1</td>
<td width="8%">The classification of the protected site based on the purpose for protection.</td>
<td width="8%"><a href="#DomainProtectionClassificationValue_value">ProtectionClassificationValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">protectionClass_1_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">protectionClass_1_href</td>
<td width="8%">URI from the INSPIRE code list register - ProtectionClassificationValue <a href="https://inspire.ec.europa.eu/codelist/ProtectionClassificationValue">https://inspire.ec.europa.eu/codelist/ProtectionClassificationValue</a></td>
<td width="8%"><a href="#DomainProtectionClassificationValue">ProtectionClassificationValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">protectionClass_2</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">protectionClass_2</td>
<td width="8%">The classification of the protected site based on the purpose for protection.</td>
<td width="8%"><a href="#DomainProtectionClassificationValue_value">ProtectionClassificationValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">protectionClass_2_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">protectionClass_2_href</td>
<td width="8%">URI from the INSPIRE code list register - ProtectionClassificationValue <a href="https://inspire.ec.europa.eu/codelist/ProtectionClassificationValue">https://inspire.ec.europa.eu/codelist/ProtectionClassificationValue</a></td>
<td width="8%"><a href="#DomainProtectionClassificationValue">ProtectionClassificationValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">protectionClass_3</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">protectionClass_3</td>
<td width="8%">The classification of the protected site based on the purpose for protection.</td>
<td width="8%"><a href="#DomainProtectionClassificationValue_value">ProtectionClassificationValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">protectionClass_3_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">protectionClass_3_href</td>
<td width="8%">URI from the INSPIRE code list register - ProtectionClassificationValue <a href="https://inspire.ec.europa.eu/codelist/ProtectionClassificationValue">https://inspire.ec.europa.eu/codelist/ProtectionClassificationValue</a></td>
<td width="8%"><a href="#DomainProtectionClassificationValue">ProtectionClassificationValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">siteName_name_1</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">siteName_name_1</td>
<td width="8%">The name of the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">siteName_name_1_lang</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">siteName_name_1_lang</td>
<td width="8%">Language of the Name.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">siteName_name_2</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">siteName_name_2</td>
<td width="8%">The name of the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">siteName_name_2_lang</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">siteName_name_2_lang</td>
<td width="8%">Language of the Name.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">siteName_name_3</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">siteName_name_3</td>
<td width="8%">The name of the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">siteName_name_3_lang</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">siteName_name_3_lang</td>
<td width="8%">Language of the Name.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">thematicId_identifier</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">thematicId_identifier</td>
<td width="8%">External object identifier of the spatial object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">thematicId_identifierScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">thematicId_identifierScheme</td>
<td width="8%">Identifier defining the scheme used to assign the identifier.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p></p><p><hr/><br/><a name="FeatureClassProtectedSiteS"/>
<p><strong>ProtectedSiteS - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">ProtectedSiteS</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>ShapeType</strong></td>
<td width="*" style="border-color: white">Polyline</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FeatureType</strong></td>
<td width="*" style="border-color: white">Simple</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">ProtectedSiteS</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>HasM</strong></td>
<td width="*" style="border-color: white">false</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>HasZ</strong></td>
<td width="*" style="border-color: white">false</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>HasAttachments</strong></td>
<td width="*" style="border-color: white">false</td>
</tr>
</tbody>
</table>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Description</strong></td>
<td width="*" style="border-color: white">ProtectedSiteS</td>
</tr>
</tbody>
</table><br/>
<table width="100%">
<tbody>
<tr style="border:0px">
<td width="8%" style="border:0px"><strong>Field</strong></td>
<td width="8%" style="border:0px"><strong>DataType</strong></td>
<td width="5%" style="border:0px"><strong>Length</strong></td>
<td width="8%" style="border:0px"><strong>AliasName</strong></td>
<td width="8%" style="border:0px"><strong>Description</strong></td>
<td width="8%" style="border:0px"><strong>Domain</strong></td>
<td width="8%" style="border:0px"><strong>DefaultValue</strong></td>
<td width="8%" style="border:0px"><strong>IsNullable</strong></td>
<td width="5%" style="border:0px"><strong>Precision</strong></td>
<td width="5%" style="border:0px"><strong>Scale</strong></td>
</tr>
<tr>
<td width="8%">OBJECTID</td>
<td width="8%">OID</td>
<td width="3%">4</td>
<td width="8%">OBJECTID</td>
<td width="8%"/>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">SHAPE</td>
<td width="8%">Geometry</td>
<td width="3%">0</td>
<td width="8%">SHAPE</td>
<td width="8%"/>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_designation</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_designation</td>
<td width="8%">The actual Site designation.</td>
<td width="8%"><a href="#DomainDesignationValue_value">DesignationValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_designation_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_designation_href</td>
<td width="8%">URI from the INSPIRE code list register - DesignationValue <a href="https://inspire.ec.europa.eu/codelist/DesignationValue">https://inspire.ec.europa.eu/codelist/DesignationValue</a></td>
<td width="8%"><a href="#DomainDesignationValue">DesignationValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_designationScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_designationScheme</td>
<td width="8%">The scheme from which the designation code comes.</td>
<td width="8%"><a href="#DomainDesignationSchemeValue_value">DesignationSchemeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_designationScheme_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_designationScheme_href</td>
<td width="8%">URI from the INSPIRE code list register - DesignationSchemeValue <a href="https://inspire.ec.europa.eu/codelist/DesignationSchemeValue">https://inspire.ec.europa.eu/codelist/DesignationSchemeValue</a></td>
<td width="8%"><a href="#DomainDesignationSchemeValue">DesignationSchemeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_legalDoc_citationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">d_1_legalDoc_citationDate</td>
<td width="8%">The date that the protected site was legally created. This is the date that the real world object was created, not the date that its representation in an information system was created.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_legalDoc_citationLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_legalDoc_citationLevel</td>
<td width="8%">Level of the the cited document. Can be a value from https://inspire.ec.europa.eu/codelist/LegislationLevelValue</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_legalDoc_citationLink</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_legalDoc_citationLink</td>
<td width="8%">A URL or text citation referencing the legal act that created the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_legalDoc_citationName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_legalDoc_citationName</td>
<td width="8%">Name of the cited Legal Document</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_legalDoc_citationType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_legalDoc_citationType</td>
<td width="8%">Either DocumentCitation, CI_Citation, or LegislationCitation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_legalFoundationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">d_1_legalFoundationDate</td>
<td width="8%">The date that the protected site was legally created. This is the date that the real world object was created, not the date that its representation in an information system was created.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_1_percentageUnderDesignation</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_1_percentageUnderDesignation</td>
<td width="8%">The percentage of the site that falls under the designation. This is used in particular for the IUCN categorisation. If a value is not provided for this attribute, it is assumed to be 100%</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_designation</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_designation</td>
<td width="8%">The actual Site designation.</td>
<td width="8%"><a href="#DomainDesignationValue_value">DesignationValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_designation_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_designation_href</td>
<td width="8%">URI from the INSPIRE code list register - DesignationValue <a href="https://inspire.ec.europa.eu/codelist/DesignationValue">https://inspire.ec.europa.eu/codelist/DesignationValue</a></td>
<td width="8%"><a href="#DomainDesignationValue">DesignationValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_designationScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_designationScheme</td>
<td width="8%">The scheme from which the designation code comes.</td>
<td width="8%"><a href="#DomainDesignationSchemeValue_value">DesignationSchemeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_designationScheme_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_designationScheme_href</td>
<td width="8%">URI from the INSPIRE code list register - DesignationSchemeValue <a href="https://inspire.ec.europa.eu/codelist/DesignationSchemeValue">https://inspire.ec.europa.eu/codelist/DesignationSchemeValue</a></td>
<td width="8%"><a href="#DomainDesignationSchemeValue">DesignationSchemeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_legalDoc_citationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">d_2_legalDoc_citationDate</td>
<td width="8%">Date of the citation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_legalDoc_citationLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_legalDoc_citationLevel</td>
<td width="8%">Level of the the cited document. Can be a value from https://inspire.ec.europa.eu/codelist/LegislationLevelValue</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_legalDoc_citationLink</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_legalDoc_citationLink</td>
<td width="8%">A URL or text citation referencing the legal act that created the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_legalDoc_citationName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_legalDoc_citationName</td>
<td width="8%">Name of the cited Legal Document</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_legalDoc_citationType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_legalDoc_citationType</td>
<td width="8%">Either DocumentCitation, CI_Citation, or LegislationCitation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_legalFoundationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">d_2_legalFoundationDate</td>
<td width="8%">The date that the protected site was legally created. This is the date that the real world object was created, not the date that its representation in an information system was created.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">d_2_percentageUnderDesignation</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">d_2_percentageUnderDesignation</td>
<td width="8%">The percentage of the site that falls under the designation. This is used in particular for the IUCN categorisation. If a value is not provided for this attribute, it is assumed to be 100%</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">featureId</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">featureId</td>
<td width="8%">Identifier, used in references to this object</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inspireId_localId</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">inspireId_localId</td>
<td width="8%">A local identifier, assigned by the data provider. The local identifier is unique within the namespace, that is no other spatial object carries the same unique identifier.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inspireId_namespace</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">inspireId_namespace</td>
<td width="8%">Namespace uniquely identifying the data source of the spatial object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inspireId_versionId</td>
<td width="8%">String</td>
<td width="3%">25</td>
<td width="8%">inspireId_versionId</td>
<td width="8%">The identifier of the particular version of the spatial object, with a maximum length of 25 characters. If the specification of a spatial object type with an external object identifier includes life-cycle information, the version identifier is used to distinguish between the different versions of a spatial object. Within the set of all versions of a spatial object, the version identifier is unique</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">protectionClass_1</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">protectionClass_1</td>
<td width="8%">The classification of the protected site based on the purpose for protection.</td>
<td width="8%"><a href="#DomainProtectionClassificationValue_value">ProtectionClassificationValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">protectionClass_1_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">protectionClass_1_href</td>
<td width="8%">URI from the INSPIRE code list register - ProtectionClassificationValue <a href="https://inspire.ec.europa.eu/codelist/ProtectionClassificationValue">https://inspire.ec.europa.eu/codelist/ProtectionClassificationValue</a></td>
<td width="8%"><a href="#DomainProtectionClassificationValue">ProtectionClassificationValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">protectionClass_2</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">protectionClass_2</td>
<td width="8%">The classification of the protected site based on the purpose for protection.</td>
<td width="8%"><a href="#DomainProtectionClassificationValue_value">ProtectionClassificationValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">protectionClass_2_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">protectionClass_2_href</td>
<td width="8%">URI from the INSPIRE code list register - ProtectionClassificationValue <a href="https://inspire.ec.europa.eu/codelist/ProtectionClassificationValue">https://inspire.ec.europa.eu/codelist/ProtectionClassificationValue</a></td>
<td width="8%"><a href="#DomainProtectionClassificationValue">ProtectionClassificationValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">protectionClass_3</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">protectionClass_3</td>
<td width="8%">The classification of the protected site based on the purpose for protection.</td>
<td width="8%"><a href="#DomainProtectionClassificationValue_value">ProtectionClassificationValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">protectionClass_3_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">protectionClass_3_href</td>
<td width="8%">URI from the INSPIRE code list register - ProtectionClassificationValue <a href="https://inspire.ec.europa.eu/codelist/ProtectionClassificationValue">https://inspire.ec.europa.eu/codelist/ProtectionClassificationValue</a></td>
<td width="8%"><a href="#DomainProtectionClassificationValue">ProtectionClassificationValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">siteName_name_1</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">siteName_name_1</td>
<td width="8%">The name of the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">siteName_name_1_lang</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">siteName_name_1_lang</td>
<td width="8%">Language of the Name.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">siteName_name_2</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">siteName_name_2</td>
<td width="8%">The name of the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">siteName_name_2_lang</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">siteName_name_2_lang</td>
<td width="8%">Language of the Name.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">siteName_name_3</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">siteName_name_3</td>
<td width="8%">The name of the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">siteName_name_3_lang</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">siteName_name_3_lang</td>
<td width="8%">Language of the Name.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">thematicId_identifier</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">thematicId_identifier</td>
<td width="8%">External object identifier of the spatial object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">thematicId_identifierScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">thematicId_identifierScheme</td>
<td width="8%">Identifier defining the scheme used to assign the identifier.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">SHAPE_Length</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">SHAPE_Length</td>
<td width="8%"/>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">SHAPE_Area</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">SHAPE_Area</td>
<td width="8%"/>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p></p>
    <p>
    <hr/><a name="DomainDesignationSchemeValue"/>
<p><strong>DesignationSchemeValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">DesignationSchemeValue</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FieldType</strong></td>
<td width="*" style="border-color: white">String</td>
</tr>
<tr>
<td width="20%" style="border-color: white"><strong>Domain Type</strong></td>
<td width="*%" style="border-color: white">CodedValue</td>
</tr>
</tbody>
</table><br/>
<table width="100%">
<tbody>
<tr style="border-width:0px"><strong>
<td width="10%" style="border-width:0px"><strong>Code</strong></td>
</strong>
<td width="20%" style="border-width:0px"><strong>Name</strong></td>
</tr>
<tr>
<tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/DesignationSchemeValue/emeraldNetwork</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/DesignationSchemeValue/emeraldNetwork</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/DesignationSchemeValue/IUCN</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/DesignationSchemeValue/IUCN</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/DesignationSchemeValue/nationalMonumentsRecord</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/DesignationSchemeValue/nationalMonumentsRecord</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/DesignationSchemeValue/natura2000</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/DesignationSchemeValue/natura2000</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/DesignationSchemeValue/ramsar</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/DesignationSchemeValue/ramsar</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/DesignationSchemeValue/UNESCOManAndBiosphereProgramme</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/DesignationSchemeValue/UNESCOManAndBiosphereProgramme</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/DesignationSchemeValue/UNESCOWorldHeritage</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/DesignationSchemeValue/UNESCOWorldHeritage</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainDesignationSchemeValue_value"/>
<p><strong>DesignationSchemeValue_value - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">DesignationSchemeValue_value</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FieldType</strong></td>
<td width="*" style="border-color: white">String</td>
</tr>
<tr>
<td width="20%" style="border-color: white"><strong>Domain Type</strong></td>
<td width="*%" style="border-color: white">CodedValue</td>
</tr>
</tbody>
</table><br/>
<table width="100%">
<tbody>
<tr style="border-width:0px"><strong>
<td width="10%" style="border-width:0px"><strong>Code</strong></td>
</strong>
<td width="20%" style="border-width:0px"><strong>Name</strong></td>
</tr>
<tr>
<tr>
<td width="20%">emeraldNetwork</td>
<td width="20%">emeraldNetwork</td>
</tr><tr>
<td width="20%">IUCN</td>
<td width="20%">IUCN</td>
</tr><tr>
<td width="20%">nationalMonumentsRecord</td>
<td width="20%">nationalMonumentsRecord</td>
</tr><tr>
<td width="20%">natura2000</td>
<td width="20%">natura2000</td>
</tr><tr>
<td width="20%">ramsar</td>
<td width="20%">ramsar</td>
</tr><tr>
<td width="20%">UNESCOManAndBiosphereProgramme</td>
<td width="20%">UNESCOManAndBiosphereProgramme</td>
</tr><tr>
<td width="20%">UNESCOWorldHeritage</td>
<td width="20%">UNESCOWorldHeritage</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainDesignationValue"/>
<p><strong>DesignationValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">DesignationValue</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FieldType</strong></td>
<td width="*" style="border-color: white">String</td>
</tr>
<tr>
<td width="20%" style="border-color: white"><strong>Domain Type</strong></td>
<td width="*%" style="border-color: white">CodedValue</td>
</tr>
</tbody>
</table><br/>
<table width="100%">
<tbody>
<tr style="border-width:0px"><strong>
<td width="10%" style="border-width:0px"><strong>Code</strong></td>
</strong>
<td width="20%" style="border-width:0px"><strong>Name</strong></td>
</tr>
<tr>
<tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/IUCNDesignationValue/habitatSpeciesManagementArea</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/IUCNDesignationValue/habitatSpeciesManagementArea</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/IUCNDesignationValue/managedResourceProtectedArea</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/IUCNDesignationValue/managedResourceProtectedArea</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/IUCNDesignationValue/nationalPark</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/IUCNDesignationValue/nationalPark</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/IUCNDesignationValue/naturalMonument</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/IUCNDesignationValue/naturalMonument</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/IUCNDesignationValue/ProtectedLandscapeOrSeascape</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/IUCNDesignationValue/ProtectedLandscapeOrSeascape</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/IUCNDesignationValue/strictNatureReserve</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/IUCNDesignationValue/strictNatureReserve</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/IUCNDesignationValue/wildernessArea</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/IUCNDesignationValue/wildernessArea</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/IUCNDesignationValue/protectedLandscapeOrSeascape</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/IUCNDesignationValue/protectedLandscapeOrSeascape</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/agricultureAndSubsistence</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/agricultureAndSubsistence</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/civil</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/civil</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/commemorative</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/commemorative</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/commercial</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/commercial</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/communications</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/communications</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/defence</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/defence</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/domestic</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/domestic</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/education</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/education</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/gardensParksAndUrbanSpaces</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/gardensParksAndUrbanSpaces</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/healthAndWelfare</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/healthAndWelfare</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/industrial</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/industrial</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/maritime</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/maritime</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/monument</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/monument</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/recreational</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/recreational</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/religiousRitualAndFunerary</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/religiousRitualAndFunerary</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/settlement</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/settlement</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/transport</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/transport</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/waterSupplyAndDrainage</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NationalMonumentsRecordDesignationValue/waterSupplyAndDrainage</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/Natura2000DesignationValue/proposedSiteOfCommunityImportance</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/Natura2000DesignationValue/proposedSiteOfCommunityImportance</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/Natura2000DesignationValue/proposedSpecialProtectionArea</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/Natura2000DesignationValue/proposedSpecialProtectionArea</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/Natura2000DesignationValue/siteOfCommunityImportance</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/Natura2000DesignationValue/siteOfCommunityImportance</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/Natura2000DesignationValue/specialAreaOfConservation</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/Natura2000DesignationValue/specialAreaOfConservation</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/Natura2000DesignationValue/specialProtectionArea</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/Natura2000DesignationValue/specialProtectionArea</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/RamsarDesignationValue/ramsar</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/RamsarDesignationValue/ramsar</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/UNESCOManAndBiosphereProgrammeDesignationValue/biosphereReserve</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/UNESCOManAndBiosphereProgrammeDesignationValue/biosphereReserve</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/UNESCOWorldHeritageDesignationValue/cultural</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/UNESCOWorldHeritageDesignationValue/cultural</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/UNESCOWorldHeritageDesignationValue/mixed</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/UNESCOWorldHeritageDesignationValue/mixed</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/UNESCOWorldHeritageDesignationValue/natural</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/UNESCOWorldHeritageDesignationValue/natural</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainDesignationValue_value"/>
<p><strong>DesignationValue_value - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">DesignationValue_value</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FieldType</strong></td>
<td width="*" style="border-color: white">String</td>
</tr>
<tr>
<td width="20%" style="border-color: white"><strong>Domain Type</strong></td>
<td width="*%" style="border-color: white">CodedValue</td>
</tr>
</tbody>
</table><br/>
<table width="100%">
<tbody>
<tr style="border-width:0px"><strong>
<td width="10%" style="border-width:0px"><strong>Code</strong></td>
</strong>
<td width="20%" style="border-width:0px"><strong>Name</strong></td>
</tr>
<tr>
<tr>
<td width="20%">habitatSpeciesManagementArea</td>
<td width="20%">habitatSpeciesManagementArea</td>
</tr><tr>
<td width="20%">managedResourceProtectedArea</td>
<td width="20%">managedResourceProtectedArea</td>
</tr><tr>
<td width="20%">nationalPark</td>
<td width="20%">nationalPark</td>
</tr><tr>
<td width="20%">naturalMonument</td>
<td width="20%">naturalMonument</td>
</tr><tr>
<td width="20%">ProtectedLandscapeOrSeascape</td>
<td width="20%">ProtectedLandscapeOrSeascape</td>
</tr><tr>
<td width="20%">strictNatureReserve</td>
<td width="20%">strictNatureReserve</td>
</tr><tr>
<td width="20%">wildernessArea</td>
<td width="20%">wildernessArea</td>
</tr><tr>
<td width="20%">protectedLandscapeOrSeascape</td>
<td width="20%">protectedLandscapeOrSeascape</td>
</tr><tr>
<td width="20%">agricultureAndSubsistence</td>
<td width="20%">agricultureAndSubsistence</td>
</tr><tr>
<td width="20%">civil</td>
<td width="20%">civil</td>
</tr><tr>
<td width="20%">commemorative</td>
<td width="20%">commemorative</td>
</tr><tr>
<td width="20%">commercial</td>
<td width="20%">commercial</td>
</tr><tr>
<td width="20%">communications</td>
<td width="20%">communications</td>
</tr><tr>
<td width="20%">defence</td>
<td width="20%">defence</td>
</tr><tr>
<td width="20%">domestic</td>
<td width="20%">domestic</td>
</tr><tr>
<td width="20%">education</td>
<td width="20%">education</td>
</tr><tr>
<td width="20%">gardensParksAndUrbanSpaces</td>
<td width="20%">gardensParksAndUrbanSpaces</td>
</tr><tr>
<td width="20%">healthAndWelfare</td>
<td width="20%">healthAndWelfare</td>
</tr><tr>
<td width="20%">industrial</td>
<td width="20%">industrial</td>
</tr><tr>
<td width="20%">maritime</td>
<td width="20%">maritime</td>
</tr><tr>
<td width="20%">monument</td>
<td width="20%">monument</td>
</tr><tr>
<td width="20%">recreational</td>
<td width="20%">recreational</td>
</tr><tr>
<td width="20%">religiousRitualAndFunerary</td>
<td width="20%">religiousRitualAndFunerary</td>
</tr><tr>
<td width="20%">settlement</td>
<td width="20%">settlement</td>
</tr><tr>
<td width="20%">transport</td>
<td width="20%">transport</td>
</tr><tr>
<td width="20%">waterSupplyAndDrainage</td>
<td width="20%">waterSupplyAndDrainage</td>
</tr><tr>
<td width="20%">proposedSiteOfCommunityImportance</td>
<td width="20%">proposedSiteOfCommunityImportance</td>
</tr><tr>
<td width="20%">proposedSpecialProtectionArea</td>
<td width="20%">proposedSpecialProtectionArea</td>
</tr><tr>
<td width="20%">siteOfCommunityImportance</td>
<td width="20%">siteOfCommunityImportance</td>
</tr><tr>
<td width="20%">specialAreaOfConservation</td>
<td width="20%">specialAreaOfConservation</td>
</tr><tr>
<td width="20%">specialProtectionArea</td>
<td width="20%">specialProtectionArea</td>
</tr><tr>
<td width="20%">ramsar</td>
<td width="20%">ramsar</td>
</tr><tr>
<td width="20%">biosphereReserve</td>
<td width="20%">biosphereReserve</td>
</tr><tr>
<td width="20%">cultural</td>
<td width="20%">cultural</td>
</tr><tr>
<td width="20%">mixed</td>
<td width="20%">mixed</td>
</tr><tr>
<td width="20%">natural</td>
<td width="20%">natural</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainProtectionClassificationValue"/>
<p><strong>ProtectionClassificationValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">ProtectionClassificationValue</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FieldType</strong></td>
<td width="*" style="border-color: white">String</td>
</tr>
<tr>
<td width="20%" style="border-color: white"><strong>Domain Type</strong></td>
<td width="*%" style="border-color: white">CodedValue</td>
</tr>
</tbody>
</table><br/>
<table width="100%">
<tbody>
<tr style="border-width:0px"><strong>
<td width="10%" style="border-width:0px"><strong>Code</strong></td>
</strong>
<td width="20%" style="border-width:0px"><strong>Name</strong></td>
</tr>
<tr>
<tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ProtectionClassificationValue/archaeological</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ProtectionClassificationValue/archaeological</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ProtectionClassificationValue/ecological</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ProtectionClassificationValue/ecological</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ProtectionClassificationValue/natureConservation</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ProtectionClassificationValue/natureConservation</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ProtectionClassificationValue/landscape</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ProtectionClassificationValue/landscape</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ProtectionClassificationValue/environment</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ProtectionClassificationValue/environment</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ProtectionClassificationValue/geological</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ProtectionClassificationValue/geological</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ProtectionClassificationValue/cultural</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ProtectionClassificationValue/cultural</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainProtectionClassificationValue_value"/>
<p><strong>ProtectionClassificationValue_value - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">ProtectionClassificationValue_value</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FieldType</strong></td>
<td width="*" style="border-color: white">String</td>
</tr>
<tr>
<td width="20%" style="border-color: white"><strong>Domain Type</strong></td>
<td width="*%" style="border-color: white">CodedValue</td>
</tr>
</tbody>
</table><br/>
<table width="100%">
<tbody>
<tr style="border-width:0px"><strong>
<td width="10%" style="border-width:0px"><strong>Code</strong></td>
</strong>
<td width="20%" style="border-width:0px"><strong>Name</strong></td>
</tr>
<tr>
<tr>
<td width="20%">archaeological</td>
<td width="20%">archaeological</td>
</tr><tr>
<td width="20%">ecological</td>
<td width="20%">ecological</td>
</tr><tr>
<td width="20%">natureConservation</td>
<td width="20%">natureConservation</td>
</tr><tr>
<td width="20%">landscape</td>
<td width="20%">landscape</td>
</tr><tr>
<td width="20%">environment</td>
<td width="20%">environment</td>
</tr><tr>
<td width="20%">geological</td>
<td width="20%">geological</td>
</tr><tr>
<td width="20%">cultural</td>
<td width="20%">cultural</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p>