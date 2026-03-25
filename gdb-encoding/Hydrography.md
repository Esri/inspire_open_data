# Geodatabase Encoding Rule for INSPIRE Administrative Units

`Version: 0.5`
`Date: 2025-06-11`

The Simple Hydrography encoding can be used as an *alternative encoding* for hydrography data that fulfills the following requirements:

* There are not more than three values for `name` in `DrainageBasin`,`SurfaceWater`, `Shore`, `Wetland`,`ManMadeObj`, `POIP`. 
* There are not more than three values for `GeographicalName` and `hydroId` (hyId_classificationScheme, hyId_localId, hyId_namespace) in relation to HydroObject in  `DrainageBasin`,`SurfaceWater`, `Shore`, `Wetland`,`ManMadeObj`, `POIP.
* There is no networkElementS as a Hydro - Network element.
* There is no networkProperty and NetworkReference dependent Object Class as a Hydro - Network element.
* There is no NetworkConnection since only one single Hydro - Network si implemented.

## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Hydrography version 3.1](https://github.com/INSPIRE-MIF/technical-guidelines/blob/main/data/hy/dataspecification_hy.pdf)

## Conformance Class Administrative Units

The Hydrography theme has three application schemas: Hydro - base, Hydro - Network, Hydro - Physical Waters. This application schema-specific encoding rule defines a conformance class for all three schemas without including Water Transport Network and transport related feature tpes included in Source application schemas other than Hydro.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Hydrography conceptual model before applying the general rules of this encoding rule:
 

1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`.
2. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
3. Limit the Multiplicity for `name` in `DrainageBasin`,`SurfaceWater`, `Shore`, `Wetland`,`ManMadeObj`, `POIP` to 3 through Rule `MT012(3)`
5. Limit the Multiplicity for `GeographicalName` and `hydroId` (hyId_classificationScheme, hyId_localId, hyId_namespace) in relation to HydroObject in  `DrainageBasin`,`SurfaceWater`, `Shore`, `Wetland`,`ManMadeObj`, `POIP` to 3 through Rule `MT012(3)`
6. Limit the Multiplicity for `name` in `networkElementL`, `networkElementP`, `networkElement`, `networkNetwork` to 3 through Rule `MT012(3)`
7. Limit the Multiplicity for `hydroId` (hyId_classificationScheme, hyId_localId, hyId_namespace) in `networkElementL`, `networkElementP`, `networkElement` to 3 through Rule `MT012(3)`
8. Represent the n:m Relationships in Relationship Tables: `MT013`


#### DrainageBasin

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|area|Area|area|Float|
|||area_uom|Text|
|basinOrder|HydroOrderCode|basinOrder_order|Text|
|||basinOrder_orderScheme|Text|
|||basinOrder_scope|Text|
|origin|OriginValue|origin|Text|
|||origin_href|Text|
|||type|Text|
|HydroIdentifier|HydroIdentifier|hyId_classificationScheme1|Text|
|||hyId_classificationScheme2|Text|
|||hyId_classificationScheme3|Text|
|||hyId_localId1|Text|
|||hyId_localId2|Text|
|||hyId_localId3|Text|
|||hyId_namespace1|Text|
|||hyId_namespace2|Text|
|||hyId_namespace3|Text|
|||name_1|Text|
|||name_1_lang|Text|
|||name_2|Text|
|||name_2_lang|Text|
|||name_3|Text|
|||name_3_lang|Text|

#### HydroPOIL

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|height|height|falls_height|Float|
|||falls_height _uom|Text|
|||type|Text|
|HydroIdentifier|HydroIdentifier|hyId_classificationScheme1|Text|
|||hyId_classificationScheme2|Text|
|||hyId_classificationScheme3|Text|
|||hyId_localId1|Text|
|||hyId_localId2|Text|
|||hyId_localId3|Text|
|||hyId_namespace1|Text|
|||hyId_namespace2|Text|
|||hyId_namespace3|Text|
|||name_1|Text|
|||name_1_lang|Text|
|||name_2|Text|
|||name_2_lang|Text|
|||name_3|Text|
|||name_3_lang|Text|

#### HydroPOIP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|height|height|falls_height|Float|
|||falls_height _uom|Text|
|||type|Text|
|HydroIdentifier|HydroIdentifier|hyId_classificationScheme1|Text|
|||hyId_classificationScheme2|Text|
|||hyId_classificationScheme3|Text|
|||hyId_localId1|Text|
|||hyId_localId2|Text|
|||hyId_localId3|Text|
|||hyId_namespace1|Text|
|||hyId_namespace2|Text|
|||hyId_namespace3|Text|
|||name_1|Text|
|||name_1_lang|Text|
|||name_2|Text|
|||name_2_lang|Text|
|||name_3|Text|
|||name_3_lang|Text|

#### HydroPOIS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|height|height|falls_height|Float|
|||falls_height _uom|Text|
|||type|Text|
|HydroIdentifier|HydroIdentifier|hyId_classificationScheme1|Text|
|||hyId_classificationScheme2|Text|
|||hyId_classificationScheme3|Text|
|||hyId_localId1|Text|
|||hyId_localId2|Text|
|||hyId_localId3|Text|
|||hyId_namespace1|Text|
|||hyId_namespace2|Text|
|||hyId_namespace3|Text|
|||name_1|Text|
|||name_1_lang|Text|
|||name_2|Text|
|||name_2_lang|Text|
|||name_3|Text|
|||name_3_lang|Text|

#### LandWaterBoundaryL

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|origin|OriginValue|origin|Text|
|||origin_href|Text|
|waterLevelCategory|WaterLevelValue|waterLevelCategory|Text|
|||waterLevelCategory_href|Text|

#### ManMadeObjL

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|condition|ConditionOfFacilityValue|condition|Float|
|||condition_href|Text|
|||type|Text|
|levelOfDetail|levelOfDetail|lod|Long|
|crossing_type|CrossingTypeValue|crossing_type|Text|
|||crossing_type_href|Text|
|HydroIdentifier|HydroIdentifier|hyId_classificationScheme1|Text|
|||hyId_classificationScheme2|Text|
|||hyId_classificationScheme3|Text|
|||hyId_localId1|Text|
|||hyId_localId2|Text|
|||hyId_localId3|Text|
|||hyId_namespace1|Text|
|||hyId_namespace2|Text|
|||hyId_namespace3|Text|
|||name_1|Text|
|||name_1_lang|Text|
|||name_2|Text|
|||name_2_lang|Text|
|||name_3|Text|
|||name_3_lang|Text|

#### ManMadeObjP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|condition|ConditionOfFacilityValue|condition|Float|
|||condition_href|Text|
|||type|Text|
|levelOfDetail|levelOfDetail|lod|Long|
|crossing_type|CrossingTypeValue|crossing_type|Text|
|||crossing_type_href|Text|
|HydroIdentifier|HydroIdentifier|hyId_classificationScheme1|Text|
|||hyId_classificationScheme2|Text|
|||hyId_classificationScheme3|Text|
|||hyId_localId1|Text|
|||hyId_localId2|Text|
|||hyId_localId3|Text|
|||hyId_namespace1|Text|
|||hyId_namespace2|Text|
|||hyId_namespace3|Text|
|||name_1|Text|
|||name_1_lang|Text|
|||name_2|Text|
|||name_2_lang|Text|
|||name_3|Text|
|||name_3_lang|Text|


#### ManMadeObjS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|condition|ConditionOfFacilityValue|condition|Float|
|||condition_href|Text|
|||type|Text|
|levelOfDetail|levelOfDetail|lod|Long|
|crossing_type|CrossingTypeValue|crossing_type|Text|
|||crossing_type_href|Text|
|HydroIdentifier|HydroIdentifier|hyId_classificationScheme1|Text|
|||hyId_classificationScheme2|Text|
|||hyId_classificationScheme3|Text|
|||hyId_localId1|Text|
|||hyId_localId2|Text|
|||hyId_localId3|Text|
|||hyId_namespace1|Text|
|||hyId_namespace2|Text|
|||hyId_namespace3|Text|
|||name_1|Text|
|||name_1_lang|Text|
|||name_2|Text|
|||name_2_lang|Text|
|||name_3|Text|
|||name_3_lang|Text|

#### networkElementL

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|fictitious|Boolean|fictitious|Short|
|endNode|Long|endNode|Long|
|startNode|Long|startNode|Long|
|flowDirection|LinkDirectionValue|flowDirection|Text|
|||flowDirection_href|Text|
|length|length|length|Float|
|||length_uom|Text|
|||type|Text|
|HydroIdentifier|HydroIdentifier|hyId_classificationScheme1|Text|
|||hyId_classificationScheme2|Text|
|||hyId_classificationScheme3|Text|
|||hyId_localId1|Text|
|||hyId_localId2|Text|
|||hyId_localId3|Text|
|||hyId_namespace1|Text|
|||hyId_namespace2|Text|
|||hyId_namespace3|Text|
|||name_1|Text|
|||name_1_lang|Text|
|||name_2|Text|
|||name_2_lang|Text|
|||name_3|Text|
|||name_3_lang|Text|

#### networkElementP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|hydroNodeCategory|HydroNodeCategoryValue|hydroNodeCategory|Text|
|||hydroNodeCategory_href|Text|
|||type|Text|
|HydroIdentifier|HydroIdentifier|hyId_classificationScheme1|Text|
|||hyId_classificationScheme2|Text|
|||hyId_classificationScheme3|Text|
|||hyId_localId1|Text|
|||hyId_localId2|Text|
|||hyId_localId3|Text|
|||hyId_namespace1|Text|
|||hyId_namespace2|Text|
|||hyId_namespace3|Text|
|||name_1|Text|
|||name_1_lang|Text|
|||name_2|Text|
|||name_2_lang|Text|
|||name_3|Text|
|||name_3_lang|Text|

#### ShoreS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|composition|ShoreTypeValue|composition|Float|
|||composition_href|Text|
|delineationKnown|Boolean|delineationKnown|Long|
|HydroIdentifier|HydroIdentifier|hyId_classificationScheme1|Text|
|||hyId_classificationScheme2|Text|
|||hyId_classificationScheme3|Text|
|||hyId_localId1|Text|
|||hyId_localId2|Text|
|||hyId_localId3|Text|
|||hyId_namespace1|Text|
|||hyId_namespace2|Text|
|||hyId_namespace3|Text|
|||name_1|Text|
|||name_1_lang|Text|
|||name_2|Text|
|||name_2_lang|Text|
|||name_3|Text|
|||name_3_lang|Text|

#### SurfaceWaterL

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|levelOfDetail|levelOfDetail|lod|Float|
|localType|LocalisedCharacterString|localType|Text|
|||localType_locale|Text|
|origin|OriginValue|origin|Text|
|||origin_href|Text|
|persistence|HydrologicalPersistenceValue|persistence|Text|
|||persistence_href|Text|
|tidal|Boolean|tidal|Short|
|condition|ConditionOfFacilityValue|wc_condition|Text|
|||wc_condition_href|Text|
|delineationKnown|Boolean|wc_delineationKnown|Short|
|length|length|wc_length|Float|
|||wc_length_uom|Text|
|level|VerticalPositionValue|wc_level|Text|
|streamOrder|HydroOrderCode|wc_streamOrder_order|Text|
|||wc_streamOrder_orderScheme|Text|
|||wc_streamOrder_scope|Text|
|width|WidthRange|wc_width_lower|Float|
|||wc_width_lower_uom|Text|
|||wc_width_upper|Float|
|||wc_width_upper_uom|Text|
|elevation|Length|stw_elevation|Float|
|||stw_elevation_uom|Text|
|meanDepth|Length|stw_meanDepth|Float|
|||stw_meanDepth_uom|Text|
|surfaceArea|Area|stw_surfaceArea|Float|
|||stw_surfaceArea_uom|Text|
|||type|Text|
|HydroIdentifier|HydroIdentifier|hyId_classificationScheme1|Text|
|||hyId_classificationScheme2|Text|
|||hyId_classificationScheme3|Text|
|||hyId_localId1|Text|
|||hyId_localId2|Text|
|||hyId_localId3|Text|
|||hyId_namespace1|Text|
|||hyId_namespace2|Text|
|||hyId_namespace3|Text|
|||name_1|Text|
|||name_1_lang|Text|
|||name_2|Text|
|||name_2_lang|Text|
|||name_3|Text|
|||name_3_lang|Text|

#### SurfaceWaterP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|levelOfDetail|levelOfDetail|lod|Float|
|localType|LocalisedCharacterString|localType|Text|
|||localType_locale|Text|
|origin|OriginValue|origin|Text|
|||origin_href|Text|
|persistence|HydrologicalPersistenceValue|persistence|Text|
|||persistence_href|Text|
|tidal|Boolean|tidal|Short|
|condition|ConditionOfFacilityValue|wc_condition|Text|
|||wc_condition_href|Text|
|delineationKnown|Boolean|wc_delineationKnown|Short|
|length|length|wc_length|Float|
|||wc_length_uom|Text|
|level|VerticalPositionValue|wc_level|Text|
|streamOrder|HydroOrderCode|wc_streamOrder_order|Text|
|||wc_streamOrder_orderScheme|Text|
|||wc_streamOrder_scope|Text|
|width|WidthRange|wc_width_lower|Float|
|||wc_width_lower_uom|Text|
|||wc_width_upper|Float|
|||wc_width_upper_uom|Text|
|elevation|Length|stw_elevation|Float|
|||stw_elevation_uom|Text|
|meanDepth|Length|stw_meanDepth|Float|
|||stw_meanDepth_uom|Text|
|surfaceArea|Area|stw_surfaceArea|Float|
|||stw_surfaceArea_uom|Text|
|||type|Text|
|HydroIdentifier|HydroIdentifier|hyId_classificationScheme1|Text|
|||hyId_classificationScheme2|Text|
|||hyId_classificationScheme3|Text|
|||hyId_localId1|Text|
|||hyId_localId2|Text|
|||hyId_localId3|Text|
|||hyId_namespace1|Text|
|||hyId_namespace2|Text|
|||hyId_namespace3|Text|
|||name_1|Text|
|||name_1_lang|Text|
|||name_2|Text|
|||name_2_lang|Text|
|||name_3|Text|
|||name_3_lang|Text|

#### SurfaceWaterS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|levelOfDetail|levelOfDetail|lod|Float|
|localType|LocalisedCharacterString|localType|Text|
|||localType_locale|Text|
|origin|OriginValue|origin|Text|
|||origin_href|Text|
|persistence|HydrologicalPersistenceValue|persistence|Text|
|||persistence_href|Text|
|tidal|Boolean|tidal|Short|
|condition|ConditionOfFacilityValue|wc_condition|Text|
|||wc_condition_href|Text|
|delineationKnown|Boolean|wc_delineationKnown|Short|
|length|length|wc_length|Float|
|||wc_length_uom|Text|
|level|VerticalPositionValue|wc_level|Text|
|streamOrder|HydroOrderCode|wc_streamOrder_order|Text|
|||wc_streamOrder_orderScheme|Text|
|||wc_streamOrder_scope|Text|
|width|WidthRange|wc_width_lower|Float|
|||wc_width_lower_uom|Text|
|||wc_width_upper|Float|
|||wc_width_upper_uom|Text|
|elevation|Length|stw_elevation|Float|
|||stw_elevation_uom|Text|
|meanDepth|Length|stw_meanDepth|Float|
|||stw_meanDepth_uom|Text|
|surfaceArea|Area|stw_surfaceArea|Float|
|||stw_surfaceArea_uom|Text|
|||type|Text|
|HydroIdentifier|HydroIdentifier|hyId_classificationScheme1|Text|
|||hyId_classificationScheme2|Text|
|||hyId_classificationScheme3|Text|
|||hyId_localId1|Text|
|||hyId_localId2|Text|
|||hyId_localId3|Text|
|||hyId_namespace1|Text|
|||hyId_namespace2|Text|
|||hyId_namespace3|Text|
|||name_1|Text|
|||name_1_lang|Text|
|||name_2|Text|
|||name_2_lang|Text|
|||name_3|Text|
|||name_3_lang|Text|

#### WetlandS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|localType|LocalisedCharacterString|localType|Text|
|||localType_locale|Text|
|tidal|Boolean|tidal|Short|
|HydroIdentifier|HydroIdentifier|hyId_classificationScheme1|Text|
|||hyId_classificationScheme2|Text|
|||hyId_classificationScheme3|Text|
|||hyId_localId1|Text|
|||hyId_localId2|Text|
|||hyId_localId3|Text|
|||hyId_namespace1|Text|
|||hyId_namespace2|Text|
|||hyId_namespace3|Text|
|||name_1|Text|
|||name_1_lang|Text|
|||name_2|Text|
|||name_2_lang|Text|
|||name_3|Text|
|||name_3_lang|Text|
#### Tables

#### DrainageBasin_contains
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdDrainageBasin1|Long|
|||IdDrainageBasin2|Long|

#### DrainageBasin_HyObj
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdDrainageBasin|Long|
|relatedHydroObject||IdHyObj|Text|

#### HydroPOI_HyObj
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdHydroPOI|Long|
|relatedHydroObject||IdHyObj|Text|

#### ManMadeObj_HyObj
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdManMadeObj|Long|
|relatedHydroObject||IdHyObj|Text|

#### netCrossing_Element
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdNetworkElement1|Long|
|||IdNetworkElement2|Text|

#### netCrossReference_Elements
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdNetworkCrossReference|Long|
|||IdNetworkElement|Text|

#### netElement_HyObj
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdNetworkElement|Long|
|relatedHydroObject||IdHyObj|Text|

#### netElement_Link
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdNetworkElementLink|Long|
|||IdNetworkElement|Text|
|||direction|Text|

#### netElementL_HyObj
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdNetworkElement|Long|
|relatedHydroObject||IdHyObj|Text|

#### netElementP_HyObj
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdNetworkElement|Long|
|relatedHydroObject||IdHyObj|Text|

#### netLinkSet_Link
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdNetworkElement1|Long|
|||IdNetworkElement2|Text|

#### netNetwork_Elements
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdNetwork|Long|
|||IdNetworkElement|Text|

#### networkCrossReference
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|

#### networkElement
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|

#### networkNetwork
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|||typeOfTransport|Text|
|||type|Text|
|geographicalName|GeographicalName|name_1_lang|Text|
|||name_2|Text|
|||name_2_lang|Text|
|||name_3|Text|
|||name_3_lang|Text|

#### Shore_HyObj
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdShore|Long|
|relatedHydroObject||IdHyObj|Text|

#### SurfaceWater_bank
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdSurfaceWater|Long|
|||IdShore|Text|

#### SurfaceWater_HyObj
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdSurfaceWater|Long|
|relatedHydroObject||IdHyObj|Text|

#### SurfaceWater_neighbour
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdSurfaceWater1|Long|
|||IdSurfaceWater2|Long|

#### SurfaceWaterL_DrainageBasin
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdSurfaceWaterL|Long|
|||IdDrainageBasin|Long|

#### SurfaceWaterP_DrainageBasin
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdSurfaceWaterP|Long|
|||IdDrainageBasin|Long|

#### SurfaceWaterS_DrainageBasin
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdSurfaceWaterS|Long|
|||IdDrainageBasin|Long|

#### Wetland_HyObj
|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||IdWetland|Long|
|relatedHydroObject||IdHyObj|Text|