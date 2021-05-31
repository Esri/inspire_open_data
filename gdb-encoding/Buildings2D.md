# Geodatabase Encoding Rule for INSPIRE Buildings2D

`Version: 0.5`
`Date: 2021-05-31`

The Simple Buildings2D encoding can be used as an *alternative encoding* for Buildings2D data that fulfills the following requirements:

* There is not more than one value for the attribute `elevation` for `Building` or `BuildingPart`. 
* There is not more than one value for the attribute `externalReference` for `Building` or `BuildingPart`. 
* There is not more than one value for the attribute `heightAboveGround` for `Building` or `BuildingPart`. 
* There are not more than three values for the attribute `name` for `Building` or `BuildingPart`. 
* There are not more than three values for the attribute `buildingNature` for `Building` or `BuildingPart`. 
* There are not more than three values for the attribute `currentUse` for `Building` or `BuildingPart`. 


## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Buildings version 3.1](https://inspire.ec.europa.eu/Themes/126/2892)

## Conformance Class Buildings2D

The Buildings theme has three application schema. This application schema-specific encoding rule defines a conformance class for the application schema Buildings2D.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Buildings2D conceptual model before applying the general rules of this encoding rule:
 
1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. (works in GDB)
2. Limit the Multiplicity for `elevation` for `Building` or `BuildingPart` to 1 through Rule `MT012(3)`
3. Limit the Multiplicity for `externalReference` for `Building` or `BuildingPart` to 1 through Rule `MT012(3)`
4. Limit the Multiplicity for `heightAboveGround` for `Building` or `BuildingPart` to 1 through Rule `MT012(3)`
5. Limit the Multiplicity for `buildingNature` for `Building` or `BuildingPart` to 3 through Rule `MT012(1)`
6. Limit the Multiplicity for `currentUse` for `Building` or `BuildingPart` to 3 through Rule `MT012(1)`
7. Substitute all occurences of `GeographicName` with the Simple Geographic Name through Rule `MT005(separator: '_')`.
8. Apply MT011 on `part` for `Building`.
8. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 




#### Building

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Text|
|||conditionOfConstruction_href|Text|
|dateOfConstruction|DateOfEvent|dateOfConstruction_beginning|Date|
|||dateOfConstruction_end|Date|
|dateOfDemolition|DateOfEvent|dateOfDemolition_beginning|Date|
|||dateOfDemolition_end|Date|
|dateOfRenovation|DateOfEvent|dateOfRenovation_beginning|Date|
|||dateOfRenovation_end|Date|
|elevation|Elevation|elevationReference|Text|
|||elevationReference_href|Text|
|||elevationValue|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Text|
|externalReference|ExternalReference|extRef_informationSystem|Text|
|||extRef_informationSystemName|Text|
|||extRef_reference|Text|
|heightAboveGround|HeightAboveGround|heightReference|Text|
|||heightReference_href|Text|
|||lowReference|Text|
|||lowReference_href|Text|
|||status|Text|
|||status_href|Text|
|||heightAboveGround_value|Text|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|name|GeographicalName|name_1|Text|
|||name_1_language|Text|
|||name_2|Text|
|||name_2_language|Text|
|||name_3|Text|
|||name_3_language|Text|
|buildingNature|BuildingNatureValue|buildingNature_1|Text|
|||buildingNature_1_href|Text|
|||buildingNature_2|Text|
|||buildingNature_2_href|Text|
|||buildingNature_3|Text|
|||buildingNature_3_href|Text|
|currentUse|CurrentUse|currentUse_1_currentUse|Text|
|||currentUse_1_currentUse_href|Text|
|||currentUse_1_percentage|Float|
|||currentUse_2_currentUse|Text|
|||currentUse_2_currentUse_href|Text|
|||currentUse_2_percentage|Float|
|||currentUse_3_currentUse|Text|
|||currentUse_3_currentUse_href|Text|
|||currentUse_3_percentage|Float|
|numberOfDwellings|Integer|numberOfDwellings|Long|
|numberOfBuildingUnits|Integer|numberOfBuildingUnits|Long|
|numberOfFloorsAboveGround|Integer|numberOfFloorsAboveGround|Long|
|referenceGeometry|Boolean|referenceGeometry|Text|
|horizontalGeometryReference|HorizontalGeometryReferenceValue|horizontalReference|Text|
|||horizontalReference_href|Text|
|verticalGeometryReference|ElevationReferenceValue|verticalReference|Text|
|||verticalReference_href|Text|
|horizontalEstimatedAccuracy|Length|horizontalEstimatedAccuracy|Float|
|verticalEstimatedAccuracy|Length|verticalEstimatedAccuracy|Float|

#### BuildingPart

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|conditionOfConstruction|ConditionOfConstructionValue|conditionOfConstruction|Text|
|||conditionOfConstruction_href|Text|
|dateOfConstruction|DateOfEvent|dateOfConstruction_beginning|Text|
|||dateOfConstruction_end|Text|
|dateOfDemolition|DateOfEvent|dateOfDemolition_beginning|Text|
|||dateOfDemolition_end|Text|
|dateOfRenovation|DateOfEvent|dateOfRenovation_beginning|Text|
|||dateOfRenovation_end|Text|
|elevation|Elevation|elevationReference|Text|
||ElevationReferenceValue|elevationReference_href|Text|
|||elevationValue|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Text|
|externalReference|ExternalReference|extRef_informationSystem|Text|
|||extRef_informationSystemName|Text|
|||extRef_reference|Text|
|heightAboveGround|HeightAboveGround|heightReference|Text|
|||heightReference_href|Text|
|||lowReference|Text|
|||lowReference_href|Text|
|||status|Text|
|||status_href|Text|
|||value|Text|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|name|GeographicalName|name_1|Text|
|||name_1_language|Text|
|||name_2|Text|
|||name_2_language|Text|
|||name_3|Text|
|||name_3_language|Text|
|buildingNature|BuildingNatureValue|buildingNature_1|Text|
|||buildingNature_1_href|Text|
|||buildingNature_2|Text|
|||buildingNature_2_href|Text|
|||buildingNature_3|Text|
|||buildingNature_3_href|Text|
|||currentUse_1_currentUse|Text|
|||currentUse_1_currentUse_href|Text|
|||currentUse_1_percentage|Float|
|||currentUse_2_currentUse|Text|
|||currentUse_2_currentUse_href|Text|
|||currentUse_2_percentage|Float|
|||currentUse_3_currentUse|Text|
|||currentUse_3_currentUse_href|Text|
|||currentUse_3_percentage|Float|
|numberOfDwellings|Integer|numberOfDwellings|Long|
|numberOfBuildingUnits|Integer|numberOfBuildingUnits|Long|
|numberOfFloorsAboveGround|Integer|numberOfFloorsAboveGround|Long|
|referenceGeometry|Boolean|referenceGeometry|Long|
|horizontalReference|HorizontalGeometryReferenceValue|horizontalReference|Text|
|||horizontalReference_href|Text|
|verticalReference|ElevationReferenceValue|verticalReference|Text|
|||verticalReference_href|Text|
|horizontalEstimatedAccuracy|Length|horizontalEstimatedAccuracy|Float|
|verticalEstimatedAccuracy|Length|verticalEstimatedAccuracy|Float|

#### Building_part

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|part|BuildingPart|RID|Long|
|||part|Long|
