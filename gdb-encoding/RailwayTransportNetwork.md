# Geodatabase Encoding Rule for INSPIRE Railway Transport Network

`Version: 1.0`
`Date: 2025-02-28`

The Simple Rail Transport Network encoding can be used as an *alternative encoding* for Railway Transport Network data that fulfills the following requirements:

* There is no NetworkProperty for any Object in the data. 
* There is no `inNetwork` relation for any Object in the data. 
* There is no `RailwayLinkSequence` or `RailwayLinkSet` in the data. 



## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Transport Networks version 3.3.0](https://github.com/INSPIRE-MIF/technical-guidelines/tree/main/data/tn)

## Conformance Class Rail Transport Network

The Transport Networks theme has five application schemas. This application schema-specific encoding rule defines a conformance class for the application schema Railway Transport Network.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Rail Transport Network conceptual model before applying the general rules of this encoding rule:
 
1. Substitute all attributes that have a property type with a Codelist Stereotype through an inline codelist reference using `MT008()`. 
2. Substitute all occurrences of `GeographicName` with the Simple Geographic Name through Rule `MT005(separator: '_')`.
3. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` .
4. `spokeStart` and `spokeEnd` on `RailwayNode` can be derived as the inverse property of `startNode` and `endNode` from `RailwayLink`.
5. Apply the High Cardinality Properties to Extra Tables rule to `TransportNetwork` and `RailwayLine`: `MT011()`. 




#### RailwayArea

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

#### RailwayLine

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
|railwayLineCode|CharacterString|railwayLineCode|Text|

#### RailwayLine_link

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|link|RailwayLink|RID|Long|
|||link|Long|

#### RailwayLink

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
|endNode|RailwayNode|endNode|Long|
|startNode|RailwayNode|startNode|Long|
|geographicalName|GeographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|

#### RailwayNode

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
|formOfNode|FormOfRailwayNodeValue|formOfNode_href|Text|
|||formOfNode|Text|

#### RailwayStationArea

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

#### RailwayStationNode

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
|formOfNode|FormOfRailwayNodeValue|formOfNode_href|Text|
|||formOfNode|Text|
|numberOfPlatforms|Integer|numberOfPlatforms|Long|

#### RailwayYardArea

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

#### RailwayYardNode

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
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
|formOfNode|FormOfNodeValue|formOfNode_href|Text|
|||formOfNode|Text|

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
|elements|NetworkElement|RID|Long|
|||element|Long|
