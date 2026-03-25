#SampledLandUse

<br/>
<strong>Geodatabase Documentation</strong>
<hr/>
<strong>Date: </strong>20210702115738.4372231<br/>
<hr/>
<p><strong>Summary Information and Links</strong><br/><br/><a href="#FeatureDatasets">0 Feature Datasets and 2
Feature Classes</a><br/>No Topology Datasets<br/>No Geometric Networks<br/>No Rasters<br/><a href="#ObjectClasses">5 Tables (Object Classes)</a><br/><a href="#RelationshipClasses">5 Relationship
Classes</a><br/><a href="#Domains">1 Domains</a><br/></p>
<hr/>
<p><a name="FeatureDatasets"/><strong>Feature Datasets and Child Classes</strong></p><a name="Raster"/>
<p><strong>Rasters</strong></p><br/>
<hr/><a name="ObjectClasses"/>
<p><strong>Workspace-Level Tables and Feature Classes</strong></p>
    <a href="#FeatureClassExistingLandUseSample">ExistingLandUseSample - FeatureClass</a><br/><a href="#TableExistingLandUseSample_hilucsLandUse">ExistingLandUseSample_hilucsLandUse - Table</a><br/><a href="#TableExistingLandUseSample_hilucsPresence">ExistingLandUseSample_hilucsPresence - Table</a><br/><a href="#TableExistingLandUseSample_specificLandUse">ExistingLandUseSample_specificLandUse - Table</a><br/><a href="#TableExistingLandUseSample_specificPresence">ExistingLandUseSample_specificPresence - Table</a><br/><a href="#FeatureClassSampledExistingLandUseDataSet">SampledExistingLandUseDataSet - FeatureClass</a><br/><a href="#TableSampledExistingLandUseDataSet_member">SampledExistingLandUseDataSet_member - Table</a><br/>
<p/><br/>
<hr/><a name="RelationshipClasses"/>
<p><strong>Relationship Classes</strong></p>
    <a href="#RelationshipClassRelELUS_ELUS_hilucsLandUse">RelELUS_ELUS_hilucsLandUse</a><br/><a href="#RelationshipClassRelELUS_ELUS_hilucsPresence">RelELUS_ELUS_hilucsPresence</a><br/><a href="#RelationshipClassRelELUS_ELUS_specificLandUse">RelELUS_ELUS_specificLandUse</a><br/><a href="#RelationshipClassRelELUS_ELUS_specificPresence">RelELUS_ELUS_specificPresence</a><br/><a href="#RelationshipClassRelSELUDS_SELUDS_member">RelSELUDS_SELUDS_member</a><br/>
<p/>
<hr/><br/><a name="Domains"/>
<p><strong>Domains</strong></p>
   <a href="#DomainHILUCSValue">HILUCSValue</a><br/>
    <p><hr/><br/><a name="FeatureClassExistingLandUseSample"/>
<p><strong>ExistingLandUseSample - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">ExistingLandUseSample</td>
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
<td width="*" style="border-color: white">ExistingLandUseSample</td>
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
<td width="*" style="border-color: white">ExistingLandUseSample</td>
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
<td width="8%">beginLifespanVersion</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">beginLifespanVersion</td>
<td width="8%">Date and time at which this version of the spatial object was inserted or changed in the spatial data set.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dataset</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">dataset</td>
<td width="8%">Reference to the featureID of the 'SampledExistingLandUseDataSet' set to which this sample belongs.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">endLifespanVersion</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">endLifespanVersion</td>
<td width="8%">Date and time at which this version of the spatial object was superseded or retired in the spatial data set.</td>
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
<td width="3%">254</td>
<td width="8%">inspireId_versionId</td>
<td width="8%">The identifier of the particular version of the spatial object, with a maximum length of 25 characters. If the specification of a spatial object type with an external object identifier includes life-cycle information, the version identifier is used to distinguish between the different versions of a spatial object. Within the set of all versions of a spatial object, the version identifier is unique</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">observationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">observationDate</td>
<td width="8%">Defines the observation date of the description. It could be the date of an aerial/satellital acquisition or a field survey. The observation date allows the user to have accurate date of when the description was made in the real word. In a database, not all object informations are necessarily captured at the same time.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">validFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">validFrom</td>
<td width="8%">Date and time of which this version of the address component was or will be valid in the real world.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">validTo</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">validTo</td>
<td width="8%">Date and time at which the address component ceased or will cease to exist in the real world.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p></p><p><hr/><br/><a name="FeatureClassSampledExistingLandUseDataSet"/>
<p><strong>SampledExistingLandUseDataSet - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">SampledExistingLandUseDataSet</td>
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
<td width="*" style="border-color: white">SampledExistingLandUseDataSet</td>
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
<td width="*" style="border-color: white">SampledExistingLandUseDataSet</td>
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
<td width="8%">beginLifespanVersion</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">beginLifespanVersion</td>
<td width="8%">Date and time at which this version of the spatial object was inserted or changed in the spatial data set.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">endLifespanVersion</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">endLifespanVersion</td>
<td width="8%">Date and time at which this version of the spatial object was superseded or retired in the spatial data set.</td>
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
<td width="3%">254</td>
<td width="8%">inspireId_versionId</td>
<td width="8%">The identifier of the particular version of the spatial object, with a maximum length of 25 characters. If the specification of a spatial object type with an external object identifier includes life-cycle information, the version identifier is used to distinguish between the different versions of a spatial object. Within the set of all versions of a spatial object, the version identifier is unique</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name</td>
<td width="8%">Human readable name of the data set.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">validFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">validFrom</td>
<td width="8%">Date and time of which this version of the address component was or will be valid in the real world.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">validTo</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">validTo</td>
<td width="8%">Date and time at which the address component ceased or will cease to exist in the real world.</td>
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
<p><hr/><a name="TableExistingLandUseSample_hilucsLandUse"/>
<p><strong>ExistingLandUseSample_hilucsLandUse - Table</strong></p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">ExistingLandUseSample_hilucsLandUse</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">ExistingLandUseSample_hilucsLandUse</td>
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
<td width="*" style="border-color: white">ExistingLandUseSample_hilucsLandUse</td>
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
<td width="8%">hilucsLandUse</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hilucsLandUse</td>
<td width="8%">Land use HILUCS classes that are present in this existing land use sample.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hilucsLandUse_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hilucsLandUse_href</td>
<td width="8%">URI from the INSPIRE code list register - HILUCSValue <a href="https://inspire.ec.europa.eu/codelist/HILUCSValue">https://inspire.ec.europa.eu/codelist/HILUCSValue</a></td>
<td width="8%"><a href="#DomainHILUCSValue">HILUCSValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">RID</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">RID</td>
<td width="8%">Reference to featureId field in parent 'ExistingLandUseSample'.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p><p><hr/><a name="TableExistingLandUseSample_hilucsPresence"/>
<p><strong>ExistingLandUseSample_hilucsPresence - Table</strong></p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">ExistingLandUseSample_hilucsPresence</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">ExistingLandUseSample_hilucsPresence</td>
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
<td width="*" style="border-color: white">ExistingLandUseSample_hilucsPresence</td>
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
<td width="8%">orderedList</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">orderedList</td>
<td width="8%">Land use HILUCS classes that are present in this existing land use sample.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">orderedList_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">orderedList_href</td>
<td width="8%">URI from the INSPIRE code list register - HILUCSValue <a href="https://inspire.ec.europa.eu/codelist/HILUCSValue">https://inspire.ec.europa.eu/codelist/HILUCSValue</a></td>
<td width="8%"><a href="#DomainHILUCSValue">HILUCSValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">percentage_hilucsValue</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">percentage_hilucsValue</td>
<td width="8%">Land use HILUCS classes that are present in this existing land use sample.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">percentage_hilucsValue_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">percentage_hilucsValue_href</td>
<td width="8%">URI from the INSPIRE code list register - HILUCSValue <a href="https://inspire.ec.europa.eu/codelist/HILUCSValue">https://inspire.ec.europa.eu/codelist/HILUCSValue</a></td>
<td width="8%"><a href="#DomainHILUCSValue">HILUCSValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">percentage_percentage</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">percentage_percentage</td>
<td width="8%">Percentage of land use object that is covered by this specific presence.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">RID</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">RID</td>
<td width="8%">Reference to featureId field in parent 'ExistingLandUseSample'.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p><p><hr/><a name="TableExistingLandUseSample_specificLandUse"/>
<p><strong>ExistingLandUseSample_specificLandUse - Table</strong></p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">ExistingLandUseSample_specificLandUse</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">ExistingLandUseSample_specificLandUse</td>
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
<td width="*" style="border-color: white">ExistingLandUseSample_specificLandUse</td>
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
<td width="8%">RID</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">RID</td>
<td width="8%">Reference to featureId field in parent 'ExistingLandUseSample'.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">specificLandUse</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">specificLandUse</td>
<td width="8%">Specific value category for this specific percentage. </td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">specificLandUse_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">specificLandUse_href</td>
<td width="8%">URI from the INSPIRE code list register - LandUseClassificationValue <a href="https://inspire.ec.europa.eu/codelist/LandUseClassificationValue">https://inspire.ec.europa.eu/codelist/LandUseClassificationValue</a></td>
<td width="8%"><a href="#DomainLandUseClassificationValue">LandUseClassificationValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p><p><hr/><a name="TableExistingLandUseSample_specificPresence"/>
<p><strong>ExistingLandUseSample_specificPresence - Table</strong></p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">ExistingLandUseSample_specificPresence</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">ExistingLandUseSample_specificPresence</td>
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
<td width="*" style="border-color: white">ExistingLandUseSample_specificPresence</td>
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
<td width="8%">orderedList</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">orderedList</td>
<td width="8%">Presence of one or several land use classification values in an area according to the code list.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">orderedList_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">orderedList_href</td>
<td width="8%">URI from the INSPIRE code list register - LandUseClassificationValue <a href="https://inspire.ec.europa.eu/codelist/LandUseClassificationValue">https://inspire.ec.europa.eu/codelist/LandUseClassificationValue</a></td>
<td width="8%"><a href="#DomainLandUseClassificationValue">LandUseClassificationValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">percentage_specificPercentage</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">percentage_specificPercentage</td>
<td width="8%">Percentage of land use object that is covered by a specific presence.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">percentage_specificValue</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">percentage_specificValue</td>
<td width="8%">Presence of one or several land use classification values in an area according to the code list.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">percentage_specificValue_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">percentage_specificValue_href</td>
<td width="8%">URI from the INSPIRE code list register - LandUseClassificationValue <a href="https://inspire.ec.europa.eu/codelist/LandUseClassificationValue">https://inspire.ec.europa.eu/codelist/LandUseClassificationValue</a></td>
<td width="8%"><a href="#DomainLandUseClassificationValue">LandUseClassificationValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">RID</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">RID</td>
<td width="8%">Reference to featureId field in parent 'ExistingLandUseSample'.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p><p><hr/><a name="TableSampledExistingLandUseDataSet_member"/>
<p><strong>SampledExistingLandUseDataSet_member - Table</strong></p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">SampledExistingLandUseDataSet_member</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">SampledExistingLandUseDataSet_member</td>
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
<td width="*" style="border-color: white">SampledExistingLandUseDataSet_member</td>
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
<td width="8%">member</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">member</td>
<td width="8%">Reference to the featureId of the  members (ExistingLandUseSample) of the sampled existing land use data set.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">RID</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">RID</td>
<td width="8%">Reference to featureId field in parent 'SampledExistingLandUseDataSet'.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p>
    <p><hr/><a name="RelationshipClassRelELUS_ELUS_hilucsLandUse"/>
<p><strong>RelELUS_ELUS_hilucsLandUse - RelationshipClass</strong></p>
<table width="100%">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">RelELUS_ELUS_hilucsLandUse</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>Cardinality</strong></td>
<td width="*" style="border-color: white">OneToMany</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>IsAttributed</strong></td>
<td width="*" style="border-color: white">False</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>IsComposite</strong></td>
<td width="*" style="border-color: white">False</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>ForwardPathLabel</strong></td>
<td width="*" style="border-color: white">ExistingLandUseSample_hilucsLandUse</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>BackwardPathLabel</strong></td>
<td width="*" style="border-color: white">ExistingLandUseSample</td>
</tr>
</tbody>
</table>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Description</strong></td>
<td width="*" style="border-color: white">RelELUS_ELUS_hilucsLandUse</td>
</tr>
</tbody>
</table>
<table width="50%">
<tbody>
<tr style="border:0px">
<td width="30%" style="border:0px"><strong>Origin Class Name</strong></td>
<td width="30%" style="border:0px"><strong>Origin Primary Key</strong></td>
<td width="30%" style="border:0px"><strong>Origin Foreign Key</strong></td>
</tr><br/>
<tr>
<td width="30%">ExistingLandUseSample</td>
<td width="30%">featureId</td>
<td width="30%">RID</td>
</tr>
</tbody>
</table><br/>
<table width="50%">
<tbody>
<tr style="border:0px">
<td width="30%" style="border:0px"><strong>Destination Class Name</strong></td>
<td width="30%" style="border:0px"><strong>Destination Primary Key</strong></td>
<td width="30%" style="border:0px"><strong>Destination Foreign Key</strong></td>
</tr>
<tr>
<td width="30%">ExistingLandUseSample_hilucsLandUse</td>
<td width="30%"/>
<td width="30%"/>
</tr>
</tbody>
</table></p><p><hr/><a name="RelationshipClassRelELUS_ELUS_hilucsPresence"/>
<p><strong>RelELUS_ELUS_hilucsPresence - RelationshipClass</strong></p>
<table width="100%">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">RelELUS_ELUS_hilucsPresence</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>Cardinality</strong></td>
<td width="*" style="border-color: white">OneToMany</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>IsAttributed</strong></td>
<td width="*" style="border-color: white">False</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>IsComposite</strong></td>
<td width="*" style="border-color: white">False</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>ForwardPathLabel</strong></td>
<td width="*" style="border-color: white">ExistingLandUseSample_hilucsPresence</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>BackwardPathLabel</strong></td>
<td width="*" style="border-color: white">ExistingLandUseSample</td>
</tr>
</tbody>
</table>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Description</strong></td>
<td width="*" style="border-color: white">RelELUS_ELUS_hilucsPresence</td>
</tr>
</tbody>
</table>
<table width="50%">
<tbody>
<tr style="border:0px">
<td width="30%" style="border:0px"><strong>Origin Class Name</strong></td>
<td width="30%" style="border:0px"><strong>Origin Primary Key</strong></td>
<td width="30%" style="border:0px"><strong>Origin Foreign Key</strong></td>
</tr><br/>
<tr>
<td width="30%">ExistingLandUseSample</td>
<td width="30%">featureId</td>
<td width="30%">RID</td>
</tr>
</tbody>
</table><br/>
<table width="50%">
<tbody>
<tr style="border:0px">
<td width="30%" style="border:0px"><strong>Destination Class Name</strong></td>
<td width="30%" style="border:0px"><strong>Destination Primary Key</strong></td>
<td width="30%" style="border:0px"><strong>Destination Foreign Key</strong></td>
</tr>
<tr>
<td width="30%">ExistingLandUseSample_hilucsPresence</td>
<td width="30%"/>
<td width="30%"/>
</tr>
</tbody>
</table></p><p><hr/><a name="RelationshipClassRelELUS_ELUS_specificLandUse"/>
<p><strong>RelELUS_ELUS_specificLandUse - RelationshipClass</strong></p>
<table width="100%">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">RelELUS_ELUS_specificLandUse</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>Cardinality</strong></td>
<td width="*" style="border-color: white">OneToMany</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>IsAttributed</strong></td>
<td width="*" style="border-color: white">False</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>IsComposite</strong></td>
<td width="*" style="border-color: white">False</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>ForwardPathLabel</strong></td>
<td width="*" style="border-color: white">ExistingLandUseSample_specificLandUse</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>BackwardPathLabel</strong></td>
<td width="*" style="border-color: white">ExistingLandUseSample</td>
</tr>
</tbody>
</table>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Description</strong></td>
<td width="*" style="border-color: white">RelELUS_ELUS_specificLandUse</td>
</tr>
</tbody>
</table>
<table width="50%">
<tbody>
<tr style="border:0px">
<td width="30%" style="border:0px"><strong>Origin Class Name</strong></td>
<td width="30%" style="border:0px"><strong>Origin Primary Key</strong></td>
<td width="30%" style="border:0px"><strong>Origin Foreign Key</strong></td>
</tr><br/>
<tr>
<td width="30%">ExistingLandUseSample</td>
<td width="30%">featureId</td>
<td width="30%">RID</td>
</tr>
</tbody>
</table><br/>
<table width="50%">
<tbody>
<tr style="border:0px">
<td width="30%" style="border:0px"><strong>Destination Class Name</strong></td>
<td width="30%" style="border:0px"><strong>Destination Primary Key</strong></td>
<td width="30%" style="border:0px"><strong>Destination Foreign Key</strong></td>
</tr>
<tr>
<td width="30%">ExistingLandUseSample_specificLandUse</td>
<td width="30%"/>
<td width="30%"/>
</tr>
</tbody>
</table></p><p><hr/><a name="RelationshipClassRelELUS_ELUS_specificPresence"/>
<p><strong>RelELUS_ELUS_specificPresence - RelationshipClass</strong></p>
<table width="100%">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">RelELUS_ELUS_specificPresence</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>Cardinality</strong></td>
<td width="*" style="border-color: white">OneToMany</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>IsAttributed</strong></td>
<td width="*" style="border-color: white">False</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>IsComposite</strong></td>
<td width="*" style="border-color: white">False</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>ForwardPathLabel</strong></td>
<td width="*" style="border-color: white">ExistingLandUseSample_specificPresence</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>BackwardPathLabel</strong></td>
<td width="*" style="border-color: white">ExistingLandUseSample</td>
</tr>
</tbody>
</table>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Description</strong></td>
<td width="*" style="border-color: white">RelELUS_ELUS_specificPresence</td>
</tr>
</tbody>
</table>
<table width="50%">
<tbody>
<tr style="border:0px">
<td width="30%" style="border:0px"><strong>Origin Class Name</strong></td>
<td width="30%" style="border:0px"><strong>Origin Primary Key</strong></td>
<td width="30%" style="border:0px"><strong>Origin Foreign Key</strong></td>
</tr><br/>
<tr>
<td width="30%">ExistingLandUseSample</td>
<td width="30%">featureId</td>
<td width="30%">RID</td>
</tr>
</tbody>
</table><br/>
<table width="50%">
<tbody>
<tr style="border:0px">
<td width="30%" style="border:0px"><strong>Destination Class Name</strong></td>
<td width="30%" style="border:0px"><strong>Destination Primary Key</strong></td>
<td width="30%" style="border:0px"><strong>Destination Foreign Key</strong></td>
</tr>
<tr>
<td width="30%">ExistingLandUseSample_specificPresence</td>
<td width="30%"/>
<td width="30%"/>
</tr>
</tbody>
</table></p><p><hr/><a name="RelationshipClassRelSELUDS_SELUDS_member"/>
<p><strong>RelSELUDS_SELUDS_member - RelationshipClass</strong></p>
<table width="100%">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">RelSELUDS_SELUDS_member</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>Cardinality</strong></td>
<td width="*" style="border-color: white">OneToMany</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>IsAttributed</strong></td>
<td width="*" style="border-color: white">False</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>IsComposite</strong></td>
<td width="*" style="border-color: white">False</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>ForwardPathLabel</strong></td>
<td width="*" style="border-color: white">SampledExistingLandUseDataSet_member</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>BackwardPathLabel</strong></td>
<td width="*" style="border-color: white">SampledExistingLandUseDataSet</td>
</tr>
</tbody>
</table>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Description</strong></td>
<td width="*" style="border-color: white">RelSELUDS_SELUDS_member</td>
</tr>
</tbody>
</table>
<table width="50%">
<tbody>
<tr style="border:0px">
<td width="30%" style="border:0px"><strong>Origin Class Name</strong></td>
<td width="30%" style="border:0px"><strong>Origin Primary Key</strong></td>
<td width="30%" style="border:0px"><strong>Origin Foreign Key</strong></td>
</tr><br/>
<tr>
<td width="30%">SampledExistingLandUseDataSet</td>
<td width="30%">featureId</td>
<td width="30%">RID</td>
</tr>
</tbody>
</table><br/>
<table width="50%">
<tbody>
<tr style="border:0px">
<td width="30%" style="border:0px"><strong>Destination Class Name</strong></td>
<td width="30%" style="border:0px"><strong>Destination Primary Key</strong></td>
<td width="30%" style="border:0px"><strong>Destination Foreign Key</strong></td>
</tr>
<tr>
<td width="30%">SampledExistingLandUseDataSet_member</td>
<td width="30%"/>
<td width="30%"/>
</tr>
</tbody>
</table></p>
    <p>
    <hr/><a name="DomainHILUCSValue"/>
<p><strong>HILUCSValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">HILUCSValue</td>
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
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_PrimaryProduction</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_PrimaryProduction</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_1_Agriculture</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_1_Agriculture</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_1_1_CommercialAgriculturalProduction</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_1_1_CommercialAgriculturalProduction</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_1_2_FarmingInfrastructure</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_1_2_FarmingInfrastructure</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_1_3_AgriculturalProductionForOwnConsumption</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_1_3_AgriculturalProductionForOwnConsumption</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_2_Forestry</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_2_Forestry</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_2_1_ForestryBasedOnShortRotation</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_2_1_ForestryBasedOnShortRotation</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_2_2_ForestryBasedOnIntermediateOrLongRotation</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_2_2_ForestryBasedOnIntermediateOrLongRotation</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_2_3_ForestryBasedOnContinuousCover</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_2_3_ForestryBasedOnContinuousCover</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_3_MiningAndQuarrying</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_3_MiningAndQuarrying</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_3_1_MiningOfEnergyProducingMaterials</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_3_1_MiningOfEnergyProducingMaterials</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_3_2_MiningOfMetalOres</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_3_2_MiningOfMetalOres</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_3_3_OtherMiningAndQuarrying</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_3_3_OtherMiningAndQuarrying</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_4_AquacultureAndFishing</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_4_AquacultureAndFishing</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_4_1_Aquaculture</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_4_1_Aquaculture</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_4_2_ProfessionalFishing</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_4_2_ProfessionalFishing</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_5_OtherPrimaryProduction</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_5_OtherPrimaryProduction</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_5_1_Hunting</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_5_1_Hunting</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_5_2_ManagementOfMigratoryAnimals</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_5_2_ManagementOfMigratoryAnimals</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_5_3_PickingOfNaturalProducts</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/1_5_3_PickingOfNaturalProducts</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_SecondaryProduction</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_SecondaryProduction</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_RawIndustry</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_RawIndustry</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_1_ManufacturingOfTextileProducts</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_1_ManufacturingOfTextileProducts</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_2_ManufacturingOfWoodAndWoodBasedProducts</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_2_ManufacturingOfWoodAndWoodBasedProducts</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_3_ManufacturingOfPulpPaperAndPaperProducts</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_3_ManufacturingOfPulpPaperAndPaperProducts</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_4_ManufacturingOfCokeRefinedPetroleumProductsAndNuclearFuel</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_4_ManufacturingOfCokeRefinedPetroleumProductsAndNuclearFuel</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_5_ManufacturingOfChemicalsChemicalProductsManMadeFibers</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_5_ManufacturingOfChemicalsChemicalProductsManMadeFibers</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_6_ManufacturingOfBasicMetalsAndFabricatedMetals</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_6_ManufacturingOfBasicMetalsAndFabricatedMetals</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_7_ManufacturingOfNonMetallicMineralProducts</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_7_ManufacturingOfNonMetallicMineralProducts</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_8_ManufacturingOfRubberPlasticProducts</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_8_ManufacturingOfRubberPlasticProducts</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_9_ManufacturingOfOtherRawMaterials</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_1_9_ManufacturingOfOtherRawMaterials</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_2_HeavyEndProductIndustry</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_2_HeavyEndProductIndustry</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_2_1_ManufacturingOfMachinery</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_2_1_ManufacturingOfMachinery</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_2_2_ManufacturingOfVehiclesAndTransportEquipment</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_2_2_ManufacturingOfVehiclesAndTransportEquipment</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_2_3_ManufacturingOfOtherHeavyEndProducts</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_2_3_ManufacturingOfOtherHeavyEndProducts</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_3_LightEndProductIndustry</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_3_LightEndProductIndustry</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_3_1_ManufacturingOfFoodBeveragesAndTobaccoProducts</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_3_1_ManufacturingOfFoodBeveragesAndTobaccoProducts</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_3_2_ManufacturingOfClothesAndLeather</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_3_2_ManufacturingOfClothesAndLeather</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_3_3_PublishingAndPrinting</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_3_3_PublishingAndPrinting</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_3_4_ManufacturingOfElectricalAndOpticalEquipment</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_3_4_ManufacturingOfElectricalAndOpticalEquipment</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_3_5_ManufacturingOfOtherLightEndProducts</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_3_5_ManufacturingOfOtherLightEndProducts</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_4_EnergyProduction</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_4_EnergyProduction</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_4_1_NuclearBasedEnergyProduction</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_4_1_NuclearBasedEnergyProduction</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_4_2_FossilFuelBasedEnergyProduction</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_4_2_FossilFuelBasedEnergyProduction</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_4_3_BiomassBasedEnergyProduction</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_4_3_BiomassBasedEnergyProduction</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_4_4_RenewableEnergyProduction</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_4_4_RenewableEnergyProduction</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_5_OtherIndustry</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/2_5_OtherIndustry</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_TertiaryProduction</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_TertiaryProduction</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_1_CommercialServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_1_CommercialServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_1_1_WholesaleAndRetailTradeAndRepairOfVehiclesAndPersonalAndHouseholdGoods</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_1_1_WholesaleAndRetailTradeAndRepairOfVehiclesAndPersonalAndHouseholdGoods</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_1_2_RealEstateServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_1_2_RealEstateServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_1_3_AccommodationAndFoodServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_1_3_AccommodationAndFoodServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_1_4_OtherCommercialServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_1_4_OtherCommercialServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_2_FinancialProfessionalAndInformationServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_2_FinancialProfessionalAndInformationServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_2_1_FinancialAndInsuranceServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_2_1_FinancialAndInsuranceServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_2_2_ProfessionalTechnicalAndScientificServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_2_2_ProfessionalTechnicalAndScientificServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_2_3_InformationAndCommunicationServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_2_3_InformationAndCommunicationServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_2_4_AdministrativeAndSupportServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_2_4_AdministrativeAndSupportServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_2_5_OtherFinancialProfessionalAndInformationServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_2_5_OtherFinancialProfessionalAndInformationServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_3_CommunityServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_3_CommunityServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_3_1_PublicAdministrationDefenceAndSocialSecurityServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_3_1_PublicAdministrationDefenceAndSocialSecurityServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_3_2_EducationalServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_3_2_EducationalServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_3_3_HealthAndSocialServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_3_3_HealthAndSocialServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_3_4_ReligiousServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_3_4_ReligiousServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_3_5_OtherCommunityServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_3_5_OtherCommunityServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_4_CulturalEntertainmentAndRecreationalServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_4_CulturalEntertainmentAndRecreationalServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_4_1_CulturalServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_4_1_CulturalServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_4_2_EntertainmentServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_4_2_EntertainmentServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_4_3_SportsInfrastructure</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_4_3_SportsInfrastructure</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_4_4_OpenAirRecreationalAreas</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_4_4_OpenAirRecreationalAreas</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_4_5_OtherRecreationalServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_4_5_OtherRecreationalServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_5_OtherServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/3_5_OtherServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_TransportNetworksLogisticsAndUtilities</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_TransportNetworksLogisticsAndUtilities</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_1_TransportNetworks</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_1_TransportNetworks</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_1_1_RoadTransport</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_1_1_RoadTransport</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_1_2_RailwayTransport</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_1_2_RailwayTransport</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_1_3_AirTransport</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_1_3_AirTransport</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_1_4_WaterTransport</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_1_4_WaterTransport</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_1_5_OtherTransportNetwork</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_1_5_OtherTransportNetwork</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_2_LogisticalAndStorageServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_2_LogisticalAndStorageServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_3_Utilities</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_3_Utilities</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_3_1_ElectricityGasAndThermalPowerDistributionServices</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_3_1_ElectricityGasAndThermalPowerDistributionServices</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_3_2_WaterAndSewageInfrastructure</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_3_2_WaterAndSewageInfrastructure</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_3_3_WasteTreatment</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_3_3_WasteTreatment</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_3_4_OtherUtilities</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/4_3_4_OtherUtilities</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/5_ResidentialUse</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/5_ResidentialUse</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/5_1_PermanentResidentialUse</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/5_1_PermanentResidentialUse</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/5_2_ResidentialUseWithOtherCompatibleUses</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/5_2_ResidentialUseWithOtherCompatibleUses</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/5_3_OtherResidentialUse</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/5_3_OtherResidentialUse</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/6_OtherUses</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/6_OtherUses</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/6_1_TransitionalAreas</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/6_1_TransitionalAreas</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/6_2_AbandonedAreas</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/6_2_AbandonedAreas</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/6_3_NaturalAreasNotInOtherEconomicUse</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/6_3_NaturalAreasNotInOtherEconomicUse</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/6_3_1_LandAreasNotInOtherEconomicUse</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/6_3_1_LandAreasNotInOtherEconomicUse</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/6_3_2_WaterAreasNotInOtherEconomicUse</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/6_3_2_WaterAreasNotInOtherEconomicUse</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/6_4_AreasWhereAnyUseAllowed</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/6_4_AreasWhereAnyUseAllowed</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/6_5_AreasWithoutAnySpecifiedPlannedUse</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/6_5_AreasWithoutAnySpecifiedPlannedUse</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/6_6_NotKnownUse</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/HILUCSValue/6_6_NotKnownUse</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p>
