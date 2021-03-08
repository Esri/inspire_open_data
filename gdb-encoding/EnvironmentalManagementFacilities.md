# Geodatabase Encoding Rule for INSPIRE Environmental Managemment Facilities

`Version: 0.2`
`Date: 2021-03-08`

The Simple EnvironmentalManagemmentFacility encoding can be used as an *alternative encoding* for Environmental Managemment Facilities data that fulfills the following requirements:

* It is sufficient to provide the `activity` for the `Function` in function. 
* It is sufficient to provide the `activity` for the `Capacity` in physicalCapacity.  
* There is no information on permittedCapacity for Permissions.


## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](/gdb-encoding/geodatabse encoding.md)
* [Data Specification - INSPIRE Utility and governmental services version 3.1](https://inspire.ec.europa.eu/Themes/136/2892)

## Conformance Class Environmental Managemment Facilities

The Utility and governmental services theme has 3 application schema. This application schema-specific encoding rule defines a conformance class for the schema Environmental Managemment Facilities.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Environmental Managemment Facilities conceptual model before applying the general rules of this encoding rule:
 

1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. (works in GDB)
2. Use Simplified Contact for all occurences `MT012()`. 
3. Use Simplified Related Party for all occurences `MT013()`. 
4. Create seperate Tables for each Geometry Type, add suffix for P for Points, L for Lines and S for Areas `MT014()`.
5. Create seperate Tables for the remaining one-to-many relationships `MT015()`.
6. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` (works in GDB as ong as not to long)
7. Apply Attribute shortening rules for EnvironmentalManagemmentFacility:

    |Replace|With|
    |----|----|
    |`facilityDescription_`|`'' `|
    |`relatedParty_`|`'related_' `|
    |`permittedFunction_`|`'permitted_' `|




ToDO: 
5. References to Objects by URL (String)





|||featureId|Long|

#### EnvironmentalManagementFacility

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|RelatedParty||related_individualName|Text|
|||related_organisationName|Text|
|||related_positionName|Text|
|||related_address|Text|
|||name|Text|
|||geometry||
|||related_contactInstructions|Text|
|||related_electronicMailAddress|Text|
|||related_hoursOfService|Text|
|||related_telephoneFacsimile|Text|
|||related_telephoneVoice|Text|
|DateTime|validFrom|validFrom|Date|
|DateTime|validTo|validTo|Date|
|DateTime|beginLifespanVersion|beginLifespanVersion|Date|
|DateTime|endLifespanVersion|endLifespanVersion|Date|
|||related_website|Text|
|||related_role|Text|
|ConditionOfFacilityValue||status|Text|
|||status_href|Text|
|PT_FreeText|serviceHours|serviceHours|Text|
|ActivityComplexDescription|facilityDescription|description|Text|
|AddressRepresentation||address|Text|
|AddressRepresentation||contact_address|Text|
|Contact||contact_contactInstructions|Text|
|||contact_electronicMailAddress|Text|
|||contact_hoursOfService|Text|
|||contact_telephoneFacsimile|Text|
|||contact_telephoneVoice|Text|
|||contact_website|Text|
|||activity_href|Text|
|||activity|Text|
|||description|Text|

#### EnvironmentalManagementFacility_capacity

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|

#### EnvironmentalManagementFacility_function

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||activity_href|Text|
|||RID|Long|
|||activity|Text|
|||description||

#### EnvironmentalManagementFacility_parentFacility

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|||parentFacility|Text|
|||permitted_activity|Text|
|||dateTo|Date|
|||related_organisationName|Text|
|||RID|Long|

#### EnvironmentalManagementFacility_permission

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||permissionId|Long|
|Permission|permission|thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
|RelatedParty||related_individualName|Text|
|||RID|Long|
|||related_positionName|Text|
|||related_address|Text|
|||related_contactInstructions|Text|
|||related_hoursOfService|Text|
|||related_telephoneFacsimile|Text|
|||related_telephoneVoice|Text|
|||related_website|Text|
|||related_role|Text|
|||relatedParty*|Text|
|||decisionDate|Date|
|||dateFrom|Date|
|||related_electronicMailAddress|Text|
|||description|Text|
|EconomicActivityValue||permitted_activity_href|Text|

#### EnvironmentalManagementFacility_thematicId

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|thematicId|ThematicIdentifier|thematicId_identifier|Text|
|||RID|Long|
|||thematicId_identifierScheme|Text|
|||type||

#### EnvironmentalManagementFacility_type

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|EnvironmentalManagementFacilityTypeValue|type|type_href|Text|
|||RID||
