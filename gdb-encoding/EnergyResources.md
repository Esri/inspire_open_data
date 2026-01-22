# Geodatabase Encoding Rule for INSPIRE NaturalRiskZones

`Version: 1.0`
`Date: 2024-10-01`

The Simple Natural Risk Zones encoding can be used as an *alternative encoding* for Natural Risk Zone data that fulfills the following requirements:

* There is not Coverage data.
* There is not more than 1 `validityPeriod` per `RiskZone`
* There is not more than 1 `assessmentOfVulnerability` per `ExposedElement`
* There is not more than 1 `magnitudeOrIntensity` per `HazardArea`
* There is not more than 1 `magnitudeOrIntensity` per `ObservedEvent`
* There is no `isMonitoredBy` relation for `ObservedEvent`




## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Natural Risk Zones version 3.1.0](https://github.com/INSPIRE-MIF/technical-guidelines/tree/main/data/nz)

## Conformance Class Core

The Natural Risk Zones theme has one application schema, therefore this theme-specific encoding rule defines a single core conformance class.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Natural Risk Zones conceptual model before applying the general rules of this encoding rule:
 
1. Substitute all attributes that have a property type with a Codelist Stereotype through an inline codelist reference using `MT008()`. 
2. Apply the SimpleCitation rule `MT007()`.
3. Apply the SimplePeriod rule `MT009()`.
4. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
5. Limit the Multiplicity for `validityPeriod` for `RiskZone` to 1 through Rule `MT012(1)`
6. Limit the Multiplicity for `assessmentOfVulnerability` for `ExposedElement` to 1 through Rule `MT012(1)`
7. Limit the Multiplicity for `magnitudeOrIntensity` for `HazardArea` to 1 through Rule `MT012(1)`
8. Limit the Multiplicity for `magnitudeOrIntensity` for `ObservedEvent` to 1 through Rule `MT012(1)`
9. Apply Attribute shortening rule for RiskZone:

    |Replace|With|
    |----|----|
    |`'sourceOfRisk_'`|`'sOR_' `|
    |`'assessmentMethod_'`|`'method_' `|
    |`'levelOfRisk_'`|`'lOR__' `|

10. Apply Attribute shortening rule for ExposedElement:

    |Replace|With|
    |----|----|
    |`'assessmentOfVulnerability_magnitudeOrIntensityOfHazard_assessmentMethod_'`|`'aOV_mOIHazard_' `|
    |`'assessmentOfVulnerability_typeOfElement_exposedElementCategory'`|`'aOV_elementCategory' `|
    |`'assessmentOfVulnerability_typeOfElement_specificExposedElementType'`|`'aOV_specificElementType' `|

11. Apply Attribute shortening rule for HazardArea:

    |Replace|With|
    |----|----|
    |`'typeOfHazard_'`|`'tOH_' `|
    |`'likelihoodOfOccurrence_'`|`'lOO_' `|
    |`'quantitativeLikelihood_probabilityOfOccurrence'`|`'quantitative_probability' `|
    |`'quantitativeLikelihood_returnPeriod'`|`'quantitative_retPeriod' `|
    |`'assessmentMethod_'`|`'method_' `|
    |`'magnitudeOrIntensity_'`|`'mOI_' `|

12. Apply Attribute shortening rule for ObservedEvent:

    |Replace|With|
    |----|----|
    |`'typeOfHazard_'`|`'tOH_' `|
    |`'assessmentMethod_'`|`'method_' `|
    |`'magnitudeOrIntensity_'`|`'mOI_' `|
    

    


#### FossilFuelResourceP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|||ClassAndQuantFramework_href|Text|
|||ClassAndQuantFramework|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|||exploitationPeriod_beginTime|Date|
|||exploitationPeriod_endTime|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|||reportingAuthority_orgName|Text|
|||resourceName_language|Text|
|||resourceName_name|Text|
|||vertExt_range_lowerBound|Float|
|||vertExt_range_lowerBound_uom|Text|
|||vertExt_range_upperBound|Float|
|||vertExt_range_upperBound_uom|Text|
|||vertExt_scalar|Float|
|||vertExt_scalar_uom|Text|
|||vertExt_verticalReference_href|Text|
|||vertExt_verticalReference|Text|
|dateOfDiscovery||dateOfDiscovery|Date|
|FossilFuelResourceType||res_calVal_range_lowerB|Float|
|||res_calVal_range_lowerB_uom|Text|
|||res_calVal_range_upperB|Float|
|||res_calVal_range_upperB_uom|Text|
|||res_calVal_calorificScalar|Float|
|||res_calVal_calorificScalar_uom|Text|
|||res_quantity_amount|Float|
|||res_quantity_amount_uom|Text|
|||res_quantity_dateOfDeterm|Date|
|||res_quantity_resClass_href|Text|
|||res_quantity_resClass|Text|
|||res_typeOfResource_href|Text|
|||res_typeOfResource|Text|

#### FossilFuelResourceS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|||ClassAndQuantFramework_href|Text|
|||ClassAndQuantFramework|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|||exploitationPeriod_beginTime|Date|
|||exploitationPeriod_endTime|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|||reportingAuthority_orgName|Text|
|||resourceName_language|Text|
|||resourceName_name|Text|
|||vertExt_range_lowerBound|Float|
|||vertExt_range_lowerBound_uom|Text|
|||vertExt_range_upperBound|Float|
|||vertExt_range_upperBound_uom|Text|
|||vertExt_scalar|Float|
|||vertExt_scalar_uom|Text|
|||vertExt_verticalReference_href|Text|
|||vertExt_verticalReference|Text|
|dateOfDiscovery||dateOfDiscovery|Date|
|FossilFuelResourceType||res_calVal_range_lowerB|Float|
|||res_calVal_range_lowerB_uom|Text|
|||res_calVal_range_upperB|Float|
|||res_calVal_range_upperB_uom|Text|
|||res_calVal_calorificScalar|Float|
|||res_calVal_calorificScalar_uom|Text|
|||res_quantity_amount|Float|
|||res_quantity_amount_uom|Text|
|||res_quantity_dateOfDeterm|Date|
|||res_quantity_resClass_href|Text|
|||res_quantity_resClass|Text|
|||res_typeOfResource_href|Text|
|||res_typeOfResource|Text|

#### RenewableAndWasteResourceP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|||ClassAndQuantFramework_href|Text|
|||ClassAndQuantFramework|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|exploitationPeriod||exploitationPeriod_beginTime|Date|
|||exploitationPeriod_endTime|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|reportingAuthority||reportingAuthority_orgName|Text|
|resourceName||resourceName_language|Text|
|||resourceName_name|Text|
|verticalExtent||vertExt_range_lowerBound|Float|
|||vertExt_range_lowerBound_uom|Text|
|||vertExt_range_upperBound|Float|
|||vertExt_range_upperBound_uom|Text|
|||vertExt_scalar|Float|
|||vertExt_scalar_uom|Text|
|||vertExt_verticalReference_href|Text|
|||vertExt_verticalReference|Text|
|Capacity||Capacity|Float|
|Capacity||Capacity_uom|Text|
|dateOfDetermination||dateOfDetermination|Date|
|||typeOfResource_href|Text|
|||typeOfResource|Text|

#### RenewableAndWasteResourceS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|||ClassAndQuantFramework_href|Text|
|||ClassAndQuantFramework|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|exploitationPeriod||exploitationPeriod_beginTime|Date|
|||exploitationPeriod_endTime|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|reportingAuthority||reportingAuthority_orgName|Text|
|resourceName||resourceName_language|Text|
|||resourceName_name|Text|
|verticalExtent||vertExt_range_lowerBound|Float|
|||vertExt_range_lowerBound_uom|Text|
|||vertExt_range_upperBound|Float|
|||vertExt_range_upperBound_uom|Text|
|||vertExt_scalar|Float|
|||vertExt_scalar_uom|Text|
|||vertExt_verticalReference_href|Text|
|||vertExt_verticalReference|Text|
|Capacity||Capacity|Float|
|Capacity||Capacity_uom|Text|
|dateOfDetermination||dateOfDetermination|Date|
|||typeOfResource_href|Text|
|||typeOfResource|Text|
