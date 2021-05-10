# Geodatabase Encoding Rule for INSPIRE ExistingLandUse

`Version: 0.0`
`Date: 2021-02-22`

The Simple ExistingLandUse encoding can be used as an *alternative encoding* for ExistingLandUse data that fulfills the following requirements:

* It is sufficient to provide the `activity` for the `Function` in function. 
* It is sufficient to provide the `activity` for the `Capacity` in physicalCapacity.  
* There is no information on permittedCapacity for Permissions.


## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](/gdb-encoding/geodatabse encoding.md)
* [Data Specification - INSPIRE Land Use version 3.1](https://inspire.ec.europa.eu/Themes/129/2892)

## Conformance Class Existing Land Use

The Land Use theme has five application schema. This application schema-specific encoding rule defines a single conformance class for the application schema Existing Land Use.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the ExistingLandUse conceptual model before applying the general rules of this encoding rule:
 

1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. (works in GDB)
2. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` (works in GDB as ong as not to long)
4. Create seperate Tables for each Geometry Type, add suffix for P for Points, L for Lines and S for Areas.
5. References to Objects by URL (String)


ToDO: 
SimpleRelatedParty beschreiben, Multiplizität bei RelatedParty erlauben
Contact in einzelne Attribute zerlegen.




#### ExistingLandUseDataSet

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId||
|inspireId|Identifier|inspireId_localId||
|||inspireId_namespace||
|||inspireId_versionId||
|extent|GM_MultiSurface|extent||
|beginLifespanVersion|DateTime|beginLifespanVersion||
|endLifespanVersion|DateTime|endLifespanVersion||
|name|CharacterString|name||
|validFrom|DateTime|validFrom||
|validTo|DateTime|validTo||

#### ExistingLandUseDataSet_member

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID||
|||member||

#### ExistingLandUseObject

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId||
|inspireId|Identifier|inspireId.localId||
|||inspireId_namespace||
|||inspireId_versionId||
|geometry|GM_MultiSurface|geometry||
|beginLifespanVersion|DateTime|beginLifespanVersion||
|endLifespanVersion|DateTime|endLifespanVersion||
|observationDate|Date|observationDate||
|validFrom|DateTime|validFrom||
|validTo|DateTime|validTo||
|dataset|ExistingLandUseDataSet|dataset||

#### ExistingLandUseObject_hilucsLandUse

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|hilucsLandUse|HILUCSValue|RID||
|||hilucsLandUse||
|||hilucsLandUse_href||

#### ExistingLandUseObject_hilucsPresence

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|hilucsPresence| HILUCSPresence|RID||
|||orderedList||
|||orderedList_href||
|||percentage_hilucsValue_href||
|||percentage_hilucsValue||
|||percentage_percentage||

#### ExistingLandUseObject_specificLandUse

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|specificLandUse|LandUseClassificationValue|RID||
|||specificLandUse||
|||specificLandUse_href||

#### ExistingLandUseObject_specificPresence

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|specificPresence|SpecificPresence|RID||
|||orderedList||
|||orderedList_href||
|||percentage_specificValue||
|||percentage_specificValue_href||
|||percentage_specificPercentage||
