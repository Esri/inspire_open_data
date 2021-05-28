# Geodatabase Encoding Rule for INSPIRE PlannedLandUse

`Version: 0.0`
`Date: 2021-02-22`

The Simple PlannedLandUse encoding can be used as an *alternative encoding* for PlannedLandUse data that fulfills the following requirements:

* There are not more than three values for the attribute `name` for `SupplementaryRegulation`. 
( Possible limitations could be on the multiplicity of hilucLandUse and specificLanUSe to be a static number.)


## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](/gdb-encoding/geodatabse encoding.md)
* [Data Specification - INSPIRE Land Use version 3.1](https://inspire.ec.europa.eu/Themes/129/2892)

## Conformance Class Planned Land Use

The Land Use theme has five application schema. This application schema-specific encoding rule defines a single conformance class for the application schema Planned Land Use.
### Model Transformation

This section describes which transformation rules with which parameters are applied to the PlannedLandUse conceptual model before applying the general rules of this encoding rule:
 

1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. 
2. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
3. Substitute all occurences of LegislationCitation and DocumentCitation with the Simple Citation through Rule `MT007()`






#### OfficialDocumentation

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|legislationCitation|LegislationCitation|legislationCitation_name|Text|
|||legislationCitation_type|Text|
|||legislationCitation_date|Date|
|||legislationCitation_link|Text|
|||legislationCitation_level|Text|
|||legislationCitation_level_href|Text|
|||regulationText|Text|
|||planDocument_name|Text|
|||planDocument_type|Text|
|||planDocument_date|Date|
|||planDocument_link|Text|
|||planDocument_level|Text|
|||planDocument_level_href|Text|

#### SpatialPlan

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|officialTitle|CharacterString|officialTitle|Text|
|levelOfSpatialPlan|LevelOfSpatialPlanValue|levelOfSpatialPlan|Text|
|||levelOfSpatialPlan_href|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|alternativeTitle|CharacterString|alternativeTitle|Text|
|planTypeName|PlanTypeNameValue|planTypeName|Text|
|||planTypeName_href|Text|
|processStepGeneral|ProcessStepGeneralValue|processStepGeneral|Text|
|||processStepGeneral_href|Text|
|backgroundMap|BackgroundMapValue|backgroundMap_Date|Text|
|||backgroundMap_Reference|Text|
|||backgroundMap_URI|Text|

#### SpatialPlan_member

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|member|ZoningElement|member|Long|

#### SpatialPlan_officialDocument

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|officialDocument|OfficialDocumentation|officialDocument|Long|

#### SpatialPlan_ordinance

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|ordinance|OrdinanceValue |RID|Long|
|||ordinanceDate|Date|
|||ordinanceReference|Text|

#### SpatialPlan_restriction

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|restriction|SupplementaryRegulation|restriction|Long|

#### SupplementaryRegulation

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|processStepGeneral|ProcessStepGeneralValue|processStepGeneral|Text|
|||processStepGeneral_href|Text|
|backgroundMap|BackgroundMapValue|backgroundMap_Date|Text|
|||backgroundMap_Reference|Text|
|||backgroundMap_URI|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inheritedFromOtherPlans|Boolean|inheritedFromOtherPlans|Short|
|specificRegulationNature|CharacterString|specificRegulationNature|Text|
|name|CharacterString|name_1|Text|
|name|CharacterString|name_2|Text|
|name|CharacterString|name_3|Text|
|regulationNature|RegulationNatureValue|regulationNature|Text|
|||regulationNature_href|Text|
|||plan|Long|

#### SupplementaryRegulation_dimensioningIndication

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|dimensioningIndication|DimensioningIndicationValue|RID|Long|
|||indicationReference|Text|
|||CharacterValue_value|Text|
|||IntegerValue_value|Long|
|||MeasureValue_value|Float|
|||MeasureValue_value_uom|Text|
|||RealValue_value|Float|

#### SupplementaryRegulation_officialDocument

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|||officialDocument|Long|

#### SupplementaryRegulation_specificRegulation

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|specificSupplementaryRegulation|SpecificSupplementaryRegulationValue|specificSupRegulation|Text|
|||specificSupRegulation_href|Text|

#### SupplementaryRegulation_supplementaryRegulation

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|supplementaryRegulation|SupplementaryRegulationValue|RID|Long|
|||supplementaryRegulation|Text|
|||supplementaryRegulation_href|Text|

#### ZoningElement

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|regulationNature|RegulationNatureValue|regulationNature|Text|
|||regulationNature_href|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|processStepGeneral|ProcessStepGeneralValue|processStepGeneral|Text|
|||processStepGeneral_href|Text|
|backgroundMap|BackgroundMapValue|backgroundMap_Date|Text|
|||backgroundMap_Reference|Text|
|||backgroundMap_URI|Text|
|plan||plan|Long|

#### ZoningElement_dimensioningIndication

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|dimensioningIndication|DimensioningIndicationValue|RID|Long|
|||indicationReference|Text|
|||CharacterValue_value|Text|
|||IntegerValue_value|Long|
|||MeasureValue_value|Float|
|||MeasureValue_value_uom|Text|
|||RealValue_value|Float|

#### ZoningElement_hilucsLandUse

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|hilucsLandUse|HILUCSValue|RID|Long|
|||hilucsLandUse|Text|
|||hilucsLandUse_href|Text|

#### ZoningElement_hilucsPresence

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|hilucsPresence| HILUCSPresence|RID|Long|
|||orderedList|Text|
|||orderedList_href|Text|
|||percentage_hilucsValue_href|Text|
|||percentage_hilucsValue|Text|
|||percentage_percentage|Text|

#### ZoningElement_officialDocument

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|officialDocument||officialDocument|Long|

#### ZoningElement_specificLandUse

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|specificLandUse|LandUseClassificationValue|RID|Long|
|||specificLandUse|Text|
|||specificLandUse_href|Text|

#### ZoningElement_specificPresence

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|specificPresence|SpecificPresence|RID|Long|
|||orderedList|Text|
|||orderedList_href|Text|
|||percentage_specificValue|Text|
|||percentage_specificValue_href|Text|
|||percentage_specificPercentage|Text|
