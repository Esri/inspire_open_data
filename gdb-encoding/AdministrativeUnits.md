# Geodatabase Encoding Rule for INSPIRE Administrative Units

`Version: 0.0`
`Date: 2021-02-22`

The Simple AdministrativeUnits encoding can be used as an *alternative encoding* for Administrative Units data that fulfills the following requirements:

* There are not more than three values for `nationalLevelName` in `AdministrtiveUnit`. 
* There are not more than three values for `name` in `AdministrtiveUnit`.  
* There is no Condominium in the Dataset.


## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](/gdb-encoding/geodatabse encoding.md)
* [Data Specification - INSPIRE Administrative Units version 3.1](https://inspire.ec.europa.eu/Themes/114/2892)

## Conformance Class Administrative Units

The Administrative Units theme has two application schema. This application schema-specific encoding rule defines a conformance class for the schema Administrative Units.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Administrative Units conceptual model before applying the general rules of this encoding rule:
 

1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`.
2. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
3. Substitute all occurences of `GeographicName` with the Simple Geographic Name through Rule `MT005(separator: '_')`.





#### AdministrativeBoundary

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|geometry|GM_Curve|geometry|Line|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|country|CountryCode|country|Text|
|nationalLevel|AdministrativeHierarchyLevel|nationalLevel_1|Text|
|||nationalLevel_2|Text|
|||nationalLevel_3|Text|
|||nationalLevel_4|Text|
|||nationalLevel_5|Text|
|||nationalLevel_6|Text|
|||nationalLevel_1_href|Text|
|||nationalLevel_2_href|Text|
|||nationalLevel_3_href|Text|
|||nationalLevel_4_href|Text|
|||nationalLevel_5_href|Text|
|||nationalLevel_6_href|Text|
|legalStatus|LegalStatusValue|legalStatus|Text|
|technicalStatus|TechnicalStatusValue|technicalStatus|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|

#### AdministrativeUnit

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|geometry|GM_MultiSurface|geometry|Polygon|
|nationalCode|CharacterString|nationalCode|Text|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|nationalLevel|AdministrativeHierarchyLevel|nationalLevel|Text|
|||nationalLevel_href|Text|
|nationalLevelName|LocalisedCharacterString|nationalLevelName_1|Text|
|||nationalLevelName_1_locale|Text|
|country|CountryCode|country|Text|
|name|GeographicalName|name_1_lang|Text|
|||name_1|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|upperLevelUnit|AdministrativeUnit|upperLevelUnit|Long|

#### AdministrativeUnit_residenceOfAuthority

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|name|GeographicalName|name_lang|Text|
|||name|Text|
|geometry|GM_Point|geometry|Point|

#### Relation_Unit_Boundary

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|boundary|AdministrativeBoundary|boundaryId|Long|
|admUnit|AdministrativeUnit|unitId|Long|
