# Geodatabase Encoding Rule for INSPIRE Area Management Restriction And RegulationZones

`Version: 0.2`
`Date: 2021-03-08`

The Simple AreaManagementRestrictionAndRegulationZones encoding can be used as an *alternative encoding* for Area Management Restriction And Regulation Zones data that fulfills the following requirements:

* tbd
* maybe limit to Area Geometries, the name Zone already indicates its mostly areas, didn't find a single dataset with points or lines
* only one thematic identifier (not sure here, discussion needed)
*only one zone type (not sure here, discussion needed)

## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](/gdb-encoding/geodatabse encoding.md)
* [Data Specification - INSPIRE Area Management Restriction And Regulation Zones version 3.1](https://inspire.ec.europa.eu/Themes/139/2892)

## Conformance Class Core

The Area Management Restriction And Regulation Zones theme has one application schema, therefore this theme-specific encoding rule defines a single core conformance class.

### Model Transformation


This section describes which transformation rules with which parameters are applied to the Area Management Restriction And Regulation Zones conceptual model before applying the general rules of this encoding rule:
 

1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. (works in GDB)
2. Use Simplified Contact for all occurences `MT012()`. 
3. Use Simplified Related Party for all occurences `MT013()`. 
4. Use Simple Citation for all occurences `MT007()`.
5. Create seperate Tables for each Geometry Type, add suffix for P for Points, L for Lines and S for Areas `MT014()`.
6. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` (works in GDB as ong as not to long) 5.
7. Apply Attribute shortening rules for AreaManagementRestrictionAndRegulationZones:

    |Replace|With|
    |----|----|
    |`designationPeriod_beginPosition`|`'designationPeriod_begin' `|
    |`designationPeriod_endPosition`|`'designationPeriod_end' `|
    |`legalBasis_journalCitation_officialJournalIdentification`|`'legal_officialJournalIdentification' `|
    |`legalBasis_`|`'legal_' `|
    |`relatedParty_`|`'related_' `|




|||featureId||

#### ManagementRestrictionOrRegulationZone

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|thematicId|ThematicIdentifer|thematicId_identifier|Text|
|||thematicId_identifierScheme|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|geometry|GM_Object|geometry||
|zoneType|ZoneTypeCode|zoneType_href|Text|
|specialisedZoneType|SpecialisedZoneTypeCode|specialisedZoneType_href|Text|
|designationPeriod|TM_Period|designationPeriod_begin|Date|
|||designationPeriod_end||
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|||related_website|Text|
|||related_role|Text|
||RelatedParty|RID|Long|

#### ManagementRestrictionOrRegulationZone_competentAuthority

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|competentAuthority||related_individualName|Text|
|||related_organisationName|Text|
|||related_positionName|Text|
|||related_address|Text|
|||related_contactInstructions|Text|
|||related_electronicMailAddress|Text|
|||related_hoursOfService|Text|
|||related_telephoneFacsimile|Text|
|||related_telephoneVoice|Text|
|||environmentalDomain_href|Text|
|environmentalDomain|EnvironmentalDomain|RID|Text|

#### ManagementRestrictionOrRegulationZone_environmentalDomain

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||environmentalDomain|Text|
|||legal_dateRepealed|Date|
|||legal_level_href|Text|
|||legal_officialJournalIdentification|Text|
|||legal_journal_ISSN|Text|
|||legal_journal_ISBN|Text|
|||legal_journal_link|Text|
|||legal_dateEnteredIntoForce|Text|
|legalBasis|LegislationCitation|RID|Long|

#### ManagementRestrictionOrRegulationZone_legalBasis

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||legal_name|Text|
|||legal_shortName|Text|
|||legal_date|Date|
|||legal_link|Text|
|||legal_specificReference|Text|
|||legal_identificationNumber|Text|
|||legal_officialDocumentNumber|Text|
|||RID|Long|

#### ManagementRestrictionOrRegulationZone_name

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||name_lang|Text|
|name|GeographicalName|name|Text|
|plan|DocumentCitation|RID|Long|

#### ManagementRestrictionOrRegulationZone_plan

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||plan_date|Date|
|||plan_link|Text|
|||plan_specificReference|Text|
|||plan_shortName|Text|
|||plan_date|Date|
|||plan_link|Text|
|||plan_specificReference|Text|
|||plan_identificationNumber|Text|
|||plan_officialDocumentNumber|Text|
|||plan_dateEnteredIntoForce|Text|
|||plan_dateRepealed|Date|
|||plan_level_href|Text|
|||plan_name|Text|
|||plan_journalCitation_officialJournalIdentification|Text|
|||plan_journalCitation_ISSN|Text|
|||plan_journalCitation_ISBN|Text|
|||plan_journalCitation_linkToJournal|Text|
|||plan_name|Text|
|||plan_shortName|Text|
|relatedZone|ManagementRestrictionOrRegulationZone|RID|Long|

#### ManagementRestrictionOrRegulationZone_relatedZone

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||relatedZone|Text|
