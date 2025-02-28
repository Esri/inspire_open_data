# Geodatabase Encoding Rule for INSPIRE Environmental Monitoring Facilities

`Version: 1.0`
`Date: 2025-02-28`

The Simple Environmental Monitoring Facilities encoding can be used as an *alternative encoding* for Environmental Monitoring Facilities data that fulfills the following requirements:

* There is not more than 3 `mediaMonitored` for `AbstractMonitoringObject`
* There is not more than 1 `onlineResource` for `AbstractMonitoringObject`
* There is not more than 1 `legalBackground` for `AbstractMonitoringObject`
* There is not more than 1 `responsibleParty` for `AbstractMonitoringObject`
* There is not more than 1 `thematicId` for `AbstractMonitoringObject`
* There is not more than 1 `name` for `AbstractMonitoringObject`
* There is not more than 2 `purpose` for `AbstractMonitoringObject`
* There is no hierarchy and no genealogy for `AbstractMonitoringObject`
* There is no `observingCapability` for `AbstractMonitoringObject`
* There is not more than 1 `reportedTo` for `AbstractMonitoringFeature`
* There is not more than 1 `onlineResource` for `AbstractMonitoringActivity`
* There is not more than 1 `resultAcquisitionSource` for `EnvironmentalMonitoringFacility`
* There is not more than 1 `operationalActivityPeriod` for `EnvironmentalMonitoringFacility`
* There is not more than 1 `setUpFor` for `EnvironmentalMonitoringProgramme`
* There is no `hasObservation` for `AbstractMonitoringFeature`


## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Environmental Monitoring Facilities version 3.2.0](https://github.com/INSPIRE-MIF/technical-guidelines/tree/main/data/ef)

## Conformance Class Core

The Environmental Monitoring Facilities theme has one application schema, therefore this theme-specific encoding rule defines a single core conformance class.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Environmental Monitoring Facilities conceptual model before applying the general rules of this encoding rule:
 
1. Substitute all attributes that have a property type with a Codelist Stereotype through an inline codelist reference using `MT008()`. 
2. Apply the SimpleCitation rule `MT007()`.
3. Apply the SimplePeriod rule `MT009()`.
4. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
5. Apply the High Cardinality Properties to Extra Tables rule to `EnvironmentalMonitoringProgramme`, `EnvironmentalMonitoringFacility` and `EnvironmentalMonitoringNetwork`: `MT011()`. 
6. Apply Attribute shortening rule for EnvironmentalMonitoringNetwork:

    |Replace|With|
    |----|----|
    |`'responsibleParty_'`|`'resParty_' `|
    |`'reportedTo_legalAct_'`|`'legalAct_' `|
    |`'operationalActivityPeriod_'`|`'opActPeriod_' `|

7. Apply Attribute shortening rule for EnvironmentalMonitoringProgramme:

    |Replace|With|
    |----|----|
    |`'responsibleParty_'`|`'resParty_' `|
    

8. Apply Attribute shortening rule for EnvironmentalMonitoringFacility:

    |Replace|With|
    |----|----|
    |`'responsibleParty_'`|`'resParty_' `|
    
    

    


#### EnvironmentalMonitoringActivity

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|responsibleParty|RelatedParty|resParty_individualName|Text|
|||resParty_organisationName|Text|
|||resParty_positionName|Text|
|||resParty_address|Text|
|||resParty_contactInstructions|Text|
|||resParty_electronicMailAddress|Text|
|||resParty_hoursOfService|Text|
|||resParty_telephoneFacsimile|Text|
|||resParty_telephoneVoice|Text|
|||resParty_website|Text|
|||resParty_role|Text|
||Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|onlineResource|URL|onlineResource|Text|
|setUpFor|EnvironmentalMonitoringProgramme|setUpFor|Long|

#### EnvironmentalMonitoringActivity_uses

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|||uses|Long|

#### EnvironmentalMonitoringFacilityL

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|thematicId|ThematicIdentifier |thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
|name|CharacterString|name|Text|
|additionalDescription|CharacterString|additionalDescription|Text|
|mediaMonitored|MediaValue|mediaMonitored_1_href|Text|
|||mediaMonitored_1|Text|
||MediaValue|mediaMonitored_2_href|Text|
|||mediaMonitored_2|Text|
||MediaValue|mediaMonitored_3_href|Text|
|||mediaMonitored_3|Text|
||LegislationCitation|legalBackground_citationDate|Date|
|||legalBackground_citationLink|Text|
|||legalBackground_citationName|Text|
|||legalBackground_citationLevel|Text|
|||legalBackground_citationType|Text|
|responsibleParty|RelatedParty|resParty_individualName|Text|
|||resParty_organisationName|Text|
|||resParty_positionName|Text|
|||resParty_address|Text|
|||resParty_contactInstructions|Text|
|||resParty_electronicMailAddress|Text|
|||resParty_hoursOfService|Text|
|||resParty_telephoneFacsimile|Text|
|||resParty_telephoneVoice|Text|
|||resParty_website|Text|
|||resParty_role|Text|
|||onlineResource|Text|
|purpose|PurposeOfCollectionValue|purpose_1_href|Text|
|||purpose_1|Text|
||PurposeOfCollectionValue|purpose_2_href|Text|
|||purpose_2|Text|
||LegislationCitation|legalBackground_citationDate|Date|
|||legalBackground_citationLink|Text|
|||legalBackground_citationName|Text|
|||legalBackground_citationLevel|Text|
|||legalBackground_citationType|Text|
|measurementRegime|MeasurementRegimeValue|measurementRegime_href|Text|
|||measurementRegime|Text|
|||mobile|Short|
|resultAcquisitionSource|ResultAcquisitionSourceValue|resultAcquisitionSource_href|Text|
|||resultAcquisitionSource|Text|
|specialisedEMFType|SpecialisedEMFTypeValue|specialisedEMFType_href|Text|
|||specialisedEMFType|Text|

#### EnvironmentalMonitoringFacilityP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|thematicId|ThematicIdentifier |thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
|name|CharacterString|name|Text|
|additionalDescription|CharacterString|additionalDescription|Text|
|mediaMonitored|MediaValue|mediaMonitored_1_href|Text|
|||mediaMonitored_1|Text|
||MediaValue|mediaMonitored_2_href|Text|
|||mediaMonitored_2|Text|
||MediaValue|mediaMonitored_3_href|Text|
|||mediaMonitored_3|Text|
||LegislationCitation|legalBackground_citationDate|Date|
|||legalBackground_citationLink|Text|
|||legalBackground_citationName|Text|
|||legalBackground_citationLevel|Text|
|||legalBackground_citationType|Text|
|responsibleParty|RelatedParty|resParty_individualName|Text|
|||resParty_organisationName|Text|
|||resParty_positionName|Text|
|||resParty_address|Text|
|||resParty_contactInstructions|Text|
|||resParty_electronicMailAddress|Text|
|||resParty_hoursOfService|Text|
|||resParty_telephoneFacsimile|Text|
|||resParty_telephoneVoice|Text|
|||resParty_website|Text|
|||resParty_role|Text|
|||onlineResource|Text|
|purpose|PurposeOfCollectionValue|purpose_1_href|Text|
|||purpose_1|Text|
||PurposeOfCollectionValue|purpose_2_href|Text|
|||purpose_2|Text|
||LegislationCitation|legalBackground_citationDate|Date|
|||legalBackground_citationLink|Text|
|||legalBackground_citationName|Text|
|||legalBackground_citationLevel|Text|
|||legalBackground_citationType|Text|
|measurementRegime|MeasurementRegimeValue|measurementRegime_href|Text|
|||measurementRegime|Text|
|||mobile|Short|
|resultAcquisitionSource|ResultAcquisitionSourceValue|resultAcquisitionSource_href|Text|
|||resultAcquisitionSource|Text|
|specialisedEMFType|SpecialisedEMFTypeValue|specialisedEMFType_href|Text|
|||specialisedEMFType|Text|

#### EnvironmentalMonitoringFacilityS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|thematicId|ThematicIdentifier |thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
|name|CharacterString|name|Text|
|additionalDescription|CharacterString|additionalDescription|Text|
|mediaMonitored|MediaValue|mediaMonitored_1_href|Text|
|||mediaMonitored_1|Text|
||MediaValue|mediaMonitored_2_href|Text|
|||mediaMonitored_2|Text|
||MediaValue|mediaMonitored_3_href|Text|
|||mediaMonitored_3|Text|
||LegislationCitation|legalBackground_citationDate|Date|
|||legalBackground_citationLink|Text|
|||legalBackground_citationName|Text|
|||legalBackground_citationLevel|Text|
|||legalBackground_citationType|Text|
|responsibleParty|RelatedParty|resParty_individualName|Text|
|||resParty_organisationName|Text|
|||resParty_positionName|Text|
|||resParty_address|Text|
|||resParty_contactInstructions|Text|
|||resParty_electronicMailAddress|Text|
|||resParty_hoursOfService|Text|
|||resParty_telephoneFacsimile|Text|
|||resParty_telephoneVoice|Text|
|||resParty_website|Text|
|||resParty_role|Text|
|||onlineResource|Text|
|purpose|PurposeOfCollectionValue|purpose_1_href|Text|
|||purpose_1|Text|
||PurposeOfCollectionValue|purpose_2_href|Text|
|||purpose_2|Text|
||LegislationCitation|legalBackground_citationDate|Date|
|||legalBackground_citationLink|Text|
|||legalBackground_citationName|Text|
|||legalBackground_citationLevel|Text|
|||legalBackground_citationType|Text|
|measurementRegime|MeasurementRegimeValue|measurementRegime_href|Text|
|||measurementRegime|Text|
|||mobile|Short|
|resultAcquisitionSource|ResultAcquisitionSourceValue|resultAcquisitionSource_href|Text|
|||resultAcquisitionSource|Text|
|specialisedEMFType|SpecialisedEMFTypeValue|specialisedEMFType_href|Text|
|||specialisedEMFType|Text|

#### EnvironmentalMonitoringFacility_belongsTo

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|belongsTo|EnvironmentalMonitoringNetwork|RID|Long|
|||belongsTo|Long|

#### EnvironmentalMonitoringFacility_involvedIn

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|involvedIn|EnvironmentalMonitoringActivity|RID|Long|
|||involvedIn|Long|

#### EnvironmentalMonitoringNetworkL

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|thematicId|ThematicIdentifier |thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
|name|CharacterString|name|Text|
|additionalDescription|CharacterString|additionalDescription|Text|
|mediaMonitored|MediaValue|mediaMonitored_1_href|Text|
||MediaValue|mediaMonitored_1|Text|
||MediaValue|mediaMonitored_2_href|Text|
||MediaValue|mediaMonitored_2|Text|
||MediaValue|mediaMonitored_3_href|Text|
||MediaValue|mediaMonitored_3|Text|
|legalBackground|LegislationCitation|legalBackground_citationDate|Date|
|||legalBackground_citationLink|Text|
|||legalBackground_citationName|Text|
|||legalBackground_citationLevel|Text|
|||legalBackground_citationType|Text|
|responsibleParty|RelatedParty|resParty_individualName|Text|
|||resParty_organisationName|Text|
|||resParty_positionName|Text|
|||resParty_address|Text|
|||resParty_contactInstructions|Text|
|||resParty_electronicMailAddress|Text|
|||resParty_hoursOfService|Text|
|||resParty_telephoneFacsimile|Text|
|||resParty_telephoneVoice|Text|
|||resParty_website|Text|
|||resParty_role|Text|
|onlineResource|URL|onlineResource|Text|
|purpose|PurposeOfCollectionValue|purpose_1_href|Text|
|||purpose_1|Text|
||PurposeOfCollectionValue|purpose_2_href|Text|
|||purpose_2|Text|
||CI_Citation|legalAct_citationDate|Date|
|||legalAct_citationLink|Text|
|||legalAct_citationName|Text|
|||legalAct_citationLevel|Text|
|||legalAct_citationType|Text|
|organisationLevel|LegislationLevelValue|organisationLevel_href|Text|
|||organisationLevel|Text|

#### EnvironmentalMonitoringNetworkP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|thematicId|ThematicIdentifier |thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
|name|CharacterString|name|Text|
|additionalDescription|CharacterString|additionalDescription|Text|
|mediaMonitored|MediaValue|mediaMonitored_1_href|Text|
||MediaValue|mediaMonitored_1|Text|
||MediaValue|mediaMonitored_2_href|Text|
||MediaValue|mediaMonitored_2|Text|
||MediaValue|mediaMonitored_3_href|Text|
||MediaValue|mediaMonitored_3|Text|
|legalBackground|LegislationCitation|legalBackground_citationDate|Date|
|||legalBackground_citationLink|Text|
|||legalBackground_citationName|Text|
|||legalBackground_citationLevel|Text|
|||legalBackground_citationType|Text|
|responsibleParty|RelatedParty|resParty_individualName|Text|
|||resParty_organisationName|Text|
|||resParty_positionName|Text|
|||resParty_address|Text|
|||resParty_contactInstructions|Text|
|||resParty_electronicMailAddress|Text|
|||resParty_hoursOfService|Text|
|||resParty_telephoneFacsimile|Text|
|||resParty_telephoneVoice|Text|
|||resParty_website|Text|
|||resParty_role|Text|
|onlineResource|URL|onlineResource|Text|
|purpose|PurposeOfCollectionValue|purpose_1_href|Text|
|||purpose_1|Text|
||PurposeOfCollectionValue|purpose_2_href|Text|
|||purpose_2|Text|
||CI_Citation|legalAct_citationDate|Date|
|||legalAct_citationLink|Text|
|||legalAct_citationName|Text|
|||legalAct_citationLevel|Text|
|||legalAct_citationType|Text|
|organisationLevel|LegislationLevelValue|organisationLevel_href|Text|
|||organisationLevel|Text|

#### EnvironmentalMonitoringNetworkS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|thematicId|ThematicIdentifier |thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
|name|CharacterString|name|Text|
|additionalDescription|CharacterString|additionalDescription|Text|
|mediaMonitored|MediaValue|mediaMonitored_1_href|Text|
||MediaValue|mediaMonitored_1|Text|
||MediaValue|mediaMonitored_2_href|Text|
||MediaValue|mediaMonitored_2|Text|
||MediaValue|mediaMonitored_3_href|Text|
||MediaValue|mediaMonitored_3|Text|
|legalBackground|LegislationCitation|legalBackground_citationDate|Date|
|||legalBackground_citationLink|Text|
|||legalBackground_citationName|Text|
|||legalBackground_citationLevel|Text|
|||legalBackground_citationType|Text|
|responsibleParty|RelatedParty|resParty_individualName|Text|
|||resParty_organisationName|Text|
|||resParty_positionName|Text|
|||resParty_address|Text|
|||resParty_contactInstructions|Text|
|||resParty_electronicMailAddress|Text|
|||resParty_hoursOfService|Text|
|||resParty_telephoneFacsimile|Text|
|||resParty_telephoneVoice|Text|
|||resParty_website|Text|
|||resParty_role|Text|
|onlineResource|URL|onlineResource|Text|
|purpose|PurposeOfCollectionValue|purpose_1_href|Text|
|||purpose_1|Text|
||PurposeOfCollectionValue|purpose_2_href|Text|
|||purpose_2|Text|
||CI_Citation|legalAct_citationDate|Date|
|||legalAct_citationLink|Text|
|||legalAct_citationName|Text|
|||legalAct_citationLevel|Text|
|||legalAct_citationType|Text|
|organisationLevel|LegislationLevelValue|organisationLevel_href|Text|
|||organisationLevel|Text|

#### EnvironmentalMonitoringNetwork_contains

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|contains|EnvironmentalMonitoringFacility|RID|Long|
|||contains|Long|

#### EnvironmentalMonitoringNetwork_involvedIn

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
||EnvironmentalMonitoringActivity|RID|Long|
|||involvedIn|Long|

#### EnvironmentalMonitoringProgrammeL

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
||ThematicIdentifier |thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
||CharacterString|name|Text|
||CharacterString|additionalDescription|Text|
|mediaMonitored|MediaValue|mediaMonitored_1_href|Text|
|||mediaMonitored_1|Text|
||MediaValue|mediaMonitored_2_href|Text|
|||mediaMonitored_2|Text|
||MediaValue|mediaMonitored_3_href|Text|
|||mediaMonitored_3|Text|
|legalBackground|LegislationCitation|legalBackground_citationDate|Date|
|||legalBackground_citationLink|Text|
|||legalBackground_citationName|Text|
|||legalBackground_citationLevel|Text|
|||legalBackground_citationType|Text|
|responsibleParty|RelatedParty|resParty_individualName|Text|
|||resParty_organisationName|Text|
|||resParty_positionName|Text|
|||resParty_address|Text|
|||resParty_contactInstructions|Text|
|||resParty_electronicMailAddress|Text|
|||resParty_hoursOfService|Text|
|||resParty_telephoneFacsimile|Text|
|||resParty_telephoneVoice|Text|
|||resParty_website|Text|
|||resParty_role|Text|
|onlineResource|URL|onlineResource|Text|
|purpose|PurposeOfCollectionValue|purpose_1_href|Text|
|||purpose_1|Text|
||PurposeOfCollectionValue|purpose_2_href|Text|
|||purpose_2|Text|

#### EnvironmentalMonitoringProgrammeP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
||ThematicIdentifier |thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
||CharacterString|name|Text|
||CharacterString|additionalDescription|Text|
|mediaMonitored|MediaValue|mediaMonitored_1_href|Text|
|||mediaMonitored_1|Text|
||MediaValue|mediaMonitored_2_href|Text|
|||mediaMonitored_2|Text|
||MediaValue|mediaMonitored_3_href|Text|
|||mediaMonitored_3|Text|
|legalBackground|LegislationCitation|legalBackground_citationDate|Date|
|||legalBackground_citationLink|Text|
|||legalBackground_citationName|Text|
|||legalBackground_citationLevel|Text|
|||legalBackground_citationType|Text|
|responsibleParty|RelatedParty|resParty_individualName|Text|
|||resParty_organisationName|Text|
|||resParty_positionName|Text|
|||resParty_address|Text|
|||resParty_contactInstructions|Text|
|||resParty_electronicMailAddress|Text|
|||resParty_hoursOfService|Text|
|||resParty_telephoneFacsimile|Text|
|||resParty_telephoneVoice|Text|
|||resParty_website|Text|
|||resParty_role|Text|
|onlineResource|URL|onlineResource|Text|
|purpose|PurposeOfCollectionValue|purpose_1_href|Text|
|||purpose_1|Text|
||PurposeOfCollectionValue|purpose_2_href|Text|
|||purpose_2|Text|

#### EnvironmentalMonitoringProgrammeS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
||ThematicIdentifier |thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
||CharacterString|name|Text|
||CharacterString|additionalDescription|Text|
|mediaMonitored|MediaValue|mediaMonitored_1_href|Text|
|||mediaMonitored_1|Text|
||MediaValue|mediaMonitored_2_href|Text|
|||mediaMonitored_2|Text|
||MediaValue|mediaMonitored_3_href|Text|
|||mediaMonitored_3|Text|
|legalBackground|LegislationCitation|legalBackground_citationDate|Date|
|||legalBackground_citationLink|Text|
|||legalBackground_citationName|Text|
|||legalBackground_citationLevel|Text|
|||legalBackground_citationType|Text|
|responsibleParty|RelatedParty|resParty_individualName|Text|
|||resParty_organisationName|Text|
|||resParty_positionName|Text|
|||resParty_address|Text|
|||resParty_contactInstructions|Text|
|||resParty_electronicMailAddress|Text|
|||resParty_hoursOfService|Text|
|||resParty_telephoneFacsimile|Text|
|||resParty_telephoneVoice|Text|
|||resParty_website|Text|
|||resParty_role|Text|
|onlineResource|URL|onlineResource|Text|
|purpose|PurposeOfCollectionValue|purpose_1_href|Text|
|||purpose_1|Text|
||PurposeOfCollectionValue|purpose_2_href|Text|
|||purpose_2|Text|

#### EnvironmentalMonitoringProgramme_triggers

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|triggers|EnvironmentalMonitoringActivity|RID|Long|
|||triggers|Long|
