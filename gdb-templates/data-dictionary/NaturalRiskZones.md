
#NaturalRiskZones


<br/>
<strong>Geodatabase Documentation</strong>
<hr/>
<strong>Date: </strong>20241127102130.1204706<br/>
<hr/>
<p><strong>Summary Information and Links</strong><br/><br/><a href="#FeatureDatasets">0 Feature Datasets and 8
Feature Classes</a><br/>No Topology Datasets<br/>No Geometric Networks<br/>No Rasters<br/><a href="#ObjectClasses">2 Tables (Object Classes)</a><br/><a href="#RelationshipClasses">2 Relationship
Classes</a><br/><a href="#Domains">6 Domains</a><br/></p>
<hr/>
<p><a name="FeatureDatasets"/><strong>Feature Datasets and Child Classes</strong></p><a name="Raster"/>
<p><strong>Rasters</strong></p><br/>
<hr/><a name="ObjectClasses"/>
<p><strong>Workspace-Level Tables and Feature Classes</strong></p>
    <a href="#FeatureClassExposedElementL">ExposedElementL - FeatureClass</a><br/><a href="#FeatureClassExposedElementP">ExposedElementP - FeatureClass</a><br/><a href="#FeatureClassExposedElementS">ExposedElementS - FeatureClass</a><br/><a href="#FeatureClassHazardArea">HazardArea - FeatureClass</a><br/><a href="#TableHazardArea_source">HazardArea_source - Table</a><br/><a href="#FeatureClassObservedEventL">ObservedEventL - FeatureClass</a><br/><a href="#FeatureClassObservedEventP">ObservedEventP - FeatureClass</a><br/><a href="#FeatureClassObservedEventS">ObservedEventS - FeatureClass</a><br/><a href="#FeatureClassRiskZone">RiskZone - FeatureClass</a><br/><a href="#TableRiskZone_exposedElement">RiskZone_exposedElement - Table</a><br/>
<p/><br/>
<hr/><a name="RelationshipClasses"/>
<p><strong>Relationship Classes</strong></p>
    <a href="#RelationshipClassRelHA_HA_source">RelHA_HA_source</a><br/><a href="#RelationshipClassRelRZ_RZ_exposedElement">RelRZ_RZ_exposedElement</a><br/>
<p/>
<hr/><br/><a name="Domains"/>
<p><strong>Domains</strong></p>
   <a href="#DomainDeterminationMethodValue">DeterminationMethodValue</a><br/><a href="#DomainDeterminationMethodValue_value">DeterminationMethodValue_value</a><br/><a href="#DomainExposedElementCategoryValue">ExposedElementCategoryValue</a><br/><a href="#DomainExposedElementCategoryValue_value">ExposedElementCategoryValue_value</a><br/><a href="#DomainNaturalHazardCategoryValue">NaturalHazardCategoryValue</a><br/><a href="#DomainNaturalHazardCategoryValue_value">NaturalHazardCategoryValue_value</a><br/>
    <p><hr/><br/><a name="FeatureClassExposedElementL"/>
<p><strong>ExposedElementL - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">ExposedElementL</td>
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
<td width="*" style="border-color: white">ExposedElementL</td>
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
<td width="*" style="border-color: white">ExposedElementL</td>
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
<td width="8%">aOV_elementCategory</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_elementCategory</td>
<td width="8%">A generic classification of the types of elements that are exposed to a risk.</td>
<td width="8%"><a href="#DomainExposedElementCategoryValue_value">ExposedElementCategoryValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_elementCategory_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_elementCategory_href</td>
<td width="8%">URI from the INSPIRE code list register - ExposedElementCategoryValue <a href="https://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue">https://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue</a></td>
<td width="8%"><a href="#DomainExposedElementCategoryValue">ExposedElementCategoryValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_mOIHazard_citationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">aOV_mOIHazard_citationDate</td>
<td width="8%">Date of the citation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_mOIHazard_citationLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_mOIHazard_citationLevel</td>
<td width="8%">Level of the the cited document. Can be a value from https://inspire.ec.europa.eu/codelist/LegislationLevelValue</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_mOIHazard_citationLink</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_mOIHazard_citationLink</td>
<td width="8%">A URL or text citation referencing the legal act that created the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_mOIHazard_citationName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_mOIHazard_citationName</td>
<td width="8%">Name of the cited Legal Document</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_mOIHazard_citationType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_mOIHazard_citationType</td>
<td width="8%">Either DocumentCitation, CI_Citation, or LegislationCitation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_specificElementType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_specificElementType</td>
<td width="8%">An additional denomination of exposed element according to a nomenclature that is specific to this dataset.</td>
<td width="8%"><a href="#DomainSpecificExposedElementTypeValue_value">SpecificExposedElementTypeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_specificElementType_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_specificElementType_href</td>
<td width="8%">URI from the INSPIRE code list register - SpecificExposedElementTypeValue <a href="https://inspire.ec.europa.eu/codelist/SpecificExposedElementTypeValue">https://inspire.ec.europa.eu/codelist/SpecificExposedElementTypeValue</a></td>
<td width="8%"><a href="#DomainSpecificExposedElementTypeValue">SpecificExposedElementTypeValue</a></td>
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
<td width="8%">validFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">validFrom</td>
<td width="8%">The time when the exposed element started to exist in the real world.</td>
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
<td width="8%">The time from which the exposed element no longer exists in the real world.</td>
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
</p></p><p><hr/><br/><a name="FeatureClassExposedElementP"/>
<p><strong>ExposedElementP - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">ExposedElementP</td>
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
<td width="*" style="border-color: white">ExposedElementP</td>
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
<td width="*" style="border-color: white">ExposedElementP</td>
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
<td width="8%">aOV_elementCategory</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_elementCategory</td>
<td width="8%">A generic classification of the types of elements that are exposed to a risk.</td>
<td width="8%"><a href="#DomainExposedElementCategoryValue_value">ExposedElementCategoryValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_elementCategory_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_elementCategory_href</td>
<td width="8%">URI from the INSPIRE code list register - ExposedElementCategoryValue <a href="https://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue">https://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue</a></td>
<td width="8%"><a href="#DomainExposedElementCategoryValue">ExposedElementCategoryValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_mOIHazard_citationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">aOV_mOIHazard_citationDate</td>
<td width="8%">Date of the citation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_mOIHazard_citationLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_mOIHazard_citationLevel</td>
<td width="8%">Level of the the cited document. Can be a value from https://inspire.ec.europa.eu/codelist/LegislationLevelValue</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_mOIHazard_citationLink</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_mOIHazard_citationLink</td>
<td width="8%">A URL or text citation referencing the legal act that created the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_mOIHazard_citationName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_mOIHazard_citationName</td>
<td width="8%">Name of the cited Legal Document</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_mOIHazard_citationType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_mOIHazard_citationType</td>
<td width="8%">Either DocumentCitation, CI_Citation, or LegislationCitation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_specificElementType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_specificElementType</td>
<td width="8%">An additional denomination of exposed element according to a nomenclature that is specific to this dataset.</td>
<td width="8%"><a href="#DomainSpecificExposedElementTypeValue_value">SpecificExposedElementTypeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_specificElementType_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_specificElementType_href</td>
<td width="8%">URI from the INSPIRE code list register - SpecificExposedElementTypeValue <a href="https://inspire.ec.europa.eu/codelist/SpecificExposedElementTypeValue">https://inspire.ec.europa.eu/codelist/SpecificExposedElementTypeValue</a></td>
<td width="8%"><a href="#DomainSpecificExposedElementTypeValue">SpecificExposedElementTypeValue</a></td>
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
<td width="8%">validFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">validFrom</td>
<td width="8%">The time when the exposed element started to exist in the real world.</td>
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
<td width="8%">The time from which the exposed element no longer exists in the real world.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p></p><p><hr/><br/><a name="FeatureClassExposedElementS"/>
<p><strong>ExposedElementS - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">ExposedElementS</td>
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
<td width="*" style="border-color: white">ExposedElementS</td>
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
<td width="*" style="border-color: white">ExposedElementS</td>
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
<td width="8%">aOV_elementCategory</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_elementCategory</td>
<td width="8%">A generic classification of the types of elements that are exposed to a risk.</td>
<td width="8%"><a href="#DomainExposedElementCategoryValue_value">ExposedElementCategoryValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_elementCategory_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_elementCategory_href</td>
<td width="8%">URI from the INSPIRE code list register - ExposedElementCategoryValue <a href="https://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue">https://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue</a></td>
<td width="8%"><a href="#DomainExposedElementCategoryValue">ExposedElementCategoryValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_mOIHazard_citationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">aOV_mOIHazard_citationDate</td>
<td width="8%">Date of the citation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_mOIHazard_citationLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_mOIHazard_citationLevel</td>
<td width="8%">Level of the the cited document. Can be a value from https://inspire.ec.europa.eu/codelist/LegislationLevelValue</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_mOIHazard_citationLink</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_mOIHazard_citationLink</td>
<td width="8%">A URL or text citation referencing the legal act that created the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_mOIHazard_citationName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_mOIHazard_citationName</td>
<td width="8%">Name of the cited Legal Document</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_mOIHazard_citationType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_mOIHazard_citationType</td>
<td width="8%">Either DocumentCitation, CI_Citation, or LegislationCitation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_specificElementType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_specificElementType</td>
<td width="8%">An additional denomination of exposed element according to a nomenclature that is specific to this dataset.</td>
<td width="8%"><a href="#DomainSpecificExposedElementTypeValue_value">SpecificExposedElementTypeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">aOV_specificElementType_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">aOV_specificElementType_href</td>
<td width="8%">URI from the INSPIRE code list register - SpecificExposedElementTypeValue <a href="https://inspire.ec.europa.eu/codelist/SpecificExposedElementTypeValue">https://inspire.ec.europa.eu/codelist/SpecificExposedElementTypeValue</a></td>
<td width="8%"><a href="#DomainSpecificExposedElementTypeValue">SpecificExposedElementTypeValue</a></td>
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
<td width="8%">validFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">validFrom</td>
<td width="8%">The time when the exposed element started to exist in the real world.</td>
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
<td width="8%">The time from which the exposed element no longer exists in the real world.</td>
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
</p></p><p><hr/><br/><a name="FeatureClassHazardArea"/>
<p><strong>HazardArea - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">HazardArea</td>
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
<td width="*" style="border-color: white">HazardArea</td>
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
<td width="*" style="border-color: white">HazardArea</td>
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
<td width="8%">determinationMethod</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">determinationMethod</td>
<td width="8%">An enumeration to describe the method used to define the area of hazard or risk.</td>
<td width="8%"><a href="#DomainDeterminationMethodValue_value">DeterminationMethodValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">determinationMethod_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">determinationMethod_href</td>
<td width="8%">URI from the INSPIRE code list register - DeterminationMethodValue <a href="https://inspire.ec.europa.eu/codelist/DeterminationMethodValue">https://inspire.ec.europa.eu/codelist/DeterminationMethodValue</a></td>
<td width="8%"><a href="#DomainDeterminationMethodValue">DeterminationMethodValue</a></td>
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
<td width="8%">lOO_method_citationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">lOO_method_citationDate</td>
<td width="8%">Date of the citation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">lOO_method_citationLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">lOO_method_citationLevel</td>
<td width="8%">Level of the the cited document. Can be a value from https://inspire.ec.europa.eu/codelist/LegislationLevelValue</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">lOO_method_citationLink</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">lOO_method_citationLink</td>
<td width="8%">A URL or text citation referencing the legal act that created the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">lOO_method_citationName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">lOO_method_citationName</td>
<td width="8%">Name of the cited Legal Document</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">lOO_method_citationType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">lOO_method_citationType</td>
<td width="8%">Either DocumentCitation, CI_Citation, or LegislationCitation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">lOO_qualitativeLikelihood</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">lOO_qualitativeLikelihood</td>
<td width="8%">A qualitative assessment of the likelihood of occurrence of a hazard.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">lOO_quantitative_probability</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">lOO_quantitative_probability</td>
<td width="8%">The probability of occurrence of a hazard event, expressed as a value between 0 and 1.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">lOO_quantitative_retPeriod</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">lOO_quantitative_retPeriod</td>
<td width="8%">Long-term average interval of time or number of years within which an event will be equalled or exceeded [UNESCO].</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_method_citationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">mOI_method_citationDate</td>
<td width="8%">Date of the citation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_method_citationLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_method_citationLevel</td>
<td width="8%">Level of the the cited document. Can be a value from https://inspire.ec.europa.eu/codelist/LegislationLevelValue</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_method_citationLink</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_method_citationLink</td>
<td width="8%">A URL or text citation referencing the legal act that created the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_method_citationName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_method_citationName</td>
<td width="8%">Name of the cited Legal Document</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_method_citationType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_method_citationType</td>
<td width="8%">Either DocumentCitation, CI_Citation, or LegislationCitation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_qualitativeValue</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_qualitativeValue</td>
<td width="8%">A qualitative assessment of the level or intensity.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_quantitativeValue</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">mOI_quantitativeValue</td>
<td width="8%">A quantitative assessment of the level or intensity.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_quantitativeValue_uom</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_quantitativeValue_uom</td>
<td width="8%">Unit of Measure for the quantitative assessment value.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">tOH_hazardCategory</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">tOH_hazardCategory</td>
<td width="8%">A generic classification of types of natural hazards or risks.</td>
<td width="8%"><a href="#DomainNaturalHazardCategoryValue_value">NaturalHazardCategoryValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">tOH_hazardCategory_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">tOH_hazardCategory_href</td>
<td width="8%">URI from the INSPIRE code list register - NaturalHazardCategoryValue <a href="https://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue">https://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue</a></td>
<td width="8%"><a href="#DomainNaturalHazardCategoryValue">NaturalHazardCategoryValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">tOH_specificHazardType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">tOH_specificHazardType</td>
<td width="8%">Additional classification of the natural hazard that further specifies the hazard type according to a nomenclature that is specific to this dataset.</td>
<td width="8%"><a href="#DomainSpecificHazardTypeValue_value">SpecificHazardTypeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">tOH_specificHazardType_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">tOH_specificHazardType_href</td>
<td width="8%">URI from the INSPIRE code list register - SpecificHazardTypeValue <a href="https://inspire.ec.europa.eu/codelist/SpecificHazardTypeValue">https://inspire.ec.europa.eu/codelist/SpecificHazardTypeValue</a></td>
<td width="8%"><a href="#DomainSpecificHazardTypeValue">SpecificHazardTypeValue</a></td>
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
</p></p><p><hr/><br/><a name="FeatureClassObservedEventL"/>
<p><strong>ObservedEventL - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">ObservedEventL</td>
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
<td width="*" style="border-color: white">ObservedEventL</td>
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
<td width="*" style="border-color: white">ObservedEventL</td>
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
<td width="8%">mOI_method_citationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">mOI_method_citationDate</td>
<td width="8%">Date of the citation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_method_citationLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_method_citationLevel</td>
<td width="8%">Level of the the cited document. Can be a value from https://inspire.ec.europa.eu/codelist/LegislationLevelValue</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_method_citationLink</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_method_citationLink</td>
<td width="8%">A URL or text citation referencing the legal act that created the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_method_citationName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_method_citationName</td>
<td width="8%">Name of the cited Legal Document</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_method_citationType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_method_citationType</td>
<td width="8%">Either DocumentCitation, CI_Citation, or LegislationCitation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_qualitativeValue</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_qualitativeValue</td>
<td width="8%">A qualitative assessment of the level or intensity.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_quantitativeValue</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">mOI_quantitativeValue</td>
<td width="8%">A quantitative assessment of the level or intensity.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_quantitativeValue_uom</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_quantitativeValue_uom</td>
<td width="8%">Unit of Measure for the quantitative assessment value.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">nameOfEvent</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">nameOfEvent</td>
<td width="8%">common name of the observed event.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">tOH_hazardCategory</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">tOH_hazardCategory</td>
<td width="8%">A generic classification of types of natural hazards or risks.</td>
<td width="8%"><a href="#DomainNaturalHazardCategoryValue_value">NaturalHazardCategoryValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">tOH_hazardCategory_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">tOH_hazardCategory_href</td>
<td width="8%">URI from the INSPIRE code list register - NaturalHazardCategoryValue <a href="https://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue">https://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue</a></td>
<td width="8%"><a href="#DomainNaturalHazardCategoryValue">NaturalHazardCategoryValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">tOH_specificHazardType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">tOH_specificHazardType</td>
<td width="8%">Additional classification of the natural hazard that further specifies the hazard type according to a nomenclature that is specific to this dataset.</td>
<td width="8%"><a href="#DomainSpecificHazardTypeValue_value">SpecificHazardTypeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">tOH_specificHazardType_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">tOH_specificHazardType_href</td>
<td width="8%">URI from the INSPIRE code list register - SpecificHazardTypeValue <a href="https://inspire.ec.europa.eu/codelist/SpecificHazardTypeValue">https://inspire.ec.europa.eu/codelist/SpecificHazardTypeValue</a></td>
<td width="8%"><a href="#DomainSpecificHazardTypeValue">SpecificHazardTypeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">validFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">validFrom</td>
<td width="8%">The time when the exposed element started to exist in the real world.</td>
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
<td width="8%">The time from which the exposed element no longer exists in the real world.</td>
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
</p></p><p><hr/><br/><a name="FeatureClassObservedEventP"/>
<p><strong>ObservedEventP - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">ObservedEventP</td>
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
<td width="*" style="border-color: white">ObservedEventP</td>
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
<td width="*" style="border-color: white">ObservedEventP</td>
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
<td width="8%">mOI_method_citationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">mOI_method_citationDate</td>
<td width="8%">Date of the citation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_method_citationLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_method_citationLevel</td>
<td width="8%">Level of the the cited document. Can be a value from https://inspire.ec.europa.eu/codelist/LegislationLevelValue</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_method_citationLink</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_method_citationLink</td>
<td width="8%">A URL or text citation referencing the legal act that created the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_method_citationName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_method_citationName</td>
<td width="8%">Name of the cited Legal Document</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_method_citationType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_method_citationType</td>
<td width="8%">Either DocumentCitation, CI_Citation, or LegislationCitation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_qualitativeValue</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_qualitativeValue</td>
<td width="8%">A qualitative assessment of the level or intensity.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_quantitativeValue</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">mOI_quantitativeValue</td>
<td width="8%">A quantitative assessment of the level or intensity.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_quantitativeValue_uom</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_quantitativeValue_uom</td>
<td width="8%">Unit of Measure for the quantitative assessment value.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">nameOfEvent</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">nameOfEvent</td>
<td width="8%">common name of the observed event.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">tOH_hazardCategory</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">tOH_hazardCategory</td>
<td width="8%">A generic classification of types of natural hazards or risks.</td>
<td width="8%"><a href="#DomainNaturalHazardCategoryValue_value">NaturalHazardCategoryValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">tOH_hazardCategory_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">tOH_hazardCategory_href</td>
<td width="8%">URI from the INSPIRE code list register - NaturalHazardCategoryValue <a href="https://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue">https://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue</a></td>
<td width="8%"><a href="#DomainNaturalHazardCategoryValue">NaturalHazardCategoryValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">tOH_specificHazardType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">tOH_specificHazardType</td>
<td width="8%">Additional classification of the natural hazard that further specifies the hazard type according to a nomenclature that is specific to this dataset.</td>
<td width="8%"><a href="#DomainSpecificHazardTypeValue_value">SpecificHazardTypeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">tOH_specificHazardType_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">tOH_specificHazardType_href</td>
<td width="8%">URI from the INSPIRE code list register - SpecificHazardTypeValue <a href="https://inspire.ec.europa.eu/codelist/SpecificHazardTypeValue">https://inspire.ec.europa.eu/codelist/SpecificHazardTypeValue</a></td>
<td width="8%"><a href="#DomainSpecificHazardTypeValue">SpecificHazardTypeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">validFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">validFrom</td>
<td width="8%">The time when the exposed element started to exist in the real world.</td>
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
<td width="8%">The time from which the exposed element no longer exists in the real world.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p></p><p><hr/><br/><a name="FeatureClassObservedEventS"/>
<p><strong>ObservedEventS - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">ObservedEventS</td>
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
<td width="*" style="border-color: white">ObservedEventS</td>
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
<td width="*" style="border-color: white">ObservedEventS</td>
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
<td width="8%">mOI_method_citationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">mOI_method_citationDate</td>
<td width="8%">Date of the citation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_method_citationLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_method_citationLevel</td>
<td width="8%">Level of the the cited document. Can be a value from https://inspire.ec.europa.eu/codelist/LegislationLevelValue</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_method_citationLink</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_method_citationLink</td>
<td width="8%">A URL or text citation referencing the legal act that created the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_method_citationName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_method_citationName</td>
<td width="8%">Name of the cited Legal Document</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_method_citationType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_method_citationType</td>
<td width="8%">Either DocumentCitation, CI_Citation, or LegislationCitation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_qualitativeValue</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_qualitativeValue</td>
<td width="8%">A qualitative assessment of the level or intensity.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_quantitativeValue</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">mOI_quantitativeValue</td>
<td width="8%">A quantitative assessment of the level or intensity.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">mOI_quantitativeValue_uom</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">mOI_quantitativeValue_uom</td>
<td width="8%">Unit of Measure for the quantitative assessment value.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">nameOfEvent</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">nameOfEvent</td>
<td width="8%">common name of the observed event.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">tOH_hazardCategory</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">tOH_hazardCategory</td>
<td width="8%">A generic classification of types of natural hazards or risks.</td>
<td width="8%"><a href="#DomainNaturalHazardCategoryValue_value">NaturalHazardCategoryValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">tOH_hazardCategory_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">tOH_hazardCategory_href</td>
<td width="8%">URI from the INSPIRE code list register - NaturalHazardCategoryValue <a href="https://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue">https://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue</a></td>
<td width="8%"><a href="#DomainNaturalHazardCategoryValue">NaturalHazardCategoryValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">tOH_specificHazardType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">tOH_specificHazardType</td>
<td width="8%">Additional classification of the natural hazard that further specifies the hazard type according to a nomenclature that is specific to this dataset.</td>
<td width="8%"><a href="#DomainSpecificHazardTypeValue_value">SpecificHazardTypeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">tOH_specificHazardType_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">tOH_specificHazardType_href</td>
<td width="8%">URI from the INSPIRE code list register - SpecificHazardTypeValue <a href="https://inspire.ec.europa.eu/codelist/SpecificHazardTypeValue">https://inspire.ec.europa.eu/codelist/SpecificHazardTypeValue</a></td>
<td width="8%"><a href="#DomainSpecificHazardTypeValue">SpecificHazardTypeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">validFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">validFrom</td>
<td width="8%">The time when the exposed element started to exist in the real world.</td>
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
<td width="8%">The time from which the exposed element no longer exists in the real world.</td>
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
</p></p><p><hr/><br/><a name="FeatureClassRiskZone"/>
<p><strong>RiskZone - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">RiskZone</td>
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
<td width="*" style="border-color: white">RiskZone</td>
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
<td width="*" style="border-color: white">RiskZone</td>
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
<td width="8%">lOR_method_citationDate</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">lOR_method_citationDate</td>
<td width="8%">Date of the citation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">lOR_method_citationLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">lOR_method_citationLevel</td>
<td width="8%">Level of the the cited document. Can be a value from https://inspire.ec.europa.eu/codelist/LegislationLevelValue</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">lOR_method_citationLink</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">lOR_method_citationLink</td>
<td width="8%">A URL or text citation referencing the legal act that created the Protected Site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">lOR_method_citationName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">lOR_method_citationName</td>
<td width="8%">Name of the cited Legal Document</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">lOR_method_citationType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">lOR_method_citationType</td>
<td width="8%">Either DocumentCitation, CI_Citation, or LegislationCitation</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">lOR_qualitativeValue</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">lOR_qualitativeValue</td>
<td width="8%">A qualitative assessment of the level or intensity.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">lOR_quantitativeValue</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">lOR_quantitativeValue</td>
<td width="8%">A quantitative assessment of the level or intensity.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">lOR_quantitativeValue_uom</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">lOR_quantitativeValue_uom</td>
<td width="8%">Unit of Measure for the quantitative assessment value.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">sOR_hazardCategory</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">sOR_hazardCategory</td>
<td width="8%">A generic classification of types of natural hazards or risks.</td>
<td width="8%"><a href="#DomainNaturalHazardCategoryValue_value">NaturalHazardCategoryValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">sOR_hazardCategory_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">sOR_hazardCategory_href</td>
<td width="8%">URI from the INSPIRE code list register - NaturalHazardCategoryValue <a href="https://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue">https://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue</a></td>
<td width="8%"><a href="#DomainNaturalHazardCategoryValue">NaturalHazardCategoryValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">sOR_specificHazardType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">sOR_specificHazardType</td>
<td width="8%">Additional classification of the natural hazard that further specifies the hazard type according to a nomenclature that is specific to this dataset.</td>
<td width="8%"><a href="#DomainSpecificHazardTypeValue_value">SpecificHazardTypeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">sOR_specificHazardType_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">sOR_specificHazardType_href</td>
<td width="8%">URI from the INSPIRE code list register - SpecificHazardTypeValue <a href="https://inspire.ec.europa.eu/codelist/SpecificHazardTypeValue">https://inspire.ec.europa.eu/codelist/SpecificHazardTypeValue</a></td>
<td width="8%"><a href="#DomainSpecificHazardTypeValue">SpecificHazardTypeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">source</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">source</td>
<td width="8%">featureId of the HazardArea feature which is considered for the creation of the risk zone object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">validityPeriod_beginPosition</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">validityPeriod_beginPosition</td>
<td width="8%">Begin of time frame where the model applies.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">validityPeriod_endPosition</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">validityPeriod_endPosition</td>
<td width="8%">End of Time frame where the model applies.</td>
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
<p><hr/><a name="TableHazardArea_source"/>
<p><strong>HazardArea_source - Table</strong></p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">HazardArea_source</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">HazardArea_source</td>
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
<td width="*" style="border-color: white">HazardArea_source</td>
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
<td width="8%">Reference to featureId field in parent 'HazardArea'.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">source</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">source</td>
<td width="8%">featureId of the ObservedEvent. The observed event that triggered the modelling of a hazard area.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p><p><hr/><a name="TableRiskZone_exposedElement"/>
<p><strong>RiskZone_exposedElement - Table</strong></p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">RiskZone_exposedElement</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">RiskZone_exposedElement</td>
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
<td width="*" style="border-color: white">RiskZone_exposedElement</td>
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
<td width="8%">exposedElement</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">exposedElement</td>
<td width="8%">featureId of the ExposedElement. The element that is within a hazardous area.</td>
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
<td width="8%">Reference to featureId field in parent 'RiskZone'.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p>
    <p><hr/><a name="RelationshipClassRelHA_HA_source"/>
<p><strong>RelHA_HA_source - RelationshipClass</strong></p>
<table width="100%">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">RelHA_HA_source</td>
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
<td width="*" style="border-color: white">HazardArea_source</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>BackwardPathLabel</strong></td>
<td width="*" style="border-color: white">HazardArea</td>
</tr>
</tbody>
</table>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Description</strong></td>
<td width="*" style="border-color: white">RelHA_HA_source</td>
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
<td width="30%">HazardArea</td>
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
<td width="30%">HazardArea_source</td>
<td width="30%"/>
<td width="30%"/>
</tr>
</tbody>
</table></p><p><hr/><a name="RelationshipClassRelRZ_RZ_exposedElement"/>
<p><strong>RelRZ_RZ_exposedElement - RelationshipClass</strong></p>
<table width="100%">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">RelRZ_RZ_exposedElement</td>
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
<td width="*" style="border-color: white">RiskZone_exposedElement</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>BackwardPathLabel</strong></td>
<td width="*" style="border-color: white">RiskZone</td>
</tr>
</tbody>
</table>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Description</strong></td>
<td width="*" style="border-color: white">RelRZ_RZ_exposedElement</td>
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
<td width="30%">RiskZone</td>
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
<td width="30%">RiskZone_exposedElement</td>
<td width="30%"/>
<td width="30%"/>
</tr>
</tbody>
</table></p>
    <p>
    <hr/><a name="DomainDeterminationMethodValue"/>
<p><strong>DeterminationMethodValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">DeterminationMethodValue</td>
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
<td width="20%">http://inspire.ec.europa.eu/codelist/DeterminationMethodValue/indirectDetermination</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/DeterminationMethodValue/indirectDetermination</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/DeterminationMethodValue/modelling</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/DeterminationMethodValue/modelling</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainDeterminationMethodValue_value"/>
<p><strong>DeterminationMethodValue_value - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">DeterminationMethodValue_value</td>
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
<td width="20%">indirectDetermination</td>
<td width="20%">indirectDetermination</td>
</tr><tr>
<td width="20%">modelling</td>
<td width="20%">modelling</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainExposedElementCategoryValue"/>
<p><strong>ExposedElementCategoryValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">ExposedElementCategoryValue</td>
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
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/social</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/social</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/people</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/people</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/community</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/community</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/political</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/political</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/socialService</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/socialService</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/economic</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/economic</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/property</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/property</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/infrastructure</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/infrastructure</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/economicActivity</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/economicActivity</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/ruralLandUse</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/ruralLandUse</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/environmental</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/environmental</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/waterBody</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/waterBody</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/protectedArea</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/protectedArea</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/pollutionSource</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/pollutionSource</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/heritage</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/heritage</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/culturalAsset</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/culturalAsset</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/historicalAsset</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/historicalAsset</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/worldHeritageSite</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ExposedElementCategoryValue/worldHeritageSite</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainExposedElementCategoryValue_value"/>
<p><strong>ExposedElementCategoryValue_value - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">ExposedElementCategoryValue_value</td>
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
<td width="20%">social</td>
<td width="20%">social</td>
</tr><tr>
<td width="20%">people</td>
<td width="20%">people</td>
</tr><tr>
<td width="20%">community</td>
<td width="20%">community</td>
</tr><tr>
<td width="20%">political</td>
<td width="20%">political</td>
</tr><tr>
<td width="20%">socialService</td>
<td width="20%">socialService</td>
</tr><tr>
<td width="20%">economic</td>
<td width="20%">economic</td>
</tr><tr>
<td width="20%">property</td>
<td width="20%">property</td>
</tr><tr>
<td width="20%">infrastructure</td>
<td width="20%">infrastructure</td>
</tr><tr>
<td width="20%">economicActivity</td>
<td width="20%">economicActivity</td>
</tr><tr>
<td width="20%">ruralLandUse</td>
<td width="20%">ruralLandUse</td>
</tr><tr>
<td width="20%">environmental</td>
<td width="20%">environmental</td>
</tr><tr>
<td width="20%">waterBody</td>
<td width="20%">waterBody</td>
</tr><tr>
<td width="20%">protectedArea</td>
<td width="20%">protectedArea</td>
</tr><tr>
<td width="20%">pollutionSource</td>
<td width="20%">pollutionSource</td>
</tr><tr>
<td width="20%">heritage</td>
<td width="20%">heritage</td>
</tr><tr>
<td width="20%">culturalAsset</td>
<td width="20%">culturalAsset</td>
</tr><tr>
<td width="20%">historicalAsset</td>
<td width="20%">historicalAsset</td>
</tr><tr>
<td width="20%">worldHeritageSite</td>
<td width="20%">worldHeritageSite</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainNaturalHazardCategoryValue"/>
<p><strong>NaturalHazardCategoryValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">NaturalHazardCategoryValue</td>
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
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/geologicalHydrological</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/geologicalHydrological</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/tsunami</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/tsunami</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/volcanic</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/volcanic</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/earthquake</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/earthquake</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/subsidenceAndCollapse</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/subsidenceAndCollapse</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/landslide</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/landslide</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/snowAvalanche</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/snowAvalanche</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/flood</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/flood</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/toxicOrRadioactive</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/toxicOrRadioactive</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/meteorologicalClimatological</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/meteorologicalClimatological</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/drought</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/drought</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/extremeTemperature</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/extremeTemperature</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/tornadosAndHurricanesStrongWinds</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/tornadosAndHurricanesStrongWinds</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/lightning</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/lightning</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/stormSurge</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/stormSurge</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/fires</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/fires</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/forestFireWildfire</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/forestFireWildfire</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/undergroundFires</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/undergroundFires</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/biological</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/biological</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/infestation</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/infestation</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/epidemic</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/epidemic</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/allergens</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/allergens</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/cosmic</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/cosmic</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/meteoriteImpact</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/meteoriteImpact</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/magneticDisruption</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/magneticDisruption</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/solarAndCosmicRadiation</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/solarAndCosmicRadiation</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/otherGeologicalHydrological</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/otherGeologicalHydrological</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/otherMeteorologicalClimatological</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/otherMeteorologicalClimatological</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/otherBiological</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/otherBiological</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/otherCosmic</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/NaturalHazardCategoryValue/otherCosmic</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainNaturalHazardCategoryValue_value"/>
<p><strong>NaturalHazardCategoryValue_value - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">NaturalHazardCategoryValue_value</td>
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
<td width="20%">geologicalHydrological</td>
<td width="20%">geologicalHydrological</td>
</tr><tr>
<td width="20%">tsunami</td>
<td width="20%">tsunami</td>
</tr><tr>
<td width="20%">volcanic</td>
<td width="20%">volcanic</td>
</tr><tr>
<td width="20%">earthquake</td>
<td width="20%">earthquake</td>
</tr><tr>
<td width="20%">subsidenceAndCollapse</td>
<td width="20%">subsidenceAndCollapse</td>
</tr><tr>
<td width="20%">landslide</td>
<td width="20%">landslide</td>
</tr><tr>
<td width="20%">snowAvalanche</td>
<td width="20%">snowAvalanche</td>
</tr><tr>
<td width="20%">flood</td>
<td width="20%">flood</td>
</tr><tr>
<td width="20%">toxicOrRadioactive</td>
<td width="20%">toxicOrRadioactive</td>
</tr><tr>
<td width="20%">meteorologicalClimatological</td>
<td width="20%">meteorologicalClimatological</td>
</tr><tr>
<td width="20%">drought</td>
<td width="20%">drought</td>
</tr><tr>
<td width="20%">extremeTemperature</td>
<td width="20%">extremeTemperature</td>
</tr><tr>
<td width="20%">tornadosAndHurricanesStrongWinds</td>
<td width="20%">tornadosAndHurricanesStrongWinds</td>
</tr><tr>
<td width="20%">lightning</td>
<td width="20%">lightning</td>
</tr><tr>
<td width="20%">stormSurge</td>
<td width="20%">stormSurge</td>
</tr><tr>
<td width="20%">fires</td>
<td width="20%">fires</td>
</tr><tr>
<td width="20%">forestFireWildfire</td>
<td width="20%">forestFireWildfire</td>
</tr><tr>
<td width="20%">undergroundFires</td>
<td width="20%">undergroundFires</td>
</tr><tr>
<td width="20%">biological</td>
<td width="20%">biological</td>
</tr><tr>
<td width="20%">infestation</td>
<td width="20%">infestation</td>
</tr><tr>
<td width="20%">epidemic</td>
<td width="20%">epidemic</td>
</tr><tr>
<td width="20%">allergens</td>
<td width="20%">allergens</td>
</tr><tr>
<td width="20%">cosmic</td>
<td width="20%">cosmic</td>
</tr><tr>
<td width="20%">meteoriteImpact</td>
<td width="20%">meteoriteImpact</td>
</tr><tr>
<td width="20%">magneticDisruption</td>
<td width="20%">magneticDisruption</td>
</tr><tr>
<td width="20%">solarAndCosmicRadiation</td>
<td width="20%">solarAndCosmicRadiation</td>
</tr><tr>
<td width="20%">otherGeologicalHydrological</td>
<td width="20%">otherGeologicalHydrological</td>
</tr><tr>
<td width="20%">otherMeteorologicalClimatological</td>
<td width="20%">otherMeteorologicalClimatological</td>
</tr><tr>
<td width="20%">otherBiological</td>
<td width="20%">otherBiological</td>
</tr><tr>
<td width="20%">otherCosmic</td>
<td width="20%">otherCosmic</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p>
