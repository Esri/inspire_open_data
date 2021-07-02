# Geodatabase Encoding Rule for INSPIRE Environmental Managemment Facilities

`Version: 0.5`
`Date: 2021-05-31`

The Simple EnvironmentalManagemmentFacility encoding can be used as an *alternative encoding* for Environmental Managemment Facilities data that fulfills the following requirements:

* It is sufficient to provide the `activity` for the `Function` in function. 
* It is sufficient to provide the `activity` for the `Capacity` in physicalCapacity.  
* There is no information on permittedCapacity for Permissions.
* There is not more than one thematicId per EnvironmentalManagemmentFacility

## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Utility and governmental services version 3.1](https://inspire.ec.europa.eu/Themes/136/2892)

## Conformance Class Environmental Managemment Facilities

The Utility and governmental services theme has 3 application schema. This application schema-specific encoding rule defines a conformance class for the schema Environmental Managemment Facilities.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Environmental Managemment Facilities conceptual model before applying the general rules of this encoding rule:
 

1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. (works in GDB)
2. Apply MT011 on capacity, permission and parentFacility.
3. Limit the Multiplicity for type in EnvironmentalManagemmentFacility to 3 through Rule `MT012(3)`
4. Limit the Multiplicity for telephoneVoice in Contact to 1 through Rule `MT012(1)`
5. Limit the Multiplicity for telephoneFax in Contact to 1 through Rule `MT012(1)`
6. Limit the Multiplicity for role in RelatedParty to 1 through Rule `MT012(1)`
7. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
8. Apply Attribute shortening rules for EnvironmentalManagemmentFacility:

    |Replace|With|
    |----|----|
    |`'facilityDescription_'`|`'' `|
    |`'relatedParty_'`|`'related_' `|
    |`'permittedFunction_'`|`'permitted_' `|







#### EnvironmentalManagementFacilityL

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
||id|featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|thematicId|ThematicIdentifier|thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
|||name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|type|EnvironmentalManagementFacilityTypeValue|type_1|Text|
|||type_1_href|Text|
|||type_2|Text|
|||type_2_href|Text|
|serviceHours|PT_FreeText|serviceHours|Text|
|facilityDescription|ActivityComplexDescription|description|Text|
||AddressRepresentation|address|Text|
||AddressRepresentation|contact_address|Text|
||Contact|contact_contactInstructions|Text|
|||contact_electronicMailAddress|Text|
|||contact_hoursOfService|Text|
|||contact_telephoneFacsimile|Text|
|||contact_telephoneVoice|Text|
|||contact_website|Text|
||RelatedParty|related_individualName|Text|
|||related_organisationName|Text|
|||related_positionName|Text|
|||related_address|Text|
|||related_contactInstructions|Text|
|||related_electronicMailAddress|Text|
|||related_hoursOfService|Text|
|||related_telephoneFacsimile|Text|
|||related_telephoneVoice|Text|
|||related_website|Text|
|||related_role|Text|
||ConditionOfFacilityValue|status|Text|
|||status_href|Text|

#### EnvironmentalManagementFacilityP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
||id|featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|thematicId|ThematicIdentifier|thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
|||name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|type|EnvironmentalManagementFacilityTypeValue|type_1|Text|
|||type_1_href|Text|
|||type_2|Text|
|||type_2_href|Text|
|serviceHours|PT_FreeText|serviceHours|Text|
|facilityDescription|ActivityComplexDescription|description|Text|
||AddressRepresentation|address|Text|
||AddressRepresentation|contact_address|Text|
||Contact|contact_contactInstructions|Text|
|||contact_electronicMailAddress|Text|
|||contact_hoursOfService|Text|
|||contact_telephoneFacsimile|Text|
|||contact_telephoneVoice|Text|
|||contact_website|Text|
||RelatedParty|related_individualName|Text|
|||related_organisationName|Text|
|||related_positionName|Text|
|||related_address|Text|
|||related_contactInstructions|Text|
|||related_electronicMailAddress|Text|
|||related_hoursOfService|Text|
|||related_telephoneFacsimile|Text|
|||related_telephoneVoice|Text|
|||related_website|Text|
|||related_role|Text|
||ConditionOfFacilityValue|status|Text|
|||status_href|Text|

#### EnvironmentalManagementFacilityS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
||id|featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|thematicId|ThematicIdentifier|thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
|||name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|type|EnvironmentalManagementFacilityTypeValue|type_1|Text|
|||type_1_href|Text|
|||type_2|Text|
|||type_2_href|Text|
|serviceHours|PT_FreeText|serviceHours|Text|
|facilityDescription|ActivityComplexDescription|description|Text|
||AddressRepresentation|address|Text|
||AddressRepresentation|contact_address|Text|
||Contact|contact_contactInstructions|Text|
|||contact_electronicMailAddress|Text|
|||contact_hoursOfService|Text|
|||contact_telephoneFacsimile|Text|
|||contact_telephoneVoice|Text|
|||contact_website|Text|
||RelatedParty|related_individualName|Text|
|||related_organisationName|Text|
|||related_positionName|Text|
|||related_address|Text|
|||related_contactInstructions|Text|
|||related_electronicMailAddress|Text|
|||related_hoursOfService|Text|
|||related_telephoneFacsimile|Text|
|||related_telephoneVoice|Text|
|||related_website|Text|
|||related_role|Text|
||ConditionOfFacilityValue|status|Text|
|||status_href|Text|

#### EnvironmentalManagementFacility_capacity

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|||activity|Text|
|||activity_href|Text|
|||description|Text|

#### EnvironmentalManagementFacility_function

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|||activity|Text|
|||activity_href|Text|
||Text|description|Text|

#### EnvironmentalManagementFacility_parentFacility

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|||parentFacility|Text|

#### EnvironmentalManagementFacility_permission

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|||permissionId|Long|
|permission|Permission|thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
||RelatedParty|related_individualName|Text|
|||related_organisationName|Text|
|||related_positionName|Text|
|||related_address|Text|
|||related_contactInstructions|Text|
|||related_electronicMailAddress|Text|
|||related_hoursOfService|Text|
|||related_telephoneFacsimile|Text|
|||related_telephoneVoice|Text|
|||related_website|Text|
|||related_role|Text|
|||decisionDate|Date|
|||dateFrom|Date|
|||dateTo|Date|
|||description|Text|
||EconomicActivityValue|permitted_activity|Text|
|||permitted_activity_href|Text|
