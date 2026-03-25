# Geodatabase Encoding Rule for Species Distribution

`Version: 1.0`
`Date: 2025-10-29`

The Species Distribution encoding can be used as an *alternative encoding* for Species Distribution data that fulfills the following requirements:


* There is not more than 1 `distributionInfo` per `SpeciesDistributionUnit`
* There is not more than 1 `documentBasis` per `SpeciesDistributionUnitDataSet`







## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - Species Distribution version 3.2.0](https://github.com/INSPIRE-MIF/technical-guidelines/tree/main/data/sd)

## Conformance Class Core

The Species Distribution theme has one application schema, therefore this theme-specific encoding rule defines a single core conformance class.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Species Distribution conceptual model before applying the general rules of this encoding rule:
 
1. Substitute all attributes that have a property type with a Codelist Stereotype through an inline codelist reference using `MT008()`. 
2. `SpeciesDistributionUnitDataSet.member` is modeled as the inverse of `SpeciesDistributionUnit.dataSet`
3. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
4. Limit the Multiplicity for `distributionInfo` for `SpeciesDistributionUnit` to 1 through Rule `MT012(1)`
5. Limit the Multiplicity for `documentBasis` for `SpeciesDistributionUnitDataSet` to 1 through Rule `MT012(1)`
6. Apply Attribute shortening rule for SpeciesDistributionUnit:

|Replace|With|
|----|----|
|`'speciesName_'`|`'name_' `|
|`'referenceSpecies'`|`'refSpecies' `|
|`'distributionInfo_'`|`'dI_' `|
|`'populationSize'`|`'popSize' `|
|`'habitat_localHabitatName_'`|`'h_l_' `|



#### SpeciesDistributionDataSet

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|||name|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|||documentBasis_name|Text|
|||documentBasis_type|Text|
|||documentBasis_date|Date|
|||documentBasis_link|Text|
|||documentBasis_level_href|Text|
|||documentBasis_level_href|Text|

#### SpeciesDistributionUnitL

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|||name_refSpeciesId_href|Text|
|||name_refSpeciesId|Text|
|||name_refSpeciesScheme_href|Text|
|||name_refSpeciesScheme|Text|
|||name_refSpeciesName|Text|
|||name_localSpeciesId_href|Text|
|||name_localSpeciesId|Text|
|||name_localSpeciesScheme|Text|
|||name_localSpeciesName|Text|
|||name_qualifier_href|Text|
|||name_qualifier|Text|
|||dI_occurrenceCategory_href|Text|
|||dI_occurrenceCategory|Text|
|||dI_residencyStatus_href|Text|
|||dI_residencyStatus|Text|
|||dI_popSize_countingMethod_href|Text|
|||dI_popSize_countingMethod|Text|
|||dI_popSize_countingUnit_href|Text|
|||dI_popSize_countingUnit|Text|
|||dI_popSize_upperBound|Long|
|||dI_popSize_lowerBound|Long|
|||dI_sensitiveInfo|Short|
|||dI_populationType_href|Text|
|||dI_populationType|Text|
|||dI_collectedFrom|Date|
|||dI_collectedTo|Date|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|||dataSet|Long|

#### SpeciesDistributionUnitP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|||name_refSpeciesId_href|Text|
|||name_refSpeciesId|Text|
|||name_refSpeciesScheme_href|Text|
|||name_refSpeciesScheme|Text|
|||name_refSpeciesName|Text|
|||name_localSpeciesId_href|Text|
|||name_localSpeciesId|Text|
|||name_localSpeciesScheme|Text|
|||name_localSpeciesName|Text|
|||name_qualifier_href|Text|
|||name_qualifier|Text|
|||dI_occurrenceCategory_href|Text|
|||dI_occurrenceCategory|Text|
|||dI_residencyStatus_href|Text|
|||dI_residencyStatus|Text|
|||dI_popSize_countingMethod_href|Text|
|||dI_popSize_countingMethod|Text|
|||dI_popSize_countingUnit_href|Text|
|||dI_popSize_countingUnit|Text|
|||dI_popSize_upperBound|Long|
|||dI_popSize_lowerBound|Long|
|||dI_sensitiveInfo|Short|
|||dI_populationType_href|Text|
|||dI_populationType|Text|
|||dI_collectedFrom|Date|
|||dI_collectedTo|Date|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|||dataSet|Long|

#### SpeciesDistributionUnitS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|||name_refSpeciesId_href|Text|
|||name_refSpeciesId|Text|
|||name_refSpeciesScheme_href|Text|
|||name_refSpeciesScheme|Text|
|||name_refSpeciesName|Text|
|||name_localSpeciesId_href|Text|
|||name_localSpeciesId|Text|
|||name_localSpeciesScheme|Text|
|||name_localSpeciesName|Text|
|||name_qualifier_href|Text|
|||name_qualifier|Text|
|||dI_occurrenceCategory_href|Text|
|||dI_occurrenceCategory|Text|
|||dI_residencyStatus_href|Text|
|||dI_residencyStatus|Text|
|||dI_popSize_countingMethod_href|Text|
|||dI_popSize_countingMethod|Text|
|||dI_popSize_countingUnit_href|Text|
|||dI_popSize_countingUnit|Text|
|||dI_popSize_upperBound|Long|
|||dI_popSize_lowerBound|Long|
|||dI_sensitiveInfo|Short|
|||dI_populationType_href|Text|
|||dI_populationType|Text|
|||dI_collectedFrom|Date|
|||dI_collectedTo|Date|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|||dataSet|Long|
