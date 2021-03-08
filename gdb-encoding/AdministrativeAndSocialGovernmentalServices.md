# Geodatabase Encoding Rule for INSPIRE AdministrativeAndSocialGovermentalServices

`Version: 0.2`
`Date: 2021-03-06`

The Simple AdministrativeAndSocialGovermentalServices encoding can be used as an *alternative encoding* for AdministrativeAndSocialGovermentalServices data that fulfills the following requirements:

* It is sufficient to provide the `AreaOfResponsibility` by Polygon. 
* It is sufficient to provide the `ServiceLocation` by Geometry.  
* There is only one `pointOfContact` per GovermentalService



## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](/gdb-encoding/geodatabse encoding.md)
* [Data Specification - INSPIRE Utility and governmental services version 3.1](https://inspire.ec.europa.eu/Themes/136/2892)

## Conformance Class Administrative And SocialGovermental Services

The Utility and governmental services theme has 3 application schema. This application schema-specific encoding rule defines a conformance class for the schema Administrative And SocialGovermental Services.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Administrative And SocialGovermental Services conceptual model before applying the general rules of this encoding rule:
 

1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. (works in GDB)
2. Use Simplified Contact for all occurences `MT012()`. 
2. Use Simplified Related Party for all occurences `MT013()`. 
3. Create seperate Tables for each Geometry Type, add suffix for P for Points, L for Lines and S for Areas `MT014()`.
4. Create seperate Tables for the remaining one-to-many relationships `MT015()`.
5. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` (works in GDB as ong as not to long)
6. Apply Attribute shortening rule for AdministrativeAndSocialGovermentalServices:

    |Replace|With|
    |----|----|
    |`pointOfContact_`|`'contact_' `|
    






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
|serviceLocation|ServiceLocationType|serviceLocation_serviceLocationByGeometry|Geometry|
|serviceType|ServiceTypeValue|serviceType_href|Text|

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
|serviceLocation|ServiceLocationType|serviceLocation_serviceLocationByGeometry|Geometry|
|serviceType|ServiceTypeValue|serviceType_href|Text|

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
|serviceLocation|ServiceLocationType|serviceLocation_serviceLocationByGeometry|Geometry|
|serviceType|ServiceTypeValue|serviceType_href|Text|

#### GovernmentalService_areaOfResponsibility

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|areaOfResponsibility|AreaOfResponsibilityType|areaOfResponsibility|Geometry|
|||RID|Long|
