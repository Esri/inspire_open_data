# Geodatabase Encoding Rule for INSPIRE PlannedLandUse

`Version: 0.0`
`Date: 2021-02-22`

The Simple PlannedLandUse encoding can be used as an *alternative encoding* for PlannedLandUse data that fulfills the following requirements:

* It is sufficient to provide the `activity` for the `Function` in function. 
* It is sufficient to provide the `activity` for the `Capacity` in physicalCapacity.  
* There is no information on permittedCapacity for Permissions.


## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](/gdb-encoding/geodatabse encoding.md)
* [Data Specification - INSPIRE Land Use version 3.1](https://inspire.ec.europa.eu/Themes/129/2892)

## Conformance Class Planned Land Use

The Land Use theme has five application schema. This application schema-specific encoding rule defines a single conformance class for the application schema Planned Land Use.
### Model Transformation

This section describes which transformation rules with which parameters are applied to the PlannedLandUse conceptual model before applying the general rules of this encoding rule:
 

1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. (works in GDB)
2. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` (works in GDB as ong as not to long)
4. Create seperate Tables for each Geometry Type, add suffix for P for Points, L for Lines and S for Areas.
5. References to Objects by URL (String)


ToDO: 
SimpleRelatedParty beschreiben, Multiplizität bei RelatedParty erlauben
Contact in einzelne Attribute zerlegen.




#### OfficialDocumentation

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId||
|inspireId|Identifier|inspireId_localId||
|||inspireId_namespace||
|||inspireId_versionId||
|legislationCitation|LegislationCitation|legislationCitation_name||
|||legislationCitation_type||
|||legislationCitation_date||
|||legislationCitation_link||
|||legislationCitation_level||
|||legislationCitation_level_href||
|||regulationText||
|||planDocument_name||
|||planDocument_type||
|||planDocument_date||
|||planDocument_link||
|||planDocument_level||
|||planDocument_level_href||

#### SpatialPlan

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId||
|inspireId|Identifier|inspireId_localId||
|||inspireId_namespace||
|||inspireId_versionId||
|extent|GM_MultiSurface|extent||
|beginLifespanVersion|DateTime|beginLifespanVersion||
|officialTitle|CharacterString|officialTitle||
|levelOfSpatialPlan|LevelOfSpatialPlanValue|levelOfSpatialPlan||
|||levelOfSpatialPlan_href||
|endLifespanVersion|DateTime|endLifespanVersion||
|validFrom|DateTime|validFrom||
|validTo|DateTime|validTo||
|alternativeTitle|CharacterString|alternativeTitle||
|planTypeName|PlanTypeNameValue|planTypeName||
|||planTypeName_href||
|processStepGeneral|ProcessStepGeneralValue|processStepGeneral||
|||processStepGeneral_href||
|backgroundMap|BackgroundMapValue|backgroundMap_Date||
|||backgroundMap_Reference||
|||backgroundMap_URI||

#### SpatialPlan_member

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID||
|member|ZoningElement|member||

#### SpatialPlan_officialDocument

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID||
|officialDocument|OfficialDocumentation|officialDocument||

#### SpatialPlan_ordinance

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|ordinance|OrdinanceValue |RID||
|||ordinanceDate||
|||ordinanceReference||

#### SpatialPlan_restriction

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID||
|restriction|SupplementaryRegulation|restriction||

#### SupplementaryRegulation

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId||
|validFrom|DateTime|validFrom||
|validTo|DateTime|validTo||
|processStepGeneral|ProcessStepGeneralValue|processStepGeneral||
|||processStepGeneral_href||
|backgroundMap|BackgroundMapValue|backgroundMap_Date||
|||backgroundMap_Reference||
|||backgroundMap_URI||
|beginLifespanVersion|DateTime|beginLifespanVersion||
|inspireId|Identifier|inspireId_localId||
|||inspireId_namespace||
|||inspireId_versionId||
|endLifespanVersion|DateTime|endLifespanVersion||
|geometry|GM_Object|geometry||
|inheritedFromOtherPlans|Boolean|inheritedFromOtherPlans||
|specificRegulationNature|CharacterString|specificRegulationNature||
|regulationNature|RegulationNatureValue|regulationNature||
|||regulationNature_href||
|||plan||

#### SupplementaryRegulation_dimensioningIndication

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|dimensioningIndication|DimensioningIndicationValue|RID||
|||indicationReference||
|||CharacterValue_value||
|||IntegerValue_value||
|||MeasureValue_value||
|||MeasureValue_value_uom||
|||RealValue_value||

#### SupplementaryRegulation_name

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID||
|name|CharacterString|name||

#### SupplementaryRegulation_officialDocument

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID||
|||officialDocument||

#### SupplementaryRegulation_specificRegulation

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID||
|specificSupplementaryRegulation|SpecificSupplementaryRegulationValue|specificSupRegulation||
|||specificSupRegulation_href||

#### SupplementaryRegulation_supplementaryRegulation

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|supplementaryRegulation|SupplementaryRegulationValue|RID||
|||supplementaryRegulation||
|||supplementaryRegulation_href||

#### ZoningElement

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId||
|inspireId|Identifier|inspireId_localId||
|||inspireId_namespace||
|||inspireId_versionId||
|geometry|GM_MultiSurface|geometry||
|validFrom|DateTime|validFrom||
|validTo|DateTime|validTo||
|beginLifespanVersion|DateTime|beginLifespanVersion||
|regulationNature|RegulationNatureValue|regulationNature||
|||regulationNature_href||
|endLifespanVersion|DateTime|endLifespanVersion||
|processStepGeneral|ProcessStepGeneralValue|processStepGeneral||
|||processStepGeneral_href||
|backgroundMap|BackgroundMapValue|backgroundMap_Date||
|||backgroundMap_Reference||
|||backgroundMap_URI||
|plan||plan||

#### ZoningElement_dimensioningIndication

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|dimensioningIndication|DimensioningIndicationValue|RID||
|||indicationReference||
|||CharacterValue_value||
|||IntegerValue_value||
|||MeasureValue_value||
|||MeasureValue_value_uom||
|||RealValue_value||

#### ZoningElement_hilucsLandUse

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|hilucsLandUse|HILUCSValue|RID||
|||hilucsLandUse||
|||hilucsLandUse_href||

#### ZoningElement_hilucsPresence

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|hilucsPresence| HILUCSPresence|RID||
|||orderedList||
|||orderedList_href||
|||percentage_hilucsValue||
|||percentage_percentage||

#### ZoningElement_officialDocument

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID||
|officialDocument||officialDocument||

#### ZoningElement_specificLandUse

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||specificLandUse_href||

#### ZoningElement_specificPresence

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||orderedList_href||
|||percentage_specificValue_href||
|||percentage_specificPercentage||
