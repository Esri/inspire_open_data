# Geodatabase Encoding Rule for INSPIRE Buildings3D

`Version: 0.0`
`Date: 2021-02-22`

The Simple Buildings3D encoding can be used as an *alternative encoding* for Buildings3D data that fulfills the following requirements:

* There is not more than one value for the attribute `elevation` for `Building` or `BuildingPart`. 
* There is not more than one value for the attribute `externalReference` for `Building` or `BuildingPart`. 
* There is not more than one value for the attribute `heightAboveGround` for `Building` or `BuildingPart`. 
* There are not more than three values for the attribute `name` for `Building` or `BuildingPart`. 
* There are not more than three values for the attribute `buildingNature` for `Building` or `BuildingPart`. 
* There are not more than three values for the attribute `currentUse` for `Building` or `BuildingPart`. 
* There is only one LoD Geometry for each `Building` or `BuildingPart`.

## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](/gdb-encoding/geodatabse encoding.md)
* [Data Specification - INSPIRE Addresses version 3.1](https://inspire.ec.europa.eu/Themes/126/2892)

## Conformance Class Buildings3D

The Buildings theme has three application schema. This application schema-specific encoding rule defines a conformance class for the application schema Buildings3D.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Buildings3D conceptual model before applying the general rules of this encoding rule:
 
1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. (works in GDB)
2. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` (works in GDB as ong as not to long)
3. Substitute all occurences of `GeographicName` with the Simple Geographic Name through Rule `MT005(separator: '_')`.





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
|endLifespanVersion|DateTime|endLifespanVersion|Text|
|externalReference|ExternalReference|externalReference_informationSystem|Text|
|||externalReference_informationSystemName|Text|
|||externalReference_reference|Text|
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
|name|GeographicalName|name_1_language|Text|
|||name_2_language|Text|
|||name_3_language|Text|
|||name_1|Text|
|||name_2|Text|
|||name_3|Text|
|buildingNature|BuildingNatureValue|buildingNature_1|Text|
|||buildingNature_2|Text|
|||buildingNature_3|Text|
|||buildingNature_1_href|Text|
|||buildingNature_2_href|Text|
|||buildingNature_3_href|Text|
|||numberOfDwellings|Text|
|numberOfDwellings|Integer|numberOfBuildingUnits|Text|
|numberOfBuildingUnits|Integer|numberOfFloorsAboveGround|Text|
|||geometry3DLoD1_geometrySolid|Multipatch|
|verticalGeometryReference3DBottom|ElevationReferenceValue|verticalReference3DBottom|Text|
|||verticalReference3DBottom_href|Text|
|horizontalEstimatedAccuracy|Length|horizontalEstimatedAccuracy|Text|
|verticalEstimatedAccuracy|Length|verticalEstimatedAccuracy|Text|
|horizontalGeometryReference|HorizontalGeometryReferenceValue|horizontalReference|Text|
|||horizontalReference_href|Text|
|verticalGeometryReference3DTop|ElevationReferenceValue|verticalReference3DTop|Text|
|||verticalReference3DTop_href|Text|

#### BuildingPart

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||partOf|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|conditionOfConstruction|ConditionOfConstructionValue|conditionOfConstruction|Text|
|||conditionOfConstruction_href|Text|
|dateOfConstruction|DateOfEvent|dateOfConstruction_beginning|Text|
|||dateOfConstruction_end|Text|
|dateOfDemolition|DateOfEvent|dateOfDemolition_beginning|Text|
|||dateOfDemolition_end|Text|
|dateOfRenovation|DateOfEvent|dateOfRenovation_beginning|Text|
|||dateOfRenovation_end|Text|
|elevation|Elevation|elevationReference_href|Text|
|||elevationValue|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Text|
|externalReference|ExternalReference|externalReference_informationSystem|Text|
|||externalReference_informationSystemName|Text|
|||externalReference_reference|Text|
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
|name|GeographicalName|name_1_language|Text|
|||name_2_language|Text|
|||name_3_language|Text|
|||name_1|Text|
|||name_2|Text|
|||name_3|Text|
|buildingNature|BuildingNatureValue|buildingNature_1|Text|
|||buildingNature_2|Text|
|||buildingNature_3|Text|
|||buildingNature_1_href|Text|
|||buildingNature_2_href|Text|
|||buildingNature_3_href|Text|
|numberOfDwellings|Integer|numberOfDwellings|Text|
|numberOfBuildingUnits|Integer|numberOfBuildingUnits|Text|
|numberOfFloorsAboveGround|Integer|numberOfFloorsAboveGround|Text|
|geometrySolid|GM_Solid|geometrySolid|Multipatch|
|verticalGeometryReference3DBottom|ElevationReferenceValue|verticalReference3DBottom|Text|
|||verticalReference3DBottom|Text|
|horizontalEstimatedAccuracy|Length|horizontalEstimatedAccuracy|Text|
|verticalEstimatedAccuracy|Length|verticalEstimatedAccuracy|Text|
|horizontalGeometryReference|HorizontalGeometryReferenceValue|horizontalReference|Text|
|||horizontalReference_href|Text|
|verticalGeometryReference3DTop|ElevationReferenceValue|verticalReference3DTop|Text|
|||verticalReference3DTop_href|Text|

#### BuildingPart_currentUse

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|currentUse|CurrentUse|RID|Long|
|||currentUse|Text|
|||currentUse_href|Text|
|||currentUse_percentage|Text|

#### BuildingPart_terrainIntersection

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|terrainIntersection|GM_MultiCurve|RID|Long|
|||terrainIntersection|Line|

#### Building_currentUse

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|currentUse|CurrentUse|currentUse|Text|
|||currentUse_href|Text|
|||percentage|Text|

#### Building_elevation

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|elevation|Elevation|RID|Long|
|||elevationReference_href|Text|
|||elevationValue|Text|

#### Building_terrainIntersection

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|terrainIntersection|GM_MultiCurve|RID|Long|
|||terrainIntersection|Line|
