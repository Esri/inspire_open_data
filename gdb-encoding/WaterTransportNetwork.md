# Geodatabase Encoding Rule for INSPIRE Water Transport Network

`Version: 1.0`
`Date: 2025-02-28`

The Simple Water Transport Network encoding can be used as an *alternative encoding* for WaterTransportNetwork data that fulfills the following requirements:

* There is no NetworkProperty for any Object in the data. 
* There is no `inNetwork` relation for any Object in the data. 
* There is no `WaterwayLinkSequence` or `WaterwayLinkSet` in the data. 



## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Transport Networks version 3.3.0](https://github.com/INSPIRE-MIF/technical-guidelines/tree/main/data/tn)

## Conformance Class Water Transport Network

The Transport Networks theme has five application schema. This application schema-specific encoding rule defines a conformance class for the application schema Water Transport Network.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Water Transport Network conceptual model before applying the general rules of this encoding rule:
 
1. Substitute all attributes that have a property type with a Codelist Sterotype through an inline codelist reference using `MT008()`. 
2. Substitute all occurrences of `GeographicName` with the Simple Geographic Name through Rule `MT005(separator: '_')`.
3. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` .
4. `spokeStart` and `spokeEnd` on `WaterwayNode` can be derived as the inverse property of `startNode` and `endNode` from `WaterwayLink`. 
5. Apply the High Cardinality Properties to Extra Tables rule to `TransportNetwork`, `MarineWaterway` and `Inlandwaterway`: `MT011()`. 




#### Beacon

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
|inNetwork|TransportNetwork|inNetwork|Long|

#### Buoy

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

#### FairwayArea

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

#### FerryCrossing

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

#### FerryCrossing_link

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|link|WaterwayLink|RID|Long|
|||link|Long|

#### InlandWaterway

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

#### InlandWaterway_link

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|link|WaterwayLink|RID|Long|
|||link|Long|

#### MarineWaterway

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
||Boolean|deepWaterRoute|Long|

#### MarineWaterway_link

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|link|WaterwayLink|RID|Long|
|||link|Long|

#### PortArea

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|geographicalName|GeographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|

#### PortNode

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
|||elements|Long|

#### WaterwayLink

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inNetwork|TransportNetwork|inNetwork|Text|
|fictitious|Boolean|fictitious|Long|
|endNode|WaterwayNode|endNode|Long|
|startNode|WaterwayNode|startNode|Long|
|geographicalName|GeographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|

#### WaterwayNode

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
||FormOfWaterwayNodeValue|formOfWaterwayNode_href|Text|
|||formOfWaterwayNode|Text|
