# Geodatabase Encoding Rule for INSPIRE Buildings2D

`Version: 0.0`
`Date: 2021-02-22`

The Simple Buildings2D encoding can be used as an *alternative encoding* for Buildings2D data that fulfills the following requirements:

* It is sufficient to provide the `activity` for the `Function` in function. 
* It is sufficient to provide the `activity` for the `Capacity` in physicalCapacity.  
* There is no information on permittedCapacity for Permissions.


## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](/gdb-encoding/geodatabse encoding.md)
* [Data Specification - INSPIRE Buildings version 3.1](https://inspire.ec.europa.eu/Themes/126/2892)

## Conformance Class Buildings2D

The Buildings theme has three application schema. This application schema-specific encoding rule defines a conformance class for the application schema Buildings2D.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Buildings2D conceptual model before applying the general rules of this encoding rule:
 

1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. (works in GDB)
2. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` (works in GDB as ong as not to long)
4. Create seperate Tables for each Geometry Type, add suffix for P for Points, L for Lines and S for Areas.
5. References to Objects by URL (String)


ToDO: 
SimpleRelatedParty beschreiben, Multiplizität bei RelatedParty erlauben
Contact in einzelne Attribute zerlegen.




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
|numberOfDwellings|Integer|numberOfDwellings|Text|
|numberOfBuildingUnits|Integer|numberOfBuildingUnits|Text|
|numberOfFloorsAboveGround|Integer|numberOfFloorsAboveGround|Text|
|geometry|GM_Object|geometry||
|referenceGeometry|Boolean|referenceGeometry|Text|
|horizontalGeometryReference|HorizontalGeometryReferenceValue|horizontalReference|Text|
|||horizontalReference_href|Text|
|verticalGeometryReference|ElevationReferenceValue|verticalReference|Text|
|||verticalReference_href|Text|
|horizontalEstimatedAccuracy|Length|horizontalEstimatedAccuracy|Text|
|verticalEstimatedAccuracy|Length|verticalEstimatedAccuracy|Text|

#### BuildingPart

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId||
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
|||geometry|Text|
|referenceGeometry|Boolean|referenceGeometry||
|horizontalReference|HorizontalGeometryReferenceValue|horizontalReference|Text|
|||horizontalReference_href|Text|
|verticalReference|ElevationReferenceValue|verticalReference|Text|
|||verticalReference_href|Text|
|horizontalEstimatedAccuracy|Length|horizontalEstimatedAccuracy|Text|
|verticalEstimatedAccuracy|Length|verticalEstimatedAccuracy|Text|

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
|||reference|Text|

#### BuildingPart_heightAboveGround

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|heightAboveGround|HeightAboveGround|RID||
|||heightReference|Text|
|||heightReference_href|Text|
|||lowReference|Text|
|||lowReference_href|Text|
|||status|Text|
|||status_href|Text|
|||value|Text|

#### BuildingPart_name

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|name|GeographicalName|RID||
|||name_language|Text|
|||name|Text|

#### Building_buildingNature

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|buildingNature|BuildingNatureValue|RID||
|||buildingNature|Text|
|||buildingNature_href|Text|

#### Building_currentUse

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|currentUse|CurrentUse|RID||
|||currentUse_href|Text|
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
|||reference|Text|

#### Building_heightAboveGround

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|heightAboveGround|HeightAboveGround|RID||
|||heightReference_href|Text|
|||lowReference_href|Text|
|||status_href|Text|
|||heightAboveGround_value|Text|

#### Building_name

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|name|GeographicalName|RID||
|||name_language|Text|
|||name|Text|

#### Building_part

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|part|BuildingPart|RID||
|||part|Text|
