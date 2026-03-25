# Geodatabase Encoding Rule for INSPIRE Hydro - Physical Waters

`Version: 1.0`
`Date: 2026-01-10`

The Simple Hydro - Physical Waters encoding can be used as an *alternative encoding* for Hydro - Physical Waters data that fulfills the following requirements:

* There is no `HydroObject` relatedHydroObject per `HydroObject`
* There is no `Shore` bank per `SurfaceWater`
* There is not more than 1 `HydroIdentifier` hydroId per `HydroObject`



## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Hydrography version 4.0.0](https://github.com/INSPIRE-MIF/technical-guidelines/tree/main/data/hy)

## Conformance Class Core

The Hydro - Physical Waters theme has one application schema, therefore this theme-specific encoding rule defines a single core conformance class.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Hydro - Physical Waters conceptual model before applying the general rules of this encoding rule:
 
1. Substitute all occurrences of `GeographicName` with the Simple Geographic Name through Rule `MT005(separator: '_')`.  
2. Substitute all attributes that have a property type with a Codelist Stereotype through an inline codelist reference using `MT008()`. 
3. Limit the Multiplicity for `hydroId` for `HydroObject` to 3 through Rule `MT012(1)`
4. `DrainageBasin.outlet` is modelled as the inverse of `SurfaceWater.drainsBasin`
5. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')`



#### Crossing

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||name_lang|Text|
|||name|Text|
|||hydroId_classificationScheme|Text|
|||hydroId_localId|Text|
|||hydroId_namespace|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|condition|ConditionOfFacilityValue|condition_href|Text|
|||condition|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|levelOfDetail||levelOfDetail|Text|
|||type_href|Text|
|||type|Text|

#### DamOrWeir

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||name_lang|Text|
|||name|Text|
|||hydroId_classificationScheme|Text|
|||hydroId_localId|Text|
|||hydroId_namespace|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|condition|ConditionOfFacilityValue|condition_href|Text|
|||condition|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|levelOfDetail||levelOfDetail|Text|

#### DrainageBasin

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||name_lang|Text|
|||name|Text|
|||hydroId_classificationScheme|Text|
|||hydroId_localId|Text|
|||hydroId_namespace|Text|
|||area|Float|
|||area_uom|Text|
|||basinOrder_order|Text|
|||basinOrder_orderScheme|Text|
|||basinOrder_scope|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|origin||origin|Text|

#### DrainageBasin_containsBasin

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|||containsBasin|Long|

#### Embankment

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||name_lang|Text|
|||name|Text|
|||hydroId_classificationScheme|Text|
|||hydroId_localId|Text|
|||hydroId_namespace|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|condition|ConditionOfFacilityValue|condition_href|Text|
|||condition|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|levelOfDetail||levelOfDetail|Text|

#### Falls

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||name_lang|Text|
|||name|Text|
|||hydroId_classificationScheme|Text|
|||hydroId_localId|Text|
|||hydroId_namespace|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|levelOfDetail||levelOfDetail|Text|
|||height|Float|
|||height_uom|Text|

#### Ford

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||name_lang|Text|
|||name|Text|
|||hydroId_classificationScheme|Text|
|||hydroId_localId|Text|
|||hydroId_namespace|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|condition|ConditionOfFacilityValue|condition_href|Text|
|||condition|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|levelOfDetail||levelOfDetail|Text|

#### LandWaterBoundary

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|origin||origin|Text|
|||waterLevelCategory_href|Text|
|||waterLevelCategory|Text|

#### Lock

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||name_lang|Text|
|||name|Text|
|||hydroId_classificationScheme|Text|
|||hydroId_localId|Text|
|||hydroId_namespace|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|condition|ConditionOfFacilityValue|condition_href|Text|
|||condition|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|levelOfDetail||levelOfDetail|Text|

#### Rapids

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||name_lang|Text|
|||name|Text|
|||hydroId_classificationScheme|Text|
|||hydroId_localId|Text|
|||hydroId_namespace|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|levelOfDetail||levelOfDetail|Text|

#### RiverBasin

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||name_lang|Text|
|||name|Text|
|||hydroId_classificationScheme|Text|
|||hydroId_localId|Text|
|||hydroId_namespace|Text|
|||area|Float|
|||area_uom|Text|
|||basinOrder_order|Text|
|||basinOrder_orderScheme|Text|
|||basinOrder_scope|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|origin||origin|Text|

#### RiverBasin_containsBasin

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|||containsBasin|Long|

#### Shore

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||name_lang|Text|
|||name|Text|
|||hydroId_classificationScheme|Text|
|||hydroId_localId|Text|
|||hydroId_namespace|Text|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|||composition_href|Text|
|||composition|Text|
|delineationKnown||delineationKnown|Short|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|

#### ShorelineConstruction

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||name_lang|Text|
|||name|Text|
|||hydroId_classificationScheme|Text|
|||hydroId_localId|Text|
|||hydroId_namespace|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|condition|ConditionOfFacilityValue|condition_href|Text|
|||condition|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|levelOfDetail||levelOfDetail|Text|

#### Sluice

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||name_lang|Text|
|||name|Text|
|||hydroId_classificationScheme|Text|
|||hydroId_localId|Text|
|||hydroId_namespace|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|condition|ConditionOfFacilityValue|condition_href|Text|
|||condition|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|levelOfDetail||levelOfDetail|Text|

#### StandingWater

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||name_lang|Text|
|||name|Text|
|||hydroId_classificationScheme|Text|
|||hydroId_localId|Text|
|||hydroId_namespace|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|levelOfDetail||levelOfDetail|Text|
|||localType|Text|
|origin||origin|Text|
|||persistence_href|Text|
|||persistence|Text|
|tidal||tidal|Short|
|elevation||elevation|Float|
|||elevation_uom|Text|
|meanDepth||meanDepth|Float|
|||meanDepth_uom|Text|
|surfaceArea||surfaceArea|Float|
|||surfaceArea_uom|Text|

#### StandingWater_drainsBasin

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|||drainsBasin|Long|

#### Watercourse

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||name_lang|Text|
|||name|Text|
|||hydroId_classificationScheme|Text|
|||hydroId_localId|Text|
|||hydroId_namespace|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|levelOfDetail||levelOfDetail|Text|
|||localType|Text|
|origin||origin|Text|
|||persistence_href|Text|
|||persistence|Text|
|tidal||tidal|Short|
|condition|ConditionOfFacilityValue|condition_href|Text|
|||condition|Text|
|delineationKnown||delineationKnown|Short|
|length||length|Float|
|length.uom||length_uom|Text|
|level||level|Text|
|streamOrder||streamOrder_order|Text|
|||streamOrder_orderScheme|Text|
|||streamOrder_scope|Text|
|||width_lower|Float|
|||width_lower_uom|Text|
|||width_upper|Float|
|||width_upper_uom|Text|

#### Watercourse_drainsBasin

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|||drainsBasin|Long|

#### Wetland

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||name_lang|Text|
|||name|Text|
|||hydroId_classificationScheme|Text|
|||hydroId_localId|Text|
|||hydroId_namespace|Text|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|||localType|Text|
|tidal||tidal|Short|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
