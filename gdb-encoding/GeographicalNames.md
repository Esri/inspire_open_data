# Geodatabase Encoding Rule for INSPIRE Geographical Names

`Version: 0.5`
`Date: 2021-05-31`

The Simple GeographicalNames encoding can be used as an *alternative encoding* for Geographical Names data that fulfills the following requirements:

* There is not more than one value for `spelling` in `GeographicalName`. 
* There is not more than one value for `type` in `NamedPlace`. 
* There is not more than one value for `localType` in `NamedPlace`. 
* There is not more than one value for `relatedSpatialObject` in `NamedPlace`. 
*

## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Geographical Names version 3.1](https://inspire.ec.europa.eu/Themes/132/2892)

## Conformance Class Geographical Names

The Geographical Names theme has one application schema. This application schema-specific encoding rule defines a conformance class for the schema Geographical Names.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Geographical Names conceptual model before applying the general rules of this encoding rule:
 

1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`.
2. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
4. Limit the Multiplicity for spelling in GeographicalName to 1 through Rule `MT012(1)`
5. Limit the Multiplicity for type in NamedPlace to 1 through Rule `MT012(1)`
6. Limit the Multiplicity for localType in NamedPlace to 1 through Rule `MT012(1)`
7. Limit the Multiplicity for relatedSpatialObject in NamedPlace to 1 through Rule `MT012(1)`
8. Apply MT011 on `name` for `NamedPlace`.





#### NamedPlaceL

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Text|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|leastDetailedViewingResolution|MD_Resolution|leastDetailedViewingResolution|Long|
|||localType|Text|
|||localType_locale|Text|
|mostDetailedViewingResolution|MD_Resolution|mostDetailedViewingResolution|Long|
|relatedSpatialObject|Identifier|relatedSpatialObject_localId|Text|
|||relatedSpatialObject_namespace|Text|
|||relatedSpatialObject_versionId|Text|
|type||type|Text|
|||type_href|Text|

#### NamedPlaceP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Text|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|leastDetailedViewingResolution|MD_Resolution|leastDetailedViewingResolution|Long|
|||localType|Text|
|||localType_locale|Text|
|mostDetailedViewingResolution|MD_Resolution|mostDetailedViewingResolution|Long|
|relatedSpatialObject|Identifier|relatedSpatialObject_localId|Text|
|||relatedSpatialObject_namespace|Text|
|||relatedSpatialObject_versionId|Text|
|type||type|Text|
|||type_href|Text|

#### NamedPlaceS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Text|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|leastDetailedViewingResolution|MD_Resolution|leastDetailedViewingResolution|Long|
|||localType|Text|
|||localType_locale|Text|
|mostDetailedViewingResolution|MD_Resolution|mostDetailedViewingResolution|Long|
|relatedSpatialObject|Identifier|relatedSpatialObject_localId|Text|
|||relatedSpatialObject_namespace|Text|
|||relatedSpatialObject_versionId|Text|
|type||type|Text|
|||type_href|Text|

#### NamedPlace_name

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|name|GeographicalName|RID|Long|
|||language|Text|
|||nativeness|Text|
|||nativeness_href|Text|
|||nameStatus|Text|
|||nameStatus_href|Text|
|||sourceOfName|Text|
|||pronunciationSoundLink|Text|
|||pronunciationIPA|Text|
|||spelling_text|Text|
|||spelling_script|Text|
|||spelling_transliterationScheme|Text|
|||grammaticalGender|Text|
|||grammaticalGender_href|Text|
|||grammaticalNumber|Text|
|||grammaticalNumber_href|Text|
