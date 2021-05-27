
#Addresses


<br/>
<strong>Geodatabase Documentation</strong>
<hr/>
<strong>Date: </strong>20210526173957.549057<br/>
<hr/>
<p><strong>Summary Information and Links</strong><br/><br/><a href="#FeatureDatasets">0 Feature Datasets and 1
Feature Classes</a><br/>No Topology Datasets<br/>No Geometric Networks<br/>No Rasters<br/><a href="#ObjectClasses">0 Tables (Object Classes)</a><br/><a href="#RelationshipClasses">0 Relationship
Classes</a><br/><a href="#Domains">1 Domain</a><br/></p>
<hr/>
<p><a name="FeatureDatasets"/><strong>Feature Datasets and Child Classes</strong></p><a name="Raster"/>
<p><strong>Rasters</strong></p><br/>
<hr/><a name="ObjectClasses"/>
<p><strong>Workspace-Level Tables and Feature Classes</strong></p>
    <a href="#FeatureClassAddress">Address - FeatureClass</a><br/>
<p/><br/>
<hr/><a name="RelationshipClasses"/>
<p><strong>Relationship Classes</strong></p><p/>
<hr/><br/><a name="Domains"/>
<p><strong>Domains</strong></p><a href="#DomainDomainExample">DomainExample</a><br/>
<p/>
    <p><hr/><br/><a name="FeatureClassAddress"/>
<p><strong>Address - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">Address</td>
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
<td width="*" style="border-color: white">Address</td>
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
<td width="*" style="border-color: white">Address</td>
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
<td width="8%">AddressAreaName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">AddressAreaName</td>
<td width="8%">An address component which represents the name of a geographic area or locality that groups a number of addressable objects for addressing purposes, without being an administrative unit.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">AdminUnitName_1stLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">AdminUnitName_1stLevel</td>
<td width="8%">Name of the Administrative Unit at the highest level in the national administrative hierarchy (country level).</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">AdminUnitName_2ndLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">AdminUnitName_2ndLevel</td>
<td width="8%">Name of the Administrative Unit at the 2nd level in the national administrative hierarchy.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">AdminUnitName_3rdLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">AdminUnitName_3rdLevel</td>
<td width="8%">Name of the Administrative Unit at the 3rd level in the national administrative hierarchy.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">AdminUnitName_4thLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">AdminUnitName_4thLevel</td>
<td width="8%">Name of the Administrative Unit at the 4th level in the national administrative hierarchy.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">AdminUnitName_5thLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">AdminUnitName_5thLevel</td>
<td width="8%">Name of the Administrative Unit at the 5th level in the national administrative hierarchy.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">AdminUnitName_6thLevel</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">AdminUnitName_6thLevel</td>
<td width="8%">Name of the Administrative Unit at the 6th level in the national administrative hierarchy.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">alternativeIdentifier</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">alternativeIdentifier</td>
<td width="8%">External, thematic identifier of the address spatial object, which enables interoperability with existing legacy systems or applications.</td>
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
<td width="8%">building_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">building_href</td>
<td width="8%">Building that the address is assigned to or associated with.</td>
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
<td width="8%"/>
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
<td width="8%">ld_addressIdentifierGeneral</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">ld_addressIdentifierGeneral</td>
<td width="8%">Address identifier composed by numbers and/or characters.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">ld_addressNumber</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">ld_addressNumber</td>
<td width="8%">Address identifier composed only by numbers.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">ld_addressNumber2ndExtension</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">ld_addressNumber2ndExtension</td>
<td width="8%">Second extension to the address number.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">ld_addressNumberExtension</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">ld_addressNumberExtension</td>
<td width="8%">Address identifier composed only by numbers.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">ld_buildingIdentifier</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">ld_buildingIdentifier</td>
<td width="8%">Building identifier composed by numbers and/or characters.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">ld_buildingIdentifierPrefix</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">ld_buildingIdentifierPrefix</td>
<td width="8%">Prefix to the building number.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">ld_cornerAddress1stIdentifier</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">ld_cornerAddress1stIdentifier</td>
<td width="8%">Address identifier related to the primary thoroughfare name in a corner address.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">ld_cornerAddress2ndIdentifier</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">ld_cornerAddress2ndIdentifier</td>
<td width="8%">Address identifier related to the secondary thoroughfare name in a corner address.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">ld_entranceDoorIdentifier</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">ld_entranceDoorIdentifier</td>
<td width="8%">Identifier for an entrance door, entrance gate, or covered entranceway.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">ld_floorIdentifier</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">ld_floorIdentifier</td>
<td width="8%">Identifier of a floor or level inside a building.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">ld_kilometrePoint</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">ld_kilometrePoint</td>
<td width="8%">A mark on a road whose number identifies the existing distance between the origin point of the road and that mark, measured along the road.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">ld_postalDeliveryIdentifier</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">ld_postalDeliveryIdentifier</td>
<td width="8%">Identifier of a postal delivery point.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">ld_staircaseIdentifier</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">ld_staircaseIdentifier</td>
<td width="8%">Identifier for a staircase, normally inside a building.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">ld_unitIdentifier</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">ld_unitIdentifier</td>
<td width="8%">Identifier of a door, dwelling, suite or room inside a building.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">locator_level</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">locator_level</td>
<td width="8%">The level to which the locator refers.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">locator_level_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">locator_level_href</td>
<td width="8%">The level to which the locator refers.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">locator_name</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">locator_name</td>
<td width="8%">A geographic name or descriptive text associated to a property identified by the locator.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">parentAddress</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">parentAddress</td>
<td width="8%">The main (parent) address with which this (sub) address is tightly connected.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">position_method</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">position_method</td>
<td width="8%">Description of how and by whom the geographic position of the address was created or derived.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">position_method_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">position_method_href</td>
<td width="8%">URI from the GeometryMethodValue Codelist</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">position_specification</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">position_specification</td>
<td width="8%">Information defining the specification used to create or derive this geographic position of the address.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">position_specification_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">position_specification_href</td>
<td width="8%">URI from the GeometrySpecificationValue Codelist</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">PostalDescriptor</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">PostalDescriptor</td>
<td width="8%">An address component which represents the identification of a subdivision of addresses and postal delivery points in a country, region or city for postal purposes.</td>
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
<td width="8%">Validity of the address component within the life-cycle (version) of the address component spatial object.</td>
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
<td width="8%">URI from the StatusValue Codelist</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">ThoroughfareName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">ThoroughfareName</td>
<td width="8%">Proper noun applied to thoroughfare.</td>
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
<td width="8%">ate and time at which the address component ceased or will cease to exist in the real world.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p></p>
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
