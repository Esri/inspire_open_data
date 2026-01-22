
#SpeciesDistribution


<br/>
<strong>Geodatabase Documentation</strong>
<hr/>
<strong>Date: </strong>20251028125915.4109073<br/>
<hr/>
<p><strong>Summary Information and Links</strong><br/><br/><a href="#FeatureDatasets">0 Feature Datasets and 4
Feature Classes</a><br/>No Topology Datasets<br/>No Geometric Networks<br/>No Rasters<br/><a href="#ObjectClasses">0 Tables (Object Classes)</a><br/><a href="#RelationshipClasses">0 Relationship
Classes</a><br/><a href="#Domains">9 Domains</a><br/></p>
<hr/>
<p><a name="FeatureDatasets"/><strong>Feature Datasets and Child Classes</strong></p><a name="Raster"/>
<p><strong>Rasters</strong></p><br/>
<hr/><a name="ObjectClasses"/>
<p><strong>Workspace-Level Tables and Feature Classes</strong></p>
    <a href="#FeatureClassSpeciesDistributionDataSet">SpeciesDistributionDataSet - FeatureClass</a><br/><a href="#FeatureClassSpeciesDistributionUnitL">SpeciesDistributionUnitL - FeatureClass</a><br/><a href="#FeatureClassSpeciesDistributionUnitP">SpeciesDistributionUnitP - FeatureClass</a><br/><a href="#FeatureClassSpeciesDistributionUnitS">SpeciesDistributionUnitS - FeatureClass</a><br/>
<p/><br/>
<hr/><a name="RelationshipClasses"/>
<p><strong>Relationship Classes</strong></p><p/>
<hr/><br/><a name="Domains"/>
<p><strong>Domains</strong></p>
   <a href="#DomainCountingMethodValue">CountingMethodValue</a><br/><a href="#DomainCountingMethodValue_value">CountingMethodValue_value</a><br/><a href="#DomainLegislationLevelValue">LegislationLevelValue</a><br/><a href="#DomainOccurrenceCategoryValue">OccurrenceCategoryValue</a><br/><a href="#DomainOccurrenceCategoryValue_value">OccurrenceCategoryValue_value</a><br/><a href="#DomainQualifierValue">QualifierValue</a><br/><a href="#DomainQualifierValue_value">QualifierValue_value</a><br/><a href="#DomainReferenceSpeciesSchemeValue">ReferenceSpeciesSchemeValue</a><br/><a href="#DomainReferenceSpeciesSchemeValue_value">ReferenceSpeciesSchemeValue_value</a><br/>
    <p><hr/><br/><a name="FeatureClassSpeciesDistributionDataSet"/>
<p><strong>SpeciesDistributionDataSet - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">SpeciesDistributionDataSet</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>ShapeType</strong></td>
<td width="*" style="border-color: white">Polygon</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FeatureType</strong></td>
<td width="*" style="border-color: white">Simple</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">SpeciesDistributionDataSet</td>
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
<td width="*" style="border-color: white">SpeciesDistributionDataSet</td>
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
<td width="8%">documentBasis_date</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">documentBasis_date</td>
<td width="8%">Date of creation, publication or revision of the document.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">documentBasis_level_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">documentBasis_level_href</td>
<td width="8%">URI from the INSPIRE code list register - LegislationLevelValue <a href="https://inspire.ec.europa.eu/codelist/LegislationLevelValue">https://inspire.ec.europa.eu/codelist/LegislationLevelValue</a></td>
<td width="8%"><a href="#DomainLegislationLevelValue">LegislationLevelValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">documentBasis_link</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">documentBasis_link</td>
<td width="8%">Link to an online version of the document</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">documentBasis_name</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">documentBasis_name</td>
<td width="8%">Name of the document.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">documentBasis_type</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">documentBasis_type</td>
<td width="8%">Type of the Document. Either DocumentCitation or LegislationCitation.</td>
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
<td width="3%">25</td>
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
<td width="8%">Name of the residence of authority.</td>
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
</p></p><p><hr/><br/><a name="FeatureClassSpeciesDistributionUnitL"/>
<p><strong>SpeciesDistributionUnitL - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">SpeciesDistributionUnitL</td>
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
<td width="*" style="border-color: white">SpeciesDistributionUnitL</td>
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
<td width="*" style="border-color: white">SpeciesDistributionUnitL</td>
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
<td width="8%">dataSet</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">dataSet</td>
<td width="8%">featureId of the SpeciesdistributiinDataset this feature belongs to.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_collectedFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">dI_collectedFrom</td>
<td width="8%">The date when the collecting of the original species occurrence data started.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_collectedTo</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">dI_collectedTo</td>
<td width="8%">The date when the collecting of the original species occurrence data stopped.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_occurrenceCategory</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_occurrenceCategory</td>
<td width="8%">The species population density in the species distribution unit. A species abundance (population density) in classes (common, rare, very rare, present or absent) in an individual species distribution unit.</td>
<td width="8%"><a href="#DomainOccurrenceCategoryValue_value">OccurrenceCategoryValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_occurrenceCategory_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_occurrenceCategory_href</td>
<td width="8%">URI from the INSPIRE code list register - OccurrenceCategoryValue <a href="https://inspire.ec.europa.eu/codelist/OccurrenceCategoryValue">https://inspire.ec.europa.eu/codelist/OccurrenceCategoryValue</a></td>
<td width="8%"><a href="#DomainOccurrenceCategoryValue">OccurrenceCategoryValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_popSize_countingMethod</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_popSize_countingMethod</td>
<td width="8%">Method of providing a number for the indication of the abundance of a species within a specific species distribution unit. To obtain a density or abundance estimate the data set provider can either count, estimate or calculate the population abundance.</td>
<td width="8%"><a href="#DomainCountingMethodValue_value">CountingMethodValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_popSize_countingMethod_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_popSize_countingMethod_href</td>
<td width="8%">URI from the INSPIRE code list register - CountingMethodValue <a href="https://inspire.ec.europa.eu/codelist/CountingMethodValue">https://inspire.ec.europa.eu/codelist/CountingMethodValue</a></td>
<td width="8%"><a href="#DomainCountingMethodValue">CountingMethodValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_popSize_countingUnit</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_popSize_countingUnit</td>
<td width="8%">What has been counted, estimated or calculated when compiling information on the abundance of a species within the species distribution unit. This parameter defines which species population units that has collected or retrieved. EXAMPLE Colonies, individuals, juvenile, larvae, pairs, shoals, shoots, tufts.</td>
<td width="8%"><a href="#DomainCountingUnitValue_value">CountingUnitValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_popSize_countingUnit_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_popSize_countingUnit_href</td>
<td width="8%">URI from the INSPIRE code list register - CountingUnitValue <a href="https://inspire.ec.europa.eu/codelist/CountingUnitValue">https://inspire.ec.europa.eu/codelist/CountingUnitValue</a></td>
<td width="8%"><a href="#DomainCountingUnitValue">CountingUnitValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_popSize_lowerBound</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">dI_popSize_lowerBound</td>
<td width="8%">A range value indicating the counted, estimated or calculated occurrences or population sizes using upper and lower bounds. Value of upper bound.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_popSize_upperBound</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">dI_popSize_upperBound</td>
<td width="8%">A range value indicating the counted, estimated or calculated occurrences or population sizes using upper and lower bounds. Value of lower bound.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_populationType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_populationType</td>
<td width="8%">The permanency of populations, particularly with regard to migratory species within a given species distribution unit. These values are used for Natura2000 (revised SDF).</td>
<td width="8%"><a href="#DomainPopulationTypeValue_value">PopulationTypeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_populationType_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_populationType_href</td>
<td width="8%">URI from the INSPIRE code list register - PopulationTypeValue <a href="https://inspire.ec.europa.eu/codelist/PopulationTypeValue">https://inspire.ec.europa.eu/codelist/PopulationTypeValue</a></td>
<td width="8%"><a href="#DomainPopulationTypeValue">PopulationTypeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_residencyStatus</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_residencyStatus</td>
<td width="8%">Information on the status of residency of a species regarding nativeness versus introduction and permanency.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_residencyStatus_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_residencyStatus_href</td>
<td width="8%">Information on the status of residency of a species regarding nativeness versus introduction and permanency.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_sensitiveInfo</td>
<td width="8%">SmallInteger</td>
<td width="3%">2</td>
<td width="8%">dI_sensitiveInfo</td>
<td width="8%">Boolean value that indicates whether the location of a specific species is sensitive.</td>
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
<td width="3%">25</td>
<td width="8%">inspireId_versionId</td>
<td width="8%">The identifier of the particular version of the spatial object, with a maximum length of 25 characters. If the specification of a spatial object type with an external object identifier includes life-cycle information, the version identifier is used to distinguish between the different versions of a spatial object. Within the set of all versions of a spatial object, the version identifier is unique</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_localSpeciesId</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_localSpeciesId</td>
<td width="8%">Identifier used in national nomenclature. The taxonID used in national nomenclature databases.</td>
<td width="8%"><a href="#DomainLocalSpeciesNameCodeValue_value">LocalSpeciesNameCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_localSpeciesId_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_localSpeciesId_href</td>
<td width="8%">URI from the INSPIRE code list register - LocalSpeciesNameCodeValue <a href="https://inspire.ec.europa.eu/codelist/LocalSpeciesNameCodeValue">https://inspire.ec.europa.eu/codelist/LocalSpeciesNameCodeValue</a></td>
<td width="8%"><a href="#DomainLocalSpeciesNameCodeValue">LocalSpeciesNameCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_localSpeciesName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_localSpeciesName</td>
<td width="8%">Scientific name, including the author, used in national nomenclature with its national taxonomic concept.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_localSpeciesScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_localSpeciesScheme</td>
<td width="8%">Name of local species classification scheme (bibliographic reference).</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_qualifier</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_qualifier</td>
<td width="8%">Specifies the taxonomic concept relationship between local species identifier and the reference species identifier. Defines how the local species name conceptually is related to the referenceSpeciesID, either congruent, included in, includes,  overlaps or excludes</td>
<td width="8%"><a href="#DomainQualifierValue_value">QualifierValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_qualifier_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_qualifier_href</td>
<td width="8%">URI from the INSPIRE code list register - QualifierValue <a href="https://inspire.ec.europa.eu/codelist/QualifierValue">https://inspire.ec.europa.eu/codelist/QualifierValue</a></td>
<td width="8%"><a href="#DomainQualifierValue">QualifierValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_refSpeciesId</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_refSpeciesId</td>
<td width="8%">Identifier of one of the reference lists given by the referenceSpeciesScheme. In the referenceSpeciesScheme the species IDs are linked to scientific names and corresponding authors using GUIDs</td>
<td width="8%"><a href="#DomainReferenceSpeciesCodeValue_value">ReferenceSpeciesCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_refSpeciesId_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_refSpeciesId_href</td>
<td width="8%">URI from the INSPIRE code list register - ReferenceSpeciesCodeValue <a href="https://inspire.ec.europa.eu/codelist/ReferenceSpeciesCodeValue">https://inspire.ec.europa.eu/codelist/ReferenceSpeciesCodeValue</a></td>
<td width="8%"><a href="#DomainReferenceSpeciesCodeValue">ReferenceSpeciesCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_refSpeciesName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_refSpeciesName</td>
<td width="8%">The scientific name, including the author, used in the authorized ReferenceSpeciesScheme. The authorized ReferenceSpeciesScheme (EU-Nomen, Unis and Nature Directives) provides reference species lists which defines the ReferenceSpeciesName with its scientific name plus author and ReferenceSpeciesId.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_refSpeciesScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_refSpeciesScheme</td>
<td width="8%">Reference list defining a nomenclatural and taxonomical standard to which all local names and taxonomic concepts shall be mapped. Code list of accepted PAN-European taxonomical reference lists defining the nomenclature and taxonomical concept of a given species name. This must not be regarded as the ultimate taxonomic truth: this will always change. It serves as a definition of a taxonomic concept described by systematic and synonym relations where other names and there inherent taxonomic concepts can be mapped to. The code list comprises of Eu-Nomen, EUNIS and Natura2000. In these sources harmonized species GUIDs and names are maintained by institutions with an assignment outside INSPIRE and the species names are to be retrieved through webservices using GUIDs. Only one of these list must be used for one taxon. The priority is as follows: 1) EU-Nomen, 2) EUNIS, 3) Natura2000. This implies: if a taxon is listed in EU-Nomen, this reference must be used as first choice. If it is not listed in EU-Nomen, the second choice is EUNIS, if not in EUNIS, Natura2000 can be used.</td>
<td width="8%"><a href="#DomainReferenceSpeciesSchemeValue_value">ReferenceSpeciesSchemeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_refSpeciesScheme_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_refSpeciesScheme_href</td>
<td width="8%">URI from the INSPIRE code list register - ReferenceSpeciesSchemeValue <a href="https://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue">https://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue</a></td>
<td width="8%"><a href="#DomainReferenceSpeciesSchemeValue">ReferenceSpeciesSchemeValue</a></td>
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
</p></p><p><hr/><br/><a name="FeatureClassSpeciesDistributionUnitP"/>
<p><strong>SpeciesDistributionUnitP - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">SpeciesDistributionUnitP</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>ShapeType</strong></td>
<td width="*" style="border-color: white">Point</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FeatureType</strong></td>
<td width="*" style="border-color: white">Simple</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">SpeciesDistributionUnitP</td>
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
<td width="*" style="border-color: white">SpeciesDistributionUnitP</td>
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
<td width="8%">dataSet</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">dataSet</td>
<td width="8%">featureId of the SpeciesdistributiinDataset this feature belongs to.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_collectedFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">dI_collectedFrom</td>
<td width="8%">The date when the collecting of the original species occurrence data started.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_collectedTo</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">dI_collectedTo</td>
<td width="8%">The date when the collecting of the original species occurrence data stopped.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_occurrenceCategory</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_occurrenceCategory</td>
<td width="8%">The species population density in the species distribution unit. A species abundance (population density) in classes (common, rare, very rare, present or absent) in an individual species distribution unit.</td>
<td width="8%"><a href="#DomainOccurrenceCategoryValue_value">OccurrenceCategoryValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_occurrenceCategory_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_occurrenceCategory_href</td>
<td width="8%">URI from the INSPIRE code list register - OccurrenceCategoryValue <a href="https://inspire.ec.europa.eu/codelist/OccurrenceCategoryValue">https://inspire.ec.europa.eu/codelist/OccurrenceCategoryValue</a></td>
<td width="8%"><a href="#DomainOccurrenceCategoryValue">OccurrenceCategoryValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_popSize_countingMethod</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_popSize_countingMethod</td>
<td width="8%">Method of providing a number for the indication of the abundance of a species within a specific species distribution unit. To obtain a density or abundance estimate the data set provider can either count, estimate or calculate the population abundance.</td>
<td width="8%"><a href="#DomainCountingMethodValue_value">CountingMethodValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_popSize_countingMethod_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_popSize_countingMethod_href</td>
<td width="8%">URI from the INSPIRE code list register - CountingMethodValue <a href="https://inspire.ec.europa.eu/codelist/CountingMethodValue">https://inspire.ec.europa.eu/codelist/CountingMethodValue</a></td>
<td width="8%"><a href="#DomainCountingMethodValue">CountingMethodValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_popSize_countingUnit</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_popSize_countingUnit</td>
<td width="8%">What has been counted, estimated or calculated when compiling information on the abundance of a species within the species distribution unit. This parameter defines which species population units that has collected or retrieved. EXAMPLE Colonies, individuals, juvenile, larvae, pairs, shoals, shoots, tufts.</td>
<td width="8%"><a href="#DomainCountingUnitValue_value">CountingUnitValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_popSize_countingUnit_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_popSize_countingUnit_href</td>
<td width="8%">URI from the INSPIRE code list register - CountingUnitValue <a href="https://inspire.ec.europa.eu/codelist/CountingUnitValue">https://inspire.ec.europa.eu/codelist/CountingUnitValue</a></td>
<td width="8%"><a href="#DomainCountingUnitValue">CountingUnitValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_popSize_lowerBound</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">dI_popSize_lowerBound</td>
<td width="8%">A range value indicating the counted, estimated or calculated occurrences or population sizes using upper and lower bounds. Value of upper bound.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_popSize_upperBound</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">dI_popSize_upperBound</td>
<td width="8%">A range value indicating the counted, estimated or calculated occurrences or population sizes using upper and lower bounds. Value of lower bound.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_populationType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_populationType</td>
<td width="8%">The permanency of populations, particularly with regard to migratory species within a given species distribution unit. These values are used for Natura2000 (revised SDF).</td>
<td width="8%"><a href="#DomainPopulationTypeValue_value">PopulationTypeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_populationType_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_populationType_href</td>
<td width="8%">URI from the INSPIRE code list register - PopulationTypeValue <a href="https://inspire.ec.europa.eu/codelist/PopulationTypeValue">https://inspire.ec.europa.eu/codelist/PopulationTypeValue</a></td>
<td width="8%"><a href="#DomainPopulationTypeValue">PopulationTypeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_residencyStatus</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_residencyStatus</td>
<td width="8%">Information on the status of residency of a species regarding nativeness versus introduction and permanency.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_residencyStatus_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_residencyStatus_href</td>
<td width="8%">Information on the status of residency of a species regarding nativeness versus introduction and permanency.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_sensitiveInfo</td>
<td width="8%">SmallInteger</td>
<td width="3%">2</td>
<td width="8%">dI_sensitiveInfo</td>
<td width="8%">Boolean value that indicates whether the location of a specific species is sensitive.</td>
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
<td width="3%">25</td>
<td width="8%">inspireId_versionId</td>
<td width="8%">The identifier of the particular version of the spatial object, with a maximum length of 25 characters. If the specification of a spatial object type with an external object identifier includes life-cycle information, the version identifier is used to distinguish between the different versions of a spatial object. Within the set of all versions of a spatial object, the version identifier is unique</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_localSpeciesId</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_localSpeciesId</td>
<td width="8%">Identifier used in national nomenclature. The taxonID used in national nomenclature databases.</td>
<td width="8%"><a href="#DomainLocalSpeciesNameCodeValue_value">LocalSpeciesNameCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_localSpeciesId_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_localSpeciesId_href</td>
<td width="8%">URI from the INSPIRE code list register - LocalSpeciesNameCodeValue <a href="https://inspire.ec.europa.eu/codelist/LocalSpeciesNameCodeValue">https://inspire.ec.europa.eu/codelist/LocalSpeciesNameCodeValue</a></td>
<td width="8%"><a href="#DomainLocalSpeciesNameCodeValue">LocalSpeciesNameCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_localSpeciesName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_localSpeciesName</td>
<td width="8%">Scientific name, including the author, used in national nomenclature with its national taxonomic concept.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_localSpeciesScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_localSpeciesScheme</td>
<td width="8%">Name of local species classification scheme (bibliographic reference).</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_qualifier</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_qualifier</td>
<td width="8%">Specifies the taxonomic concept relationship between local species identifier and the reference species identifier. Defines how the local species name conceptually is related to the referenceSpeciesID, either congruent, included in, includes,  overlaps or excludes</td>
<td width="8%"><a href="#DomainQualifierValue_value">QualifierValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_qualifier_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_qualifier_href</td>
<td width="8%">URI from the INSPIRE code list register - QualifierValue <a href="https://inspire.ec.europa.eu/codelist/QualifierValue">https://inspire.ec.europa.eu/codelist/QualifierValue</a></td>
<td width="8%"><a href="#DomainQualifierValue">QualifierValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_refSpeciesId</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_refSpeciesId</td>
<td width="8%">Identifier of one of the reference lists given by the referenceSpeciesScheme. In the referenceSpeciesScheme the species IDs are linked to scientific names and corresponding authors using GUIDs</td>
<td width="8%"><a href="#DomainReferenceSpeciesCodeValue_value">ReferenceSpeciesCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_refSpeciesId_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_refSpeciesId_href</td>
<td width="8%">URI from the INSPIRE code list register - ReferenceSpeciesCodeValue <a href="https://inspire.ec.europa.eu/codelist/ReferenceSpeciesCodeValue">https://inspire.ec.europa.eu/codelist/ReferenceSpeciesCodeValue</a></td>
<td width="8%"><a href="#DomainReferenceSpeciesCodeValue">ReferenceSpeciesCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_refSpeciesName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_refSpeciesName</td>
<td width="8%">The scientific name, including the author, used in the authorized ReferenceSpeciesScheme. The authorized ReferenceSpeciesScheme (EU-Nomen, Unis and Nature Directives) provides reference species lists which defines the ReferenceSpeciesName with its scientific name plus author and ReferenceSpeciesId.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_refSpeciesScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_refSpeciesScheme</td>
<td width="8%">Reference list defining a nomenclatural and taxonomical standard to which all local names and taxonomic concepts shall be mapped. Code list of accepted PAN-European taxonomical reference lists defining the nomenclature and taxonomical concept of a given species name. This must not be regarded as the ultimate taxonomic truth: this will always change. It serves as a definition of a taxonomic concept described by systematic and synonym relations where other names and there inherent taxonomic concepts can be mapped to. The code list comprises of Eu-Nomen, EUNIS and Natura2000. In these sources harmonized species GUIDs and names are maintained by institutions with an assignment outside INSPIRE and the species names are to be retrieved through webservices using GUIDs. Only one of these list must be used for one taxon. The priority is as follows: 1) EU-Nomen, 2) EUNIS, 3) Natura2000. This implies: if a taxon is listed in EU-Nomen, this reference must be used as first choice. If it is not listed in EU-Nomen, the second choice is EUNIS, if not in EUNIS, Natura2000 can be used.</td>
<td width="8%"><a href="#DomainReferenceSpeciesSchemeValue_value">ReferenceSpeciesSchemeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_refSpeciesScheme_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_refSpeciesScheme_href</td>
<td width="8%">URI from the INSPIRE code list register - ReferenceSpeciesSchemeValue <a href="https://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue">https://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue</a></td>
<td width="8%"><a href="#DomainReferenceSpeciesSchemeValue">ReferenceSpeciesSchemeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p></p><p><hr/><br/><a name="FeatureClassSpeciesDistributionUnitS"/>
<p><strong>SpeciesDistributionUnitS - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">SpeciesDistributionUnitS</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>ShapeType</strong></td>
<td width="*" style="border-color: white">Polygon</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FeatureType</strong></td>
<td width="*" style="border-color: white">Simple</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">SpeciesDistributionUnitS</td>
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
<td width="*" style="border-color: white">SpeciesDistributionUnitS</td>
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
<td width="8%">dataSet</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">dataSet</td>
<td width="8%">featureId of the SpeciesdistributiinDataset this feature belongs to.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_collectedFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">dI_collectedFrom</td>
<td width="8%">The date when the collecting of the original species occurrence data started.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_collectedTo</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">dI_collectedTo</td>
<td width="8%">The date when the collecting of the original species occurrence data stopped.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_occurrenceCategory</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_occurrenceCategory</td>
<td width="8%">The species population density in the species distribution unit. A species abundance (population density) in classes (common, rare, very rare, present or absent) in an individual species distribution unit.</td>
<td width="8%"><a href="#DomainOccurrenceCategoryValue_value">OccurrenceCategoryValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_occurrenceCategory_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_occurrenceCategory_href</td>
<td width="8%">URI from the INSPIRE code list register - OccurrenceCategoryValue <a href="https://inspire.ec.europa.eu/codelist/OccurrenceCategoryValue">https://inspire.ec.europa.eu/codelist/OccurrenceCategoryValue</a></td>
<td width="8%"><a href="#DomainOccurrenceCategoryValue">OccurrenceCategoryValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_popSize_countingMethod</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_popSize_countingMethod</td>
<td width="8%">Method of providing a number for the indication of the abundance of a species within a specific species distribution unit. To obtain a density or abundance estimate the data set provider can either count, estimate or calculate the population abundance.</td>
<td width="8%"><a href="#DomainCountingMethodValue_value">CountingMethodValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_popSize_countingMethod_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_popSize_countingMethod_href</td>
<td width="8%">URI from the INSPIRE code list register - CountingMethodValue <a href="https://inspire.ec.europa.eu/codelist/CountingMethodValue">https://inspire.ec.europa.eu/codelist/CountingMethodValue</a></td>
<td width="8%"><a href="#DomainCountingMethodValue">CountingMethodValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_popSize_countingUnit</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_popSize_countingUnit</td>
<td width="8%">What has been counted, estimated or calculated when compiling information on the abundance of a species within the species distribution unit. This parameter defines which species population units that has collected or retrieved. EXAMPLE Colonies, individuals, juvenile, larvae, pairs, shoals, shoots, tufts.</td>
<td width="8%"><a href="#DomainCountingUnitValue_value">CountingUnitValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_popSize_countingUnit_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_popSize_countingUnit_href</td>
<td width="8%">URI from the INSPIRE code list register - CountingUnitValue <a href="https://inspire.ec.europa.eu/codelist/CountingUnitValue">https://inspire.ec.europa.eu/codelist/CountingUnitValue</a></td>
<td width="8%"><a href="#DomainCountingUnitValue">CountingUnitValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_popSize_lowerBound</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">dI_popSize_lowerBound</td>
<td width="8%">A range value indicating the counted, estimated or calculated occurrences or population sizes using upper and lower bounds. Value of upper bound.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_popSize_upperBound</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">dI_popSize_upperBound</td>
<td width="8%">A range value indicating the counted, estimated or calculated occurrences or population sizes using upper and lower bounds. Value of lower bound.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_populationType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_populationType</td>
<td width="8%">The permanency of populations, particularly with regard to migratory species within a given species distribution unit. These values are used for Natura2000 (revised SDF).</td>
<td width="8%"><a href="#DomainPopulationTypeValue_value">PopulationTypeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_populationType_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_populationType_href</td>
<td width="8%">URI from the INSPIRE code list register - PopulationTypeValue <a href="https://inspire.ec.europa.eu/codelist/PopulationTypeValue">https://inspire.ec.europa.eu/codelist/PopulationTypeValue</a></td>
<td width="8%"><a href="#DomainPopulationTypeValue">PopulationTypeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_residencyStatus</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_residencyStatus</td>
<td width="8%">Information on the status of residency of a species regarding nativeness versus introduction and permanency.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_residencyStatus_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">dI_residencyStatus_href</td>
<td width="8%">Information on the status of residency of a species regarding nativeness versus introduction and permanency.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">dI_sensitiveInfo</td>
<td width="8%">SmallInteger</td>
<td width="3%">2</td>
<td width="8%">dI_sensitiveInfo</td>
<td width="8%">Boolean value that indicates whether the location of a specific species is sensitive.</td>
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
<td width="3%">25</td>
<td width="8%">inspireId_versionId</td>
<td width="8%">The identifier of the particular version of the spatial object, with a maximum length of 25 characters. If the specification of a spatial object type with an external object identifier includes life-cycle information, the version identifier is used to distinguish between the different versions of a spatial object. Within the set of all versions of a spatial object, the version identifier is unique</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_localSpeciesId</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_localSpeciesId</td>
<td width="8%">Identifier used in national nomenclature. The taxonID used in national nomenclature databases.</td>
<td width="8%"><a href="#DomainLocalSpeciesNameCodeValue_value">LocalSpeciesNameCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_localSpeciesId_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_localSpeciesId_href</td>
<td width="8%">URI from the INSPIRE code list register - LocalSpeciesNameCodeValue <a href="https://inspire.ec.europa.eu/codelist/LocalSpeciesNameCodeValue">https://inspire.ec.europa.eu/codelist/LocalSpeciesNameCodeValue</a></td>
<td width="8%"><a href="#DomainLocalSpeciesNameCodeValue">LocalSpeciesNameCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_localSpeciesName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_localSpeciesName</td>
<td width="8%">Scientific name, including the author, used in national nomenclature with its national taxonomic concept.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_localSpeciesScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_localSpeciesScheme</td>
<td width="8%">Name of local species classification scheme (bibliographic reference).</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_qualifier</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_qualifier</td>
<td width="8%">Specifies the taxonomic concept relationship between local species identifier and the reference species identifier. Defines how the local species name conceptually is related to the referenceSpeciesID, either congruent, included in, includes,  overlaps or excludes</td>
<td width="8%"><a href="#DomainQualifierValue_value">QualifierValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_qualifier_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_qualifier_href</td>
<td width="8%">URI from the INSPIRE code list register - QualifierValue <a href="https://inspire.ec.europa.eu/codelist/QualifierValue">https://inspire.ec.europa.eu/codelist/QualifierValue</a></td>
<td width="8%"><a href="#DomainQualifierValue">QualifierValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_refSpeciesId</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_refSpeciesId</td>
<td width="8%">Identifier of one of the reference lists given by the referenceSpeciesScheme. In the referenceSpeciesScheme the species IDs are linked to scientific names and corresponding authors using GUIDs</td>
<td width="8%"><a href="#DomainReferenceSpeciesCodeValue_value">ReferenceSpeciesCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_refSpeciesId_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_refSpeciesId_href</td>
<td width="8%">URI from the INSPIRE code list register - ReferenceSpeciesCodeValue <a href="https://inspire.ec.europa.eu/codelist/ReferenceSpeciesCodeValue">https://inspire.ec.europa.eu/codelist/ReferenceSpeciesCodeValue</a></td>
<td width="8%"><a href="#DomainReferenceSpeciesCodeValue">ReferenceSpeciesCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_refSpeciesName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_refSpeciesName</td>
<td width="8%">The scientific name, including the author, used in the authorized ReferenceSpeciesScheme. The authorized ReferenceSpeciesScheme (EU-Nomen, Unis and Nature Directives) provides reference species lists which defines the ReferenceSpeciesName with its scientific name plus author and ReferenceSpeciesId.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_refSpeciesScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_refSpeciesScheme</td>
<td width="8%">Reference list defining a nomenclatural and taxonomical standard to which all local names and taxonomic concepts shall be mapped. Code list of accepted PAN-European taxonomical reference lists defining the nomenclature and taxonomical concept of a given species name. This must not be regarded as the ultimate taxonomic truth: this will always change. It serves as a definition of a taxonomic concept described by systematic and synonym relations where other names and there inherent taxonomic concepts can be mapped to. The code list comprises of Eu-Nomen, EUNIS and Natura2000. In these sources harmonized species GUIDs and names are maintained by institutions with an assignment outside INSPIRE and the species names are to be retrieved through webservices using GUIDs. Only one of these list must be used for one taxon. The priority is as follows: 1) EU-Nomen, 2) EUNIS, 3) Natura2000. This implies: if a taxon is listed in EU-Nomen, this reference must be used as first choice. If it is not listed in EU-Nomen, the second choice is EUNIS, if not in EUNIS, Natura2000 can be used.</td>
<td width="8%"><a href="#DomainReferenceSpeciesSchemeValue_value">ReferenceSpeciesSchemeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_refSpeciesScheme_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_refSpeciesScheme_href</td>
<td width="8%">URI from the INSPIRE code list register - ReferenceSpeciesSchemeValue <a href="https://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue">https://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue</a></td>
<td width="8%"><a href="#DomainReferenceSpeciesSchemeValue">ReferenceSpeciesSchemeValue</a></td>
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
    <hr/><a name="DomainCountingMethodValue"/>
<p><strong>CountingMethodValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">CountingMethodValue</td>
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
<td width="20%">http://inspire.ec.europa.eu/codelist/CountingMethodValue/counted</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/CountingMethodValue/counted</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/CountingMethodValue/estimated</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/CountingMethodValue/estimated</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/CountingMethodValue/calculated</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/CountingMethodValue/calculated</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainCountingMethodValue_value"/>
<p><strong>CountingMethodValue_value - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">CountingMethodValue_value</td>
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
<td width="20%">counted</td>
<td width="20%">counted</td>
</tr><tr>
<td width="20%">estimated</td>
<td width="20%">estimated</td>
</tr><tr>
<td width="20%">calculated</td>
<td width="20%">calculated</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainLegislationLevelValue"/>
<p><strong>LegislationLevelValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">LegislationLevelValue</td>
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
<td width="20%">http://inspire.ec.europa.eu/codelist/LegislationLevelValue/international</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/LegislationLevelValue/international</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/LegislationLevelValue/european</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/LegislationLevelValue/european</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/LegislationLevelValue/national</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/LegislationLevelValue/national</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/LegislationLevelValue/sub-national</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/LegislationLevelValue/sub-national</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainOccurrenceCategoryValue"/>
<p><strong>OccurrenceCategoryValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">OccurrenceCategoryValue</td>
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
<td width="20%">http://inspire.ec.europa.eu/codelist/OccurrenceCategoryValue/common</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/OccurrenceCategoryValue/common</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/OccurrenceCategoryValue/rare</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/OccurrenceCategoryValue/rare</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/OccurrenceCategoryValue/veryRare</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/OccurrenceCategoryValue/veryRare</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/OccurrenceCategoryValue/present</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/OccurrenceCategoryValue/present</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/OccurrenceCategoryValue/absent</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/OccurrenceCategoryValue/absent</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainOccurrenceCategoryValue_value"/>
<p><strong>OccurrenceCategoryValue_value - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">OccurrenceCategoryValue_value</td>
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
<td width="20%">common</td>
<td width="20%">common</td>
</tr><tr>
<td width="20%">rare</td>
<td width="20%">rare</td>
</tr><tr>
<td width="20%">veryRare</td>
<td width="20%">veryRare</td>
</tr><tr>
<td width="20%">present</td>
<td width="20%">present</td>
</tr><tr>
<td width="20%">absent</td>
<td width="20%">absent</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainQualifierValue"/>
<p><strong>QualifierValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">QualifierValue</td>
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
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierValue/congruent</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierValue/congruent</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierValue/includedIn</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierValue/includedIn</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierValue/includes</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierValue/includes</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierValue/overlaps</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierValue/overlaps</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierValue/excludes</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierValue/excludes</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainQualifierValue_value"/>
<p><strong>QualifierValue_value - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">QualifierValue_value</td>
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
<td width="20%">congruent</td>
<td width="20%">congruent</td>
</tr><tr>
<td width="20%">includedIn</td>
<td width="20%">includedIn</td>
</tr><tr>
<td width="20%">includes</td>
<td width="20%">includes</td>
</tr><tr>
<td width="20%">overlaps</td>
<td width="20%">overlaps</td>
</tr><tr>
<td width="20%">excludes</td>
<td width="20%">excludes</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainReferenceSpeciesSchemeValue"/>
<p><strong>ReferenceSpeciesSchemeValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">ReferenceSpeciesSchemeValue</td>
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
<td width="20%">http://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue/eunomen</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue/eunomen</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue/eunis</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue/eunis</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue/natureDirectives</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue/natureDirectives</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainReferenceSpeciesSchemeValue_value"/>
<p><strong>ReferenceSpeciesSchemeValue_value - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">ReferenceSpeciesSchemeValue_value</td>
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
<td width="20%">eunomen</td>
<td width="20%">eunomen</td>
</tr><tr>
<td width="20%">eunis</td>
<td width="20%">eunis</td>
</tr><tr>
<td width="20%">natureDirectives</td>
<td width="20%">natureDirectives</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p>
