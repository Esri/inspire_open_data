
#ProductionAndIndustrialFacilities


<br/>
<strong>Geodatabase Documentation</strong>
<hr/>
<strong>Date: </strong>20260121163237.3951203<br/>
<hr/>
<p><strong>Summary Information and Links</strong><br/><br/><a href="#FeatureDatasets">0 Feature Datasets and 4
Feature Classes</a><br/>No Topology Datasets<br/>No Geometric Networks<br/>No Rasters<br/><a href="#ObjectClasses">0 Tables (Object Classes)</a><br/><a href="#RelationshipClasses">0 Relationship
Classes</a><br/><a href="#Domains">6 Domains</a><br/></p>
<hr/>
<p><a name="FeatureDatasets"/><strong>Feature Datasets and Child Classes</strong></p><a name="Raster"/>
<p><strong>Rasters</strong></p><br/>
<hr/><a name="ObjectClasses"/>
<p><strong>Workspace-Level Tables and Feature Classes</strong></p>
    <a href="#FeatureClassProductionFacilityP">ProductionFacilityP - FeatureClass</a><br/><a href="#FeatureClassProductionFacilityS">ProductionFacilityS - FeatureClass</a><br/><a href="#FeatureClassProductionInstallation">ProductionInstallation - FeatureClass</a><br/><a href="#FeatureClassProductionSite">ProductionSite - FeatureClass</a><br/>
<p/><br/>
<hr/><a name="RelationshipClasses"/>
<p><strong>Relationship Classes</strong></p><p/>
<hr/><br/><a name="Domains"/>
<p><strong>Domains</strong></p>
   <a href="#DomainConditionOfFacilityValue">ConditionOfFacilityValue</a><br/><a href="#DomainConditionOfFacilityValue_value">ConditionOfFacilityValue_value</a><br/><a href="#DomainEconomicActivityValue">EconomicActivityValue</a><br/><a href="#DomainEconomicActivityValue_value">EconomicActivityValue_value</a><br/><a href="#DomainLegislationLevelValue">LegislationLevelValue</a><br/><a href="#DomainLegislationLevelValue_value">LegislationLevelValue_value</a><br/>
    <p><hr/><br/><a name="FeatureClassProductionFacilityP"/>
<p><strong>ProductionFacilityP - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">ProductionFacilityP</td>
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
<td width="*" style="border-color: white">ProductionFacilityP</td>
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
<td width="*" style="border-color: white">ProductionFacilityP</td>
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
<td width="8%">function_1_activity</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">function_1_activity</td>
<td width="8%">Categorized description of individual or organized set of technically related processes that are carried out by a economical unit, private or public, profit or non profit character. NOTE  The Activity described as part of the Function for “Activity Complex” should be recorded using a controlled vocabulary where a particular controlled vocabulary is in use within a given context, such as SIC codes in the UK, it is acceptable to use these, however, the preferred choice for European interoperability is whenever possible NACE [NACE].</td>
<td width="8%"><a href="#DomainEconomicActivityValue_value">EconomicActivityValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">function_1_activity_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">function_1_activity_href</td>
<td width="8%">URI from the INSPIRE code list register - EconomicActivityValue <a href="https://inspire.ec.europa.eu/codelist/EconomicActivityValue">https://inspire.ec.europa.eu/codelist/EconomicActivityValue</a></td>
<td width="8%"><a href="#DomainEconomicActivityValue">EconomicActivityValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">function_1_description</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">function_1_description</td>
<td width="8%">A more detailed description of the function.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">function_2_activity</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">function_2_activity</td>
<td width="8%">Categorized description of individual or organized set of technically related processes that are carried out by a economical unit, private or public, profit or non profit character. NOTE  The Activity described as part of the Function for “Activity Complex” should be recorded using a controlled vocabulary where a particular controlled vocabulary is in use within a given context, such as SIC codes in the UK, it is acceptable to use these, however, the preferred choice for European interoperability is whenever possible NACE [NACE].</td>
<td width="8%"><a href="#DomainEconomicActivityValue_value">EconomicActivityValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">function_2_activity_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">function_2_activity_href</td>
<td width="8%">URI from the INSPIRE code list register - EconomicActivityValue <a href="https://inspire.ec.europa.eu/codelist/EconomicActivityValue">https://inspire.ec.europa.eu/codelist/EconomicActivityValue</a></td>
<td width="8%"><a href="#DomainEconomicActivityValue">EconomicActivityValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">function_2_description</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">function_2_description</td>
<td width="8%">A more detailed description of the function.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">function_3_activity</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">function_3_activity</td>
<td width="8%">Categorized description of individual or organized set of technically related processes that are carried out by a economical unit, private or public, profit or non profit character. NOTE  The Activity described as part of the Function for “Activity Complex” should be recorded using a controlled vocabulary where a particular controlled vocabulary is in use within a given context, such as SIC codes in the UK, it is acceptable to use these, however, the preferred choice for European interoperability is whenever possible NACE [NACE].</td>
<td width="8%"><a href="#DomainEconomicActivityValue_value">EconomicActivityValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">function_3_activity_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">function_3_activity_href</td>
<td width="8%">URI from the INSPIRE code list register - EconomicActivityValue <a href="https://inspire.ec.europa.eu/codelist/EconomicActivityValue">https://inspire.ec.europa.eu/codelist/EconomicActivityValue</a></td>
<td width="8%"><a href="#DomainEconomicActivityValue">EconomicActivityValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">function_3_description</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">function_3_description</td>
<td width="8%">A more detailed description of the function.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hostingSite</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hostingSite</td>
<td width="8%">featureId of the hosting ProductionSite</td>
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
<td width="8%">Descriptive name of the “Activity Complex”.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">riverBasinDistrict</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">riverBasinDistrict</td>
<td width="8%">Code identifier and/or name assigned to the basin district of a watercourse. NOTE  Information required (not registered in the Hydrography Theme) according to Article 3(1) of Directive 2000/60/EC of the European Parliament and of the Council of 23 October 2000 stablishing a framework for Community action in the field of water policy (OJ L 327, 22.12.2000, p. 1). Directive as amended by Decision No 2455/2001/EC (OJ L 331, 15.12.2001, p. 1).</td>
<td width="8%"><a href="#DomainRiverBasinDistrictValue_value">RiverBasinDistrictValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">riverBasinDistrict_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">riverBasinDistrict_href</td>
<td width="8%">URI from the INSPIRE code list register - RiverBasinDistrictValue <a href="https://inspire.ec.europa.eu/codelist/RiverBasinDistrictValue">https://inspire.ec.europa.eu/codelist/RiverBasinDistrictValue</a></td>
<td width="8%"><a href="#DomainRiverBasinDistrictValue">RiverBasinDistrictValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_description</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">status_description</td>
<td width="8%">Descriptive statement about the declared status.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_statusType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">status_statusType</td>
<td width="8%">The state or condition of a technical component referring to a list of predefined potential values. The reference values are holded in the ConditionOfFacilityValue code list.</td>
<td width="8%"><a href="#DomainConditionOfFacilityValue_value">ConditionOfFacilityValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_statusType_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">status_statusType_href</td>
<td width="8%">URI from the INSPIRE code list register - ConditionOfFacilityValue <a href="https://inspire.ec.europa.eu/codelist/ConditionOfFacilityValue">https://inspire.ec.europa.eu/codelist/ConditionOfFacilityValue</a></td>
<td width="8%"><a href="#DomainConditionOfFacilityValue">ConditionOfFacilityValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_validFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">status_validFrom</td>
<td width="8%">The starting time of validity for a status type.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_validTo</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">status_validTo</td>
<td width="8%">The ending time of validity for a status type.</td>
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
<td width="8%">Thematic identifier to uniquely identify the spatial object.</td>
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
</p></p><p><hr/><br/><a name="FeatureClassProductionFacilityS"/>
<p><strong>ProductionFacilityS - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">ProductionFacilityS</td>
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
<td width="*" style="border-color: white">ProductionFacilityS</td>
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
<td width="*" style="border-color: white">ProductionFacilityS</td>
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
<td width="8%">function_1_activity</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">function_1_activity</td>
<td width="8%">Categorized description of individual or organized set of technically related processes that are carried out by a economical unit, private or public, profit or non profit character. NOTE  The Activity described as part of the Function for “Activity Complex” should be recorded using a controlled vocabulary where a particular controlled vocabulary is in use within a given context, such as SIC codes in the UK, it is acceptable to use these, however, the preferred choice for European interoperability is whenever possible NACE [NACE].</td>
<td width="8%"><a href="#DomainEconomicActivityValue_value">EconomicActivityValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">function_1_activity_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">function_1_activity_href</td>
<td width="8%">URI from the INSPIRE code list register - EconomicActivityValue <a href="https://inspire.ec.europa.eu/codelist/EconomicActivityValue">https://inspire.ec.europa.eu/codelist/EconomicActivityValue</a></td>
<td width="8%"><a href="#DomainEconomicActivityValue">EconomicActivityValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">function_1_description</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">function_1_description</td>
<td width="8%">A more detailed description of the function.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">function_2_activity</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">function_2_activity</td>
<td width="8%">Categorized description of individual or organized set of technically related processes that are carried out by a economical unit, private or public, profit or non profit character. NOTE  The Activity described as part of the Function for “Activity Complex” should be recorded using a controlled vocabulary where a particular controlled vocabulary is in use within a given context, such as SIC codes in the UK, it is acceptable to use these, however, the preferred choice for European interoperability is whenever possible NACE [NACE].</td>
<td width="8%"><a href="#DomainEconomicActivityValue_value">EconomicActivityValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">function_2_activity_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">function_2_activity_href</td>
<td width="8%">URI from the INSPIRE code list register - EconomicActivityValue <a href="https://inspire.ec.europa.eu/codelist/EconomicActivityValue">https://inspire.ec.europa.eu/codelist/EconomicActivityValue</a></td>
<td width="8%"><a href="#DomainEconomicActivityValue">EconomicActivityValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">function_2_description</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">function_2_description</td>
<td width="8%">A more detailed description of the function.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">function_3_activity</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">function_3_activity</td>
<td width="8%">Categorized description of individual or organized set of technically related processes that are carried out by a economical unit, private or public, profit or non profit character. NOTE  The Activity described as part of the Function for “Activity Complex” should be recorded using a controlled vocabulary where a particular controlled vocabulary is in use within a given context, such as SIC codes in the UK, it is acceptable to use these, however, the preferred choice for European interoperability is whenever possible NACE [NACE].</td>
<td width="8%"><a href="#DomainEconomicActivityValue_value">EconomicActivityValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">function_3_activity_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">function_3_activity_href</td>
<td width="8%">URI from the INSPIRE code list register - EconomicActivityValue <a href="https://inspire.ec.europa.eu/codelist/EconomicActivityValue">https://inspire.ec.europa.eu/codelist/EconomicActivityValue</a></td>
<td width="8%"><a href="#DomainEconomicActivityValue">EconomicActivityValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">function_3_description</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">function_3_description</td>
<td width="8%">A more detailed description of the function.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hostingSite</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hostingSite</td>
<td width="8%">featureId of the hosting ProductionSite</td>
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
<td width="8%">Descriptive name of the “Activity Complex”.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">riverBasinDistrict</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">riverBasinDistrict</td>
<td width="8%">Code identifier and/or name assigned to the basin district of a watercourse. NOTE  Information required (not registered in the Hydrography Theme) according to Article 3(1) of Directive 2000/60/EC of the European Parliament and of the Council of 23 October 2000 stablishing a framework for Community action in the field of water policy (OJ L 327, 22.12.2000, p. 1). Directive as amended by Decision No 2455/2001/EC (OJ L 331, 15.12.2001, p. 1).</td>
<td width="8%"><a href="#DomainRiverBasinDistrictValue_value">RiverBasinDistrictValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">riverBasinDistrict_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">riverBasinDistrict_href</td>
<td width="8%">URI from the INSPIRE code list register - RiverBasinDistrictValue <a href="https://inspire.ec.europa.eu/codelist/RiverBasinDistrictValue">https://inspire.ec.europa.eu/codelist/RiverBasinDistrictValue</a></td>
<td width="8%"><a href="#DomainRiverBasinDistrictValue">RiverBasinDistrictValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_description</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">status_description</td>
<td width="8%">Descriptive statement about the declared status.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_statusType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">status_statusType</td>
<td width="8%">The state or condition of a technical component referring to a list of predefined potential values. The reference values are holded in the ConditionOfFacilityValue code list.</td>
<td width="8%"><a href="#DomainConditionOfFacilityValue_value">ConditionOfFacilityValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_statusType_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">status_statusType_href</td>
<td width="8%">URI from the INSPIRE code list register - ConditionOfFacilityValue <a href="https://inspire.ec.europa.eu/codelist/ConditionOfFacilityValue">https://inspire.ec.europa.eu/codelist/ConditionOfFacilityValue</a></td>
<td width="8%"><a href="#DomainConditionOfFacilityValue">ConditionOfFacilityValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_validFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">status_validFrom</td>
<td width="8%">The starting time of validity for a status type.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_validTo</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">status_validTo</td>
<td width="8%">The ending time of validity for a status type.</td>
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
<td width="8%">Thematic identifier to uniquely identify the spatial object.</td>
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
</p></p><p><hr/><br/><a name="FeatureClassProductionInstallation"/>
<p><strong>ProductionInstallation - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">ProductionInstallation</td>
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
<td width="*" style="border-color: white">ProductionInstallation</td>
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
<td width="*" style="border-color: white">ProductionInstallation</td>
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
<td width="8%">description</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">description</td>
<td width="8%">Descriptive statement about the installation.</td>
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
<td width="8%">groupingFacility</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">groupingFacility</td>
<td width="8%">featureId of the grouping ProductionFacility</td>
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
<td width="8%">name_1</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_1</td>
<td width="8%">Official denomination or proper or conventional name of the installation.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_2</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_2</td>
<td width="8%">Official denomination or proper or conventional name of the installation.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_description</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">status_description</td>
<td width="8%">Descriptive statement about the declared status.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_statusType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">status_statusType</td>
<td width="8%">The state or condition of a technical component referring to a list of predefined potential values. The reference values are holded in the ConditionOfFacilityValue code list.</td>
<td width="8%"><a href="#DomainConditionOfFacilityValue_value">ConditionOfFacilityValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_statusType_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">status_statusType_href</td>
<td width="8%">URI from the INSPIRE code list register - ConditionOfFacilityValue <a href="https://inspire.ec.europa.eu/codelist/ConditionOfFacilityValue">https://inspire.ec.europa.eu/codelist/ConditionOfFacilityValue</a></td>
<td width="8%"><a href="#DomainConditionOfFacilityValue">ConditionOfFacilityValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_validFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">status_validFrom</td>
<td width="8%">The starting time of validity for a status type.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_validTo</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">status_validTo</td>
<td width="8%">The ending time of validity for a status type.</td>
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
<td width="8%">Thematic identifier to uniquely identify the spatial object.</td>
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
</p></p><p><hr/><br/><a name="FeatureClassProductionSite"/>
<p><strong>ProductionSite - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">ProductionSite</td>
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
<td width="*" style="border-color: white">ProductionSite</td>
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
<td width="*" style="border-color: white">ProductionSite</td>
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
<td width="8%">description_1</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">description_1</td>
<td width="8%">Descriptive statement about the site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">description_2</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">description_2</td>
<td width="8%">Descriptive statement about the site.</td>
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
<td width="8%">name_1</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_1</td>
<td width="8%">Official denomination or proper or conventional name of the site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">name_2</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">name_2</td>
<td width="8%">Official denomination or proper or conventional name of the site.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">sitePlan_date</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">sitePlan_date</td>
<td width="8%">Date of creation, publication or revision of the document.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">sitePlan_level</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">sitePlan_level</td>
<td width="8%">Level of the the cited document. Can be a value from LegislationLevelValue_value <a href="https://inspire.ec.europa.eu/codelist/LegislationLevelValue">https://inspire.ec.europa.eu/codelist/LegislationLevelValue</a></td>
<td width="8%"><a href="#DomainLegislationLevelValue_value">LegislationLevelValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">sitePlan_level_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">sitePlan_level_href</td>
<td width="8%">URI from the INSPIRE code list register - LegislationLevelValue <a href="https://inspire.ec.europa.eu/codelist/LegislationLevelValue">https://inspire.ec.europa.eu/codelist/LegislationLevelValue</a></td>
<td width="8%"><a href="#DomainLegislationLevelValue">LegislationLevelValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">sitePlan_link</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">sitePlan_link</td>
<td width="8%">Link to an online version of the document</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">sitePlan_name</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">sitePlan_name</td>
<td width="8%">Name of the document.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">sitePlan_type</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">sitePlan_type</td>
<td width="8%">Type of the Document. Either DocumentCitation or LegislationCitation.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_description</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">status_description</td>
<td width="8%">Descriptive statement about the declared status.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_statusType</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">status_statusType</td>
<td width="8%">The state or condition of a technical component referring to a list of predefined potential values. The reference values are holded in the ConditionOfFacilityValue code list.</td>
<td width="8%"><a href="#DomainConditionOfFacilityValue_value">ConditionOfFacilityValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_statusType_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">status_statusType_href</td>
<td width="8%">URI from the INSPIRE code list register - ConditionOfFacilityValue <a href="https://inspire.ec.europa.eu/codelist/ConditionOfFacilityValue">https://inspire.ec.europa.eu/codelist/ConditionOfFacilityValue</a></td>
<td width="8%"><a href="#DomainConditionOfFacilityValue">ConditionOfFacilityValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_validFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">status_validFrom</td>
<td width="8%">The starting time of validity for a status type.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">status_validTo</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">status_validTo</td>
<td width="8%">The ending time of validity for a status type.</td>
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
<td width="8%">Thematic identifier to uniquely identify the spatial object.</td>
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
    <hr/><a name="DomainConditionOfFacilityValue"/>
<p><strong>ConditionOfFacilityValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">ConditionOfFacilityValue</td>
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
<td width="20%">http://inspire.ec.europa.eu/codelist/ConditionOfFacilityValue/functional</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ConditionOfFacilityValue/functional</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ConditionOfFacilityValue/projected</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ConditionOfFacilityValue/projected</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ConditionOfFacilityValue/underConstruction</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ConditionOfFacilityValue/underConstruction</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ConditionOfFacilityValue/disused</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ConditionOfFacilityValue/disused</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ConditionOfFacilityValue/decommissioned</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ConditionOfFacilityValue/decommissioned</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainConditionOfFacilityValue_value"/>
<p><strong>ConditionOfFacilityValue_value - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">ConditionOfFacilityValue_value</td>
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
<td width="20%">functional</td>
<td width="20%">functional</td>
</tr><tr>
<td width="20%">projected</td>
<td width="20%">projected</td>
</tr><tr>
<td width="20%">underConstruction</td>
<td width="20%">underConstruction</td>
</tr><tr>
<td width="20%">disused</td>
<td width="20%">disused</td>
</tr><tr>
<td width="20%">decommissioned</td>
<td width="20%">decommissioned</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainEconomicActivityValue"/>
<p><strong>EconomicActivityValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">EconomicActivityValue</td>
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
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.13</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.13</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.14</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.14</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.15</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.15</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.16</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.16</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.19</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.19</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.23</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.23</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.24</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.24</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.25</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.25</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.26</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.26</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.27</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.27</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.28</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.28</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.29</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.29</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.4</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.4</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.41</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.41</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.42</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.42</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.43</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.43</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.44</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.44</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.45</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.45</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.46</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.46</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.47</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.47</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.49</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.49</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.5</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.5</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.50</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.50</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.6</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.6</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.61</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.61</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.62</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.62</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.63</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.63</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.64</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.64</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.7</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.7</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.70</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.01.70</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.02</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.02</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.02.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.02.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.02.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.02.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.02.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.02.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.02.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.02.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.02.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.02.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.02.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.02.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.02.4</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.02.4</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.02.40</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.02.40</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.03</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.03</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.03.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.03.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.03.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.03.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.03.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.03.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.03.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.03.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.03.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.03.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.03.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/A.03.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.05</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.05</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.05.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.05.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.05.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.05.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.05.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.05.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.05.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.05.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.06</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.06</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.06.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.06.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.06.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.06.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.06.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.06.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.06.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.06.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.07</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.07</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.07.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.07.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.07.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.07.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.07.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.07.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.07.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.07.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.07.29</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.07.29</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.08</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.08</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.08.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.08.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.08.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.08.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.08.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.08.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.08.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.08.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.08.91</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.08.91</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.08.92</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.08.92</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.08.93</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.08.93</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.08.99</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.08.99</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.09</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.09</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.09.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.09.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.09.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.09.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.09.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.09.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.09.90</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/B.09.90</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.13</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.13</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.31</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.31</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.32</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.32</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.39</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.39</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.4</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.4</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.41</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.41</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.42</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.42</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.5</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.5</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.51</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.51</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.52</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.52</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.6</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.6</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.61</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.61</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.62</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.62</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.7</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.7</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.71</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.71</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.72</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.72</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.73</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.73</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.8</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.8</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.81</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.81</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.82</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.82</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.83</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.83</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.84</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.84</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.85</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.85</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.86</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.86</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.89</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.89</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.91</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.91</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.92</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.10.92</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.11.0</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.11.0</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.11.01</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.11.01</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.11.02</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.11.02</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.11.03</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.11.03</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.11.04</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.11.04</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.11.05</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.11.05</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.11.06</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.11.06</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.11.07</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.11.07</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.12.0</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.12.0</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.12.00</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.12.00</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.91</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.91</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.92</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.92</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.93</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.93</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.94</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.94</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.95</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.95</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.96</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.96</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.99</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.13.99</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.13</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.13</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.14</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.14</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.19</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.19</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.31</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.31</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.39</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.14.39</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.15</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.15</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.15.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.15.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.15.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.15.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.15.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.15.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.15.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.15.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.15.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.15.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.16</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.16</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.16.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.16.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.16.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.16.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.16.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.16.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.16.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.16.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.16.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.16.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.16.23</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.16.23</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.16.24</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.16.24</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.16.29</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.16.29</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17.23</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17.23</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17.24</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17.24</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17.29</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.17.29</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.18</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.18</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.18.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.18.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.18.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.18.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.18.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.18.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.18.13</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.18.13</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.18.14</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.18.14</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.18.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.18.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.18.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.18.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.19</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.19</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.19.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.19.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.19.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.19.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.19.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.19.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.19.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.19.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.13</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.13</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.14</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.14</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.15</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.15</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.16</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.16</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.17</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.17</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.4</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.4</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.41</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.41</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.42</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.42</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.5</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.5</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.51</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.51</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.52</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.52</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.53</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.53</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.59</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.59</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.6</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.6</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.60</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.20.60</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.21.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.21.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.21.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.21.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.21.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.21.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.21.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.21.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.22.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.22.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.22.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.22.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.22.19</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.22.19</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.22.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.22.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.22.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.22.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.22.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.22.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.22.23</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.22.23</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.22.29</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.22.29</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.13</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.13</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.14</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.14</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.19</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.19</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.31</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.31</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.32</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.32</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.4</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.4</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.41</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.41</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.42</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.42</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.43</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.43</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.44</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.44</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.49</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.49</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.5</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.5</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.51</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.51</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.52</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.52</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.6</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.6</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.61</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.61</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.62</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.62</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.63</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.63</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.64</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.64</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.65</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.65</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.69</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.69</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.7</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.7</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.70</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.70</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.91</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.91</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.99</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.23.99</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.31</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.31</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.32</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.32</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.33</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.33</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.34</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.34</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.4</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.4</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.41</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.41</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.42</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.42</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.43</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.43</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.44</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.44</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.45</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.45</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.46</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.46</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.5</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.5</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.51</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.51</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.52</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.52</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.53</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.53</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.54</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.24.54</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.29</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.29</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.4</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.4</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.40</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.40</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.5</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.5</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.50</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.50</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.6</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.6</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.61</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.61</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.62</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.62</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.7</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.7</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.71</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.71</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.72</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.72</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.73</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.73</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.91</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.91</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.92</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.92</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.93</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.93</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.94</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.94</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.99</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.25.99</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.4</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.4</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.40</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.40</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.5</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.5</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.51</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.51</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.52</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.52</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.6</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.6</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.60</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.60</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.7</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.7</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.70</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.70</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.8</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.8</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.80</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.26.80</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.31</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.31</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.32</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.32</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.33</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.33</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.4</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.4</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.40</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.40</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.5</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.5</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.51</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.51</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.52</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.52</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.90</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.27.90</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.13</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.13</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.14</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.14</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.15</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.15</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.23</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.23</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.24</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.24</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.25</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.25</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.29</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.29</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.4</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.4</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.41</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.41</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.49</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.49</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.91</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.91</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.92</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.92</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.93</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.93</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.94</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.94</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.95</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.95</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.96</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.96</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.99</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.28.99</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.29</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.29</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.29.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.29.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.29.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.29.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.29.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.29.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.29.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.29.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.29.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.29.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.29.31</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.29.31</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.29.32</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.29.32</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.4</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.4</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.40</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.40</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.91</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.91</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.92</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.92</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.99</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.30.99</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.31</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.31</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.31.0</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.31.0</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.31.01</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.31.01</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.31.02</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.31.02</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.31.03</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.31.03</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.31.09</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.31.09</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.13</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.13</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.4</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.4</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.40</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.40</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.5</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.5</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.50</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.50</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.91</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.91</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.99</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.32.99</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.13</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.13</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.14</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.14</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.15</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.15</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.16</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.16</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.17</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.17</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.19</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.19</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/C.33.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.13</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.13</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.14</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.14</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.23</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.23</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/D.35.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.36</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.36</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.36.0</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.36.0</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.36.00</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.36.00</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.37</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.37</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.37.0</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.37.0</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.37.00</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.37.00</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38.31</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38.31</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38.32</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.38.32</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.39</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.39</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.39.0</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.39.0</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.39.00</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/E.39.00</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.41</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.41</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.41.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.41.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.41.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.41.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.41.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.41.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.41.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.41.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.13</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.13</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.91</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.91</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.99</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.42.99</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.13</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.13</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.29</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.29</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.31</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.31</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.32</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.32</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.33</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.33</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.34</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.34</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.39</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.39</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.91</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.91</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.99</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/F.43.99</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.19</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.19</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.31</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.31</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.32</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.32</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.4</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.4</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.40</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.45.40</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.13</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.13</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.14</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.14</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.15</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.15</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.16</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.16</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.17</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.17</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.18</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.18</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.19</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.19</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.23</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.23</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.24</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.24</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.31</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.31</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.32</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.32</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.33</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.33</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.34</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.34</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.35</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.35</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.36</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.36</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.37</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.37</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.38</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.38</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.39</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.39</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.4</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.4</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.41</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.41</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.42</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.42</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.43</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.43</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.44</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.44</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.45</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.45</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.46</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.46</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.47</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.47</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.48</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.48</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.49</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.49</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.5</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.5</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.51</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.51</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.52</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.52</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.6</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.6</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.61</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.61</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.62</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.62</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.63</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.63</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.64</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.64</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.65</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.65</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.66</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.66</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.69</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.69</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.7</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.7</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.71</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.71</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.72</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.72</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.73</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.73</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.74</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.74</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.75</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.75</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.76</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.76</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.77</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.77</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.90</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.46.90</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.19</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.19</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.23</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.23</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.24</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.24</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.25</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.25</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.26</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.26</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.29</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.29</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.4</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.4</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.41</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.41</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.42</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.42</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.43</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.43</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.5</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.5</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.51</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.51</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.52</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.52</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.53</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.53</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.54</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.54</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.59</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.59</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.6</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.6</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.61</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.61</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.62</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.62</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.63</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.63</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.64</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.64</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.65</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.65</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.7</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.7</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.71</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.71</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.72</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.72</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.73</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.73</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.74</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.74</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.75</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.75</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.76</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.76</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.77</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.77</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.78</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.78</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.79</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.79</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.8</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.8</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.81</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.81</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.82</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.82</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.89</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.89</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.91</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.91</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.99</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/G.47.99</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.31</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.31</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.32</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.32</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.39</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.39</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.4</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.4</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.41</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.41</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.42</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.42</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.5</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.5</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.50</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.49.50</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.50</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.50</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.50.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.50.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.50.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.50.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.50.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.50.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.50.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.50.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.50.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.50.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.50.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.50.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.50.4</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.50.4</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.50.40</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.50.40</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.51</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.51</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.51.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.51.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.51.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.51.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.51.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.51.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.51.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.51.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.51.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.51.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.52</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.52</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.52.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.52.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.52.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.52.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.52.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.52.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.52.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.52.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.52.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.52.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.52.23</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.52.23</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.52.24</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.52.24</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.52.29</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.52.29</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.53</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.53</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.53.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.53.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.53.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.53.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.53.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.53.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.53.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/H.53.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.55</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.55</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.55.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.55.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.55.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.55.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.55.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.55.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.55.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.55.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.55.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.55.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.55.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.55.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.55.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.55.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.55.90</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.55.90</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.56</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.56</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.56.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.56.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.56.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.56.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.56.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.56.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.56.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.56.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.56.29</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.56.29</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.56.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.56.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.56.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/I.56.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58.13</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58.13</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58.14</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58.14</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58.19</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58.19</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58.29</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.58.29</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.59</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.59</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.59.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.59.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.59.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.59.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.59.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.59.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.59.13</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.59.13</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.59.14</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.59.14</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.59.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.59.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.59.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.59.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.60</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.60</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.60.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.60.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.60.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.60.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.60.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.60.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.60.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.60.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.61</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.61</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.61.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.61.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.61.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.61.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.61.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.61.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.61.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.61.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.61.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.61.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.61.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.61.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.61.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.61.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.61.90</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.61.90</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.62</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.62</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.62.0</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.62.0</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.62.01</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.62.01</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.62.02</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.62.02</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.62.03</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.62.03</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.62.09</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.62.09</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.63</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.63</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.63.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.63.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.63.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.63.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.63.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.63.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.63.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.63.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.63.91</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.63.91</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.63.99</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/J.63.99</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.19</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.19</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.91</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.91</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.92</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.92</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.99</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.64.99</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.65</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.65</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.65.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.65.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.65.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.65.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.65.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.65.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.65.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.65.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.65.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.65.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.65.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.65.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.65.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.65.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.19</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.19</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.29</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.29</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/K.66.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/L</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/L</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/L.68</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/L.68</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/L.68.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/L.68.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/L.68.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/L.68.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/L.68.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/L.68.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/L.68.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/L.68.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/L.68.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/L.68.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/L.68.31</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/L.68.31</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/L.68.32</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/L.68.32</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.69</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.69</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.69.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.69.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.69.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.69.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.69.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.69.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.69.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.69.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.70</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.70</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.70.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.70.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.70.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.70.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.70.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.70.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.70.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.70.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.70.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.70.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.71</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.71</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.71.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.71.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.71.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.71.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.71.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.71.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.71.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.71.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.71.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.71.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.72</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.72</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.72.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.72.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.72.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.72.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.72.19</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.72.19</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.72.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.72.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.72.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.72.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.73</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.73</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.73.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.73.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.73.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.73.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.73.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.73.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.73.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.73.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.73.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.73.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.74</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.74</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.74.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.74.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.74.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.74.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.74.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.74.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.74.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.74.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.74.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.74.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.74.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.74.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.74.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.74.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.74.90</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.74.90</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.75</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.75</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.75.0</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.75.0</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.75.00</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/M.75.00</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.29</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.29</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.31</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.31</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.32</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.32</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.33</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.33</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.34</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.34</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.35</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.35</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.39</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.39</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.4</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.4</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.40</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.77.40</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.78</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.78</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.78.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.78.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.78.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.78.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.78.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.78.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.78.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.78.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.78.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.78.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.78.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.78.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.79</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.79</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.79.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.79.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.79.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.79.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.79.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.79.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.79.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.79.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.79.90</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.79.90</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.80</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.80</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.80.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.80.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.80.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.80.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.80.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.80.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.80.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.80.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.80.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.80.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.80.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.80.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.81</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.81</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.81.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.81.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.81.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.81.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.81.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.81.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.81.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.81.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.81.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.81.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.81.29</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.81.29</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.81.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.81.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.81.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.81.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.19</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.19</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.91</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.91</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.92</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.92</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.99</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/N.82.99</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.13</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.13</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.23</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.23</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.24</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.24</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.25</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.25</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/O.84.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.31</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.31</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.32</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.32</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.4</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.4</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.41</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.41</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.42</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.42</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.5</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.5</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.51</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.51</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.52</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.52</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.53</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.53</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.59</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.59</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.6</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.6</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.60</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/P.85.60</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.86</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.86</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.86.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.86.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.86.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.86.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.86.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.86.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.86.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.86.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.86.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.86.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.86.23</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.86.23</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.86.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.86.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.86.90</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.86.90</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.87</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.87</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.87.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.87.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.87.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.87.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.87.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.87.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.87.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.87.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.87.3</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.87.3</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.87.30</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.87.30</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.87.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.87.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.87.90</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.87.90</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.88</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.88</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.88.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.88.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.88.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.88.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.88.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.88.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.88.91</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.88.91</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.88.99</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/Q.88.99</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.90</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.90</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.90.0</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.90.0</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.90.01</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.90.01</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.90.02</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.90.02</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.90.03</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.90.03</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.90.04</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.90.04</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.91</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.91</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.91.0</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.91.0</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.91.01</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.91.01</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.91.02</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.91.02</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.91.03</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.91.03</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.91.04</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.91.04</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.92</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.92</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.92.0</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.92.0</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.92.00</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.92.00</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.93</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.93</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.93.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.93.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.93.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.93.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.93.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.93.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.93.13</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.93.13</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.93.19</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.93.19</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.93.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.93.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.93.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.93.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.93.29</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/R.93.29</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94.9</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94.9</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94.91</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94.91</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94.92</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94.92</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94.99</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.94.99</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.11</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.11</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.12</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.12</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.21</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.21</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.22</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.22</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.23</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.23</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.24</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.24</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.25</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.25</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.29</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.95.29</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.96</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.96</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.96.0</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.96.0</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.96.01</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.96.01</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.96.02</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.96.02</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.96.03</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.96.03</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.96.04</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.96.04</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.96.09</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/S.96.09</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/T</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/T</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/T.97</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/T.97</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/T.97.0</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/T.97.0</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/T.97.00</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/T.97.00</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/T.98</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/T.98</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/T.98.1</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/T.98.1</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/T.98.10</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/T.98.10</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/T.98.2</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/T.98.2</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/T.98.20</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/T.98.20</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/U</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/U</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/U.99</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/U.99</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/U.99.0</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/U.99.0</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/U.99.00</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/EconomicActivityNACEValue/U.99.00</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainEconomicActivityValue_value"/>
<p><strong>EconomicActivityValue_value - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">EconomicActivityValue_value</td>
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
<td width="20%">A</td>
<td width="20%">A</td>
</tr><tr>
<td width="20%">A.01</td>
<td width="20%">A.01</td>
</tr><tr>
<td width="20%">A.01.1</td>
<td width="20%">A.01.1</td>
</tr><tr>
<td width="20%">A.01.11</td>
<td width="20%">A.01.11</td>
</tr><tr>
<td width="20%">A.01.12</td>
<td width="20%">A.01.12</td>
</tr><tr>
<td width="20%">A.01.13</td>
<td width="20%">A.01.13</td>
</tr><tr>
<td width="20%">A.01.14</td>
<td width="20%">A.01.14</td>
</tr><tr>
<td width="20%">A.01.15</td>
<td width="20%">A.01.15</td>
</tr><tr>
<td width="20%">A.01.16</td>
<td width="20%">A.01.16</td>
</tr><tr>
<td width="20%">A.01.19</td>
<td width="20%">A.01.19</td>
</tr><tr>
<td width="20%">A.01.2</td>
<td width="20%">A.01.2</td>
</tr><tr>
<td width="20%">A.01.21</td>
<td width="20%">A.01.21</td>
</tr><tr>
<td width="20%">A.01.22</td>
<td width="20%">A.01.22</td>
</tr><tr>
<td width="20%">A.01.23</td>
<td width="20%">A.01.23</td>
</tr><tr>
<td width="20%">A.01.24</td>
<td width="20%">A.01.24</td>
</tr><tr>
<td width="20%">A.01.25</td>
<td width="20%">A.01.25</td>
</tr><tr>
<td width="20%">A.01.26</td>
<td width="20%">A.01.26</td>
</tr><tr>
<td width="20%">A.01.27</td>
<td width="20%">A.01.27</td>
</tr><tr>
<td width="20%">A.01.28</td>
<td width="20%">A.01.28</td>
</tr><tr>
<td width="20%">A.01.29</td>
<td width="20%">A.01.29</td>
</tr><tr>
<td width="20%">A.01.3</td>
<td width="20%">A.01.3</td>
</tr><tr>
<td width="20%">A.01.30</td>
<td width="20%">A.01.30</td>
</tr><tr>
<td width="20%">A.01.4</td>
<td width="20%">A.01.4</td>
</tr><tr>
<td width="20%">A.01.41</td>
<td width="20%">A.01.41</td>
</tr><tr>
<td width="20%">A.01.42</td>
<td width="20%">A.01.42</td>
</tr><tr>
<td width="20%">A.01.43</td>
<td width="20%">A.01.43</td>
</tr><tr>
<td width="20%">A.01.44</td>
<td width="20%">A.01.44</td>
</tr><tr>
<td width="20%">A.01.45</td>
<td width="20%">A.01.45</td>
</tr><tr>
<td width="20%">A.01.46</td>
<td width="20%">A.01.46</td>
</tr><tr>
<td width="20%">A.01.47</td>
<td width="20%">A.01.47</td>
</tr><tr>
<td width="20%">A.01.49</td>
<td width="20%">A.01.49</td>
</tr><tr>
<td width="20%">A.01.5</td>
<td width="20%">A.01.5</td>
</tr><tr>
<td width="20%">A.01.50</td>
<td width="20%">A.01.50</td>
</tr><tr>
<td width="20%">A.01.6</td>
<td width="20%">A.01.6</td>
</tr><tr>
<td width="20%">A.01.61</td>
<td width="20%">A.01.61</td>
</tr><tr>
<td width="20%">A.01.62</td>
<td width="20%">A.01.62</td>
</tr><tr>
<td width="20%">A.01.63</td>
<td width="20%">A.01.63</td>
</tr><tr>
<td width="20%">A.01.64</td>
<td width="20%">A.01.64</td>
</tr><tr>
<td width="20%">A.01.7</td>
<td width="20%">A.01.7</td>
</tr><tr>
<td width="20%">A.01.70</td>
<td width="20%">A.01.70</td>
</tr><tr>
<td width="20%">A.02</td>
<td width="20%">A.02</td>
</tr><tr>
<td width="20%">A.02.1</td>
<td width="20%">A.02.1</td>
</tr><tr>
<td width="20%">A.02.10</td>
<td width="20%">A.02.10</td>
</tr><tr>
<td width="20%">A.02.2</td>
<td width="20%">A.02.2</td>
</tr><tr>
<td width="20%">A.02.20</td>
<td width="20%">A.02.20</td>
</tr><tr>
<td width="20%">A.02.3</td>
<td width="20%">A.02.3</td>
</tr><tr>
<td width="20%">A.02.30</td>
<td width="20%">A.02.30</td>
</tr><tr>
<td width="20%">A.02.4</td>
<td width="20%">A.02.4</td>
</tr><tr>
<td width="20%">A.02.40</td>
<td width="20%">A.02.40</td>
</tr><tr>
<td width="20%">A.03</td>
<td width="20%">A.03</td>
</tr><tr>
<td width="20%">A.03.1</td>
<td width="20%">A.03.1</td>
</tr><tr>
<td width="20%">A.03.11</td>
<td width="20%">A.03.11</td>
</tr><tr>
<td width="20%">A.03.12</td>
<td width="20%">A.03.12</td>
</tr><tr>
<td width="20%">A.03.2</td>
<td width="20%">A.03.2</td>
</tr><tr>
<td width="20%">A.03.21</td>
<td width="20%">A.03.21</td>
</tr><tr>
<td width="20%">A.03.22</td>
<td width="20%">A.03.22</td>
</tr><tr>
<td width="20%">B</td>
<td width="20%">B</td>
</tr><tr>
<td width="20%">B.05</td>
<td width="20%">B.05</td>
</tr><tr>
<td width="20%">B.05.1</td>
<td width="20%">B.05.1</td>
</tr><tr>
<td width="20%">B.05.10</td>
<td width="20%">B.05.10</td>
</tr><tr>
<td width="20%">B.05.2</td>
<td width="20%">B.05.2</td>
</tr><tr>
<td width="20%">B.05.20</td>
<td width="20%">B.05.20</td>
</tr><tr>
<td width="20%">B.06</td>
<td width="20%">B.06</td>
</tr><tr>
<td width="20%">B.06.1</td>
<td width="20%">B.06.1</td>
</tr><tr>
<td width="20%">B.06.10</td>
<td width="20%">B.06.10</td>
</tr><tr>
<td width="20%">B.06.2</td>
<td width="20%">B.06.2</td>
</tr><tr>
<td width="20%">B.06.20</td>
<td width="20%">B.06.20</td>
</tr><tr>
<td width="20%">B.07</td>
<td width="20%">B.07</td>
</tr><tr>
<td width="20%">B.07.1</td>
<td width="20%">B.07.1</td>
</tr><tr>
<td width="20%">B.07.10</td>
<td width="20%">B.07.10</td>
</tr><tr>
<td width="20%">B.07.2</td>
<td width="20%">B.07.2</td>
</tr><tr>
<td width="20%">B.07.21</td>
<td width="20%">B.07.21</td>
</tr><tr>
<td width="20%">B.07.29</td>
<td width="20%">B.07.29</td>
</tr><tr>
<td width="20%">B.08</td>
<td width="20%">B.08</td>
</tr><tr>
<td width="20%">B.08.1</td>
<td width="20%">B.08.1</td>
</tr><tr>
<td width="20%">B.08.11</td>
<td width="20%">B.08.11</td>
</tr><tr>
<td width="20%">B.08.12</td>
<td width="20%">B.08.12</td>
</tr><tr>
<td width="20%">B.08.9</td>
<td width="20%">B.08.9</td>
</tr><tr>
<td width="20%">B.08.91</td>
<td width="20%">B.08.91</td>
</tr><tr>
<td width="20%">B.08.92</td>
<td width="20%">B.08.92</td>
</tr><tr>
<td width="20%">B.08.93</td>
<td width="20%">B.08.93</td>
</tr><tr>
<td width="20%">B.08.99</td>
<td width="20%">B.08.99</td>
</tr><tr>
<td width="20%">B.09</td>
<td width="20%">B.09</td>
</tr><tr>
<td width="20%">B.09.1</td>
<td width="20%">B.09.1</td>
</tr><tr>
<td width="20%">B.09.10</td>
<td width="20%">B.09.10</td>
</tr><tr>
<td width="20%">B.09.9</td>
<td width="20%">B.09.9</td>
</tr><tr>
<td width="20%">B.09.90</td>
<td width="20%">B.09.90</td>
</tr><tr>
<td width="20%">C</td>
<td width="20%">C</td>
</tr><tr>
<td width="20%">C.10</td>
<td width="20%">C.10</td>
</tr><tr>
<td width="20%">C.10.1</td>
<td width="20%">C.10.1</td>
</tr><tr>
<td width="20%">C.10.11</td>
<td width="20%">C.10.11</td>
</tr><tr>
<td width="20%">C.10.12</td>
<td width="20%">C.10.12</td>
</tr><tr>
<td width="20%">C.10.13</td>
<td width="20%">C.10.13</td>
</tr><tr>
<td width="20%">C.10.2</td>
<td width="20%">C.10.2</td>
</tr><tr>
<td width="20%">C.10.20</td>
<td width="20%">C.10.20</td>
</tr><tr>
<td width="20%">C.10.3</td>
<td width="20%">C.10.3</td>
</tr><tr>
<td width="20%">C.10.31</td>
<td width="20%">C.10.31</td>
</tr><tr>
<td width="20%">C.10.32</td>
<td width="20%">C.10.32</td>
</tr><tr>
<td width="20%">C.10.39</td>
<td width="20%">C.10.39</td>
</tr><tr>
<td width="20%">C.10.4</td>
<td width="20%">C.10.4</td>
</tr><tr>
<td width="20%">C.10.41</td>
<td width="20%">C.10.41</td>
</tr><tr>
<td width="20%">C.10.42</td>
<td width="20%">C.10.42</td>
</tr><tr>
<td width="20%">C.10.5</td>
<td width="20%">C.10.5</td>
</tr><tr>
<td width="20%">C.10.51</td>
<td width="20%">C.10.51</td>
</tr><tr>
<td width="20%">C.10.52</td>
<td width="20%">C.10.52</td>
</tr><tr>
<td width="20%">C.10.6</td>
<td width="20%">C.10.6</td>
</tr><tr>
<td width="20%">C.10.61</td>
<td width="20%">C.10.61</td>
</tr><tr>
<td width="20%">C.10.62</td>
<td width="20%">C.10.62</td>
</tr><tr>
<td width="20%">C.10.7</td>
<td width="20%">C.10.7</td>
</tr><tr>
<td width="20%">C.10.71</td>
<td width="20%">C.10.71</td>
</tr><tr>
<td width="20%">C.10.72</td>
<td width="20%">C.10.72</td>
</tr><tr>
<td width="20%">C.10.73</td>
<td width="20%">C.10.73</td>
</tr><tr>
<td width="20%">C.10.8</td>
<td width="20%">C.10.8</td>
</tr><tr>
<td width="20%">C.10.81</td>
<td width="20%">C.10.81</td>
</tr><tr>
<td width="20%">C.10.82</td>
<td width="20%">C.10.82</td>
</tr><tr>
<td width="20%">C.10.83</td>
<td width="20%">C.10.83</td>
</tr><tr>
<td width="20%">C.10.84</td>
<td width="20%">C.10.84</td>
</tr><tr>
<td width="20%">C.10.85</td>
<td width="20%">C.10.85</td>
</tr><tr>
<td width="20%">C.10.86</td>
<td width="20%">C.10.86</td>
</tr><tr>
<td width="20%">C.10.89</td>
<td width="20%">C.10.89</td>
</tr><tr>
<td width="20%">C.10.9</td>
<td width="20%">C.10.9</td>
</tr><tr>
<td width="20%">C.10.91</td>
<td width="20%">C.10.91</td>
</tr><tr>
<td width="20%">C.10.92</td>
<td width="20%">C.10.92</td>
</tr><tr>
<td width="20%">C.11</td>
<td width="20%">C.11</td>
</tr><tr>
<td width="20%">C.11.0</td>
<td width="20%">C.11.0</td>
</tr><tr>
<td width="20%">C.11.01</td>
<td width="20%">C.11.01</td>
</tr><tr>
<td width="20%">C.11.02</td>
<td width="20%">C.11.02</td>
</tr><tr>
<td width="20%">C.11.03</td>
<td width="20%">C.11.03</td>
</tr><tr>
<td width="20%">C.11.04</td>
<td width="20%">C.11.04</td>
</tr><tr>
<td width="20%">C.11.05</td>
<td width="20%">C.11.05</td>
</tr><tr>
<td width="20%">C.11.06</td>
<td width="20%">C.11.06</td>
</tr><tr>
<td width="20%">C.11.07</td>
<td width="20%">C.11.07</td>
</tr><tr>
<td width="20%">C.12</td>
<td width="20%">C.12</td>
</tr><tr>
<td width="20%">C.12.0</td>
<td width="20%">C.12.0</td>
</tr><tr>
<td width="20%">C.12.00</td>
<td width="20%">C.12.00</td>
</tr><tr>
<td width="20%">C.13</td>
<td width="20%">C.13</td>
</tr><tr>
<td width="20%">C.13.1</td>
<td width="20%">C.13.1</td>
</tr><tr>
<td width="20%">C.13.10</td>
<td width="20%">C.13.10</td>
</tr><tr>
<td width="20%">C.13.2</td>
<td width="20%">C.13.2</td>
</tr><tr>
<td width="20%">C.13.20</td>
<td width="20%">C.13.20</td>
</tr><tr>
<td width="20%">C.13.3</td>
<td width="20%">C.13.3</td>
</tr><tr>
<td width="20%">C.13.30</td>
<td width="20%">C.13.30</td>
</tr><tr>
<td width="20%">C.13.9</td>
<td width="20%">C.13.9</td>
</tr><tr>
<td width="20%">C.13.91</td>
<td width="20%">C.13.91</td>
</tr><tr>
<td width="20%">C.13.92</td>
<td width="20%">C.13.92</td>
</tr><tr>
<td width="20%">C.13.93</td>
<td width="20%">C.13.93</td>
</tr><tr>
<td width="20%">C.13.94</td>
<td width="20%">C.13.94</td>
</tr><tr>
<td width="20%">C.13.95</td>
<td width="20%">C.13.95</td>
</tr><tr>
<td width="20%">C.13.96</td>
<td width="20%">C.13.96</td>
</tr><tr>
<td width="20%">C.13.99</td>
<td width="20%">C.13.99</td>
</tr><tr>
<td width="20%">C.14</td>
<td width="20%">C.14</td>
</tr><tr>
<td width="20%">C.14.1</td>
<td width="20%">C.14.1</td>
</tr><tr>
<td width="20%">C.14.11</td>
<td width="20%">C.14.11</td>
</tr><tr>
<td width="20%">C.14.12</td>
<td width="20%">C.14.12</td>
</tr><tr>
<td width="20%">C.14.13</td>
<td width="20%">C.14.13</td>
</tr><tr>
<td width="20%">C.14.14</td>
<td width="20%">C.14.14</td>
</tr><tr>
<td width="20%">C.14.19</td>
<td width="20%">C.14.19</td>
</tr><tr>
<td width="20%">C.14.2</td>
<td width="20%">C.14.2</td>
</tr><tr>
<td width="20%">C.14.20</td>
<td width="20%">C.14.20</td>
</tr><tr>
<td width="20%">C.14.3</td>
<td width="20%">C.14.3</td>
</tr><tr>
<td width="20%">C.14.31</td>
<td width="20%">C.14.31</td>
</tr><tr>
<td width="20%">C.14.39</td>
<td width="20%">C.14.39</td>
</tr><tr>
<td width="20%">C.15</td>
<td width="20%">C.15</td>
</tr><tr>
<td width="20%">C.15.1</td>
<td width="20%">C.15.1</td>
</tr><tr>
<td width="20%">C.15.11</td>
<td width="20%">C.15.11</td>
</tr><tr>
<td width="20%">C.15.12</td>
<td width="20%">C.15.12</td>
</tr><tr>
<td width="20%">C.15.2</td>
<td width="20%">C.15.2</td>
</tr><tr>
<td width="20%">C.15.20</td>
<td width="20%">C.15.20</td>
</tr><tr>
<td width="20%">C.16</td>
<td width="20%">C.16</td>
</tr><tr>
<td width="20%">C.16.1</td>
<td width="20%">C.16.1</td>
</tr><tr>
<td width="20%">C.16.10</td>
<td width="20%">C.16.10</td>
</tr><tr>
<td width="20%">C.16.2</td>
<td width="20%">C.16.2</td>
</tr><tr>
<td width="20%">C.16.21</td>
<td width="20%">C.16.21</td>
</tr><tr>
<td width="20%">C.16.22</td>
<td width="20%">C.16.22</td>
</tr><tr>
<td width="20%">C.16.23</td>
<td width="20%">C.16.23</td>
</tr><tr>
<td width="20%">C.16.24</td>
<td width="20%">C.16.24</td>
</tr><tr>
<td width="20%">C.16.29</td>
<td width="20%">C.16.29</td>
</tr><tr>
<td width="20%">C.17</td>
<td width="20%">C.17</td>
</tr><tr>
<td width="20%">C.17.1</td>
<td width="20%">C.17.1</td>
</tr><tr>
<td width="20%">C.17.11</td>
<td width="20%">C.17.11</td>
</tr><tr>
<td width="20%">C.17.12</td>
<td width="20%">C.17.12</td>
</tr><tr>
<td width="20%">C.17.2</td>
<td width="20%">C.17.2</td>
</tr><tr>
<td width="20%">C.17.21</td>
<td width="20%">C.17.21</td>
</tr><tr>
<td width="20%">C.17.22</td>
<td width="20%">C.17.22</td>
</tr><tr>
<td width="20%">C.17.23</td>
<td width="20%">C.17.23</td>
</tr><tr>
<td width="20%">C.17.24</td>
<td width="20%">C.17.24</td>
</tr><tr>
<td width="20%">C.17.29</td>
<td width="20%">C.17.29</td>
</tr><tr>
<td width="20%">C.18</td>
<td width="20%">C.18</td>
</tr><tr>
<td width="20%">C.18.1</td>
<td width="20%">C.18.1</td>
</tr><tr>
<td width="20%">C.18.11</td>
<td width="20%">C.18.11</td>
</tr><tr>
<td width="20%">C.18.12</td>
<td width="20%">C.18.12</td>
</tr><tr>
<td width="20%">C.18.13</td>
<td width="20%">C.18.13</td>
</tr><tr>
<td width="20%">C.18.14</td>
<td width="20%">C.18.14</td>
</tr><tr>
<td width="20%">C.18.2</td>
<td width="20%">C.18.2</td>
</tr><tr>
<td width="20%">C.18.20</td>
<td width="20%">C.18.20</td>
</tr><tr>
<td width="20%">C.19</td>
<td width="20%">C.19</td>
</tr><tr>
<td width="20%">C.19.1</td>
<td width="20%">C.19.1</td>
</tr><tr>
<td width="20%">C.19.10</td>
<td width="20%">C.19.10</td>
</tr><tr>
<td width="20%">C.19.2</td>
<td width="20%">C.19.2</td>
</tr><tr>
<td width="20%">C.19.20</td>
<td width="20%">C.19.20</td>
</tr><tr>
<td width="20%">C.20</td>
<td width="20%">C.20</td>
</tr><tr>
<td width="20%">C.20.1</td>
<td width="20%">C.20.1</td>
</tr><tr>
<td width="20%">C.20.11</td>
<td width="20%">C.20.11</td>
</tr><tr>
<td width="20%">C.20.12</td>
<td width="20%">C.20.12</td>
</tr><tr>
<td width="20%">C.20.13</td>
<td width="20%">C.20.13</td>
</tr><tr>
<td width="20%">C.20.14</td>
<td width="20%">C.20.14</td>
</tr><tr>
<td width="20%">C.20.15</td>
<td width="20%">C.20.15</td>
</tr><tr>
<td width="20%">C.20.16</td>
<td width="20%">C.20.16</td>
</tr><tr>
<td width="20%">C.20.17</td>
<td width="20%">C.20.17</td>
</tr><tr>
<td width="20%">C.20.2</td>
<td width="20%">C.20.2</td>
</tr><tr>
<td width="20%">C.20.20</td>
<td width="20%">C.20.20</td>
</tr><tr>
<td width="20%">C.20.3</td>
<td width="20%">C.20.3</td>
</tr><tr>
<td width="20%">C.20.30</td>
<td width="20%">C.20.30</td>
</tr><tr>
<td width="20%">C.20.4</td>
<td width="20%">C.20.4</td>
</tr><tr>
<td width="20%">C.20.41</td>
<td width="20%">C.20.41</td>
</tr><tr>
<td width="20%">C.20.42</td>
<td width="20%">C.20.42</td>
</tr><tr>
<td width="20%">C.20.5</td>
<td width="20%">C.20.5</td>
</tr><tr>
<td width="20%">C.20.51</td>
<td width="20%">C.20.51</td>
</tr><tr>
<td width="20%">C.20.52</td>
<td width="20%">C.20.52</td>
</tr><tr>
<td width="20%">C.20.53</td>
<td width="20%">C.20.53</td>
</tr><tr>
<td width="20%">C.20.59</td>
<td width="20%">C.20.59</td>
</tr><tr>
<td width="20%">C.20.6</td>
<td width="20%">C.20.6</td>
</tr><tr>
<td width="20%">C.20.60</td>
<td width="20%">C.20.60</td>
</tr><tr>
<td width="20%">C.21</td>
<td width="20%">C.21</td>
</tr><tr>
<td width="20%">C.21.1</td>
<td width="20%">C.21.1</td>
</tr><tr>
<td width="20%">C.21.10</td>
<td width="20%">C.21.10</td>
</tr><tr>
<td width="20%">C.21.2</td>
<td width="20%">C.21.2</td>
</tr><tr>
<td width="20%">C.21.20</td>
<td width="20%">C.21.20</td>
</tr><tr>
<td width="20%">C.22</td>
<td width="20%">C.22</td>
</tr><tr>
<td width="20%">C.22.1</td>
<td width="20%">C.22.1</td>
</tr><tr>
<td width="20%">C.22.11</td>
<td width="20%">C.22.11</td>
</tr><tr>
<td width="20%">C.22.19</td>
<td width="20%">C.22.19</td>
</tr><tr>
<td width="20%">C.22.2</td>
<td width="20%">C.22.2</td>
</tr><tr>
<td width="20%">C.22.21</td>
<td width="20%">C.22.21</td>
</tr><tr>
<td width="20%">C.22.22</td>
<td width="20%">C.22.22</td>
</tr><tr>
<td width="20%">C.22.23</td>
<td width="20%">C.22.23</td>
</tr><tr>
<td width="20%">C.22.29</td>
<td width="20%">C.22.29</td>
</tr><tr>
<td width="20%">C.23</td>
<td width="20%">C.23</td>
</tr><tr>
<td width="20%">C.23.1</td>
<td width="20%">C.23.1</td>
</tr><tr>
<td width="20%">C.23.11</td>
<td width="20%">C.23.11</td>
</tr><tr>
<td width="20%">C.23.12</td>
<td width="20%">C.23.12</td>
</tr><tr>
<td width="20%">C.23.13</td>
<td width="20%">C.23.13</td>
</tr><tr>
<td width="20%">C.23.14</td>
<td width="20%">C.23.14</td>
</tr><tr>
<td width="20%">C.23.19</td>
<td width="20%">C.23.19</td>
</tr><tr>
<td width="20%">C.23.2</td>
<td width="20%">C.23.2</td>
</tr><tr>
<td width="20%">C.23.20</td>
<td width="20%">C.23.20</td>
</tr><tr>
<td width="20%">C.23.3</td>
<td width="20%">C.23.3</td>
</tr><tr>
<td width="20%">C.23.31</td>
<td width="20%">C.23.31</td>
</tr><tr>
<td width="20%">C.23.32</td>
<td width="20%">C.23.32</td>
</tr><tr>
<td width="20%">C.23.4</td>
<td width="20%">C.23.4</td>
</tr><tr>
<td width="20%">C.23.41</td>
<td width="20%">C.23.41</td>
</tr><tr>
<td width="20%">C.23.42</td>
<td width="20%">C.23.42</td>
</tr><tr>
<td width="20%">C.23.43</td>
<td width="20%">C.23.43</td>
</tr><tr>
<td width="20%">C.23.44</td>
<td width="20%">C.23.44</td>
</tr><tr>
<td width="20%">C.23.49</td>
<td width="20%">C.23.49</td>
</tr><tr>
<td width="20%">C.23.5</td>
<td width="20%">C.23.5</td>
</tr><tr>
<td width="20%">C.23.51</td>
<td width="20%">C.23.51</td>
</tr><tr>
<td width="20%">C.23.52</td>
<td width="20%">C.23.52</td>
</tr><tr>
<td width="20%">C.23.6</td>
<td width="20%">C.23.6</td>
</tr><tr>
<td width="20%">C.23.61</td>
<td width="20%">C.23.61</td>
</tr><tr>
<td width="20%">C.23.62</td>
<td width="20%">C.23.62</td>
</tr><tr>
<td width="20%">C.23.63</td>
<td width="20%">C.23.63</td>
</tr><tr>
<td width="20%">C.23.64</td>
<td width="20%">C.23.64</td>
</tr><tr>
<td width="20%">C.23.65</td>
<td width="20%">C.23.65</td>
</tr><tr>
<td width="20%">C.23.69</td>
<td width="20%">C.23.69</td>
</tr><tr>
<td width="20%">C.23.7</td>
<td width="20%">C.23.7</td>
</tr><tr>
<td width="20%">C.23.70</td>
<td width="20%">C.23.70</td>
</tr><tr>
<td width="20%">C.23.9</td>
<td width="20%">C.23.9</td>
</tr><tr>
<td width="20%">C.23.91</td>
<td width="20%">C.23.91</td>
</tr><tr>
<td width="20%">C.23.99</td>
<td width="20%">C.23.99</td>
</tr><tr>
<td width="20%">C.24</td>
<td width="20%">C.24</td>
</tr><tr>
<td width="20%">C.24.1</td>
<td width="20%">C.24.1</td>
</tr><tr>
<td width="20%">C.24.10</td>
<td width="20%">C.24.10</td>
</tr><tr>
<td width="20%">C.24.2</td>
<td width="20%">C.24.2</td>
</tr><tr>
<td width="20%">C.24.20</td>
<td width="20%">C.24.20</td>
</tr><tr>
<td width="20%">C.24.3</td>
<td width="20%">C.24.3</td>
</tr><tr>
<td width="20%">C.24.31</td>
<td width="20%">C.24.31</td>
</tr><tr>
<td width="20%">C.24.32</td>
<td width="20%">C.24.32</td>
</tr><tr>
<td width="20%">C.24.33</td>
<td width="20%">C.24.33</td>
</tr><tr>
<td width="20%">C.24.34</td>
<td width="20%">C.24.34</td>
</tr><tr>
<td width="20%">C.24.4</td>
<td width="20%">C.24.4</td>
</tr><tr>
<td width="20%">C.24.41</td>
<td width="20%">C.24.41</td>
</tr><tr>
<td width="20%">C.24.42</td>
<td width="20%">C.24.42</td>
</tr><tr>
<td width="20%">C.24.43</td>
<td width="20%">C.24.43</td>
</tr><tr>
<td width="20%">C.24.44</td>
<td width="20%">C.24.44</td>
</tr><tr>
<td width="20%">C.24.45</td>
<td width="20%">C.24.45</td>
</tr><tr>
<td width="20%">C.24.46</td>
<td width="20%">C.24.46</td>
</tr><tr>
<td width="20%">C.24.5</td>
<td width="20%">C.24.5</td>
</tr><tr>
<td width="20%">C.24.51</td>
<td width="20%">C.24.51</td>
</tr><tr>
<td width="20%">C.24.52</td>
<td width="20%">C.24.52</td>
</tr><tr>
<td width="20%">C.24.53</td>
<td width="20%">C.24.53</td>
</tr><tr>
<td width="20%">C.24.54</td>
<td width="20%">C.24.54</td>
</tr><tr>
<td width="20%">C.25</td>
<td width="20%">C.25</td>
</tr><tr>
<td width="20%">C.25.1</td>
<td width="20%">C.25.1</td>
</tr><tr>
<td width="20%">C.25.11</td>
<td width="20%">C.25.11</td>
</tr><tr>
<td width="20%">C.25.12</td>
<td width="20%">C.25.12</td>
</tr><tr>
<td width="20%">C.25.2</td>
<td width="20%">C.25.2</td>
</tr><tr>
<td width="20%">C.25.21</td>
<td width="20%">C.25.21</td>
</tr><tr>
<td width="20%">C.25.29</td>
<td width="20%">C.25.29</td>
</tr><tr>
<td width="20%">C.25.3</td>
<td width="20%">C.25.3</td>
</tr><tr>
<td width="20%">C.25.30</td>
<td width="20%">C.25.30</td>
</tr><tr>
<td width="20%">C.25.4</td>
<td width="20%">C.25.4</td>
</tr><tr>
<td width="20%">C.25.40</td>
<td width="20%">C.25.40</td>
</tr><tr>
<td width="20%">C.25.5</td>
<td width="20%">C.25.5</td>
</tr><tr>
<td width="20%">C.25.50</td>
<td width="20%">C.25.50</td>
</tr><tr>
<td width="20%">C.25.6</td>
<td width="20%">C.25.6</td>
</tr><tr>
<td width="20%">C.25.61</td>
<td width="20%">C.25.61</td>
</tr><tr>
<td width="20%">C.25.62</td>
<td width="20%">C.25.62</td>
</tr><tr>
<td width="20%">C.25.7</td>
<td width="20%">C.25.7</td>
</tr><tr>
<td width="20%">C.25.71</td>
<td width="20%">C.25.71</td>
</tr><tr>
<td width="20%">C.25.72</td>
<td width="20%">C.25.72</td>
</tr><tr>
<td width="20%">C.25.73</td>
<td width="20%">C.25.73</td>
</tr><tr>
<td width="20%">C.25.9</td>
<td width="20%">C.25.9</td>
</tr><tr>
<td width="20%">C.25.91</td>
<td width="20%">C.25.91</td>
</tr><tr>
<td width="20%">C.25.92</td>
<td width="20%">C.25.92</td>
</tr><tr>
<td width="20%">C.25.93</td>
<td width="20%">C.25.93</td>
</tr><tr>
<td width="20%">C.25.94</td>
<td width="20%">C.25.94</td>
</tr><tr>
<td width="20%">C.25.99</td>
<td width="20%">C.25.99</td>
</tr><tr>
<td width="20%">C.26</td>
<td width="20%">C.26</td>
</tr><tr>
<td width="20%">C.26.1</td>
<td width="20%">C.26.1</td>
</tr><tr>
<td width="20%">C.26.11</td>
<td width="20%">C.26.11</td>
</tr><tr>
<td width="20%">C.26.12</td>
<td width="20%">C.26.12</td>
</tr><tr>
<td width="20%">C.26.2</td>
<td width="20%">C.26.2</td>
</tr><tr>
<td width="20%">C.26.20</td>
<td width="20%">C.26.20</td>
</tr><tr>
<td width="20%">C.26.3</td>
<td width="20%">C.26.3</td>
</tr><tr>
<td width="20%">C.26.30</td>
<td width="20%">C.26.30</td>
</tr><tr>
<td width="20%">C.26.4</td>
<td width="20%">C.26.4</td>
</tr><tr>
<td width="20%">C.26.40</td>
<td width="20%">C.26.40</td>
</tr><tr>
<td width="20%">C.26.5</td>
<td width="20%">C.26.5</td>
</tr><tr>
<td width="20%">C.26.51</td>
<td width="20%">C.26.51</td>
</tr><tr>
<td width="20%">C.26.52</td>
<td width="20%">C.26.52</td>
</tr><tr>
<td width="20%">C.26.6</td>
<td width="20%">C.26.6</td>
</tr><tr>
<td width="20%">C.26.60</td>
<td width="20%">C.26.60</td>
</tr><tr>
<td width="20%">C.26.7</td>
<td width="20%">C.26.7</td>
</tr><tr>
<td width="20%">C.26.70</td>
<td width="20%">C.26.70</td>
</tr><tr>
<td width="20%">C.26.8</td>
<td width="20%">C.26.8</td>
</tr><tr>
<td width="20%">C.26.80</td>
<td width="20%">C.26.80</td>
</tr><tr>
<td width="20%">C.27</td>
<td width="20%">C.27</td>
</tr><tr>
<td width="20%">C.27.1</td>
<td width="20%">C.27.1</td>
</tr><tr>
<td width="20%">C.27.11</td>
<td width="20%">C.27.11</td>
</tr><tr>
<td width="20%">C.27.12</td>
<td width="20%">C.27.12</td>
</tr><tr>
<td width="20%">C.27.2</td>
<td width="20%">C.27.2</td>
</tr><tr>
<td width="20%">C.27.20</td>
<td width="20%">C.27.20</td>
</tr><tr>
<td width="20%">C.27.3</td>
<td width="20%">C.27.3</td>
</tr><tr>
<td width="20%">C.27.31</td>
<td width="20%">C.27.31</td>
</tr><tr>
<td width="20%">C.27.32</td>
<td width="20%">C.27.32</td>
</tr><tr>
<td width="20%">C.27.33</td>
<td width="20%">C.27.33</td>
</tr><tr>
<td width="20%">C.27.4</td>
<td width="20%">C.27.4</td>
</tr><tr>
<td width="20%">C.27.40</td>
<td width="20%">C.27.40</td>
</tr><tr>
<td width="20%">C.27.5</td>
<td width="20%">C.27.5</td>
</tr><tr>
<td width="20%">C.27.51</td>
<td width="20%">C.27.51</td>
</tr><tr>
<td width="20%">C.27.52</td>
<td width="20%">C.27.52</td>
</tr><tr>
<td width="20%">C.27.9</td>
<td width="20%">C.27.9</td>
</tr><tr>
<td width="20%">C.27.90</td>
<td width="20%">C.27.90</td>
</tr><tr>
<td width="20%">C.28</td>
<td width="20%">C.28</td>
</tr><tr>
<td width="20%">C.28.1</td>
<td width="20%">C.28.1</td>
</tr><tr>
<td width="20%">C.28.11</td>
<td width="20%">C.28.11</td>
</tr><tr>
<td width="20%">C.28.12</td>
<td width="20%">C.28.12</td>
</tr><tr>
<td width="20%">C.28.13</td>
<td width="20%">C.28.13</td>
</tr><tr>
<td width="20%">C.28.14</td>
<td width="20%">C.28.14</td>
</tr><tr>
<td width="20%">C.28.15</td>
<td width="20%">C.28.15</td>
</tr><tr>
<td width="20%">C.28.2</td>
<td width="20%">C.28.2</td>
</tr><tr>
<td width="20%">C.28.21</td>
<td width="20%">C.28.21</td>
</tr><tr>
<td width="20%">C.28.22</td>
<td width="20%">C.28.22</td>
</tr><tr>
<td width="20%">C.28.23</td>
<td width="20%">C.28.23</td>
</tr><tr>
<td width="20%">C.28.24</td>
<td width="20%">C.28.24</td>
</tr><tr>
<td width="20%">C.28.25</td>
<td width="20%">C.28.25</td>
</tr><tr>
<td width="20%">C.28.29</td>
<td width="20%">C.28.29</td>
</tr><tr>
<td width="20%">C.28.3</td>
<td width="20%">C.28.3</td>
</tr><tr>
<td width="20%">C.28.30</td>
<td width="20%">C.28.30</td>
</tr><tr>
<td width="20%">C.28.4</td>
<td width="20%">C.28.4</td>
</tr><tr>
<td width="20%">C.28.41</td>
<td width="20%">C.28.41</td>
</tr><tr>
<td width="20%">C.28.49</td>
<td width="20%">C.28.49</td>
</tr><tr>
<td width="20%">C.28.9</td>
<td width="20%">C.28.9</td>
</tr><tr>
<td width="20%">C.28.91</td>
<td width="20%">C.28.91</td>
</tr><tr>
<td width="20%">C.28.92</td>
<td width="20%">C.28.92</td>
</tr><tr>
<td width="20%">C.28.93</td>
<td width="20%">C.28.93</td>
</tr><tr>
<td width="20%">C.28.94</td>
<td width="20%">C.28.94</td>
</tr><tr>
<td width="20%">C.28.95</td>
<td width="20%">C.28.95</td>
</tr><tr>
<td width="20%">C.28.96</td>
<td width="20%">C.28.96</td>
</tr><tr>
<td width="20%">C.28.99</td>
<td width="20%">C.28.99</td>
</tr><tr>
<td width="20%">C.29</td>
<td width="20%">C.29</td>
</tr><tr>
<td width="20%">C.29.1</td>
<td width="20%">C.29.1</td>
</tr><tr>
<td width="20%">C.29.10</td>
<td width="20%">C.29.10</td>
</tr><tr>
<td width="20%">C.29.2</td>
<td width="20%">C.29.2</td>
</tr><tr>
<td width="20%">C.29.20</td>
<td width="20%">C.29.20</td>
</tr><tr>
<td width="20%">C.29.3</td>
<td width="20%">C.29.3</td>
</tr><tr>
<td width="20%">C.29.31</td>
<td width="20%">C.29.31</td>
</tr><tr>
<td width="20%">C.29.32</td>
<td width="20%">C.29.32</td>
</tr><tr>
<td width="20%">C.30</td>
<td width="20%">C.30</td>
</tr><tr>
<td width="20%">C.30.1</td>
<td width="20%">C.30.1</td>
</tr><tr>
<td width="20%">C.30.11</td>
<td width="20%">C.30.11</td>
</tr><tr>
<td width="20%">C.30.12</td>
<td width="20%">C.30.12</td>
</tr><tr>
<td width="20%">C.30.2</td>
<td width="20%">C.30.2</td>
</tr><tr>
<td width="20%">C.30.20</td>
<td width="20%">C.30.20</td>
</tr><tr>
<td width="20%">C.30.3</td>
<td width="20%">C.30.3</td>
</tr><tr>
<td width="20%">C.30.30</td>
<td width="20%">C.30.30</td>
</tr><tr>
<td width="20%">C.30.4</td>
<td width="20%">C.30.4</td>
</tr><tr>
<td width="20%">C.30.40</td>
<td width="20%">C.30.40</td>
</tr><tr>
<td width="20%">C.30.9</td>
<td width="20%">C.30.9</td>
</tr><tr>
<td width="20%">C.30.91</td>
<td width="20%">C.30.91</td>
</tr><tr>
<td width="20%">C.30.92</td>
<td width="20%">C.30.92</td>
</tr><tr>
<td width="20%">C.30.99</td>
<td width="20%">C.30.99</td>
</tr><tr>
<td width="20%">C.31</td>
<td width="20%">C.31</td>
</tr><tr>
<td width="20%">C.31.0</td>
<td width="20%">C.31.0</td>
</tr><tr>
<td width="20%">C.31.01</td>
<td width="20%">C.31.01</td>
</tr><tr>
<td width="20%">C.31.02</td>
<td width="20%">C.31.02</td>
</tr><tr>
<td width="20%">C.31.03</td>
<td width="20%">C.31.03</td>
</tr><tr>
<td width="20%">C.31.09</td>
<td width="20%">C.31.09</td>
</tr><tr>
<td width="20%">C.32</td>
<td width="20%">C.32</td>
</tr><tr>
<td width="20%">C.32.1</td>
<td width="20%">C.32.1</td>
</tr><tr>
<td width="20%">C.32.11</td>
<td width="20%">C.32.11</td>
</tr><tr>
<td width="20%">C.32.12</td>
<td width="20%">C.32.12</td>
</tr><tr>
<td width="20%">C.32.13</td>
<td width="20%">C.32.13</td>
</tr><tr>
<td width="20%">C.32.2</td>
<td width="20%">C.32.2</td>
</tr><tr>
<td width="20%">C.32.20</td>
<td width="20%">C.32.20</td>
</tr><tr>
<td width="20%">C.32.3</td>
<td width="20%">C.32.3</td>
</tr><tr>
<td width="20%">C.32.30</td>
<td width="20%">C.32.30</td>
</tr><tr>
<td width="20%">C.32.4</td>
<td width="20%">C.32.4</td>
</tr><tr>
<td width="20%">C.32.40</td>
<td width="20%">C.32.40</td>
</tr><tr>
<td width="20%">C.32.5</td>
<td width="20%">C.32.5</td>
</tr><tr>
<td width="20%">C.32.50</td>
<td width="20%">C.32.50</td>
</tr><tr>
<td width="20%">C.32.9</td>
<td width="20%">C.32.9</td>
</tr><tr>
<td width="20%">C.32.91</td>
<td width="20%">C.32.91</td>
</tr><tr>
<td width="20%">C.32.99</td>
<td width="20%">C.32.99</td>
</tr><tr>
<td width="20%">C.33</td>
<td width="20%">C.33</td>
</tr><tr>
<td width="20%">C.33.1</td>
<td width="20%">C.33.1</td>
</tr><tr>
<td width="20%">C.33.11</td>
<td width="20%">C.33.11</td>
</tr><tr>
<td width="20%">C.33.12</td>
<td width="20%">C.33.12</td>
</tr><tr>
<td width="20%">C.33.13</td>
<td width="20%">C.33.13</td>
</tr><tr>
<td width="20%">C.33.14</td>
<td width="20%">C.33.14</td>
</tr><tr>
<td width="20%">C.33.15</td>
<td width="20%">C.33.15</td>
</tr><tr>
<td width="20%">C.33.16</td>
<td width="20%">C.33.16</td>
</tr><tr>
<td width="20%">C.33.17</td>
<td width="20%">C.33.17</td>
</tr><tr>
<td width="20%">C.33.19</td>
<td width="20%">C.33.19</td>
</tr><tr>
<td width="20%">C.33.2</td>
<td width="20%">C.33.2</td>
</tr><tr>
<td width="20%">C.33.20</td>
<td width="20%">C.33.20</td>
</tr><tr>
<td width="20%">D</td>
<td width="20%">D</td>
</tr><tr>
<td width="20%">D.35</td>
<td width="20%">D.35</td>
</tr><tr>
<td width="20%">D.35.1</td>
<td width="20%">D.35.1</td>
</tr><tr>
<td width="20%">D.35.11</td>
<td width="20%">D.35.11</td>
</tr><tr>
<td width="20%">D.35.12</td>
<td width="20%">D.35.12</td>
</tr><tr>
<td width="20%">D.35.13</td>
<td width="20%">D.35.13</td>
</tr><tr>
<td width="20%">D.35.14</td>
<td width="20%">D.35.14</td>
</tr><tr>
<td width="20%">D.35.2</td>
<td width="20%">D.35.2</td>
</tr><tr>
<td width="20%">D.35.21</td>
<td width="20%">D.35.21</td>
</tr><tr>
<td width="20%">D.35.22</td>
<td width="20%">D.35.22</td>
</tr><tr>
<td width="20%">D.35.23</td>
<td width="20%">D.35.23</td>
</tr><tr>
<td width="20%">D.35.3</td>
<td width="20%">D.35.3</td>
</tr><tr>
<td width="20%">D.35.30</td>
<td width="20%">D.35.30</td>
</tr><tr>
<td width="20%">E</td>
<td width="20%">E</td>
</tr><tr>
<td width="20%">E.36</td>
<td width="20%">E.36</td>
</tr><tr>
<td width="20%">E.36.0</td>
<td width="20%">E.36.0</td>
</tr><tr>
<td width="20%">E.36.00</td>
<td width="20%">E.36.00</td>
</tr><tr>
<td width="20%">E.37</td>
<td width="20%">E.37</td>
</tr><tr>
<td width="20%">E.37.0</td>
<td width="20%">E.37.0</td>
</tr><tr>
<td width="20%">E.37.00</td>
<td width="20%">E.37.00</td>
</tr><tr>
<td width="20%">E.38</td>
<td width="20%">E.38</td>
</tr><tr>
<td width="20%">E.38.1</td>
<td width="20%">E.38.1</td>
</tr><tr>
<td width="20%">E.38.11</td>
<td width="20%">E.38.11</td>
</tr><tr>
<td width="20%">E.38.12</td>
<td width="20%">E.38.12</td>
</tr><tr>
<td width="20%">E.38.2</td>
<td width="20%">E.38.2</td>
</tr><tr>
<td width="20%">E.38.21</td>
<td width="20%">E.38.21</td>
</tr><tr>
<td width="20%">E.38.22</td>
<td width="20%">E.38.22</td>
</tr><tr>
<td width="20%">E.38.3</td>
<td width="20%">E.38.3</td>
</tr><tr>
<td width="20%">E.38.31</td>
<td width="20%">E.38.31</td>
</tr><tr>
<td width="20%">E.38.32</td>
<td width="20%">E.38.32</td>
</tr><tr>
<td width="20%">E.39</td>
<td width="20%">E.39</td>
</tr><tr>
<td width="20%">E.39.0</td>
<td width="20%">E.39.0</td>
</tr><tr>
<td width="20%">E.39.00</td>
<td width="20%">E.39.00</td>
</tr><tr>
<td width="20%">F</td>
<td width="20%">F</td>
</tr><tr>
<td width="20%">F.41</td>
<td width="20%">F.41</td>
</tr><tr>
<td width="20%">F.41.1</td>
<td width="20%">F.41.1</td>
</tr><tr>
<td width="20%">F.41.10</td>
<td width="20%">F.41.10</td>
</tr><tr>
<td width="20%">F.41.2</td>
<td width="20%">F.41.2</td>
</tr><tr>
<td width="20%">F.41.20</td>
<td width="20%">F.41.20</td>
</tr><tr>
<td width="20%">F.42</td>
<td width="20%">F.42</td>
</tr><tr>
<td width="20%">F.42.1</td>
<td width="20%">F.42.1</td>
</tr><tr>
<td width="20%">F.42.11</td>
<td width="20%">F.42.11</td>
</tr><tr>
<td width="20%">F.42.12</td>
<td width="20%">F.42.12</td>
</tr><tr>
<td width="20%">F.42.13</td>
<td width="20%">F.42.13</td>
</tr><tr>
<td width="20%">F.42.2</td>
<td width="20%">F.42.2</td>
</tr><tr>
<td width="20%">F.42.21</td>
<td width="20%">F.42.21</td>
</tr><tr>
<td width="20%">F.42.22</td>
<td width="20%">F.42.22</td>
</tr><tr>
<td width="20%">F.42.9</td>
<td width="20%">F.42.9</td>
</tr><tr>
<td width="20%">F.42.91</td>
<td width="20%">F.42.91</td>
</tr><tr>
<td width="20%">F.42.99</td>
<td width="20%">F.42.99</td>
</tr><tr>
<td width="20%">F.43</td>
<td width="20%">F.43</td>
</tr><tr>
<td width="20%">F.43.1</td>
<td width="20%">F.43.1</td>
</tr><tr>
<td width="20%">F.43.11</td>
<td width="20%">F.43.11</td>
</tr><tr>
<td width="20%">F.43.12</td>
<td width="20%">F.43.12</td>
</tr><tr>
<td width="20%">F.43.13</td>
<td width="20%">F.43.13</td>
</tr><tr>
<td width="20%">F.43.2</td>
<td width="20%">F.43.2</td>
</tr><tr>
<td width="20%">F.43.21</td>
<td width="20%">F.43.21</td>
</tr><tr>
<td width="20%">F.43.22</td>
<td width="20%">F.43.22</td>
</tr><tr>
<td width="20%">F.43.29</td>
<td width="20%">F.43.29</td>
</tr><tr>
<td width="20%">F.43.3</td>
<td width="20%">F.43.3</td>
</tr><tr>
<td width="20%">F.43.31</td>
<td width="20%">F.43.31</td>
</tr><tr>
<td width="20%">F.43.32</td>
<td width="20%">F.43.32</td>
</tr><tr>
<td width="20%">F.43.33</td>
<td width="20%">F.43.33</td>
</tr><tr>
<td width="20%">F.43.34</td>
<td width="20%">F.43.34</td>
</tr><tr>
<td width="20%">F.43.39</td>
<td width="20%">F.43.39</td>
</tr><tr>
<td width="20%">F.43.9</td>
<td width="20%">F.43.9</td>
</tr><tr>
<td width="20%">F.43.91</td>
<td width="20%">F.43.91</td>
</tr><tr>
<td width="20%">F.43.99</td>
<td width="20%">F.43.99</td>
</tr><tr>
<td width="20%">G</td>
<td width="20%">G</td>
</tr><tr>
<td width="20%">G.45</td>
<td width="20%">G.45</td>
</tr><tr>
<td width="20%">G.45.1</td>
<td width="20%">G.45.1</td>
</tr><tr>
<td width="20%">G.45.11</td>
<td width="20%">G.45.11</td>
</tr><tr>
<td width="20%">G.45.19</td>
<td width="20%">G.45.19</td>
</tr><tr>
<td width="20%">G.45.2</td>
<td width="20%">G.45.2</td>
</tr><tr>
<td width="20%">G.45.20</td>
<td width="20%">G.45.20</td>
</tr><tr>
<td width="20%">G.45.3</td>
<td width="20%">G.45.3</td>
</tr><tr>
<td width="20%">G.45.31</td>
<td width="20%">G.45.31</td>
</tr><tr>
<td width="20%">G.45.32</td>
<td width="20%">G.45.32</td>
</tr><tr>
<td width="20%">G.45.4</td>
<td width="20%">G.45.4</td>
</tr><tr>
<td width="20%">G.45.40</td>
<td width="20%">G.45.40</td>
</tr><tr>
<td width="20%">G.46</td>
<td width="20%">G.46</td>
</tr><tr>
<td width="20%">G.46.1</td>
<td width="20%">G.46.1</td>
</tr><tr>
<td width="20%">G.46.11</td>
<td width="20%">G.46.11</td>
</tr><tr>
<td width="20%">G.46.12</td>
<td width="20%">G.46.12</td>
</tr><tr>
<td width="20%">G.46.13</td>
<td width="20%">G.46.13</td>
</tr><tr>
<td width="20%">G.46.14</td>
<td width="20%">G.46.14</td>
</tr><tr>
<td width="20%">G.46.15</td>
<td width="20%">G.46.15</td>
</tr><tr>
<td width="20%">G.46.16</td>
<td width="20%">G.46.16</td>
</tr><tr>
<td width="20%">G.46.17</td>
<td width="20%">G.46.17</td>
</tr><tr>
<td width="20%">G.46.18</td>
<td width="20%">G.46.18</td>
</tr><tr>
<td width="20%">G.46.19</td>
<td width="20%">G.46.19</td>
</tr><tr>
<td width="20%">G.46.2</td>
<td width="20%">G.46.2</td>
</tr><tr>
<td width="20%">G.46.21</td>
<td width="20%">G.46.21</td>
</tr><tr>
<td width="20%">G.46.22</td>
<td width="20%">G.46.22</td>
</tr><tr>
<td width="20%">G.46.23</td>
<td width="20%">G.46.23</td>
</tr><tr>
<td width="20%">G.46.24</td>
<td width="20%">G.46.24</td>
</tr><tr>
<td width="20%">G.46.3</td>
<td width="20%">G.46.3</td>
</tr><tr>
<td width="20%">G.46.31</td>
<td width="20%">G.46.31</td>
</tr><tr>
<td width="20%">G.46.32</td>
<td width="20%">G.46.32</td>
</tr><tr>
<td width="20%">G.46.33</td>
<td width="20%">G.46.33</td>
</tr><tr>
<td width="20%">G.46.34</td>
<td width="20%">G.46.34</td>
</tr><tr>
<td width="20%">G.46.35</td>
<td width="20%">G.46.35</td>
</tr><tr>
<td width="20%">G.46.36</td>
<td width="20%">G.46.36</td>
</tr><tr>
<td width="20%">G.46.37</td>
<td width="20%">G.46.37</td>
</tr><tr>
<td width="20%">G.46.38</td>
<td width="20%">G.46.38</td>
</tr><tr>
<td width="20%">G.46.39</td>
<td width="20%">G.46.39</td>
</tr><tr>
<td width="20%">G.46.4</td>
<td width="20%">G.46.4</td>
</tr><tr>
<td width="20%">G.46.41</td>
<td width="20%">G.46.41</td>
</tr><tr>
<td width="20%">G.46.42</td>
<td width="20%">G.46.42</td>
</tr><tr>
<td width="20%">G.46.43</td>
<td width="20%">G.46.43</td>
</tr><tr>
<td width="20%">G.46.44</td>
<td width="20%">G.46.44</td>
</tr><tr>
<td width="20%">G.46.45</td>
<td width="20%">G.46.45</td>
</tr><tr>
<td width="20%">G.46.46</td>
<td width="20%">G.46.46</td>
</tr><tr>
<td width="20%">G.46.47</td>
<td width="20%">G.46.47</td>
</tr><tr>
<td width="20%">G.46.48</td>
<td width="20%">G.46.48</td>
</tr><tr>
<td width="20%">G.46.49</td>
<td width="20%">G.46.49</td>
</tr><tr>
<td width="20%">G.46.5</td>
<td width="20%">G.46.5</td>
</tr><tr>
<td width="20%">G.46.51</td>
<td width="20%">G.46.51</td>
</tr><tr>
<td width="20%">G.46.52</td>
<td width="20%">G.46.52</td>
</tr><tr>
<td width="20%">G.46.6</td>
<td width="20%">G.46.6</td>
</tr><tr>
<td width="20%">G.46.61</td>
<td width="20%">G.46.61</td>
</tr><tr>
<td width="20%">G.46.62</td>
<td width="20%">G.46.62</td>
</tr><tr>
<td width="20%">G.46.63</td>
<td width="20%">G.46.63</td>
</tr><tr>
<td width="20%">G.46.64</td>
<td width="20%">G.46.64</td>
</tr><tr>
<td width="20%">G.46.65</td>
<td width="20%">G.46.65</td>
</tr><tr>
<td width="20%">G.46.66</td>
<td width="20%">G.46.66</td>
</tr><tr>
<td width="20%">G.46.69</td>
<td width="20%">G.46.69</td>
</tr><tr>
<td width="20%">G.46.7</td>
<td width="20%">G.46.7</td>
</tr><tr>
<td width="20%">G.46.71</td>
<td width="20%">G.46.71</td>
</tr><tr>
<td width="20%">G.46.72</td>
<td width="20%">G.46.72</td>
</tr><tr>
<td width="20%">G.46.73</td>
<td width="20%">G.46.73</td>
</tr><tr>
<td width="20%">G.46.74</td>
<td width="20%">G.46.74</td>
</tr><tr>
<td width="20%">G.46.75</td>
<td width="20%">G.46.75</td>
</tr><tr>
<td width="20%">G.46.76</td>
<td width="20%">G.46.76</td>
</tr><tr>
<td width="20%">G.46.77</td>
<td width="20%">G.46.77</td>
</tr><tr>
<td width="20%">G.46.9</td>
<td width="20%">G.46.9</td>
</tr><tr>
<td width="20%">G.46.90</td>
<td width="20%">G.46.90</td>
</tr><tr>
<td width="20%">G.47</td>
<td width="20%">G.47</td>
</tr><tr>
<td width="20%">G.47.1</td>
<td width="20%">G.47.1</td>
</tr><tr>
<td width="20%">G.47.11</td>
<td width="20%">G.47.11</td>
</tr><tr>
<td width="20%">G.47.19</td>
<td width="20%">G.47.19</td>
</tr><tr>
<td width="20%">G.47.2</td>
<td width="20%">G.47.2</td>
</tr><tr>
<td width="20%">G.47.21</td>
<td width="20%">G.47.21</td>
</tr><tr>
<td width="20%">G.47.22</td>
<td width="20%">G.47.22</td>
</tr><tr>
<td width="20%">G.47.23</td>
<td width="20%">G.47.23</td>
</tr><tr>
<td width="20%">G.47.24</td>
<td width="20%">G.47.24</td>
</tr><tr>
<td width="20%">G.47.25</td>
<td width="20%">G.47.25</td>
</tr><tr>
<td width="20%">G.47.26</td>
<td width="20%">G.47.26</td>
</tr><tr>
<td width="20%">G.47.29</td>
<td width="20%">G.47.29</td>
</tr><tr>
<td width="20%">G.47.3</td>
<td width="20%">G.47.3</td>
</tr><tr>
<td width="20%">G.47.30</td>
<td width="20%">G.47.30</td>
</tr><tr>
<td width="20%">G.47.4</td>
<td width="20%">G.47.4</td>
</tr><tr>
<td width="20%">G.47.41</td>
<td width="20%">G.47.41</td>
</tr><tr>
<td width="20%">G.47.42</td>
<td width="20%">G.47.42</td>
</tr><tr>
<td width="20%">G.47.43</td>
<td width="20%">G.47.43</td>
</tr><tr>
<td width="20%">G.47.5</td>
<td width="20%">G.47.5</td>
</tr><tr>
<td width="20%">G.47.51</td>
<td width="20%">G.47.51</td>
</tr><tr>
<td width="20%">G.47.52</td>
<td width="20%">G.47.52</td>
</tr><tr>
<td width="20%">G.47.53</td>
<td width="20%">G.47.53</td>
</tr><tr>
<td width="20%">G.47.54</td>
<td width="20%">G.47.54</td>
</tr><tr>
<td width="20%">G.47.59</td>
<td width="20%">G.47.59</td>
</tr><tr>
<td width="20%">G.47.6</td>
<td width="20%">G.47.6</td>
</tr><tr>
<td width="20%">G.47.61</td>
<td width="20%">G.47.61</td>
</tr><tr>
<td width="20%">G.47.62</td>
<td width="20%">G.47.62</td>
</tr><tr>
<td width="20%">G.47.63</td>
<td width="20%">G.47.63</td>
</tr><tr>
<td width="20%">G.47.64</td>
<td width="20%">G.47.64</td>
</tr><tr>
<td width="20%">G.47.65</td>
<td width="20%">G.47.65</td>
</tr><tr>
<td width="20%">G.47.7</td>
<td width="20%">G.47.7</td>
</tr><tr>
<td width="20%">G.47.71</td>
<td width="20%">G.47.71</td>
</tr><tr>
<td width="20%">G.47.72</td>
<td width="20%">G.47.72</td>
</tr><tr>
<td width="20%">G.47.73</td>
<td width="20%">G.47.73</td>
</tr><tr>
<td width="20%">G.47.74</td>
<td width="20%">G.47.74</td>
</tr><tr>
<td width="20%">G.47.75</td>
<td width="20%">G.47.75</td>
</tr><tr>
<td width="20%">G.47.76</td>
<td width="20%">G.47.76</td>
</tr><tr>
<td width="20%">G.47.77</td>
<td width="20%">G.47.77</td>
</tr><tr>
<td width="20%">G.47.78</td>
<td width="20%">G.47.78</td>
</tr><tr>
<td width="20%">G.47.79</td>
<td width="20%">G.47.79</td>
</tr><tr>
<td width="20%">G.47.8</td>
<td width="20%">G.47.8</td>
</tr><tr>
<td width="20%">G.47.81</td>
<td width="20%">G.47.81</td>
</tr><tr>
<td width="20%">G.47.82</td>
<td width="20%">G.47.82</td>
</tr><tr>
<td width="20%">G.47.89</td>
<td width="20%">G.47.89</td>
</tr><tr>
<td width="20%">G.47.9</td>
<td width="20%">G.47.9</td>
</tr><tr>
<td width="20%">G.47.91</td>
<td width="20%">G.47.91</td>
</tr><tr>
<td width="20%">G.47.99</td>
<td width="20%">G.47.99</td>
</tr><tr>
<td width="20%">H</td>
<td width="20%">H</td>
</tr><tr>
<td width="20%">H.49</td>
<td width="20%">H.49</td>
</tr><tr>
<td width="20%">H.49.1</td>
<td width="20%">H.49.1</td>
</tr><tr>
<td width="20%">H.49.10</td>
<td width="20%">H.49.10</td>
</tr><tr>
<td width="20%">H.49.2</td>
<td width="20%">H.49.2</td>
</tr><tr>
<td width="20%">H.49.20</td>
<td width="20%">H.49.20</td>
</tr><tr>
<td width="20%">H.49.3</td>
<td width="20%">H.49.3</td>
</tr><tr>
<td width="20%">H.49.31</td>
<td width="20%">H.49.31</td>
</tr><tr>
<td width="20%">H.49.32</td>
<td width="20%">H.49.32</td>
</tr><tr>
<td width="20%">H.49.39</td>
<td width="20%">H.49.39</td>
</tr><tr>
<td width="20%">H.49.4</td>
<td width="20%">H.49.4</td>
</tr><tr>
<td width="20%">H.49.41</td>
<td width="20%">H.49.41</td>
</tr><tr>
<td width="20%">H.49.42</td>
<td width="20%">H.49.42</td>
</tr><tr>
<td width="20%">H.49.5</td>
<td width="20%">H.49.5</td>
</tr><tr>
<td width="20%">H.49.50</td>
<td width="20%">H.49.50</td>
</tr><tr>
<td width="20%">H.50</td>
<td width="20%">H.50</td>
</tr><tr>
<td width="20%">H.50.1</td>
<td width="20%">H.50.1</td>
</tr><tr>
<td width="20%">H.50.10</td>
<td width="20%">H.50.10</td>
</tr><tr>
<td width="20%">H.50.2</td>
<td width="20%">H.50.2</td>
</tr><tr>
<td width="20%">H.50.20</td>
<td width="20%">H.50.20</td>
</tr><tr>
<td width="20%">H.50.3</td>
<td width="20%">H.50.3</td>
</tr><tr>
<td width="20%">H.50.30</td>
<td width="20%">H.50.30</td>
</tr><tr>
<td width="20%">H.50.4</td>
<td width="20%">H.50.4</td>
</tr><tr>
<td width="20%">H.50.40</td>
<td width="20%">H.50.40</td>
</tr><tr>
<td width="20%">H.51</td>
<td width="20%">H.51</td>
</tr><tr>
<td width="20%">H.51.1</td>
<td width="20%">H.51.1</td>
</tr><tr>
<td width="20%">H.51.10</td>
<td width="20%">H.51.10</td>
</tr><tr>
<td width="20%">H.51.2</td>
<td width="20%">H.51.2</td>
</tr><tr>
<td width="20%">H.51.21</td>
<td width="20%">H.51.21</td>
</tr><tr>
<td width="20%">H.51.22</td>
<td width="20%">H.51.22</td>
</tr><tr>
<td width="20%">H.52</td>
<td width="20%">H.52</td>
</tr><tr>
<td width="20%">H.52.1</td>
<td width="20%">H.52.1</td>
</tr><tr>
<td width="20%">H.52.10</td>
<td width="20%">H.52.10</td>
</tr><tr>
<td width="20%">H.52.2</td>
<td width="20%">H.52.2</td>
</tr><tr>
<td width="20%">H.52.21</td>
<td width="20%">H.52.21</td>
</tr><tr>
<td width="20%">H.52.22</td>
<td width="20%">H.52.22</td>
</tr><tr>
<td width="20%">H.52.23</td>
<td width="20%">H.52.23</td>
</tr><tr>
<td width="20%">H.52.24</td>
<td width="20%">H.52.24</td>
</tr><tr>
<td width="20%">H.52.29</td>
<td width="20%">H.52.29</td>
</tr><tr>
<td width="20%">H.53</td>
<td width="20%">H.53</td>
</tr><tr>
<td width="20%">H.53.1</td>
<td width="20%">H.53.1</td>
</tr><tr>
<td width="20%">H.53.10</td>
<td width="20%">H.53.10</td>
</tr><tr>
<td width="20%">H.53.2</td>
<td width="20%">H.53.2</td>
</tr><tr>
<td width="20%">H.53.20</td>
<td width="20%">H.53.20</td>
</tr><tr>
<td width="20%">I</td>
<td width="20%">I</td>
</tr><tr>
<td width="20%">I.55</td>
<td width="20%">I.55</td>
</tr><tr>
<td width="20%">I.55.1</td>
<td width="20%">I.55.1</td>
</tr><tr>
<td width="20%">I.55.10</td>
<td width="20%">I.55.10</td>
</tr><tr>
<td width="20%">I.55.2</td>
<td width="20%">I.55.2</td>
</tr><tr>
<td width="20%">I.55.20</td>
<td width="20%">I.55.20</td>
</tr><tr>
<td width="20%">I.55.3</td>
<td width="20%">I.55.3</td>
</tr><tr>
<td width="20%">I.55.30</td>
<td width="20%">I.55.30</td>
</tr><tr>
<td width="20%">I.55.9</td>
<td width="20%">I.55.9</td>
</tr><tr>
<td width="20%">I.55.90</td>
<td width="20%">I.55.90</td>
</tr><tr>
<td width="20%">I.56</td>
<td width="20%">I.56</td>
</tr><tr>
<td width="20%">I.56.1</td>
<td width="20%">I.56.1</td>
</tr><tr>
<td width="20%">I.56.10</td>
<td width="20%">I.56.10</td>
</tr><tr>
<td width="20%">I.56.2</td>
<td width="20%">I.56.2</td>
</tr><tr>
<td width="20%">I.56.21</td>
<td width="20%">I.56.21</td>
</tr><tr>
<td width="20%">I.56.29</td>
<td width="20%">I.56.29</td>
</tr><tr>
<td width="20%">I.56.3</td>
<td width="20%">I.56.3</td>
</tr><tr>
<td width="20%">I.56.30</td>
<td width="20%">I.56.30</td>
</tr><tr>
<td width="20%">J</td>
<td width="20%">J</td>
</tr><tr>
<td width="20%">J.58</td>
<td width="20%">J.58</td>
</tr><tr>
<td width="20%">J.58.1</td>
<td width="20%">J.58.1</td>
</tr><tr>
<td width="20%">J.58.11</td>
<td width="20%">J.58.11</td>
</tr><tr>
<td width="20%">J.58.12</td>
<td width="20%">J.58.12</td>
</tr><tr>
<td width="20%">J.58.13</td>
<td width="20%">J.58.13</td>
</tr><tr>
<td width="20%">J.58.14</td>
<td width="20%">J.58.14</td>
</tr><tr>
<td width="20%">J.58.19</td>
<td width="20%">J.58.19</td>
</tr><tr>
<td width="20%">J.58.2</td>
<td width="20%">J.58.2</td>
</tr><tr>
<td width="20%">J.58.21</td>
<td width="20%">J.58.21</td>
</tr><tr>
<td width="20%">J.58.29</td>
<td width="20%">J.58.29</td>
</tr><tr>
<td width="20%">J.59</td>
<td width="20%">J.59</td>
</tr><tr>
<td width="20%">J.59.1</td>
<td width="20%">J.59.1</td>
</tr><tr>
<td width="20%">J.59.11</td>
<td width="20%">J.59.11</td>
</tr><tr>
<td width="20%">J.59.12</td>
<td width="20%">J.59.12</td>
</tr><tr>
<td width="20%">J.59.13</td>
<td width="20%">J.59.13</td>
</tr><tr>
<td width="20%">J.59.14</td>
<td width="20%">J.59.14</td>
</tr><tr>
<td width="20%">J.59.2</td>
<td width="20%">J.59.2</td>
</tr><tr>
<td width="20%">J.59.20</td>
<td width="20%">J.59.20</td>
</tr><tr>
<td width="20%">J.60</td>
<td width="20%">J.60</td>
</tr><tr>
<td width="20%">J.60.1</td>
<td width="20%">J.60.1</td>
</tr><tr>
<td width="20%">J.60.10</td>
<td width="20%">J.60.10</td>
</tr><tr>
<td width="20%">J.60.2</td>
<td width="20%">J.60.2</td>
</tr><tr>
<td width="20%">J.60.20</td>
<td width="20%">J.60.20</td>
</tr><tr>
<td width="20%">J.61</td>
<td width="20%">J.61</td>
</tr><tr>
<td width="20%">J.61.1</td>
<td width="20%">J.61.1</td>
</tr><tr>
<td width="20%">J.61.10</td>
<td width="20%">J.61.10</td>
</tr><tr>
<td width="20%">J.61.2</td>
<td width="20%">J.61.2</td>
</tr><tr>
<td width="20%">J.61.20</td>
<td width="20%">J.61.20</td>
</tr><tr>
<td width="20%">J.61.3</td>
<td width="20%">J.61.3</td>
</tr><tr>
<td width="20%">J.61.30</td>
<td width="20%">J.61.30</td>
</tr><tr>
<td width="20%">J.61.9</td>
<td width="20%">J.61.9</td>
</tr><tr>
<td width="20%">J.61.90</td>
<td width="20%">J.61.90</td>
</tr><tr>
<td width="20%">J.62</td>
<td width="20%">J.62</td>
</tr><tr>
<td width="20%">J.62.0</td>
<td width="20%">J.62.0</td>
</tr><tr>
<td width="20%">J.62.01</td>
<td width="20%">J.62.01</td>
</tr><tr>
<td width="20%">J.62.02</td>
<td width="20%">J.62.02</td>
</tr><tr>
<td width="20%">J.62.03</td>
<td width="20%">J.62.03</td>
</tr><tr>
<td width="20%">J.62.09</td>
<td width="20%">J.62.09</td>
</tr><tr>
<td width="20%">J.63</td>
<td width="20%">J.63</td>
</tr><tr>
<td width="20%">J.63.1</td>
<td width="20%">J.63.1</td>
</tr><tr>
<td width="20%">J.63.11</td>
<td width="20%">J.63.11</td>
</tr><tr>
<td width="20%">J.63.12</td>
<td width="20%">J.63.12</td>
</tr><tr>
<td width="20%">J.63.9</td>
<td width="20%">J.63.9</td>
</tr><tr>
<td width="20%">J.63.91</td>
<td width="20%">J.63.91</td>
</tr><tr>
<td width="20%">J.63.99</td>
<td width="20%">J.63.99</td>
</tr><tr>
<td width="20%">K</td>
<td width="20%">K</td>
</tr><tr>
<td width="20%">K.64</td>
<td width="20%">K.64</td>
</tr><tr>
<td width="20%">K.64.1</td>
<td width="20%">K.64.1</td>
</tr><tr>
<td width="20%">K.64.11</td>
<td width="20%">K.64.11</td>
</tr><tr>
<td width="20%">K.64.19</td>
<td width="20%">K.64.19</td>
</tr><tr>
<td width="20%">K.64.2</td>
<td width="20%">K.64.2</td>
</tr><tr>
<td width="20%">K.64.20</td>
<td width="20%">K.64.20</td>
</tr><tr>
<td width="20%">K.64.3</td>
<td width="20%">K.64.3</td>
</tr><tr>
<td width="20%">K.64.30</td>
<td width="20%">K.64.30</td>
</tr><tr>
<td width="20%">K.64.9</td>
<td width="20%">K.64.9</td>
</tr><tr>
<td width="20%">K.64.91</td>
<td width="20%">K.64.91</td>
</tr><tr>
<td width="20%">K.64.92</td>
<td width="20%">K.64.92</td>
</tr><tr>
<td width="20%">K.64.99</td>
<td width="20%">K.64.99</td>
</tr><tr>
<td width="20%">K.65</td>
<td width="20%">K.65</td>
</tr><tr>
<td width="20%">K.65.1</td>
<td width="20%">K.65.1</td>
</tr><tr>
<td width="20%">K.65.11</td>
<td width="20%">K.65.11</td>
</tr><tr>
<td width="20%">K.65.12</td>
<td width="20%">K.65.12</td>
</tr><tr>
<td width="20%">K.65.2</td>
<td width="20%">K.65.2</td>
</tr><tr>
<td width="20%">K.65.20</td>
<td width="20%">K.65.20</td>
</tr><tr>
<td width="20%">K.65.3</td>
<td width="20%">K.65.3</td>
</tr><tr>
<td width="20%">K.65.30</td>
<td width="20%">K.65.30</td>
</tr><tr>
<td width="20%">K.66</td>
<td width="20%">K.66</td>
</tr><tr>
<td width="20%">K.66.1</td>
<td width="20%">K.66.1</td>
</tr><tr>
<td width="20%">K.66.11</td>
<td width="20%">K.66.11</td>
</tr><tr>
<td width="20%">K.66.12</td>
<td width="20%">K.66.12</td>
</tr><tr>
<td width="20%">K.66.19</td>
<td width="20%">K.66.19</td>
</tr><tr>
<td width="20%">K.66.2</td>
<td width="20%">K.66.2</td>
</tr><tr>
<td width="20%">K.66.21</td>
<td width="20%">K.66.21</td>
</tr><tr>
<td width="20%">K.66.22</td>
<td width="20%">K.66.22</td>
</tr><tr>
<td width="20%">K.66.29</td>
<td width="20%">K.66.29</td>
</tr><tr>
<td width="20%">K.66.3</td>
<td width="20%">K.66.3</td>
</tr><tr>
<td width="20%">K.66.30</td>
<td width="20%">K.66.30</td>
</tr><tr>
<td width="20%">L</td>
<td width="20%">L</td>
</tr><tr>
<td width="20%">L.68</td>
<td width="20%">L.68</td>
</tr><tr>
<td width="20%">L.68.1</td>
<td width="20%">L.68.1</td>
</tr><tr>
<td width="20%">L.68.10</td>
<td width="20%">L.68.10</td>
</tr><tr>
<td width="20%">L.68.2</td>
<td width="20%">L.68.2</td>
</tr><tr>
<td width="20%">L.68.20</td>
<td width="20%">L.68.20</td>
</tr><tr>
<td width="20%">L.68.3</td>
<td width="20%">L.68.3</td>
</tr><tr>
<td width="20%">L.68.31</td>
<td width="20%">L.68.31</td>
</tr><tr>
<td width="20%">L.68.32</td>
<td width="20%">L.68.32</td>
</tr><tr>
<td width="20%">M</td>
<td width="20%">M</td>
</tr><tr>
<td width="20%">M.69</td>
<td width="20%">M.69</td>
</tr><tr>
<td width="20%">M.69.1</td>
<td width="20%">M.69.1</td>
</tr><tr>
<td width="20%">M.69.10</td>
<td width="20%">M.69.10</td>
</tr><tr>
<td width="20%">M.69.2</td>
<td width="20%">M.69.2</td>
</tr><tr>
<td width="20%">M.69.20</td>
<td width="20%">M.69.20</td>
</tr><tr>
<td width="20%">M.70</td>
<td width="20%">M.70</td>
</tr><tr>
<td width="20%">M.70.1</td>
<td width="20%">M.70.1</td>
</tr><tr>
<td width="20%">M.70.10</td>
<td width="20%">M.70.10</td>
</tr><tr>
<td width="20%">M.70.2</td>
<td width="20%">M.70.2</td>
</tr><tr>
<td width="20%">M.70.21</td>
<td width="20%">M.70.21</td>
</tr><tr>
<td width="20%">M.70.22</td>
<td width="20%">M.70.22</td>
</tr><tr>
<td width="20%">M.71</td>
<td width="20%">M.71</td>
</tr><tr>
<td width="20%">M.71.1</td>
<td width="20%">M.71.1</td>
</tr><tr>
<td width="20%">M.71.11</td>
<td width="20%">M.71.11</td>
</tr><tr>
<td width="20%">M.71.12</td>
<td width="20%">M.71.12</td>
</tr><tr>
<td width="20%">M.71.2</td>
<td width="20%">M.71.2</td>
</tr><tr>
<td width="20%">M.71.20</td>
<td width="20%">M.71.20</td>
</tr><tr>
<td width="20%">M.72</td>
<td width="20%">M.72</td>
</tr><tr>
<td width="20%">M.72.1</td>
<td width="20%">M.72.1</td>
</tr><tr>
<td width="20%">M.72.11</td>
<td width="20%">M.72.11</td>
</tr><tr>
<td width="20%">M.72.19</td>
<td width="20%">M.72.19</td>
</tr><tr>
<td width="20%">M.72.2</td>
<td width="20%">M.72.2</td>
</tr><tr>
<td width="20%">M.72.20</td>
<td width="20%">M.72.20</td>
</tr><tr>
<td width="20%">M.73</td>
<td width="20%">M.73</td>
</tr><tr>
<td width="20%">M.73.1</td>
<td width="20%">M.73.1</td>
</tr><tr>
<td width="20%">M.73.11</td>
<td width="20%">M.73.11</td>
</tr><tr>
<td width="20%">M.73.12</td>
<td width="20%">M.73.12</td>
</tr><tr>
<td width="20%">M.73.2</td>
<td width="20%">M.73.2</td>
</tr><tr>
<td width="20%">M.73.20</td>
<td width="20%">M.73.20</td>
</tr><tr>
<td width="20%">M.74</td>
<td width="20%">M.74</td>
</tr><tr>
<td width="20%">M.74.1</td>
<td width="20%">M.74.1</td>
</tr><tr>
<td width="20%">M.74.10</td>
<td width="20%">M.74.10</td>
</tr><tr>
<td width="20%">M.74.2</td>
<td width="20%">M.74.2</td>
</tr><tr>
<td width="20%">M.74.20</td>
<td width="20%">M.74.20</td>
</tr><tr>
<td width="20%">M.74.3</td>
<td width="20%">M.74.3</td>
</tr><tr>
<td width="20%">M.74.30</td>
<td width="20%">M.74.30</td>
</tr><tr>
<td width="20%">M.74.9</td>
<td width="20%">M.74.9</td>
</tr><tr>
<td width="20%">M.74.90</td>
<td width="20%">M.74.90</td>
</tr><tr>
<td width="20%">M.75</td>
<td width="20%">M.75</td>
</tr><tr>
<td width="20%">M.75.0</td>
<td width="20%">M.75.0</td>
</tr><tr>
<td width="20%">M.75.00</td>
<td width="20%">M.75.00</td>
</tr><tr>
<td width="20%">N</td>
<td width="20%">N</td>
</tr><tr>
<td width="20%">N.77</td>
<td width="20%">N.77</td>
</tr><tr>
<td width="20%">N.77.1</td>
<td width="20%">N.77.1</td>
</tr><tr>
<td width="20%">N.77.11</td>
<td width="20%">N.77.11</td>
</tr><tr>
<td width="20%">N.77.12</td>
<td width="20%">N.77.12</td>
</tr><tr>
<td width="20%">N.77.2</td>
<td width="20%">N.77.2</td>
</tr><tr>
<td width="20%">N.77.21</td>
<td width="20%">N.77.21</td>
</tr><tr>
<td width="20%">N.77.22</td>
<td width="20%">N.77.22</td>
</tr><tr>
<td width="20%">N.77.29</td>
<td width="20%">N.77.29</td>
</tr><tr>
<td width="20%">N.77.3</td>
<td width="20%">N.77.3</td>
</tr><tr>
<td width="20%">N.77.31</td>
<td width="20%">N.77.31</td>
</tr><tr>
<td width="20%">N.77.32</td>
<td width="20%">N.77.32</td>
</tr><tr>
<td width="20%">N.77.33</td>
<td width="20%">N.77.33</td>
</tr><tr>
<td width="20%">N.77.34</td>
<td width="20%">N.77.34</td>
</tr><tr>
<td width="20%">N.77.35</td>
<td width="20%">N.77.35</td>
</tr><tr>
<td width="20%">N.77.39</td>
<td width="20%">N.77.39</td>
</tr><tr>
<td width="20%">N.77.4</td>
<td width="20%">N.77.4</td>
</tr><tr>
<td width="20%">N.77.40</td>
<td width="20%">N.77.40</td>
</tr><tr>
<td width="20%">N.78</td>
<td width="20%">N.78</td>
</tr><tr>
<td width="20%">N.78.1</td>
<td width="20%">N.78.1</td>
</tr><tr>
<td width="20%">N.78.10</td>
<td width="20%">N.78.10</td>
</tr><tr>
<td width="20%">N.78.2</td>
<td width="20%">N.78.2</td>
</tr><tr>
<td width="20%">N.78.20</td>
<td width="20%">N.78.20</td>
</tr><tr>
<td width="20%">N.78.3</td>
<td width="20%">N.78.3</td>
</tr><tr>
<td width="20%">N.78.30</td>
<td width="20%">N.78.30</td>
</tr><tr>
<td width="20%">N.79</td>
<td width="20%">N.79</td>
</tr><tr>
<td width="20%">N.79.1</td>
<td width="20%">N.79.1</td>
</tr><tr>
<td width="20%">N.79.11</td>
<td width="20%">N.79.11</td>
</tr><tr>
<td width="20%">N.79.12</td>
<td width="20%">N.79.12</td>
</tr><tr>
<td width="20%">N.79.9</td>
<td width="20%">N.79.9</td>
</tr><tr>
<td width="20%">N.79.90</td>
<td width="20%">N.79.90</td>
</tr><tr>
<td width="20%">N.80</td>
<td width="20%">N.80</td>
</tr><tr>
<td width="20%">N.80.1</td>
<td width="20%">N.80.1</td>
</tr><tr>
<td width="20%">N.80.10</td>
<td width="20%">N.80.10</td>
</tr><tr>
<td width="20%">N.80.2</td>
<td width="20%">N.80.2</td>
</tr><tr>
<td width="20%">N.80.20</td>
<td width="20%">N.80.20</td>
</tr><tr>
<td width="20%">N.80.3</td>
<td width="20%">N.80.3</td>
</tr><tr>
<td width="20%">N.80.30</td>
<td width="20%">N.80.30</td>
</tr><tr>
<td width="20%">N.81</td>
<td width="20%">N.81</td>
</tr><tr>
<td width="20%">N.81.1</td>
<td width="20%">N.81.1</td>
</tr><tr>
<td width="20%">N.81.10</td>
<td width="20%">N.81.10</td>
</tr><tr>
<td width="20%">N.81.2</td>
<td width="20%">N.81.2</td>
</tr><tr>
<td width="20%">N.81.21</td>
<td width="20%">N.81.21</td>
</tr><tr>
<td width="20%">N.81.22</td>
<td width="20%">N.81.22</td>
</tr><tr>
<td width="20%">N.81.29</td>
<td width="20%">N.81.29</td>
</tr><tr>
<td width="20%">N.81.3</td>
<td width="20%">N.81.3</td>
</tr><tr>
<td width="20%">N.81.30</td>
<td width="20%">N.81.30</td>
</tr><tr>
<td width="20%">N.82</td>
<td width="20%">N.82</td>
</tr><tr>
<td width="20%">N.82.1</td>
<td width="20%">N.82.1</td>
</tr><tr>
<td width="20%">N.82.11</td>
<td width="20%">N.82.11</td>
</tr><tr>
<td width="20%">N.82.19</td>
<td width="20%">N.82.19</td>
</tr><tr>
<td width="20%">N.82.2</td>
<td width="20%">N.82.2</td>
</tr><tr>
<td width="20%">N.82.20</td>
<td width="20%">N.82.20</td>
</tr><tr>
<td width="20%">N.82.3</td>
<td width="20%">N.82.3</td>
</tr><tr>
<td width="20%">N.82.30</td>
<td width="20%">N.82.30</td>
</tr><tr>
<td width="20%">N.82.9</td>
<td width="20%">N.82.9</td>
</tr><tr>
<td width="20%">N.82.91</td>
<td width="20%">N.82.91</td>
</tr><tr>
<td width="20%">N.82.92</td>
<td width="20%">N.82.92</td>
</tr><tr>
<td width="20%">N.82.99</td>
<td width="20%">N.82.99</td>
</tr><tr>
<td width="20%">O</td>
<td width="20%">O</td>
</tr><tr>
<td width="20%">O.84</td>
<td width="20%">O.84</td>
</tr><tr>
<td width="20%">O.84.1</td>
<td width="20%">O.84.1</td>
</tr><tr>
<td width="20%">O.84.11</td>
<td width="20%">O.84.11</td>
</tr><tr>
<td width="20%">O.84.12</td>
<td width="20%">O.84.12</td>
</tr><tr>
<td width="20%">O.84.13</td>
<td width="20%">O.84.13</td>
</tr><tr>
<td width="20%">O.84.2</td>
<td width="20%">O.84.2</td>
</tr><tr>
<td width="20%">O.84.21</td>
<td width="20%">O.84.21</td>
</tr><tr>
<td width="20%">O.84.22</td>
<td width="20%">O.84.22</td>
</tr><tr>
<td width="20%">O.84.23</td>
<td width="20%">O.84.23</td>
</tr><tr>
<td width="20%">O.84.24</td>
<td width="20%">O.84.24</td>
</tr><tr>
<td width="20%">O.84.25</td>
<td width="20%">O.84.25</td>
</tr><tr>
<td width="20%">O.84.3</td>
<td width="20%">O.84.3</td>
</tr><tr>
<td width="20%">O.84.30</td>
<td width="20%">O.84.30</td>
</tr><tr>
<td width="20%">P</td>
<td width="20%">P</td>
</tr><tr>
<td width="20%">P.85</td>
<td width="20%">P.85</td>
</tr><tr>
<td width="20%">P.85.1</td>
<td width="20%">P.85.1</td>
</tr><tr>
<td width="20%">P.85.10</td>
<td width="20%">P.85.10</td>
</tr><tr>
<td width="20%">P.85.2</td>
<td width="20%">P.85.2</td>
</tr><tr>
<td width="20%">P.85.20</td>
<td width="20%">P.85.20</td>
</tr><tr>
<td width="20%">P.85.3</td>
<td width="20%">P.85.3</td>
</tr><tr>
<td width="20%">P.85.31</td>
<td width="20%">P.85.31</td>
</tr><tr>
<td width="20%">P.85.32</td>
<td width="20%">P.85.32</td>
</tr><tr>
<td width="20%">P.85.4</td>
<td width="20%">P.85.4</td>
</tr><tr>
<td width="20%">P.85.41</td>
<td width="20%">P.85.41</td>
</tr><tr>
<td width="20%">P.85.42</td>
<td width="20%">P.85.42</td>
</tr><tr>
<td width="20%">P.85.5</td>
<td width="20%">P.85.5</td>
</tr><tr>
<td width="20%">P.85.51</td>
<td width="20%">P.85.51</td>
</tr><tr>
<td width="20%">P.85.52</td>
<td width="20%">P.85.52</td>
</tr><tr>
<td width="20%">P.85.53</td>
<td width="20%">P.85.53</td>
</tr><tr>
<td width="20%">P.85.59</td>
<td width="20%">P.85.59</td>
</tr><tr>
<td width="20%">P.85.6</td>
<td width="20%">P.85.6</td>
</tr><tr>
<td width="20%">P.85.60</td>
<td width="20%">P.85.60</td>
</tr><tr>
<td width="20%">Q</td>
<td width="20%">Q</td>
</tr><tr>
<td width="20%">Q.86</td>
<td width="20%">Q.86</td>
</tr><tr>
<td width="20%">Q.86.1</td>
<td width="20%">Q.86.1</td>
</tr><tr>
<td width="20%">Q.86.10</td>
<td width="20%">Q.86.10</td>
</tr><tr>
<td width="20%">Q.86.2</td>
<td width="20%">Q.86.2</td>
</tr><tr>
<td width="20%">Q.86.21</td>
<td width="20%">Q.86.21</td>
</tr><tr>
<td width="20%">Q.86.22</td>
<td width="20%">Q.86.22</td>
</tr><tr>
<td width="20%">Q.86.23</td>
<td width="20%">Q.86.23</td>
</tr><tr>
<td width="20%">Q.86.9</td>
<td width="20%">Q.86.9</td>
</tr><tr>
<td width="20%">Q.86.90</td>
<td width="20%">Q.86.90</td>
</tr><tr>
<td width="20%">Q.87</td>
<td width="20%">Q.87</td>
</tr><tr>
<td width="20%">Q.87.1</td>
<td width="20%">Q.87.1</td>
</tr><tr>
<td width="20%">Q.87.10</td>
<td width="20%">Q.87.10</td>
</tr><tr>
<td width="20%">Q.87.2</td>
<td width="20%">Q.87.2</td>
</tr><tr>
<td width="20%">Q.87.20</td>
<td width="20%">Q.87.20</td>
</tr><tr>
<td width="20%">Q.87.3</td>
<td width="20%">Q.87.3</td>
</tr><tr>
<td width="20%">Q.87.30</td>
<td width="20%">Q.87.30</td>
</tr><tr>
<td width="20%">Q.87.9</td>
<td width="20%">Q.87.9</td>
</tr><tr>
<td width="20%">Q.87.90</td>
<td width="20%">Q.87.90</td>
</tr><tr>
<td width="20%">Q.88</td>
<td width="20%">Q.88</td>
</tr><tr>
<td width="20%">Q.88.1</td>
<td width="20%">Q.88.1</td>
</tr><tr>
<td width="20%">Q.88.10</td>
<td width="20%">Q.88.10</td>
</tr><tr>
<td width="20%">Q.88.9</td>
<td width="20%">Q.88.9</td>
</tr><tr>
<td width="20%">Q.88.91</td>
<td width="20%">Q.88.91</td>
</tr><tr>
<td width="20%">Q.88.99</td>
<td width="20%">Q.88.99</td>
</tr><tr>
<td width="20%">R</td>
<td width="20%">R</td>
</tr><tr>
<td width="20%">R.90</td>
<td width="20%">R.90</td>
</tr><tr>
<td width="20%">R.90.0</td>
<td width="20%">R.90.0</td>
</tr><tr>
<td width="20%">R.90.01</td>
<td width="20%">R.90.01</td>
</tr><tr>
<td width="20%">R.90.02</td>
<td width="20%">R.90.02</td>
</tr><tr>
<td width="20%">R.90.03</td>
<td width="20%">R.90.03</td>
</tr><tr>
<td width="20%">R.90.04</td>
<td width="20%">R.90.04</td>
</tr><tr>
<td width="20%">R.91</td>
<td width="20%">R.91</td>
</tr><tr>
<td width="20%">R.91.0</td>
<td width="20%">R.91.0</td>
</tr><tr>
<td width="20%">R.91.01</td>
<td width="20%">R.91.01</td>
</tr><tr>
<td width="20%">R.91.02</td>
<td width="20%">R.91.02</td>
</tr><tr>
<td width="20%">R.91.03</td>
<td width="20%">R.91.03</td>
</tr><tr>
<td width="20%">R.91.04</td>
<td width="20%">R.91.04</td>
</tr><tr>
<td width="20%">R.92</td>
<td width="20%">R.92</td>
</tr><tr>
<td width="20%">R.92.0</td>
<td width="20%">R.92.0</td>
</tr><tr>
<td width="20%">R.92.00</td>
<td width="20%">R.92.00</td>
</tr><tr>
<td width="20%">R.93</td>
<td width="20%">R.93</td>
</tr><tr>
<td width="20%">R.93.1</td>
<td width="20%">R.93.1</td>
</tr><tr>
<td width="20%">R.93.11</td>
<td width="20%">R.93.11</td>
</tr><tr>
<td width="20%">R.93.12</td>
<td width="20%">R.93.12</td>
</tr><tr>
<td width="20%">R.93.13</td>
<td width="20%">R.93.13</td>
</tr><tr>
<td width="20%">R.93.19</td>
<td width="20%">R.93.19</td>
</tr><tr>
<td width="20%">R.93.2</td>
<td width="20%">R.93.2</td>
</tr><tr>
<td width="20%">R.93.21</td>
<td width="20%">R.93.21</td>
</tr><tr>
<td width="20%">R.93.29</td>
<td width="20%">R.93.29</td>
</tr><tr>
<td width="20%">S</td>
<td width="20%">S</td>
</tr><tr>
<td width="20%">S.94</td>
<td width="20%">S.94</td>
</tr><tr>
<td width="20%">S.94.1</td>
<td width="20%">S.94.1</td>
</tr><tr>
<td width="20%">S.94.11</td>
<td width="20%">S.94.11</td>
</tr><tr>
<td width="20%">S.94.12</td>
<td width="20%">S.94.12</td>
</tr><tr>
<td width="20%">S.94.2</td>
<td width="20%">S.94.2</td>
</tr><tr>
<td width="20%">S.94.20</td>
<td width="20%">S.94.20</td>
</tr><tr>
<td width="20%">S.94.9</td>
<td width="20%">S.94.9</td>
</tr><tr>
<td width="20%">S.94.91</td>
<td width="20%">S.94.91</td>
</tr><tr>
<td width="20%">S.94.92</td>
<td width="20%">S.94.92</td>
</tr><tr>
<td width="20%">S.94.99</td>
<td width="20%">S.94.99</td>
</tr><tr>
<td width="20%">S.95</td>
<td width="20%">S.95</td>
</tr><tr>
<td width="20%">S.95.1</td>
<td width="20%">S.95.1</td>
</tr><tr>
<td width="20%">S.95.11</td>
<td width="20%">S.95.11</td>
</tr><tr>
<td width="20%">S.95.12</td>
<td width="20%">S.95.12</td>
</tr><tr>
<td width="20%">S.95.2</td>
<td width="20%">S.95.2</td>
</tr><tr>
<td width="20%">S.95.21</td>
<td width="20%">S.95.21</td>
</tr><tr>
<td width="20%">S.95.22</td>
<td width="20%">S.95.22</td>
</tr><tr>
<td width="20%">S.95.23</td>
<td width="20%">S.95.23</td>
</tr><tr>
<td width="20%">S.95.24</td>
<td width="20%">S.95.24</td>
</tr><tr>
<td width="20%">S.95.25</td>
<td width="20%">S.95.25</td>
</tr><tr>
<td width="20%">S.95.29</td>
<td width="20%">S.95.29</td>
</tr><tr>
<td width="20%">S.96</td>
<td width="20%">S.96</td>
</tr><tr>
<td width="20%">S.96.0</td>
<td width="20%">S.96.0</td>
</tr><tr>
<td width="20%">S.96.01</td>
<td width="20%">S.96.01</td>
</tr><tr>
<td width="20%">S.96.02</td>
<td width="20%">S.96.02</td>
</tr><tr>
<td width="20%">S.96.03</td>
<td width="20%">S.96.03</td>
</tr><tr>
<td width="20%">S.96.04</td>
<td width="20%">S.96.04</td>
</tr><tr>
<td width="20%">S.96.09</td>
<td width="20%">S.96.09</td>
</tr><tr>
<td width="20%">T</td>
<td width="20%">T</td>
</tr><tr>
<td width="20%">T.97</td>
<td width="20%">T.97</td>
</tr><tr>
<td width="20%">T.97.0</td>
<td width="20%">T.97.0</td>
</tr><tr>
<td width="20%">T.97.00</td>
<td width="20%">T.97.00</td>
</tr><tr>
<td width="20%">T.98</td>
<td width="20%">T.98</td>
</tr><tr>
<td width="20%">T.98.1</td>
<td width="20%">T.98.1</td>
</tr><tr>
<td width="20%">T.98.10</td>
<td width="20%">T.98.10</td>
</tr><tr>
<td width="20%">T.98.2</td>
<td width="20%">T.98.2</td>
</tr><tr>
<td width="20%">T.98.20</td>
<td width="20%">T.98.20</td>
</tr><tr>
<td width="20%">U</td>
<td width="20%">U</td>
</tr><tr>
<td width="20%">U.99</td>
<td width="20%">U.99</td>
</tr><tr>
<td width="20%">U.99.0</td>
<td width="20%">U.99.0</td>
</tr><tr>
<td width="20%">U.99.00</td>
<td width="20%">U.99.00</td>
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
    <hr/><a name="DomainLegislationLevelValue_value"/>
<p><strong>LegislationLevelValue_value - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">LegislationLevelValue_value</td>
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
<td width="20%">international</td>
<td width="20%">international</td>
</tr><tr>
<td width="20%">european</td>
<td width="20%">european</td>
</tr><tr>
<td width="20%">national</td>
<td width="20%">national</td>
</tr><tr>
<td width="20%">sub-national</td>
<td width="20%">sub-national</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p>
