# Geodatabase Encoding Rule for INSPIRE Area Management Restriction And RegulationZones

`Version: 0.5`
`Date: 2021-05-31`

The Simple AreaManagementRestrictionAndRegulationZones encoding can be used as an *alternative encoding* for Area Management Restriction And Regulation Zones data that fulfills the following requirements:

* ManagementRestrictionOrRegulationZone features have an Area Geometry
* It is sufficient to provide one 'telephoneVoice' and one 'telephoneFax' for the 'competentAuthority'
* There are not more than 3 zoneTypes per ManagementRestrictionOrRegulationZone
* There are not more than 3 environmentalDomains per ManagementRestrictionOrRegulationZone
* There are not more than 3 names per ManagementRestrictionOrRegulationZone
* There is not more than one thematicId per ManagementRestrictionOrRegulationZone
* There is not more than one role per RelatedParty


## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Area Management Restriction And Regulation Zones version 3.1](https://inspire.ec.europa.eu/Themes/139/2892)

## Conformance Class Core

The Area Management Restriction And Regulation Zones theme has one application schema, therefore this theme-specific encoding rule defines a single core conformance class.

### Model Transformation


This section describes which transformation rules with which parameters are applied to the Area Management Restriction And Regulation Zones conceptual model before applying the general rules of this encoding rule:
 

1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. (works in GDB)
2. Limit the Multiplicity for zoneType in ManagementRestrictionOrRegulationZone to 3 through Rule `MT012(3)`
3. Limit the Multiplicity for environmentalDomain in ManagementRestrictionOrRegulationZone to 3 through Rule `MT012(3)`
4. Limit the Multiplicity for name in ManagementRestrictionOrRegulationZone to 3 through Rule `MT012(3)`
5. Limit the Multiplicity for thematicId in ManagementRestrictionOrRegulationZone to 1 through Rule `MT012(1)`
6. Limit the Multiplicity for telephoneVoice in Contact to 1 through Rule `MT012(1)`
7. Limit the Multiplicity for telephoneFax in Contact to 1 through Rule `MT012(1)`
8. Limit the Multiplicity for role in RelatedParty to 1 through Rule `MT012(1)`
9. Substitute `TM_Period` with the Simple Period using `MT009()`.
10. Apply MT011 on competentAuthority, legalBasis and plan.
11. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
12. Apply Attribute shortening rules for AreaManagementRestrictionAndRegulationZones:

    |Replace|With|
    |----|----|
    |`'designationPeriod_beginPosition'`|`'designationPeriod_begin' `|
    |`'designationPeriod_endPosition'`|`'designationPeriod_end' `|
    |`'legalBasis_journalCitation_officialJournalIdentification'`|`'legal_officialJournalIdentification' `|
    |`'legalBasis_'`|`'legal_' `|
    |`'relatedParty_'`|`'related_' `|






#### ManagementRestrictionOrRegulationZone

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|thematicId|ThematicIdentifer|thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
|name|GeographicalName|name_1|Text|
|||name_1_lang|Text|
|||name_2|Text|
|||name_2_lang|Text|
|||name_3|Text|
|||name_3_lang|Text|
|zoneType|ZoneTypeCode|zoneType_1|Text|
|||zoneType_1_href|Text|
|||zoneType_2|Text|
|||zoneType_2_href|Text|
|||zoneType_3|Text|
|||zoneType_3_href|Text|
|specialisedZoneType|SpecialisedZoneTypeCode|specialisedZoneType|Text|
|||specialisedZoneType_href|Text|
|designationPeriod|TM_Period|designationPeriod_begin|Date|
|||designationPeriod_end|Date|
|environmentalDomain|EnvironmentalDomain|environmentalDomain_1|Text|
|||environmentalDomain_1_href|Text|
|||environmentalDomain_2|Text|
|||environmentalDomain_2_href|Text|
|||environmentalDomain_3|Text|
|||environmentalDomain_3_href|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|

#### ManagementRestrictionOrRegulationZone_competentAuthority

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
||RelatedParty|RID|Long|
|competentAuthority||related_individualName|Text|
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

#### ManagementRestrictionOrRegulationZone_legalBasis

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|legalBasis|LegislationCitation|RID|Long|
|||legal_name|Text|
|||legal_shortName|Text|
|||legal_date|Date|
|||legal_link|Text|
|||legal_specificReference|Text|
|||legal_identificationNumber|Text|
|||legal_officialDocumentNumber|Text|
|||legal_dateEnteredIntoForce|Text|
|||legal_dateRepealed|Date|
|||legal_level_href|Text|
|||legal_journal_Identification|Text|
|||legal_journal_ISSN|Text|
|||legal_journal_ISBN|Text|
|||legal_journal_link|Text|

#### ManagementRestrictionOrRegulationZone_plan

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|plan|DocumentCitation|RID|Long|
|||plan_name|Text|
|||plan_shortName|Text|
|||plan_date|Date|
|||plan_link|Text|
|||plan_specificReference|Text|
|||plan_identificationNumber|Text|
|||plan_officialDocumentNumber|Text|
|||plan_dateEnteredIntoForce|Text|
|||plan_dateRepealed|Date|
|||plan_level_href|Text|
|||plan_journal_Identification|Text|
|||plan_journal_ISSN|Text|
|||plan_journal_ISBN|Text|
|||plan_journal_linkToJournal|Text|
|||plan_name|Text|
|||plan_shortName|Text|
|||plan_date|Date|
|||plan_link|Text|
|||plan_specificReference|Text|

#### ManagementRestrictionOrRegulationZone_relatedZone

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|relatedZone|ManagementRestrictionOrRegulationZone|RID|Long|
|||relatedZone|Long|
