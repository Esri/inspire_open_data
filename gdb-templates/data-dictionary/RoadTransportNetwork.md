
#RoadTransportNetwork


<br/>
<strong>Geodatabase Documentation</strong>
<hr/>
<strong>Date: </strong>20250228144325.982979<br/>
<hr/>
<p><strong>Summary Information and Links</strong><br/><br/><a href="#FeatureDatasets">0 Feature Datasets and 5
Feature Classes</a><br/>No Topology Datasets<br/>No Geometric Networks<br/>No Rasters<br/><a href="#ObjectClasses">8 Tables (Object Classes)</a><br/><a href="#RelationshipClasses">2 Relationship
Classes</a><br/><a href="#Domains">4 Domains</a><br/></p>
<hr/>
<p><a name="FeatureDatasets"/><strong>Feature Datasets and Child Classes</strong></p><a name="Raster"/>
<p><strong>Rasters</strong></p><br/>
<hr/><a name="ObjectClasses"/>
<p><strong>Workspace-Level Tables and Feature Classes</strong></p>
    <a href="#TableERoad">ERoad - Table</a><br/><a href="#TableEroad_link">Eroad_link - Table</a><br/><a href="#TableGradeSeparatedCrossing">GradeSeparatedCrossing - Table</a><br/><a href="#TableGradeSeparatedCrossing_element">GradeSeparatedCrossing_element - Table</a><br/><a href="#TableRoad">Road - Table</a><br/><a href="#FeatureClassRoadArea">RoadArea - FeatureClass</a><br/><a href="#FeatureClassRoadLink">RoadLink - FeatureClass</a><br/><a href="#FeatureClassRoadNode">RoadNode - FeatureClass</a><br/><a href="#FeatureClassRoadServiceArea">RoadServiceArea - FeatureClass</a><br/><a href="#TableRoad_link">Road_link - Table</a><br/><a href="#TableTransportNetwork">TransportNetwork - Table</a><br/><a href="#TableTransportNetwork_elements">TransportNetwork_elements - Table</a><br/><a href="#FeatureClassVehicleTrafficArea">VehicleTrafficArea - FeatureClass</a><br/>
<p/><br/>
<hr/><a name="RelationshipClasses"/>
<p><strong>Relationship Classes</strong></p>
    <a href="#RelationshipClassRelR_R_link">RelR_R_link</a><br/><a href="#RelationshipClassRelTN_TN_elements">RelTN_TN_elements</a><br/>
<p/>
<hr/><br/><a name="Domains"/>
<p><strong>Domains</strong></p>
   <a href="#DomainFormOfRoadNodeValue">FormOfRoadNodeValue</a><br/><a href="#DomainFormOfRoadNodeValue_value">FormOfRoadNodeValue_value</a><br/><a href="#DomainTransportTypeValue">TransportTypeValue</a><br/><a href="#DomainTransportTypeValue_value">TransportTypeValue_value</a><br/>
    <p><hr/><br/><a name="FeatureClassRoadArea"/>
<p><strong>RoadArea - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">RoadArea</td>
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
<td width="*" style="border-color: white">RoadArea</td>
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
<td width="*" style="border-color: white">RoadArea</td>
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
<td width="8%">geographicalName_language</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">geographicalName_language</td>
<td width="8%">Language of the geographical name.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">geographicalName_name</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">geographicalName_name</td>
<td width="8%">A geographical name that is used to identify the transport network object in the real world. It provides a 'key' for implicitly associating different representations of the object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inNetwork</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">inNetwork</td>
<td width="8%">RID of the TransportNetwork this element belongs to.</td>
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
<td width="8%">validFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">validFrom</td>
<td width="8%">The time when the transport property started to exist in the real world.</td>
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
<td width="8%">The time from which the transport property no longer exists in the real world.</td>
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
</p></p><p><hr/><br/><a name="FeatureClassRoadLink"/>
<p><strong>RoadLink - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">RoadLink</td>
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
<td width="*" style="border-color: white">RoadLink</td>
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
<td width="*" style="border-color: white">RoadLink</td>
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
<td width="8%">endNode</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">endNode</td>
<td width="8%">The featureId of the optional end node for this link.</td>
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
<td width="8%">fictitious</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">fictitious</td>
<td width="8%">Indicator that the centreline geometry of the link is a straight line with no intermediate control points – unless the straight line represents the geography in the resolution of the data set appropriately. A value of 0 represents false a value of 1 represents true.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">geographicalName_language</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">geographicalName_language</td>
<td width="8%">Language of the geographical name.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">geographicalName_name</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">geographicalName_name</td>
<td width="8%">A geographical name that is used to identify the transport network object in the real world. It provides a 'key' for implicitly associating different representations of the object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inNetwork</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">inNetwork</td>
<td width="8%">RID of the TransportNetwork this element belongs to.</td>
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
<td width="8%">startNode</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">startNode</td>
<td width="8%">The featureId of the optional start node for this link.</td>
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
<td width="8%">The time when the transport property started to exist in the real world.</td>
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
<td width="8%">The time from which the transport property no longer exists in the real world.</td>
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
</p></p><p><hr/><br/><a name="FeatureClassRoadNode"/>
<p><strong>RoadNode - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">RoadNode</td>
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
<td width="*" style="border-color: white">RoadNode</td>
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
<td width="*" style="border-color: white">RoadNode</td>
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
<td width="8%">formOfRoadNode</td>
<td width="8%">String</td>
<td width="3%">2048</td>
<td width="8%">formOfRoadNode</td>
<td width="8%">Description of the function of a road node in the road transport network.</td>
<td width="8%"><a href="#DomainFormOfRoadNodeValue_value">FormOfRoadNodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">formOfRoadNode_href</td>
<td width="8%">String</td>
<td width="3%">2048</td>
<td width="8%">formOfRoadNode_href</td>
<td width="8%">URI from the INSPIRE code list register - FormOfRoadNodeValue <a href="https://inspire.ec.europa.eu/codelist/FormOfRoadNodeValue">https://inspire.ec.europa.eu/codelist/FormOfRoadNodeValue</a></td>
<td width="8%"><a href="#DomainFormOfRoadNodeValue">FormOfRoadNodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">geographicalName_language</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">geographicalName_language</td>
<td width="8%">Language of the geographical name.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">geographicalName_name</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">geographicalName_name</td>
<td width="8%">A geographical name that is used to identify the transport network object in the real world. It provides a 'key' for implicitly associating different representations of the object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inNetwork</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">inNetwork</td>
<td width="8%">RID of the TransportNetwork this element belongs to.</td>
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
<td width="8%">validFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">validFrom</td>
<td width="8%">The time when the transport property started to exist in the real world.</td>
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
<td width="8%">The time from which the transport property no longer exists in the real world.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p></p><p><hr/><br/><a name="FeatureClassRoadServiceArea"/>
<p><strong>RoadServiceArea - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">RoadServiceArea</td>
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
<td width="*" style="border-color: white">RoadServiceArea</td>
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
<td width="*" style="border-color: white">RoadServiceArea</td>
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
<td width="8%">geographicalName_language</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">geographicalName_language</td>
<td width="8%">Language of the geographical name.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">geographicalName_name</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">geographicalName_name</td>
<td width="8%">A geographical name that is used to identify the transport network object in the real world. It provides a 'key' for implicitly associating different representations of the object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inNetwork</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">inNetwork</td>
<td width="8%">RID of the TransportNetwork this element belongs to.</td>
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
<td width="8%">validFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">validFrom</td>
<td width="8%">The time when the transport property started to exist in the real world.</td>
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
<td width="8%">The time from which the transport property no longer exists in the real world.</td>
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
</p></p><p><hr/><br/><a name="FeatureClassVehicleTrafficArea"/>
<p><strong>VehicleTrafficArea - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">VehicleTrafficArea</td>
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
<td width="*" style="border-color: white">VehicleTrafficArea</td>
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
<td width="*" style="border-color: white">VehicleTrafficArea</td>
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
<td width="8%">geographicalName_language</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">geographicalName_language</td>
<td width="8%">Language of the geographical name.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">geographicalName_name</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">geographicalName_name</td>
<td width="8%">A geographical name that is used to identify the transport network object in the real world. It provides a 'key' for implicitly associating different representations of the object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inNetwork</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">inNetwork</td>
<td width="8%">RID of the TransportNetwork this element belongs to.</td>
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
<td width="8%">validFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">validFrom</td>
<td width="8%">The time when the transport property started to exist in the real world.</td>
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
<td width="8%">The time from which the transport property no longer exists in the real world.</td>
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
<p><hr/><a name="TableERoad"/>
<p><strong>ERoad - Table</strong></p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">ERoad</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">ERoad</td>
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
<td width="*" style="border-color: white">ERoad</td>
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
<td width="8%">europeanRouteNumber</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">europeanRouteNumber</td>
<td width="8%">Code, identifying the route in the international E-road network. The code always starts with a letter 'E', followed by a one-, two- or three-digit number.</td>
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
<td width="8%">geographicalName_language</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">geographicalName_language</td>
<td width="8%">Language of the geographical name.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">geographicalName_name</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">geographicalName_name</td>
<td width="8%">A geographical name that is used to identify the transport network object in the real world. It provides a 'key' for implicitly associating different representations of the object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inNetwork</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">inNetwork</td>
<td width="8%">RID of the TransportNetwork this element belongs to.</td>
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
<td width="8%">validFrom</td>
<td width="8%">Date</td>
<td width="3%">8</td>
<td width="8%">validFrom</td>
<td width="8%">The time when the transport property started to exist in the real world.</td>
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
<td width="8%">The time from which the transport property no longer exists in the real world.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p><p><hr/><a name="TableEroad_link"/>
<p><strong>Eroad_link - Table</strong></p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">Eroad_link</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">Eroad_link</td>
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
<td width="*" style="border-color: white">Eroad_link</td>
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
<td width="8%">link</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">link</td>
<td width="8%">Reference to featureId of a 'RoadLink' which is part of this Eroad.</td>
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
<td width="8%">Reference to featureId field in parent 'ERoad'.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p><p><hr/><a name="TableGradeSeparatedCrossing"/>
<p><strong>GradeSeparatedCrossing - Table</strong></p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">GradeSeparatedCrossing</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">GradeSeparatedCrossing</td>
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
<td width="*" style="border-color: white">GradeSeparatedCrossing</td>
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
<td width="8%">inNetwork</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">inNetwork</td>
<td width="8%">RID of the TransportNetwork this element belongs to.</td>
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
</tr>
</tbody>
</table>
</p><p><hr/><a name="TableGradeSeparatedCrossing_element"/>
<p><strong>GradeSeparatedCrossing_element - Table</strong></p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">GradeSeparatedCrossing_element</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">GradeSeparatedCrossing_element</td>
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
<td width="*" style="border-color: white">GradeSeparatedCrossing_element</td>
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
<td width="8%">element</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">element</td>
<td width="8%">featureId of the referenced RoadLink. Sequence of crossing links. The order reflects their elevation; the first link is the lower link.</td>
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
<td width="8%">Reference to featureId field in parent 'GradeSeparatedCrossing'.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p><p><hr/><a name="TableRoad"/>
<p><strong>Road - Table</strong></p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">Road</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">Road</td>
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
<td width="*" style="border-color: white">Road</td>
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
<td width="8%">geographicalName_language</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">geographicalName_language</td>
<td width="8%">Language of the geographical name.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">geographicalName_name</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">geographicalName_name</td>
<td width="8%">A geographical name that is used to identify the transport network object in the real world. It provides a 'key' for implicitly associating different representations of the object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inNetwork</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">inNetwork</td>
<td width="8%">RID of the TransportNetwork this element belongs to.</td>
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
<td width="8%">localRoadCode</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">localRoadCode</td>
<td width="8%">Identification code assigned to the road by the local road authority.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">nationalRoadCode</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">nationalRoadCode</td>
<td width="8%">The national number of the road.</td>
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
<td width="8%">The time when the transport property started to exist in the real world.</td>
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
<td width="8%">The time from which the transport property no longer exists in the real world.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p><p><hr/><a name="TableRoad_link"/>
<p><strong>Road_link - Table</strong></p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">Road_link</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">Road_link</td>
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
<td width="*" style="border-color: white">Road_link</td>
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
<td width="8%">link</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">link</td>
<td width="8%">Reference to featureId of a 'RoadLink' which is part of this Road.</td>
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
<td width="8%">Reference to featureId field in parent 'Road'.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p><p><hr/><a name="TableTransportNetwork"/>
<p><strong>TransportNetwork - Table</strong></p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">TransportNetwork</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">TransportNetwork</td>
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
<td width="*" style="border-color: white">TransportNetwork</td>
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
<td width="8%">geographicalName_language</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">geographicalName_language</td>
<td width="8%">Language of the geographical name.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">geographicalName_name</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">geographicalName_name</td>
<td width="8%">A geographical name that is used to identify the transport network object in the real world. It provides a 'key' for implicitly associating different representations of the object.</td>
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
<td width="8%">typeOfTransport</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">typeOfTransport</td>
<td width="8%">Type of transport network, based on the type of infrastructure the network uses.</td>
<td width="8%"><a href="#DomainTransportTypeValue_value">TransportTypeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">typeOfTransport_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">typeOfTransport_href</td>
<td width="8%">URI from the INSPIRE code list register - TransportTypeValue <a href="https://inspire.ec.europa.eu/codelist/TransportTypeValue">https://inspire.ec.europa.eu/codelist/TransportTypeValue</a></td>
<td width="8%"><a href="#DomainTransportTypeValue">TransportTypeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p><p><hr/><a name="TableTransportNetwork_elements"/>
<p><strong>TransportNetwork_elements - Table</strong></p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">TransportNetwork_elements</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">TransportNetwork_elements</td>
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
<td width="*" style="border-color: white">TransportNetwork_elements</td>
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
<td width="8%">element</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">element</td>
<td width="8%">featureId of the referenced NetworkElement.</td>
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
<td width="8%">Reference to featureId field in parent 'TransportNetwork'.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p>
    <p><hr/><a name="RelationshipClassRelR_R_link"/>
<p><strong>RelR_R_link - RelationshipClass</strong></p>
<table width="100%">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">RelR_R_link</td>
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
<td width="*" style="border-color: white">Road_link</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>BackwardPathLabel</strong></td>
<td width="*" style="border-color: white">Road</td>
</tr>
</tbody>
</table>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Description</strong></td>
<td width="*" style="border-color: white">RelR_R_link</td>
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
<td width="30%">Road</td>
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
<td width="30%">Road_link</td>
<td width="30%"/>
<td width="30%"/>
</tr>
</tbody>
</table></p><p><hr/><a name="RelationshipClassRelTN_TN_elements"/>
<p><strong>RelTN_TN_elements - RelationshipClass</strong></p>
<table width="100%">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">RelTN_TN_elements</td>
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
<td width="*" style="border-color: white">TransportNetwork_elements</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>BackwardPathLabel</strong></td>
<td width="*" style="border-color: white">TransportNetwork</td>
</tr>
</tbody>
</table>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Description</strong></td>
<td width="*" style="border-color: white">RelTN_TN_elements</td>
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
<td width="30%">TransportNetwork</td>
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
<td width="30%">TransportNetwork_elements</td>
<td width="30%"/>
<td width="30%"/>
</tr>
</tbody>
</table></p>
    <p>
    <hr/><a name="DomainFormOfRoadNodeValue"/>
<p><strong>FormOfRoadNodeValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">FormOfRoadNodeValue</td>
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
<td width="20%">http://inspire.ec.europa.eu/codelist/FormOfRoadNodeValue/enclosedTrafficArea</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/FormOfRoadNodeValue/enclosedTrafficArea</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/FormOfRoadNodeValue/junction</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/FormOfRoadNodeValue/junction</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/FormOfRoadNodeValue/levelCrossing</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/FormOfRoadNodeValue/levelCrossing</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/FormOfRoadNodeValue/pseudoNode</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/FormOfRoadNodeValue/pseudoNode</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/FormOfRoadNodeValue/roadEnd</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/FormOfRoadNodeValue/roadEnd</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/FormOfRoadNodeValue/roadServiceArea</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/FormOfRoadNodeValue/roadServiceArea</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/FormOfRoadNodeValue/roundabout</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/FormOfRoadNodeValue/roundabout</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/FormOfRoadNodeValue/trafficSquare</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/FormOfRoadNodeValue/trafficSquare</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainFormOfRoadNodeValue_value"/>
<p><strong>FormOfRoadNodeValue_value - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">FormOfRoadNodeValue_value</td>
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
<td width="20%">enclosedTrafficArea</td>
<td width="20%">enclosedTrafficArea</td>
</tr><tr>
<td width="20%">junction</td>
<td width="20%">junction</td>
</tr><tr>
<td width="20%">levelCrossing</td>
<td width="20%">levelCrossing</td>
</tr><tr>
<td width="20%">pseudoNode</td>
<td width="20%">pseudoNode</td>
</tr><tr>
<td width="20%">roadEnd</td>
<td width="20%">roadEnd</td>
</tr><tr>
<td width="20%">roadServiceArea</td>
<td width="20%">roadServiceArea</td>
</tr><tr>
<td width="20%">roundabout</td>
<td width="20%">roundabout</td>
</tr><tr>
<td width="20%">trafficSquare</td>
<td width="20%">trafficSquare</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainTransportTypeValue"/>
<p><strong>TransportTypeValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">TransportTypeValue</td>
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
<td width="20%">http://inspire.ec.europa.eu/codelist/TransportTypeValue/road</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/TransportTypeValue/road</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/TransportTypeValue/air</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/TransportTypeValue/air</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/TransportTypeValue/rail</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/TransportTypeValue/rail</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/TransportTypeValue/water</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/TransportTypeValue/water</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/TransportTypeValue/cable</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/TransportTypeValue/cable</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainTransportTypeValue_value"/>
<p><strong>TransportTypeValue_value - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">TransportTypeValue_value</td>
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
<td width="20%">road</td>
<td width="20%">road</td>
</tr><tr>
<td width="20%">air</td>
<td width="20%">air</td>
</tr><tr>
<td width="20%">rail</td>
<td width="20%">rail</td>
</tr><tr>
<td width="20%">water</td>
<td width="20%">water</td>
</tr><tr>
<td width="20%">cable</td>
<td width="20%">cable</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p>
