# Geodatabase Encoding Rule for INSPIRE Sampled Land Use

`Version: 0.0`
`Date: 2021-02-22`

The Simple SampledLandUse encoding can be used as an *alternative encoding* for Sampled Land Use data that fulfills the following requirements:

* It is sufficient to provide the `activity` for the `Function` in function. 
* It is sufficient to provide the `activity` for the `Capacity` in physicalCapacity.  
* There is no information on permittedCapacity for Permissions.


## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](/gdb-encoding/geodatabse encoding.md)
* [Data Specification - INSPIRE Land Use version 3.1](https://inspire.ec.europa.eu/Themes/129/2892)

## Conformance Class Sampled Land Use

The Land Use theme has five application schema. This application schema-specific encoding rule defines a single conformance class for the application schema Sampled Land Use.
### Model Transformation

This section describes which transformation rules with which parameters are applied to the Sampled Land Use conceptual model before applying the general rules of this encoding rule:
 

1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. (works in GDB)
2. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` (works in GDB as ong as not to long)
4. Create seperate Tables for each Geometry Type, add suffix for P for Points, L for Lines and S for Areas.
5. References to Objects by URL (String)


ToDO: 
SimpleRelatedParty beschreiben, Multiplizität bei RelatedParty erlauben
Contact in einzelne Attribute zerlegen.




#### ExistingLandUseSample

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId||
|inspireId|Identifier|inspireId_localId||
|||inspireId_namespace||
|||inspireId_versionId||
|location|GM_Point|location||
|beginLifespanVersion|DateTime|beginLifespanVersion||
|observationDate|Date|observationDate||
|endLifespanVersion|DateTime|endLifespanVersion||
|validFrom|DateTime|validFrom||
|validTo|DateTime|validTo||
|dataset||dataset||

#### ExistingLandUseSample_hilucsLandUse

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|hilucsLandUse|HILUCSValue|RID||
|||hilucsLandUse||
|||hilucsLandUse_href||

#### ExistingLandUseSample_hilucsPresence

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|hilucsPresence| HILUCSPresence|RID||
|||orderedList||
|||orderedList_href||
|||percentage_hilucsValue_href||
|||percentage_hilucsValue||
|||percentage_percentage||

#### ExistingLandUseSample_specificLandUse

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|specificLandUse|LandUseClassificationValue|RID||
|||specificLandUse||
|||specificLandUse_href||

#### ExistingLandUseSample_specificPresence

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|specificPresence|SpecificPresence|RID||
|||orderedList||
|||orderedList_href||
|||percentage_specificValue||
|||percentage_specificValue_href||
|||percentage_specificPercentage||

#### SampledExistingLandUseDataSet

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId||
|inspireId|Identifier|inspireId_localId||
|||inspireId_namespace||
|||inspireId_versionId||
|extent|GM_MultiSurface|extent||
|name|CharacterString|name||
|beginLifespanVersion|DateTime|beginLifespanVersion||
|endLifespanVersion|DateTime|endLifespanVersion||
|validFrom|DateTime|validFrom||
|validTo|DateTime|validTo||

#### SampledExistingLandUseDataSet_member

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|member|ExistingLandUseSample|RID||
|||member||
