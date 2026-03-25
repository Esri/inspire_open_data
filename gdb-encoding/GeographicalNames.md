# Geodatabase Encoding Rule for INSPIRE Geographical Names

`Version: 0.5`
`Date: 2021-05-31`

The Simple GeographicalNames encoding can be used as an *alternative encoding* for Geographical Names data that fulfills the following requirements:

* There is not more than three values for `name` in `NamedPlace`. 
* There is not more than one value for `spelling` in `GeographicalName`.
* There is not more than one value for `pronunciation` in `GeographicalName`.  
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
 

1. Substitute all attributes that have a property type with a Codelist Stereotype through an inline codelist reference using `MT008()`.
2. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
3. Limit the Multiplicity for name in GeographicalName to 3 through Rule `MT012(3)`
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
|name|GeographicalName|name1_language|Text|
|||name1_nativeness|Text|
|||name1_nativeness_href|Text|
|||name1_nameStatus|Text|
|||name1_nameStatus_href|Text|
|||name1_sourceOfName|Text|
|||name1_spelling_text|Text|
|||name1_spelling_script|Text|
|||name1_grammaticalGender|Text|
|||name1_grammaticalGender_href|Text|
|||name1_grammaticalNumber|Text|
|||name1_grammaticalNumber_href|Text|
|||name2_language|Text|
|||name2_nativeness|Text|
|||name2_nativeness_href|Text|
|||name2_nameStatus|Text|
|||name2_nameStatus_href|Text|
|||name2_sourceOfName|Text|
|||name2_spelling_text|Text|
|||name2_spelling_script|Text|
|||name2_grammaticalGender|Text|
|||name2_grammaticalGender_href|Text|
|||name2_grammaticalNumber|Text|
|||name2_grammaticalNumber_href|Text|
|||name3_language|Text|
|||name3_nativeness|Text|
|||name3_nativeness_href|Text|
|||name3_nameStatus|Text|
|||name3_nameStatus_href|Text|
|||name3_sourceOfName|Text|
|||name3_spelling_text|Text|
|||name3_spelling_script|Text|
|||name3_grammaticalGender|Text|
|||name3_grammaticalGender_href|Text|
|||name3_grammaticalNumber|Text|
|||name3_grammaticalNumber_href|Text|
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
|name|GeographicalName|name1_language|Text|
|||name1_nativeness|Text|
|||name1_nativeness_href|Text|
|||name1_nameStatus|Text|
|||name1_nameStatus_href|Text|
|||name1_sourceOfName|Text|
|||name1_spelling_text|Text|
|||name1_spelling_script|Text|
|||name1_grammaticalGender|Text|
|||name1_grammaticalGender_href|Text|
|||name1_grammaticalNumber|Text|
|||name1_grammaticalNumber_href|Text|
|||name2_language|Text|
|||name2_nativeness|Text|
|||name2_nativeness_href|Text|
|||name2_nameStatus|Text|
|||name2_nameStatus_href|Text|
|||name2_sourceOfName|Text|
|||name2_spelling_text|Text|
|||name2_spelling_script|Text|
|||name2_grammaticalGender|Text|
|||name2_grammaticalGender_href|Text|
|||name2_grammaticalNumber|Text|
|||name2_grammaticalNumber_href|Text|
|||name3_language|Text|
|||name3_nativeness|Text|
|||name3_nativeness_href|Text|
|||name3_nameStatus|Text|
|||name3_nameStatus_href|Text|
|||name3_sourceOfName|Text|
|||name3_spelling_text|Text|
|||name3_spelling_script|Text|
|||name3_grammaticalGender|Text|
|||name3_grammaticalGender_href|Text|
|||name3_grammaticalNumber|Text|
|||name3_grammaticalNumber_href|Text|
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
|name|GeographicalName|name1_language|Text|
|||name1_nativeness|Text|
|||name1_nativeness_href|Text|
|||name1_nameStatus|Text|
|||name1_nameStatus_href|Text|
|||name1_sourceOfName|Text|
|||name1_spelling_text|Text|
|||name1_spelling_script|Text|
|||name1_grammaticalGender|Text|
|||name1_grammaticalGender_href|Text|
|||name1_grammaticalNumber|Text|
|||name1_grammaticalNumber_href|Text|
|||name2_language|Text|
|||name2_nativeness|Text|
|||name2_nativeness_href|Text|
|||name2_nameStatus|Text|
|||name2_nameStatus_href|Text|
|||name2_sourceOfName|Text|
|||name2_spelling_text|Text|
|||name2_spelling_script|Text|
|||name2_grammaticalGender|Text|
|||name2_grammaticalGender_href|Text|
|||name2_grammaticalNumber|Text|
|||name2_grammaticalNumber_href|Text|
|||name3_language|Text|
|||name3_nativeness|Text|
|||name3_nativeness_href|Text|
|||name3_nameStatus|Text|
|||name3_nameStatus_href|Text|
|||name3_sourceOfName|Text|
|||name3_spelling_text|Text|
|||name3_spelling_script|Text|
|||name3_grammaticalGender|Text|
|||name3_grammaticalGender_href|Text|
|||name3_grammaticalNumber|Text|
|||name3_grammaticalNumber_href|Text|
|relatedSpatialObject|Identifier|relatedSpatialObject_localId|Text|
|||relatedSpatialObject_namespace|Text|
|||relatedSpatialObject_versionId|Text|
|type||type|Text|
|||type_href|Text|
