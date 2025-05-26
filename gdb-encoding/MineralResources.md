# Geodatabase Encoding Rule for INSPIRE 
Mineral Resources

`Version: 1.0`
`Date: 2025-01-19`

The Simple Mineral Resources encoding can be used as an *alternative encoding* for Mineral Resources data that fulfills the following requirements:

* There is not more than 1 `sourceReference` for `Mine`
* There is not more than 1 `mineName` for `Mine`
* There is not more than 1 `relatedMine` for `Mine`
* There is not more than 1 `sourceReference` for `MineralOccurence`
* There is not more than 1 `expression` for `MineralOccurence`
* There is not more than 1 `form` for `MineralOccurence`
* There is not more than 1 `shape` for `MineralOccurence`
* There is not more than 1 `endUsePotetial` for `MineralOccurence`
* There is no  `linearOrientation` for `MineralOccurence`
* There is no  `planarOrientation` for `MineralOccurence`
* There is not more than 1 `themeClass` for `MineralOccurence`
* There is not more than 1 `sourceReference` for `Mine`







## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Mineral Resources version 3.0.0](https://github.com/INSPIRE-MIF/technical-guidelines/tree/main/data/mr)

## Conformance Class Core

The Mineral Resources theme has one application schema, therefore this theme-specific encoding rule defines a single core conformance class.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Mineral Resources conceptual model before applying the general rules of this encoding rule:
 
1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. 
2. Apply the SimpleCitation rule `MT007()`.
3. Apply the SimplePeriod rule `MT009()`.
4. Apply the SimpleCategory rule `MT016()`
4. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
5. Apply Attribute shortening rule for Mine:

    |Replace|With|
    |----|----|
    |`'sourceReference_'`|`'sR_' `|
    |`'reportedTo_legalAct_'`|`'legalAct_' `|
    |`'operationalActivityPeriod_'`|`'opActPeriod_' `|

6. Apply Attribute shortening rule for MineralOccurence:

    |Replace|With|
    |----|----|
    |`'themeClass_themeClass'`|`'themeClass' `|
    

7. Apply Attribute shortening rule for EnvironmentalMonitoringFacility:

    |Replace|With|
    |----|----|
    |`'responsibleParty_'`|`'resParty_' `|
    
    

    


#### Commodity

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|source|EarthResource |source|Long|
|commodity|CommodityCodeValue|commodity|Text|
|||commodity_href|Text|
|commodityImportance|ImportanceValue|commodityImportance|Text|
|||commodityImportance_href|Text|
|commodityRank||commodityRank|Long|

#### MineP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|||startDate|Date|
|||mineName|Text|
|||sourceReference_name|Text|
|||sourceReference_type|Text|
|||sourceReference_date|Date|
|||sourceReference_link|Text|
||LegislationLevelValue|sourceReference_level|Text|
|||sourceReference_level_href|Text|
|status|MineStatusValue|status|Text|
|||status_href|Text|
||Mine|relatedMine|Long|
|||endDate|Date|

#### MineS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|||startDate|Date|
|||mineName|Text|
|||sourceReference_name|Text|
|||sourceReference_type|Text|
|||sourceReference_date|Date|
|||sourceReference_link|Text|
||LegislationLevelValue|sourceReference_level|Text|
|||sourceReference_level_href|Text|
|status|MineStatusValue|status|Text|
|||status_href|Text|
||Mine|relatedMine|Long|
|||endDate|Date|

#### MineralOccurrenceP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|||name|Text|
|||expHis_actDur_beginPosition|Date|
|||expHis_actDur_endPosition|Date|
||ExplorationActivityTypeValue|expHis_activityType|Text|
|||expHis_activityType_href|Text|
||ExplorationResultValue|expHis_explorationResult|Text|
|||expHis_explorationResult_href|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanversion|Date|
|sourceReference|DocumentCitation|sourceReference_name|Text|
|||sourceReference_type|Text|
|||sourceReference_date|Date|
|||sourceReference_link|Text|
||LegislationLevelValue|sourceReference_level|Text|
|||sourceReference_level_href|Text|
|dimension|EarthResourceDimension|dimension_area_uom|Text|
|||dimension_area_value_low|Float|
|||dimension_area_value_high|Float|
|||dimension_length_uom|Text|
|||dimension_length_value_low|Float|
|||dimension_length_value_high|Float|
|||dimension_width_uom|Text|
|||dimension_width_value_low|Float|
|||dimension_width_value_high|Float|
|||dimension_depth_uom|Text|
|||dimension_depth_value_low|Float|
|||dimension_depth_value_high|Float|
|expression|Category|expression_codespace|Text|
|||expression_value|Text|
|form|Category|form_codespace|Text|
|||form_value|Text|
|shape|Category|shape_codespace|Text|
|||shape_value|Text|
||MineralDepositGroupValue|clas_mineralDepositGroup|Text|
|||clas_mineralDepositGroup_href|Text|
||MineralDepositTypeValue|clas_mineralDepositType|Text|
|||clas_mineralDepositType_href|Text|
|oreAmount|OreMeasure|oA_classMethodUsed|Text|
|||oA_classMethodUsed_href|Text|
|||oA_date|Date|
|||oA_date_beginPosition|Date|
|||oA_date_endPosition|Date|
|||oA_ore_uom|Text|
|||oA_ore_lower|Text|
|||oA_ore_higher|Text|
|||oA_sourceReference_name|Text|
|||oA_sourceReference_type|Text|
|||oA_sourceReference_date|Date|
|||oA_sourceReference_link|Text|
||LegislationLevelValue|oA_sourceReference_level|Text|
|||oA_sourceReference_level_href|Text|
|category|ResourceCategoryValue|oA_category|Text|
|||oA_category_href|Text|
|||oA_inclReserves|Text|
|||oA_inclResources|Text|
|||oA_OreMeasureType|Text|
||MineralOccurrenceTypeValue|type|Text|
|||type_href|Text|
||EndusePotentialValue|endusePotential1|Text|
|||endusePotential1_href|Text|
||EndusePotentialValue|endusePotential2|Text|
|||endusePotential2_href|Text|
||EndusePotentialValue|endusePotential3|Text|
|||endusePotential3_href|Text|
||MappingFrameValue|mappingFrame|Text|
|||mappingFrame_href|Text|

#### MineralOccurrenceS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|||name|Text|
|||expHis_actDur_beginPosition|Date|
|||expHis_actDur_endPosition|Date|
||ExplorationActivityTypeValue|expHis_activityType|Text|
|||expHis_activityType_href|Text|
||ExplorationResultValue|expHis_explorationResult|Text|
|||expHis_explorationResult_href|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanversion|Date|
|sourceReference|DocumentCitation|sourceReference_name|Text|
|||sourceReference_type|Text|
|||sourceReference_date|Date|
|||sourceReference_link|Text|
||LegislationLevelValue|sourceReference_level|Text|
|||sourceReference_level_href|Text|
|dimension|EarthResourceDimension|dimension_area_uom|Text|
|||dimension_area_value_low|Float|
|||dimension_area_value_high|Float|
|||dimension_length_uom|Text|
|||dimension_length_value_low|Float|
|||dimension_length_value_high|Float|
|||dimension_width_uom|Text|
|||dimension_width_value_low|Float|
|||dimension_width_value_high|Float|
|||dimension_depth_uom|Text|
|||dimension_depth_value_low|Float|
|||dimension_depth_value_high|Float|
|expression|Category|expression_codespace|Text|
|||expression_value|Text|
|form|Category|form_codespace|Text|
|||form_value|Text|
|shape|Category|shape_codespace|Text|
|||shape_value|Text|
||MineralDepositGroupValue|clas_mineralDepositGroup|Text|
|||clas_mineralDepositGroup_href|Text|
||MineralDepositTypeValue|clas_mineralDepositType|Text|
|||clas_mineralDepositType_href|Text|
|oreAmount|OreMeasure|oA_classMethodUsed|Text|
|||oA_classMethodUsed_href|Text|
|||oA_date|Date|
|||oA_date_beginPosition|Date|
|||oA_date_endPosition|Date|
|||oA_ore_uom|Text|
|||oA_ore_lower|Text|
|||oA_ore_higher|Text|
|||oA_sourceReference_name|Text|
|||oA_sourceReference_type|Text|
|||oA_sourceReference_date|Date|
|||oA_sourceReference_link|Text|
||LegislationLevelValue|oA_sourceReference_level|Text|
|||oA_sourceReference_level_href|Text|
|category|ResourceCategoryValue|oA_category|Text|
|||oA_category_href|Text|
|||oA_inclReserves|Text|
|||oA_inclResources|Text|
|||oA_OreMeasureType|Text|
||MineralOccurrenceTypeValue|type|Text|
|||type_href|Text|
||EndusePotentialValue|endusePotential1|Text|
|||endusePotential1_href|Text|
||EndusePotentialValue|endusePotential2|Text|
|||endusePotential2_href|Text|
||EndusePotentialValue|endusePotential3|Text|
|||endusePotential3_href|Text|
||MappingFrameValue|mappingFrame|Text|
|||mappingFrame_href|Text|

#### MineralOccurrence_commodity

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|commodityDescription|Commodity|RID|Long|
|||commodityDescription|Long|
