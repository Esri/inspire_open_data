# Geodatabase Encoding Rule for INSPIRE Production and Industrial Facilities

`Version: 1.0`
`Date: 2026-01-15`

The Production And Industrial Facilities encoding can be used as an *alternative encoding* for Production And Industrial Facilities data that fulfills the following requirements:

* There is no `ProductionPlot`
* There is no `ProductionBuilding`
* There is no `ProductionInstallationPart`
* There is not more than 1 `status`, `sitePlan` and `description` per `ProductionSite`
* There is not more than 3 `function` per `ProductionFacility`
* There is not more than 1 `thematicId` per `ProductionFacility`
* There is not more than 2 `name` per `ProductionFacility`, `ProductionInstallation`, `ProductionSite`
* There is no `input` and `output` per `ProductionFacility.function.Function`



## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Production And Industrial Facilities version 3.2.0](https://github.com/INSPIRE-MIF/technical-guidelines/tree/main/data/pf)

## Conformance Class Core

The Production And Industrial Facilities theme has one application schema, therefore this theme-specific encoding rule defines a single core conformance class.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Production And Industrial Facilities conceptual model before applying the general rules of this encoding rule:
 
1. Substitute all attributes that have a property type with a Codelist Stereotype through an inline codelist reference using `MT008()`. 
2. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
3. Limit the Multiplicity for `thematicId`, `status`, `sitePlan` and `description` for `ProductionSite` to 1 through Rule `MT012(1)`
4. Limit the Multiplicity for `thematicId`, `status` and `description` for `ProductionInstallation` to 1 through Rule `MT012(1)`
5. Limit the Multiplicity for `status` for `ProductionFacility` to 1 through Rule `MT012(1)`
6. Limit the Multiplicity for `name` for `ProductionSite` to 1 through Rule `MT012(2)`
7. Limit the Multiplicity for `name` for `ProductionInstallation` to 1 through Rule `MT012(2)`
8. Limit the Multiplicity for `name` for `ProductionFacility` to 1 through Rule `MT012(2)`
9. Limit the Multiplicity for `function` for `ProductionFacility` to 3 through Rule `MT012(3)`
   

    


#### ProductionFacilityP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|||thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
|||name|Text|
|function|Function|function_1_activity_href|Text|
|||function_1_activity|Text|
|||function_1_description|Text|
|||function_2_activity_href|Text|
|||function_2_activity|Text|
|||function_2_description|Text|
|||function_3_activity_href|Text|
|||function_3_activity|Text|
|||function_3_description|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|||riverBasinDistrict_href|Text|
|||riverBasinDistrict|Text|
|status|StatusType|status_statusType_href|Text|
|||status_statusType|Text|
|||status_description|Text|
|||status_validFrom|Date|
|||status_validTo|Date|
|||hostingSite|Text|

#### ProductionFacilityS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|||thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
|||name|Text|
|function|Function|function_1_activity_href|Text|
|||function_1_activity|Text|
|||function_1_description|Text|
|||function_2_activity_href|Text|
|||function_2_activity|Text|
|||function_2_description|Text|
|||function_3_activity_href|Text|
|||function_3_activity|Text|
|||function_3_description|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|||riverBasinDistrict_href|Text|
|||riverBasinDistrict|Text|
|status|StatusType|status_statusType_href|Text|
|||status_statusType|Text|
|||status_description|Text|
|||status_validFrom|Date|
|||status_validTo|Date|
|||hostingSite|Text|

#### ProductionInstallation

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|||thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
|||name_1|Text|
|||name_2|Text|
|||description|Text|
|status|StatusType|status_statusType_href|Text|
|||status_statusType|Text|
|||status_description|Text|
|||status_validFrom|Date|
|||status_validTo|Date|
|||groupingFacility|Long|

#### ProductionSite

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|||thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
|sitePlan|DocumentCitation|sitePlan_name|Text|
|||sitePlan_type|Text|
|||sitePlan_date|Date|
|||sitePlan_link|Text|
|||sitePlan_level|Text|
|||sitePlan_level_href|Text|
||CharacterString|name_1|Text|
||CharacterString|name_2|Text|
||CharacterString|description_1|Text|
||CharacterString|description_2|Text|
|status|StatusType|status_statusType_href|Text|
|||status_statusType|Text|
|||status_description|Text|
|||status_validFrom|Date|
|||status_validTo|Date|
