# Geodatabase Encoding Rule for INSPIRE Hydrogeology

`Version: 1.0`
`Date: 2025-05-27`

The Simple Hydrogeology encoding can be used as an *alternative encoding* for Hydrogeology data that fulfills the following requirements:

* There is not more than 1 `purpose` per `Borehole`
* There is not more than 1 `activityType` per `ActiveWellP`
* There is no `downholeGeometry` relation for `Borehole`
* There is no `MappedInterval` relation for `Borehole`
* There is no `EnvironmentalMonitoringFacility` relation for `GroundWaterBodyS`
* There is no `EnvironmentalMonitoringFacility` relation for `ActiveWellP`
* There is no `GeStructure` relation for `HGUnit`

## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Geology version 3.0.0](https://github.com/INSPIRE-MIF/technical-guidelines/tree/main/data/ge)

## Conformance Class Core

The Geology theme has three application schema. This application schema-specific encoding rule defines a single conformance class for the application schema Hydrogeology.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Hydrogeology conceptual model before applying the general rules of this encoding rule:
 
1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. 
2. Apply the SimplePeriod rule `MT009()`.
3. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
4. Represent the Relationships Aquitard.featureId and Aquifer.featureId in a Relationship Table: `MT013()`
5. Represent the Relationships GroundwaterbodyS.featureId and ActiveWellP.featureId in a Relationship Table: `MT013()`
6. Limit the Multiplicity for activityType in hgActiveWellP to 1 through Rule: `MT012()`
7. Apply Attribute shortening rule for hgGroundwaterbodyS:

    |Replace|With|
    |----|----|
    |`'conOfGroundWaterBody'`|`'cOGWB' `|
    |`'conOfGroundWaterBody_href'`|`'cOGWB_href' `|
  
  

#### ActiveWellP 

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|||description|Text|
|||hgoName|Text|
|statusCode|StatusCodeTypeValue|statusCode|Text|
|validFrom||validFrom|Date|
|validTo||validTo|Date|
|activityType|ActiveWellTypeValue|activityType|Text|
|||activityType_href|Text|
|aquifer||rid1|Long|
|borehole||rid2|Long|

#### AquicludeS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
| mappingFrame|MappingFrameValue|mappingFrame|Text|
|||mappingFrame_href|Text|
|||rid|Text|


#### AquiferS 

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
| mappingFrame|MappingFrameValue|mappingFrame|Text|
|||mappingFrame_href|Text|
|||rid|Text|

#### AquitardS 

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
| mappingFrame|MappingFrameValue|mappingFrame|Text|
|||mappingFrame_href|Text|
|||rid|Text|

#### AquiferSystemS 

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
| mappingFrame|MappingFrameValue|mappingFrame|Text|
|||mappingFrame_href|Text|
|||rid|Text|

#### Borehole 

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|elevation|DirectPosition|elevation|Long|
|||elevation_dimension|Long|
|||elevationCRS|Text|
|boreholeLength|Quantity|length|Float|
|||length_uom|Text|
|purpose|BoreholePurposeValue|purpose|Text|
|||purpose_href|Text|

#### GroundwaterbodyS 

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|piezometricState|PiezometricState|piezState_obsTime|Date|
|||length_uom|Text|
|mineralization|WaterSalinityValue|mineralization|Text|
|||mineralization_href|Text|
|ConditionOfGroundwaterValue|ConditionOfGroundwaterValue|cOGWB|Text|
|||cOGWB_href|Text|

#### HyGeObjNaturalP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|description|PT_FreeText|description|Text|
|name|PT_FreeText|hgoName|Text|
|approximateQuantityOfFlow|QuantityValue|approxQuantityOfFlow|Float|
|||approxQuantityOfFlow_from|Float|
|||approxQuantityOfFlow_to|Float|
|||approxQuantityOfFlow_uom|Text|
|naturalObjectType|NaturalObjectTypeValue|naturalObjectType|Text|
|||naturalObjectType_href|Text|
|waterPersistence|WaterPersistenceValue|waterPersistence|Text|
|||waterPersistence_href|Text|
|||rid1|Long|
|||rid2|Long|


#### Aquiclude

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|description|PT_FreeText|description|Text|
|name|PT_FreeText|name|Text|
|approximateDepth|QuantityValue|approxiDepth|Float|
|||approxiDepth_from|Float|
|||approxiDepth_to|Float|
|||approxiDepth_uom|Text|
|approximateThickness|QuantityValue|approxiThickness|Float|
|||approxiThickness_from|Float|
|||approxiThickness_to|Float|
|||approxiThickness_uom|Text|
|geologicUnitType|GeologicUnitTypeValue|geologicUnitType|Text|
|||geologicUnitType_href|Text|
|||rid1|Long|

#### Aquifer

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|description|PT_FreeText|description|Text|
|name|PT_FreeText|name|Text|
|approximateDepth|QuantityValue|approxiDepth|Float|
|||approxiDepth_from|Float|
|||approxiDepth_to|Float|
|||approxiDepth_uom|Text|
|approximateThickness|QuantityValue|approxiThickness|Float|
|||approxiThickness_from|Float|
|||approxiThickness_to|Float|
|||approxiThickness_uom|Text|
|aquiferType|AquiferTypeValue|aquiferType|Text|
|||aquiferType_href|Text|
|hydroGeochemicalRockType|HydroGeochemicalRockTypeValue|hyGeochemRockType|Text|
|||hyGeochemRockType_href|Text|
|isExploited|Boolean|isExploited|Long|
|isMainInSystem|Boolean|isMainInSystem|Long|
|mediaType|AquiferMediaTypeValue|mediaType|Text|
|||mediaType_href|Text|
|permeabilityCoefficient|QuantityValue|permeaCoef_from|Float|
|||permeaCoef_to|Float|
|||permeaCoef_uom|Text|
|||permeaCoef_value|Float|
|storativityCoefficient|QuantityValue|storaCoef_from|Float|
|||storaCoef_to|Float|
|||storaCoef_uom|Text|
|||storaCoef_value|Float|
|vulnerabilityToPollution|QuantityValue|VulnToPollution_from|Float|
|||VulnToPollution_to|Float|
|||VulnToPollution_uom|Text|
|||VulnToPollution_value|Float|
|geologicUnitType|GeologicUnitTypeValue|geologicUnitType|Text|
|||geologicUnitType_href|Text|
|||rid1|Long|

#### AquiferSystem

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|description|PT_FreeText|description|Text|
|name|PT_FreeText|name|Text|
|approximateDepth|QuantityValue|approxiDepth|Float|
|||approxiDepth_from|Float|
|||approxiDepth_to|Float|
|||approxiDepth_uom|Text|
|approximateThickness|QuantityValue|approxiThickness|Float|
|||approxiThickness_from|Float|
|||approxiThickness_to|Float|
|||approxiThickness_uom|Text|
|isLayered|Boolean|isLayered|Long|
|geologicUnitType|GeologicUnitTypeValue|geologicUnitType|Text|
|||geologicUnitType_href|Text|
|||rid1|Long|

#### Aquitard

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|description|PT_FreeText|description|Text|
|name|PT_FreeText|name|Text|
|approximateDepth|QuantityValue|approxiDepth|Float|
|||approxiDepth_from|Float|
|||approxiDepth_to|Float|
|||approxiDepth_uom|Text|
|approximateThickness|QuantityValue|approxiThickness|Float|
|||approxiThickness_from|Float|
|||approxiThickness_to|Float|
|||approxiThickness_uom|Text|
|permeabilityCoefficient|QuantityValue|permeaCoef_from|Float|
|||permeaCoef_to|Float|
|||permeaCoef_uom|Text|
|||permeaCoef_value|Float|
|storativityCoefficient|QuantityValue|storaCoef_from|Float|
|||storaCoef_to|Float|
|||storaCoef_uom|Text|
|||storaCoef_value|Float|
|geologicUnitType|GeologicUnitTypeValue|geologicUnitType|Text|
|||geologicUnitType_href|Text|
|||rid1|Long|

#### AquitardAquifer 

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||rid1|Long|
|||rid2|Long|

#### GwbdsActiveWell

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||rid1|Long|
|||rid2|Long|

#### RelActiveWellP_Borehole

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|Borehole||featureId|Long|
|ActiveWellP||rid2|Long|

#### RelActiveWellP_GwbdsActiveWell

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|ActiveWellP||featureId|Long|
|GwbdsActiveWell||rid2|Long|

#### RelAqSystem_Aquifer

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|AquiferSystem||featureId|Long|
|Aquitard||rid2|Long|

#### RelAquiclude_AquicludeS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|Aquiclude||featureId|Long|
|AquicludeS||rid|Long|

#### RelAquifer_activeWellP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|Aquifer||featureId|Long|
|ActiveWellP||rid1|Long|

#### RelAquifer_AquitardAquifer

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|Aquifer||featureId|Long|
|AquitardAquifer||rid2|Long|

#### RelAquifer_HGObjNaturalP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|Aquifer||featureId|Long|
|HyGeObjNaturalP||rid2|Long|

#### RelAquiferSystem_aquiclude

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|AquiferSystem||featureId|Long|
|Aquiclude||rid1|Long|

#### RelAquiferSystem_aquifer

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|AquiferSystem||featureId|Long|
|Aquifer||rid1|Long|

#### RelAquiferSystem_AquiferSystemS 

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|AquiferSystem||featureId|Long|
|AquiferSystemS||rid|Long|

#### RelAquitard_AquitardAquifer

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|Aquitard||featureId|Long|
|AquitardAquifer||rid1|Long|

#### RelAquitard_AquitardS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|Aquitard||featureId|Long|
|AquitardS||rid|Long|

#### RelGwbdS_AquiferSystem

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|GroundwaterbodyS||featureId|Long|
|AquiferSystem||rid1|Long|

#### RelGwbdS_GwbdsActiveWell 

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|GroundwaterbodyS||featureId|Long|
|GwbdsActiveWell||rid1|Long|

#### RelGwbdS_HGObjNaturalP 

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|GroundwaterbodyS||featureId|Long|
|HyGeObjNaturalP||rid1|Long|
