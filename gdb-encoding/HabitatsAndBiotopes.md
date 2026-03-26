# Geodatabase Encoding Rule for Habitats And Biotopes

`Version: 1.0`
`Date: 2025-10-29`

The Habitats And Biotopes encoding can be used as an *alternative encoding* for Habitats And Biotopes data that fulfills the following requirements:


* There is not more than 1 `habitat` per `Habitat`
* There is not more than 1 `habitatSpecies` per `Habitat`
* There is not more than 1 `habitatVegetation` per `Habitat`








## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - Habitats And Biotopes version 3.2.0](https://github.com/INSPIRE-MIF/technical-guidelines/tree/main/data/hb)

## Conformance Class Core

The Habitats And Biotopes theme has one application schema, therefore this theme-specific encoding rule defines a single core conformance class.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Habitats And Biotopes conceptual model before applying the general rules of this encoding rule:
 
1. Substitute all attributes that have a property type with a Codelist Stereotype through an inline codelist reference using `MT008()`. 
2. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
3. Limit the Multiplicity for `habitat` for `Habitat` to 1 through Rule `MT012(1)`
4. Limit the Multiplicity for `habitatSpecies` for `Habitat` to 1 through Rule `MT012(1)`
5. Limit the Multiplicity for `habitatVegetation` for `Habitat` to 1 through Rule `MT012(1)`

6. Apply Attribute shortening rule for Habitat:

    |Replace|With|
    |----|----|
    |`'habitatVegetation_localVegetationName_'`|`'hVeg_' `|
    |`'habitatSpecies_reference'`|`'hS_r' `|
    |`'habitatSpecies_localSpeciesName_'`|`'hS_l_' `|
    |`'habitat_reference'`|`'h_r' `|
    |`'habitat_localHabitatName_'`|`'h_l_' `|

    


#### HabitatL

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|inspireId|Identifier|featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|HabitatTypeCoverType||h_rHabitatTypeId_href|Text|
|||h_rHabitatTypeId|Text|
|||h_rHabitatTypeScheme_href|Text|
|||h_rHabitatTypeScheme|Text|
|||h_rHabitatTypeName|Text|
|||h_l_localScheme|Text|
|||h_l_localNameCode_href|Text|
|||h_l_localNameCode|Text|
|||h_l_localName|Text|
|||h_l_qualifierLocalName_href|Text|
|||h_l_qualifierLocalName|Text|
|||h_areaCovered|Float|
|||h_areaCovered_uom|Text|
|||h_lengthCovered|Float|
|||h_lengthCovered_uom|Text|
|||h_volumeCovered|Float|
|||h_volumeCovered_uom|Text|
|HabitatSpeciesType||hS_rSpeciesId_href|Text|
|||hS_rSpeciesId|Text|
|||hS_rSpeciesScheme_href|Text|
|||hS_rSpeciesScheme|Text|
|||hS_l_localScheme|Text|
|||hS_l_localNameCode_href|Text|
|||hS_l_localNameCode|Text|
|||hS_l_localName|Text|
|||hS_l_qualifierLocalName_href|Text|
|||hS_l_qualifierLocalName|Text|
|HabitatVegetationType||hVeg_localScheme|Text|
|||hVeg_localNameCode_href|Text|
|||hVeg_localNameCode|Text|
|||hVeg_localName|Text|
|||hVeg_qualifierLocalName_href|Text|
|||hVeg_qualifierLocalName|Text|

#### HabitatP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|inspireId|Identifier|featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|HabitatTypeCoverType||h_rHabitatTypeId_href|Text|
|||h_rHabitatTypeId|Text|
|||h_rHabitatTypeScheme_href|Text|
|||h_rHabitatTypeScheme|Text|
|||h_rHabitatTypeName|Text|
|||h_l_localScheme|Text|
|||h_l_localNameCode_href|Text|
|||h_l_localNameCode|Text|
|||h_l_localName|Text|
|||h_l_qualifierLocalName_href|Text|
|||h_l_qualifierLocalName|Text|
|||h_areaCovered|Float|
|||h_areaCovered_uom|Text|
|||h_lengthCovered|Float|
|||h_lengthCovered_uom|Text|
|||h_volumeCovered|Float|
|||h_volumeCovered_uom|Text|
|HabitatSpeciesType||hS_rSpeciesId_href|Text|
|||hS_rSpeciesId|Text|
|||hS_rSpeciesScheme_href|Text|
|||hS_rSpeciesScheme|Text|
|||hS_l_localScheme|Text|
|||hS_l_localNameCode_href|Text|
|||hS_l_localNameCode|Text|
|||hS_l_localName|Text|
|||hS_l_qualifierLocalName_href|Text|
|||hS_l_qualifierLocalName|Text|
|HabitatVegetationType||hVeg_localScheme|Text|
|||hVeg_localNameCode_href|Text|
|||hVeg_localNameCode|Text|
|||hVeg_localName|Text|
|||hVeg_qualifierLocalName_href|Text|
|||hVeg_qualifierLocalName|Text|

#### HabitatS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|inspireId|Identifier|featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|HabitatTypeCoverType||h_rHabitatTypeId_href|Text|
|||h_rHabitatTypeId|Text|
|||h_rHabitatTypeScheme_href|Text|
|||h_rHabitatTypeScheme|Text|
|||h_rHabitatTypeName|Text|
|||h_l_localScheme|Text|
|||h_l_localNameCode_href|Text|
|||h_l_localNameCode|Text|
|||h_l_localName|Text|
|||h_l_qualifierLocalName_href|Text|
|||h_l_qualifierLocalName|Text|
|||h_areaCovered|Float|
|||h_areaCovered_uom|Text|
|||h_lengthCovered|Float|
|||h_lengthCovered_uom|Text|
|||h_volumeCovered|Float|
|||h_volumeCovered_uom|Text|
|HabitatSpeciesType||hS_rSpeciesId_href|Text|
|||hS_rSpeciesId|Text|
|||hS_rSpeciesScheme_href|Text|
|||hS_rSpeciesScheme|Text|
|||hS_l_localScheme|Text|
|||hS_l_localNameCode_href|Text|
|||hS_l_localNameCode|Text|
|||hS_l_localName|Text|
|||hS_l_qualifierLocalName_href|Text|
|||hS_l_qualifierLocalName|Text|
|HabitatVegetationType||hVeg_localScheme|Text|
|||hVeg_localNameCode_href|Text|
|||hVeg_localNameCode|Text|
|||hVeg_localName|Text|
|||hVeg_qualifierLocalName_href|Text|
|||hVeg_qualifierLocalName|Text|
