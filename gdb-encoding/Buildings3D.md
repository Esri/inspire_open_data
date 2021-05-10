# Geodatabase Encoding Rule for INSPIRE Buildings3D

`Version: 0.0`
`Date: 2021-02-22`

The Simple Buildings3D encoding can be used as an *alternative encoding* for Buildings3D data that fulfills the following requirements:

* It is sufficient to provide the `activity` for the `Function` in function. 
* It is sufficient to provide the `activity` for the `Capacity` in physicalCapacity.  
* There is no information on permittedCapacity for Permissions.

## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](/gdb-encoding/geodatabse encoding.md)
* [Data Specification - INSPIRE Addresses version 3.1](https://inspire.ec.europa.eu/Themes/126/2892)

## Conformance Class Buildings3D

The Buildings theme has three application schema. This application schema-specific encoding rule defines a conformance class for the application schema Buildings3D.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Buildings3D conceptual model before applying the general rules of this encoding rule:
 

1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. (works in GDB)
2. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` (works in GDB as ong as not to long)
4. Create seperate Tables for each Geometry Type, add suffix for P for Points, L for Lines and S for Areas.
5. References to Objects by URL (String)


ToDO: 
Single 3D geometry per Object
externalInformation system Reference 
multiplicities




#### Building

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId||
|beginLifespanVersion|DateTime|beginLifespanVersion|Text|
|||conditionOfConstruction_href|Text|
|dateOfConstruction|DateOfEvent|dateOfConstruction_beginning|Text|
|||dateOfConstruction_end|Text|
|dateOfDemolition|DateOfEvent|dateOfDemolition_beginning|Text|
|||dateOfDemolition_end|Text|
|dateOfRenovation|DateOfEvent|dateOfRenovation_beginning|Text|
|||dateOfRenovation_end|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Text|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|||numberOfDwellings|Text|
|numberOfDwellings|Integer|numberOfBuildingUnits|Text|
|numberOfBuildingUnits|Integer|numberOfFloorsAboveGround|Text|
|||geometry3DLoD1_geometrySolid||
|verticalGeometryReference3DBottom|ElevationReferenceValue|verticalReference3DBottom||
|||verticalReference3DBottom_href||
|horizontalEstimatedAccuracy|Length|horizontalEstimatedAccuracy|Text|
|verticalEstimatedAccuracy|Length|verticalEstimatedAccuracy|Text|
|horizontalGeometryReference|HorizontalGeometryReferenceValue|horizontalReference||
|||horizontalReference_href||
|verticalGeometryReference3DTop|ElevationReferenceValue|verticalReference3DTop||
|||verticalReference3DTop_href||

#### BuildingPart

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId||
|||partOf||
|beginLifespanVersion|DateTime|beginLifespanVersion||
|conditionOfConstruction|ConditionOfConstructionValue|conditionOfConstruction|Text|
|||conditionOfConstruction_href|Text|
|dateOfConstruction|DateOfEvent|dateOfConstruction_beginning|Text|
|||dateOfConstruction_end|Text|
|dateOfDemolition|DateOfEvent|dateOfDemolition_beginning|Text|
|||dateOfDemolition_end|Text|
|dateOfRenovation|DateOfEvent|dateOfRenovation_beginning|Text|
|||dateOfRenovation_end|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Text|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|numberOfDwellings|Integer|numberOfDwellings|Text|
|numberOfBuildingUnits|Integer|numberOfBuildingUnits|Text|
|numberOfFloorsAboveGround|Integer|numberOfFloorsAboveGround|Text|
|geometrySolid|GM_Solid|geometrySolid||
|verticalGeometryReference3DBottom|ElevationReferenceValue|verticalReference3DBottom||
|||verticalReference3DBottom||
|horizontalEstimatedAccuracy|Length|horizontalEstimatedAccuracy|Text|
|verticalEstimatedAccuracy|Length|verticalEstimatedAccuracy|Text|
|horizontalGeometryReference|HorizontalGeometryReferenceValue|horizontalReference||
|||horizontalReference_href||
|verticalGeometryReference3DTop|ElevationReferenceValue|verticalReference3DTop||
|||verticalReference3DTop_href||

#### BuildingPart_buildingNature

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|buildingNature|BuildingNatureValue|RID|Text|
|||buildingNature|Text|
|||buildingNature_href|Text|

#### BuildingPart_currentUse

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|currentUse|CurrentUse|RID||
|||currentUse|Text|
|||currentUse_href|Text|
|||currentUse_percentage|Text|

#### BuildingPart_elevation

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|elevation|Elevation|RID||
|||elevationReference_href|Text|
|||elevationValue|Text|

#### BuildingPart_externalReference

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|externalReference|ExternalReference|RID||
|||informationSystem|Text|
|||informationSystemName|Text|
|||reference||

#### BuildingPart_heightAboveGround

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|heightAboveGround|HeightAboveGround|RID||
||ElevationReferenceValue|heightReference||
|||heightReference_href||
||ElevationReferenceValue|lowReference||
|||lowReference_href||
||HeightStatusValue|status||
|||status_href||
|||value||

#### BuildingPart_name

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|name|GeographicalName|RID||
|||name_language||
|||name||

#### BuildingPart_terrainIntersection

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|terrainIntersection|GM_MultiCurve|RID||
|||terrainIntersection||

#### Building_buildingNature

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|buildingNature|BuildingNatureValue|RID||
|||buildingNature|Text|
|||buildingNature_href|Text|

#### Building_currentUse

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Text|
|currentUse|CurrentUse|currentUse||
|||currentUse_href||
|||percentage|Text|

#### Building_elevation

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|elevation|Elevation|RID||
|||elevationReference_href|Text|
|||elevationValue|Text|

#### Building_externalReference

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|externalReference|ExternalReference|RID||
|||informationSystem|Text|
|||informationSystemName|Text|
|||reference||

#### Building_heightAboveGround

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|heightAboveGround|HeightAboveGround|RID||
|||heightReference|Text|
|||heightReference_href|Text|
|||lowReference|Text|
|||lowReference_href|Text|
|||status|Text|
|||status_href|Text|
|||heightAboveGround_value|Text|

#### Building_name

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|name|GeographicalName|RID||
|||name_language||
|||name||

#### Building_terrainIntersection

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|terrainIntersection|GM_MultiCurve|RID||
|||terrainIntersection||
