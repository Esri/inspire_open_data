# Geodatabase Encoding Rule for INSPIRE Road Transport Network

`Version: 1.0`
`Date: 2025-02-28`

The Simple Road Transport Network encoding can be used as an *alternative encoding* for Road Transport Network data that fulfills the following requirements:

* There is no NetworkProperty for any Object in the data. 
* There is no `inNetwork` relation for any Object in the data. 
* There is no `RoadwayLinkSequence` or `RoadwayLinkSet` in the data. 



## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Transport Networks version 3.3.0](https://github.com/INSPIRE-MIF/technical-guidelines/tree/main/data/tn)

## Conformance Class Road Transport Network

The Transport Networks theme has five application schema. This application schema-specific encoding rule defines a conformance class for the application schema Road Transport Network.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Road Transport Network conceptual model before applying the general rules of this encoding rule:
 
1. Substitute all attributes that have a property type with a Codelist Sterotype through an inline codelist reference using `MT008()`. 
2. Substitute all occurrences of `GeographicName` with the Simple Geographic Name through Rule `MT005(separator: '_')`.
3. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` .
4. `spokeStart` and `spokeEnd` on `RoadNode` can be derived as the inverse property of `startNode` and `endNode` from `RoadLink`.
5. Apply the High Cardinality Properties to Extra Tables rule to `TransportNetwork`, `Road` and `ERoad`: `MT011()`.



#### ERoad

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inNetwork|TransportNetwork|inNetwork|Long|
|geographicalName|GeographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|europeanRouteNumber|CharacterString|europeanRouteNumber|Text|

#### Eroad_link

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|link|RoadLink|RID|Long|
|||link|Long|

#### GradeSeparatedCrossing

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inNetwork|TransportNetwork|inNetwork|Long|

#### GradeSeparatedCrossing_element

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|element|RoadLink|RID|Long|
|||element|Long|

#### Road

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inNetwork|TransportNetwork|inNetwork|Long|
|geographicalName|GeographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|localRoadCode|CharacterString|localRoadCode|Text|
|nationalRoadCode|CharacterString|nationalRoadCode|Text|

#### RoadArea

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inNetwork|TransportNetwork|inNetwork|Long|
|geographicalName|GeographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|

#### RoadLink

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inNetwork|TransportNetwork|inNetwork|Long|
|fictitious|Boolean|fictitious|Long|
|endNode|RoadNode|endNode|Long|
|startNode|RoadNode|startNode|Long|
|geographicalName|GeographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|

#### RoadNode

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inNetwork|TransportNetwork|inNetwork|Long|
|geographicalName|GeographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|formOfRoadNode|FormOfRoadNodeValue|formOfRoadNode_href|Text|
||FormOfRoadNodeValue|formOfRoadNode|Text|

#### RoadServiceArea

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inNetwork|TransportNetwork|inNetwork|Long|
|geographicalName|GeographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|

#### Road_link

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|link|RoadLink|RID|Long|
|||link|Long|

#### TransportNetwork

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|geographicalName|GeographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|typeOfTransport|TransportTypeValue|typeOfTransport_href|Text|
|||typeOfTransport|Text|

#### TransportNetwork_elements

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|||element|Long|

#### VehicleTrafficArea

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inNetwork|TransportNetwork|inNetwork|Long|
|geographicalName|GeographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
