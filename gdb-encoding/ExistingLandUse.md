# Geodatabase Encoding Rule for INSPIRE ExistingLandUse

`Version: 0.0`
`Date: 2021-02-22`

The Simple ExistingLandUse encoding can be used as an *alternative encoding* for ExistingLandUse data that fulfills the following requirements:

Any Dataset can be used. ( Possible limitations could be on the multiplicity of hilucLandUse and specificLanUSe to be a static number.)

## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](/gdb-encoding/geodatabse encoding.md)
* [Data Specification - INSPIRE Land Use version 3.1](https://inspire.ec.europa.eu/Themes/129/2892)

## Conformance Class Existing Land Use

The Land Use theme has five application schema. This application schema-specific encoding rule defines a single conformance class for the application schema Existing Land Use.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the ExistingLandUse conceptual model before applying the general rules of this encoding rule:
 

1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. (works in GDB)
2. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` (works in GDB as ong as not to long)

ToDO: 
Rule for ExistingLandUseObject_hilucsPresence/ specificPresence is either orderedList or percentageList



#### ExistingLandUseDataSet

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|extent|GM_MultiSurface|extent|Polygon|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|name|CharacterString|name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|

#### ExistingLandUseDataSet_member

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|||member|Long|

#### ExistingLandUseObject

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Text|
|inspireId|Identifier|inspireId.localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|geometry|GM_MultiSurface|geometry|Polygon|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|observationDate|Date|observationDate|Date|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|dataset|ExistingLandUseDataSet|dataset|Long|

#### ExistingLandUseObject_hilucsLandUse

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|hilucsLandUse|HILUCSValue|RID|Long|
|||hilucsLandUse|Text|
|||hilucsLandUse_href|Text|

#### ExistingLandUseObject_hilucsPresence

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|hilucsPresence| HILUCSPresence|RID|Long|
|||orderedList|Text|
|||orderedList_href|Text|
|||percentage_hilucsValue_href|Text|
|||percentage_hilucsValue|Text|
|||percentage_percentage|Text|

#### ExistingLandUseObject_specificLandUse

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|specificLandUse|LandUseClassificationValue|RID|Long|
|||specificLandUse|Text|
|||specificLandUse_href|Text|

#### ExistingLandUseObject_specificPresence

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|specificPresence|SpecificPresence|RID|Long|
|||orderedList|Text|
|||orderedList_href|Text|
|||percentage_specificValue|Text|
|||percentage_specificValue_href|Text|
|||percentage_specificPercentage|Text|
