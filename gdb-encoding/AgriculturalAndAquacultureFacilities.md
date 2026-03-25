# Geodatabase Encoding Rule for INSPIRE Agricultural And Aquaculture Facilities

`Version: 1.0`
`Date: 2025-10-29`

The Agricultural And Aquaculture Facilities encoding can be used as an *alternative encoding* for Agricultural And Aquaculture Facilities data that fulfills the following requirements:


* There is not more than 3 `activity` per `Site`
* There is not more than 3 `includesAnimal` per `Site`
* There is not more than 1 `thematicId` per `Site`
* There is not more than 1 `aquaculture` per `FarmAnimalSpecies`
* There is not more than 1 `livestock` per `FarmAnimalSpecies`
* There is no `input` and `output` per `Holding.function.Function`



## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Agricultural And Aquaculture Facilities version 3.2.0](https://github.com/INSPIRE-MIF/technical-guidelines/tree/main/data/af)

## Conformance Class Core

The Agricultural And Aquaculture Facilities theme has one application schema, therefore this theme-specific encoding rule defines a single core conformance class.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Agricultural And Aquaculture Facilities conceptual model before applying the general rules of this encoding rule:
 
1. Substitute all attributes that have a property type with a Codelist Stereotype through an inline codelist reference using `MT008()`. 
2. `Holding.contains` is modeled as the inverse of `Site.holding`
3. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
4. Limit the Multiplicity for `thematicId` for `Site` to 1 through Rule `MT012(1)`
5. Limit the Multiplicity for `activity` for `Site` to 3 through Rule `MT012(3)`
6. Limit the Multiplicity for `includesAnimal` for `Site` to 3 through Rule `MT012(3)`
7. Limit the Multiplicity for `livestock` and `aquaculture` for `FarmAnimalSpecies` to 1 through Rule `MT012(1)`

    


#### Holding

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

#### HoldingP

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

#### Site

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|EconomicActivityNACEValue||activity_1_href|Text|
|||activity_1|Text|
|||activity_2_href|Text|
|||activity_2|Text|
|||activity_3_href|Text|
|||activity_3|Text|
|||includesAnimal_1_livestock|Text|
|||includesAnimal_1_aquaculture|Text|
|||includesAnimal_2_livestock|Text|
|||includesAnimal_2_aquaculture|Text|
|||includesAnimal_3_livestock|Text|
|||includesAnimal_3_aquaculture|Text|
|||holding|Long|

#### SiteP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|EconomicActivityNACEValue||activity_1_href|Text|
|||activity_1|Text|
|||activity_2_href|Text|
|||activity_2|Text|
|||activity_3_href|Text|
|||activity_3|Text|
|||includesAnimal_1_livestock|Text|
|||includesAnimal_1_aquaculture|Text|
|||includesAnimal_2_livestock|Text|
|||includesAnimal_2_aquaculture|Text|
|||includesAnimal_3_livestock|Text|
|||includesAnimal_3_aquaculture|Text|
|||holding|Long|
