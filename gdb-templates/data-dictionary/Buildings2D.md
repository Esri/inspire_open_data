	<br/>
	<strong>Geodatabase Documentation</strong>
	<hr/>
	<strong>Date: </strong>20210526173956.6645516<br/>
	<hr/>
	<p><strong>Summary Information and Links</strong><br/><br/><a href="#FeatureDatasets">0 Feature Datasets and 2
			Feature Classes</a><br/>No Topology Datasets<br/>No Geometric Networks<br/>No Rasters<br/><a href="#ObjectClasses">1 Tables (Object Classes)</a><br/><a href="#RelationshipClasses">1 Relationship
			Classes</a><br/><a href="#Domains">1 Domain</a><br/></p>
	<hr/>
	<p><a name="FeatureDatasets"/><strong>Feature Datasets and Child Classes</strong></p><a name="Raster"/>
	<p><strong>Rasters</strong></p><br/>
	<hr/><a name="ObjectClasses"/>
	<p><strong>Workspace-Level Tables and Feature Classes</strong></p>
    <a href="#FeatureClassBuilding">Building - FeatureClass</a><br/><a href="#FeatureClassBuildingPart">BuildingPart - FeatureClass</a><br/><a href="#TableBuilding_part">Building_part - Table</a><br/>
	<p/><br/>
	<hr/><a name="RelationshipClasses"/>
	<p><strong>Relationship Classes</strong></p>
    <a href="#RelationshipClassRelB_B_part">RelB_B_part</a><br/>
	<p/>
	<hr/><br/><a name="Domains"/>
	<p><strong>Domains</strong></p><a href="#DomainDomainExample">DomainExample</a><br/>
	<p/>
    <p>	<hr/><br/><a name="FeatureClassBuilding"/>
	<p><strong>Building - FeatureClass</strong></p>
	<p>
	<table width="100%" style="border-color: white">
		<tbody>
			<tr>
				<td width="12%" style="border-color: white"><strong>Name</strong></td>
				<td width="*" style="border-color: white">Building</td>
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
				<td width="*" style="border-color: white">Building</td>
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
				<td width="*" style="border-color: white">Building</td>
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
</tr><tr>
	<td width="8%">beginLifespanVersion</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">beginLifespanVersion</td>
	<td width="8%">Date and time at which this version of the spatial object was inserted or changed in the spatial data set.	</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">buildingNature_1</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">buildingNature_1</td>
	<td width="8%">Characteristic of the building that makes it generally of interest for mappings applications. The characteristic may be related to the physical aspect and/or to the function of the building. Value from the BuildingNatureValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">buildingNature_1_href</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">buildingNature_1_href</td>
	<td width="8%">Characteristic of the building that makes it generally of interest for mappings applications. The characteristic may be related to the physical aspect and/or to the function of the building. URI from the BuildingNatureValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">buildingNature_2</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">buildingNature_2</td>
	<td width="8%">Characteristic of the building that makes it generally of interest for mappings applications. The characteristic may be related to the physical aspect and/or to the function of the building. Value from the BuildingNatureValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">buildingNature_2_href</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">buildingNature_2_href</td>
	<td width="8%">Characteristic of the building that makes it generally of interest for mappings applications. The characteristic may be related to the physical aspect and/or to the function of the building. URI from the BuildingNatureValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">buildingNature_3</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">buildingNature_3</td>
	<td width="8%">Characteristic of the building that makes it generally of interest for mappings applications. The characteristic may be related to the physical aspect and/or to the function of the building. Value from the BuildingNatureValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">conditionOfConstruction_href</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">conditionOfConstruction_href</td>
	<td width="8%">Condition of construction</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">currentUse_1_currentUse</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">currentUse_1_currentUse</td>
	<td width="8%">Activity hosted within the building. This attribute addresses mainly the buildings hosting human activities. Value from CurrentUseValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">currentUse_1_percentage</td>
	<td width="8%">Single</td>
	<td width="3%">4</td>
	<td width="8%">currentUse_1_percentage</td>
	<td width="8%">The proportion of the real world object, given as a percentage, devoted to this current use.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">dateOfConstruction_beginning</td>
	<td width="8%">Date</td>
	<td width="3%">8</td>
	<td width="8%">dateOfConstruction_beginning</td>
	<td width="8%">Date of construction. Beginning.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">dateOfConstruction_end</td>
	<td width="8%">Date</td>
	<td width="3%">8</td>
	<td width="8%">dateOfConstruction_end</td>
	<td width="8%">Date of construction. End.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">dateOfDemolition_beginning</td>
	<td width="8%">Date</td>
	<td width="3%">8</td>
	<td width="8%">dateOfDemolition_beginning</td>
	<td width="8%">Date of demolition. Beginning.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">dateOfDemolition_end</td>
	<td width="8%">Date</td>
	<td width="3%">8</td>
	<td width="8%">dateOfDemolition_end</td>
	<td width="8%">Date of demolition. End.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">dateOfRenovation_beginning</td>
	<td width="8%">Date</td>
	<td width="3%">8</td>
	<td width="8%">dateOfRenovation_beginning</td>
	<td width="8%">Date of last major renovation. Beginning.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">dateOfRenovation_end</td>
	<td width="8%">Date</td>
	<td width="3%">8</td>
	<td width="8%">dateOfRenovation_end</td>
	<td width="8%">Date of last major renovation. End.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">elevationReference</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">elevationReference</td>
	<td width="8%">Element where the elevation was measured.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">elevationValue</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">elevationValue</td>
	<td width="8%">Value of the elevation in meter</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">endLifespanVersion</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">endLifespanVersion</td>
	<td width="8%">Date and time at which this version of the spatial object was superseded or retired in the spatial data set.	</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">externalReference_reference</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">externalReference_reference</td>
	<td width="8%">Reference. Thematic identifier of the spatial object or of any piece of information related to the spatial object.</td>
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
	<td width="8%">heightAboveGround_value</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">heightAboveGround_value</td>
	<td width="8%">Value of the height above ground in meters.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">heightReference</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">heightReference</td>
	<td width="8%">Element used as the high reference. Value from the ElevationReferenceValue Codelist</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">heightReference_href</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">heightReference_href</td>
	<td width="8%">Element used as the high reference. URI from the ElevationReferenceValue Codelist</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">horizontalEstimatedAccuracy</td>
	<td width="8%">Single</td>
	<td width="3%">4</td>
	<td width="8%">horizontalEstimatedAccuracy</td>
	<td width="8%">Horizontal geometry estimated accuracy in meters. The estimated absolute positional accuracy of the (X,Y) coordinates of the building geometry, in the INSPIRE official Coordinate Reference System. Absolute positional accuracy is defined as the mean value of the positional uncertainties for a set of positions where the positional uncertainties are defined as the distance between a measured position and what is considered as the corresponding true position.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">horizontalReference</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">horizontalReference</td>
	<td width="8%">Element of the real world object that was captured by the (X,Y) coordinates of the LoD1 Multisurface or Solid geometry</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">horizontalReference_href</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">horizontalReference_href</td>
	<td width="8%">Element of the real world object that was captured by the (X,Y) coordinates of the LoD1 Multisurface or Solid geometry</td>
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
	<td width="8%">A local identifier, assigned by the data provider. The local identifier is unique within the namespace, that is no other spatial object carries the same unique identifier.	</td>
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
	<td width="8%">Namespace uniquely identifying the data source of the spatial object.	</td>
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
	<td width="8%">The identifier of the particular version of the spatial object, with a maximum length of 25 characters. If the specification of a spatial object type with an external object identifier includes life-cycle information, the version identifier is used to distinguish between the different versions of a spatial object. Within the set of all versions of a spatial object, the version identifier is unique	</td>
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
	<td width="8%">Name of the Construction</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">name_1_language</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">name_1_language</td>
	<td width="8%">Language used in the name_1 field</td>
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
	<td width="8%">Name of the Construction</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">name_2_language</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">name_2_language</td>
	<td width="8%">Language used in the name_2 field</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">name_3</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">name_3</td>
	<td width="8%">Name of the Construction</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">name_3_language</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">name_3_language</td>
	<td width="8%">Language used in the name_2 field</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">numberOfBuildingUnits</td>
	<td width="8%">Integer</td>
	<td width="3%">4</td>
	<td width="8%">numberOfBuildingUnits</td>
	<td width="8%">Number of building units in the building. A BuildingUnit is a subdivision of Building with its own lockable access from the outside or from a common area (i.e. not from another BuildingUnit), which is atomic, functionally independent, and may be separately sold, rented out, inherited, etc.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">numberOfDwellings</td>
	<td width="8%">Integer</td>
	<td width="3%">4</td>
	<td width="8%">numberOfDwellings</td>
	<td width="8%">Number of dwellings</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">numberOfFloorsAboveGround</td>
	<td width="8%">Integer</td>
	<td width="3%">4</td>
	<td width="8%">numberOfFloorsAboveGround</td>
	<td width="8%">Number of floors above ground</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">referenceGeometry</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">referenceGeometry</td>
	<td width="8%">Boolean Reference geometry</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">status</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">status</td>
	<td width="8%">The way the height has been captured. Value from the HeightStatusValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">status_href</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">status_href</td>
	<td width="8%">The way the height has been captured. URI from the HeightStatusValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">verticalEstimatedAccuracy</td>
	<td width="8%">Single</td>
	<td width="3%">4</td>
	<td width="8%">verticalEstimatedAccuracy</td>
	<td width="8%">Vertical geometry estimated accuracy in meters. The estimated absolute positional accuracy of the Z coordinates of the  building geometry, in the INSPIRE official Coordinate Reference System. Absolute positional accuracy is defined as the mean value of the positional uncertainties for a set of positions where the positional uncertainties are defined as the distance between a measured position and what is considered as the corresponding true position.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">verticalReference</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">verticalReference</td>
	<td width="8%">Element of the building that was captured by vertical coordinates. Value from the ElevationReferenceValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">verticalReference_href</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">verticalReference_href</td>
	<td width="8%">Element of the building that was captured by vertical coordinates. URI from the ElevationReferenceValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr>
		</tbody>
	</table>
	</p></p><p>	<hr/><br/><a name="FeatureClassBuildingPart"/>
	<p><strong>BuildingPart - FeatureClass</strong></p>
	<p>
	<table width="100%" style="border-color: white">
		<tbody>
			<tr>
				<td width="12%" style="border-color: white"><strong>Name</strong></td>
				<td width="*" style="border-color: white">BuildingPart</td>
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
				<td width="*" style="border-color: white">BuildingPart</td>
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
				<td width="*" style="border-color: white">BuildingPart</td>
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
</tr><tr>
	<td width="8%">beginLifespanVersion</td>
	<td width="8%">Date</td>
	<td width="3%">8</td>
	<td width="8%">beginLifespanVersion</td>
	<td width="8%">Date and time at which this version of the spatial object was inserted or changed in the spatial data set.	</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">buildingNature_1</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">buildingNature_1</td>
	<td width="8%">Characteristic of the building that makes it generally of interest for mappings applications. The characteristic may be related to the physical aspect and/or to the function of the building. Value from the BuildingNatureValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">buildingNature_2</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">buildingNature_2</td>
	<td width="8%">Characteristic of the building that makes it generally of interest for mappings applications. The characteristic may be related to the physical aspect and/or to the function of the building. Value from the BuildingNatureValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">buildingNature_2_href</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">buildingNature_2_href</td>
	<td width="8%">Characteristic of the building that makes it generally of interest for mappings applications. The characteristic may be related to the physical aspect and/or to the function of the building. URI from the BuildingNatureValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">buildingNature_3</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">buildingNature_3</td>
	<td width="8%">Characteristic of the building that makes it generally of interest for mappings applications. The characteristic may be related to the physical aspect and/or to the function of the building. Value from the BuildingNatureValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">conditionOfConstruction</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">conditionOfConstruction</td>
	<td width="8%">Condition of construction. Value from the ConditionOfConstructionValue Codelist</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">conditionOfConstruction_href</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">conditionOfConstruction_href</td>
	<td width="8%">Condition of construction</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">currentUse_1_currentUse</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">currentUse_1_currentUse</td>
	<td width="8%">Activity hosted within the building. This attribute addresses mainly the buildings hosting human activities. Value from CurrentUseValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">currentUse_1_currentUse_href</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">currentUse_1_currentUse_href</td>
	<td width="8%">Activity hosted within the building. This attribute addresses mainly the buildings hosting human activities. URI from CurrentUseValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">currentUse_1_percentage</td>
	<td width="8%">Single</td>
	<td width="3%">4</td>
	<td width="8%">currentUse_1_percentage</td>
	<td width="8%">The proportion of the real world object, given as a percentage, devoted to this current use.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">currentUse_2_currentUse</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">currentUse_2_currentUse</td>
	<td width="8%">Activity hosted within the building. This attribute addresses mainly the buildings hosting human activities. Value from CurrentUseValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">currentUse_3_currentUse</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">currentUse_3_currentUse</td>
	<td width="8%">Activity hosted within the building. This attribute addresses mainly the buildings hosting human activities. Value from CurrentUseValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">dateOfConstruction_beginning</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">dateOfConstruction_beginning</td>
	<td width="8%">Date of construction. Beginning.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">dateOfConstruction_end</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">dateOfConstruction_end</td>
	<td width="8%">Date of construction. End.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">dateOfDemolition_beginning</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">dateOfDemolition_beginning</td>
	<td width="8%">Date of demolition. Beginning.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">dateOfDemolition_end</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">dateOfDemolition_end</td>
	<td width="8%">Date of demolition. End.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">dateOfRenovation_beginning</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">dateOfRenovation_beginning</td>
	<td width="8%">Date of last major renovation. Beginning.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">dateOfRenovation_end</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">dateOfRenovation_end</td>
	<td width="8%">Date of last major renovation. End.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">elevationReference</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">elevationReference</td>
	<td width="8%">Element where the elevation was measured. Value from the ElevationReferenceValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">elevationValue</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">elevationValue</td>
	<td width="8%">Value of the elevation in meters.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">endLifespanVersion</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">endLifespanVersion</td>
	<td width="8%">Date and time at which this version of the spatial object was superseded or retired in the spatial data set.	</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">externalReference_reference</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">externalReference_reference</td>
	<td width="8%">Reference. Thematic identifier of the spatial object or of any piece of information related to the spatial object.</td>
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
	<td width="8%"/>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">heightReference</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">heightReference</td>
	<td width="8%">Element used as the high reference. Value from the ElevationReferenceValue Codelist</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">heightReference_href</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">heightReference_href</td>
	<td width="8%">Element used as the high reference. URI from the ElevationReferenceValue Codelist</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">horizontalEstimatedAccuracy</td>
	<td width="8%">Single</td>
	<td width="3%">4</td>
	<td width="8%">horizontalEstimatedAccuracy</td>
	<td width="8%">Horizontal geometry estimated accuracy in meters. The estimated absolute positional accuracy of the (X,Y) coordinates of the building geometry, in the INSPIRE official Coordinate Reference System. Absolute positional accuracy is defined as the mean value of the positional uncertainties for a set of positions where the positional uncertainties are defined as the distance between a measured position and what is considered as the corresponding true position.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">horizontalReference</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">horizontalReference</td>
	<td width="8%">Element of the real world object that was captured by the (X,Y) coordinates of the LoD1 Multisurface or Solid geometry</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">horizontalReference_href</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">horizontalReference_href</td>
	<td width="8%">Element of the real world object that was captured by the (X,Y) coordinates of the LoD1 Multisurface or Solid geometry</td>
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
	<td width="8%">A local identifier, assigned by the data provider. The local identifier is unique within the namespace, that is no other spatial object carries the same unique identifier.	</td>
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
	<td width="8%">Namespace uniquely identifying the data source of the spatial object.	</td>
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
	<td width="8%">The identifier of the particular version of the spatial object, with a maximum length of 25 characters. If the specification of a spatial object type with an external object identifier includes life-cycle information, the version identifier is used to distinguish between the different versions of a spatial object. Within the set of all versions of a spatial object, the version identifier is unique	</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">lowReference</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">lowReference</td>
	<td width="8%">Element used as the low reference. Value from the ElevationReferenceValue Codelist</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">lowReference_href</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">lowReference_href</td>
	<td width="8%">Element used as the low reference. URI from the ElevationReferenceValue Codelist</td>
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
	<td width="8%">Name of the Construction</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">name_1_language</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">name_1_language</td>
	<td width="8%">Language used in the name_1 field</td>
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
	<td width="8%">Name of the Construction</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">name_2_language</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">name_2_language</td>
	<td width="8%">Language used in the name_2 field</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">name_3</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">name_3</td>
	<td width="8%">Name of the Construction</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">name_3_language</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">name_3_language</td>
	<td width="8%">Language used in the name_2 field</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">numberOfBuildingUnits</td>
	<td width="8%">Integer</td>
	<td width="3%">4</td>
	<td width="8%">numberOfBuildingUnits</td>
	<td width="8%">Number of building units in the building. A BuildingUnit is a subdivision of Building with its own lockable access from the outside or from a common area (i.e. not from another BuildingUnit), which is atomic, functionally independent, and may be separately sold, rented out, inherited, etc.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">numberOfDwellings</td>
	<td width="8%">Integer</td>
	<td width="3%">4</td>
	<td width="8%">numberOfDwellings</td>
	<td width="8%">Number of dwellings</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">numberOfFloorsAboveGround</td>
	<td width="8%">Integer</td>
	<td width="3%">4</td>
	<td width="8%">numberOfFloorsAboveGround</td>
	<td width="8%">Number of floors above ground</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">referenceGeometry</td>
	<td width="8%">Integer</td>
	<td width="3%">4</td>
	<td width="8%">referenceGeometry</td>
	<td width="8%">Boolean Reference geometry</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">status</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">status</td>
	<td width="8%">The way the height has been captured. Value from the HeightStatusValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">status_href</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">status_href</td>
	<td width="8%">The way the height has been captured. URI from the HeightStatusValue Codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">value</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">value</td>
	<td width="8%">Value of the height above ground in meters.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">verticalEstimatedAccuracy</td>
	<td width="8%">Single</td>
	<td width="3%">4</td>
	<td width="8%">verticalEstimatedAccuracy</td>
	<td width="8%">Vertical geometry estimated accuracy in meters. The estimated absolute positional accuracy of the Z coordinates of the  building geometry, in the INSPIRE official Coordinate Reference System. Absolute positional accuracy is defined as the mean value of the positional uncertainties for a set of positions where the positional uncertainties are defined as the distance between a measured position and what is considered as the corresponding true position.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">verticalReference</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">verticalReference</td>
	<td width="8%">Element of the building that was captured by vertical coordinates. Valuefrom the ElevationReferenceValue codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr><tr>
	<td width="8%">verticalReference_href</td>
	<td width="8%">String</td>
	<td width="3%">254</td>
	<td width="8%">verticalReference_href</td>
	<td width="8%">Element of the building that was captured by vertical coordinates. URI from the ElevationReferenceValue codelist.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr>
		</tbody>
	</table>
	</p></p>

	<p><hr/><a name="TableBuilding_part"/>
	<p><strong>Building_part - Table</strong></p>
	<table width="100%" style="border-color: white">
		<tbody>
			<tr>
				<td width="12%" style="border-color: white"><strong>Name</strong></td>
				<td width="*" style="border-color: white">Building_part</td>
			</tr>
			<tr>
				<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
				<td width="*" style="border-color: white">Building_part</td>
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
				<td width="*" style="border-color: white">Building_part</td>
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
	<td width="8%">part</td>
	<td width="8%">Integer</td>
	<td width="3%">4</td>
	<td width="8%">part</td>
	<td width="8%">featureId of The building parts composing the Building. A building may be a simple building (with no BuildingPart) or a composed building (with several BuildingParts).</td>
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
	<td width="8%">Reference to featureId field in parent 'Building'.</td>
	<td width="8%"><a href="#Domain"/></td>
	<td width="8%"/>
	<td width="8%">true</td>
	<td/>
	<td/>
</tr>
		</tbody>
	</table>
</p>
    <p><hr/><a name="RelationshipClassRelB_B_part"/>
	<p><strong>RelB_B_part - RelationshipClass</strong></p>
	<table width="100%">
		<tbody>
			<tr>
				<td width="12%" style="border-color: white"><strong>Name</strong></td>
				<td width="*" style="border-color: white">RelB_B_part</td>
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
				<td width="*" style="border-color: white">Building_part</td>
			</tr>
			<tr>
				<td width="12%" style="border-color: white"><strong>BackwardPathLabel</strong></td>
				<td width="*" style="border-color: white">Building</td>
			</tr>
		</tbody>
	</table>
	<table width="100%" style="border-color: white">
		<tbody>
			<tr>
				<td width="12%" style="border-color: white"><strong>Description</strong></td>
				<td width="*" style="border-color: white">RelB_B_part</td>
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
				<td width="30%">Building</td>
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
				<td width="30%">Building_part</td>
				<td width="30%"/>
				<td width="30%"/>
			</tr>
		</tbody>
	</table></p>

	<hr/><a name="DomainDomainExample"/>
	<p><strong>DomainExample - Domain</strong></p>
	<p>
	<table width="100%" style="border-color: white">
		<tbody>
			<tr>
				<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
				<td width="*" style="border-color: white">DomainExample</td>
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
				<td width="20%">Val1</td>
				<td width="20%">Val1</td>
			</tr>
			<tr>
				<td width="20%">Val2</td>
				<td width="20%">Val2</td>
			</tr>
			</tr>
		</tbody>
	</table>
	</p>
	<hr/>
