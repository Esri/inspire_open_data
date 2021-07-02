# Geodatabase Encoding Rule for INSPIRE AdministrativeAndSocialGovermentalServices

`Version: 0.5`
`Date: 2021-05-31`

The Simple AdministrativeAndSocialGovermentalServices encoding can be used as an *alternative encoding* for AdministrativeAndSocialGovermentalServices data that fulfills the following requirements:

* It is sufficient to provide the `AreaOfResponsibility` by Polygon. 
* It is sufficient to provide the `ServiceLocation` by Geometry.  
* There is only one `pointOfContact` per GovermentalService
* It is sufficient to provide one 'telephoneVoice' and one 'telephoneFax' for the 'Contact'



## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Utility and governmental services version 3.1](https://inspire.ec.europa.eu/Themes/136/2892)

## Conformance Class Administrative And SocialGovermental Services

The Utility and governmental services theme has 3 application schema. This application schema-specific encoding rule defines a conformance class for the schema Administrative And SocialGovermental Services.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Administrative And SocialGovermental Services conceptual model before applying the general rules of this encoding rule:
 

1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. 
2. Limit the Multiplicity for role in pointOfContact to 1 through Rule `MT012(1)` 
3. Limit the Multiplicity for telephoneVoice in Contact to 1 through Rule `MT012(1)`
4. Limit the Multiplicity for telephoneFax in Contact to 1 through Rule `MT012(1)`
5. Fan-out GM_Object to seperate Tables for Point, Lines and Areas through Rule `MT016(1)`
6. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
7. Apply Attribute shortening rule for AdministrativeAndSocialGovermentalServices:

    |Replace|With|
    |----|----|
    |`'pointOfContact_'`|`'contact_' `|
    



#### GovernmentalServiceL

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion||beginLifespanVersion|Text|
|endLifespanVersion||endLifespanVersion|Text|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|pointOfContact|Contact|contact_address|Text|
|||contact_contactInstructions|Text|
|||contact_electronicMailAddress|Text|
|||contact_hoursOfService|Text|
|||contact_telephoneFacsimile|Text|
|||contact_telephoneVoice|Text|
|||contact_website|Text|
|serviceType|ServiceTypeValue|serviceType|Text|
|||serviceType_href|Text|

#### GovernmentalServiceP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion||beginLifespanVersion|Text|
|endLifespanVersion||endLifespanVersion|Text|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|pointOfContact|Contact|contact_address|Text|
|||contact_contactInstructions|Text|
|||contact_electronicMailAddress|Text|
|||contact_hoursOfService|Text|
|||contact_telephoneFacsimile|Text|
|||contact_telephoneVoice|Text|
|||contact_website|Text|
|serviceType|ServiceTypeValue|serviceType|Text|
|||serviceType_href|Text|

#### GovernmentalServiceS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion||beginLifespanVersion|Text|
|endLifespanVersion||endLifespanVersion|Text|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|pointOfContact|Contact|contact_address|Text|
|||contact_contactInstructions|Text|
|||contact_electronicMailAddress|Text|
|||contact_hoursOfService|Text|
|||contact_telephoneFacsimile|Text|
|||contact_telephoneVoice|Text|
|||contact_website|Text|
|serviceType|ServiceTypeValue|serviceType|Text|
|||serviceType_href|Text|

#### GovernmentalService_areaOfResponsibility

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
