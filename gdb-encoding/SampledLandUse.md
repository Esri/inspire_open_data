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
 

1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. 
2. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')`







#### ExistingLandUseSample

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|observationDate|Date|observationDate|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|dataset||dataset|Long|

#### ExistingLandUseSample_hilucsLandUse

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|hilucsLandUse|HILUCSValue|RID|Long|
|||hilucsLandUse|Text|
|||hilucsLandUse_href|Text|

#### ExistingLandUseSample_hilucsPresence

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|hilucsPresence| HILUCSPresence|RID|Long|
|||orderedList|Text|
|||orderedList_href|Text|
|||percentage_hilucsValue_href|Text|
|||percentage_hilucsValue|Text|
|||percentage_percentage|Text|

#### ExistingLandUseSample_specificLandUse

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|specificLandUse|LandUseClassificationValue|RID|Long|
|||specificLandUse|Text|
|||specificLandUse_href|Text|

#### ExistingLandUseSample_specificPresence

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|specificPresence|SpecificPresence|RID|Long|
|||orderedList|Text|
|||orderedList_href|Text|
|||percentage_specificValue|Text|
|||percentage_specificValue_href|Text|
|||percentage_specificPercentage|Text|

#### SampledExistingLandUseDataSet

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|name|CharacterString|name|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|

#### SampledExistingLandUseDataSet_member

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|member|ExistingLandUseSample|RID|Long|
|||member|Long|
