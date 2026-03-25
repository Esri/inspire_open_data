# Geodatabase Encoding Rule for INSPIRE GeologyCore

`Version: 1.0`
`Date: 2025-08-25`

The Simple Geology Core encoding can be used as an *alternative encoding* for Geology Core data that fulfills the following requirements:

* There is no `Borehole` data.
* There is no `GeomorphologicFeature` data.
* There is no `Fold`.
* There is no `GeologicCollection`.
* There is no `proportion` on `CompositionPart`
* There is no `geologicHistory` on `GeologicStructure`
* There is no `themeClass` on `GeologicStructure`
* There is not more than 1 `EventProcess` per `GeologicEvent`
* There is not more than 1 `themeClass` per `GeologicUnit`





## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Geology Cores version 3.3.0](https://github.com/INSPIRE-MIF/technical-guidelines/tree/main/data/ge)

## Conformance Class Core

The Geology Core theme has one application schema, therefore this theme-specific encoding rule defines a single core conformance class.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Geology Core conceptual model before applying the general rules of this encoding rule:
 
1. Substitute all attributes that have a property type with a Codelist Stereotype through an inline codelist reference using `MT008()`. 
2. Apply the SimpleCitation rule `MT007()`.
3. Apply the SimplePeriod rule `MT009()`.
4. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
5. Limit the Multiplicity for `geologicHistory` for `GeologicEvent` to 1 through Rule `MT012(1)`
6. Limit the Multiplicity for `themeClass` for `GeologicUnit` to 1 through Rule `MT012(1)`


    

    


#### GeologicUnit

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|||name|Text|
|name|GeologicEvent|gH_1_name|Text|
|eventEnvironment||gH_1_eventEnvironment|Text|
|||gH_1_eventEnvironment_href|Text|
|eventProcess||gH_1_eventProcess|Text|
|||gH_1_eventProcess_href|Text|
|olderNamedAge||gH_1_olderNamedAge|Text|
|||gH_1_olderNamedAge_href|Text|
|youngerNamedAge||gH_1_youngerNamedAge|Text|
|||gH_1_youngerNamedAge_href|Text|
|name|GeologicEvent|gH_2_name|Text|
|eventEnvironment||gH_2_eventEnvironment|Text|
|||gH_2_eventEnvironment_href|Text|
|eventProcess||gH_2_eventProcess|Text|
|||gH_2_eventProcess_href|Text|
|olderNamedAge||gH_2_olderNamedAge|Text|
|||gH_2_olderNamedAge_href|Text|
|youngerNamedAge||gH_2_youngerNamedAge|Text|
|||gH_2_youngerNamedAge_href|Text|
|name|GeologicEvent|gH_3_name|Text|
|eventEnvironment||gH_3_eventEnvironment|Text|
|||gH_3_eventEnvironment_href|Text|
|eventProcess||gH_3_eventProcess|Text|
|||gH_3_eventProcess_href|Text|
|olderNamedAge||gH_3_olderNamedAge|Text|
|||gH_3_olderNamedAge_href|Text|
|youngerNamedAge||gH_3_youngerNamedAge|Text|
|||gH_3_youngerNamedAge_href|Text|
|name|GeologicEvent|gH_4_name|Text|
|eventEnvironment||gH_4_eventEnvironment|Text|
|||gH_4_eventEnvironment_href|Text|
|eventProcess||gH_4_eventProcess|Text|
|||gH_4_eventProcess_href|Text|
|olderNamedAge||gH_4_olderNamedAge|Text|
|||gH_4_olderNamedAge_href|Text|
|youngerNamedAge||gH_4_youngerNamedAge|Text|
|||gH_4_youngerNamedAge_href|Text|
|name|GeologicEvent|gH_5_name|Text|
|eventEnvironment||gH_5_eventEnvironment|Text|
|||gH_5_eventEnvironment_href|Text|
|eventProcess||gH_5_eventProcess|Text|
|||gH_5_eventProcess_href|Text|
|olderNamedAge||gH_5_olderNamedAge|Text|
|||gH_5_olderNamedAge_href|Text|
|youngerNamedAge||gH_5_youngerNamedAge|Text|
|||gH_5_youngerNamedAge_href|Text|
|||themeClassification|Text|
|||themeClassification_href|Text|
|||themeClass|Text|
|||themeClass_href|Text|
|||geologicUnitType|Text|
|||geologicUnitType_href|Text|
|||mappingFrame|Text|
|||mappingFrame_href|Text|
|||MATERIAL|Text|
|||OLDERNAMEDAGE|Text|

#### GeologicUnit_composition

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|material||material|Text|
|||material_href|Text|
|role||role|Text|
|||role_href|Text|

#### ShearDisplacementStructure

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|name||name|Text|
|faultType||faultType|Text|
|||faultType_href|Text|
|||mappingFrame|Text|
|||mappingFrame_href|Text|
