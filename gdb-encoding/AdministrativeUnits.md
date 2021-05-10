# Geodatabase Encoding Rule for INSPIRE Administrative Units

`Version: 0.0`
`Date: 2021-02-22`

The Simple AdministrativeUnits encoding can be used as an *alternative encoding* for Administrative Units data that fulfills the following requirements:

* It is sufficient to provide the `activity` for the `Function` in function. 
* It is sufficient to provide the `activity` for the `Capacity` in physicalCapacity.  
* There is no information on permittedCapacity for Permissions.


## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](/gdb-encoding/geodatabse encoding.md)
* [Data Specification - INSPIRE Administrative Units version 3.1](https://inspire.ec.europa.eu/Themes/114/2892)

## Conformance Class Administrative Units

The Administrative Units theme has two application schema. thie application schema-specific encoding rule defines a conformance class for the schema Administrative Units.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Administrative Units conceptual model before applying the general rules of this encoding rule:
 

1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. (works in GDB)
2. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` (works in GDB as ong as not to long)
4. Create seperate Tables for each Geometry Type, add suffix for P for Points, L for Lines and S for Areas.
5. References to Objects by URL (String)


ToDO: 
SimpleRelatedParty beschreiben, Multiplizität bei RelatedParty erlauben
Contact in einzelne Attribute zerlegen.




#### AdministrativeBoundary

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId||
|||geometry||
|||inspireId_localId||
|||inspireId_namespace||
|||inspireId_versionId||
|||country||
|||legalStatus||
|||technicalStatus||
|||beginLifespanVersion||
|||endLifespanVersion||

#### AdministrativeBoundary_nationalLevel

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID||
|||nationalLevel||
|||nationalLevel_href||

#### AdministrativeUnit

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId||
|||geometry||
|||nationalCode||
|||inspireId_localId||
|||inspireId_namespace||
|||inspireId_versionId||
|||nationalLevel_href||
|||country||
|||beginLifespanVersion||
|||endLifespanVersion||
|||upperLevelUnit||

#### AdministrativeUnit_name

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID||
|||name_lang||
|||name||

#### AdministrativeUnit_nationalLevelName

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID||
|||nationalLevelName||

#### AdministrativeUnit_residenceOfAuthority

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID||
|||name_lang||
|||name||
|||geometry||

#### Relation_Unit_Boundary

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||boundaryId||
|||unitId||
