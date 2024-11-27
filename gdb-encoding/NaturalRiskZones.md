# Geodatabase Encoding Rule for INSPIRE NaturalRiskZones

`Version: 1.0`
`Date: 2024-10-01`

The Simple Natural Risk Zones encoding can be used as an *alternative encoding* for Natural Risk Zone data that fulfills the following requirements:

* There is not Coverage data.
* There is not more than 1 `validtiyPeriod` per `RiskZone`
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
 
1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. 
2. Apply the SimpleCitation rule `MT007()`.
3. Apply the SimplePeriod rule `MT009()`.
4. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
5. Limit the Multiplicity for `validtiyPeriod` for `RiskZone` to 1 through Rule `MT012(1)`
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
    

    


#### ExposedElementL

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|assessmentOfVulnerability|VulnerabilityAssessment |aOV_mOIHazard_citationDate|Date|
|||aOV_mOIHazard_citationLink|Text|
|||aOV_mOIHazard_citationName|Text|
|||aOV_mOIHazard_citationLevel|Text|
|||aOV_mOIHazard_citationType|Text|
|||aOV_elementCategory_href|Text|
|||aOV_elementCategory|Text|
|||aOV_specificElementType_href|Text|
|||aOV_specificElementType|Text|

#### ExposedElementP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|assessmentOfVulnerability|VulnerabilityAssessment |aOV_mOIHazard_citationDate|Date|
|||aOV_mOIHazard_citationLink|Text|
|||aOV_mOIHazard_citationName|Text|
|||aOV_mOIHazard_citationLevel|Text|
|||aOV_mOIHazard_citationType|Text|
|||aOV_elementCategory_href|Text|
|||aOV_elementCategory|Text|
|||aOV_specificElementType_href|Text|
|||aOV_specificElementType|Text|

#### ExposedElementS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|assessmentOfVulnerability|VulnerabilityAssessment |aOV_mOIHazard_citationDate|Date|
|||aOV_mOIHazard_citationLink|Text|
|||aOV_mOIHazard_citationName|Text|
|||aOV_mOIHazard_citationLevel|Text|
|||aOV_mOIHazard_citationType|Text|
|||aOV_elementCategory_href|Text|
|||aOV_elementCategory|Text|
|||aOV_specificElementType_href|Text|
|||aOV_specificElementType|Text|

#### HazardArea

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|determinationMethod|DeterminationMethodValue|determinationMethod_href|Text|
|||determinationMethod|Text|
|typeOfHazard|NaturalHazardClassification |tOH_hazardCategory|Text|
|||tOH_hazardCategory_href|Text|
|||tOH_specificHazardType|Text|
|||tOH_specificHazardType_href|Text|
|likelihoodOfOccurrence|LikelihoodOfOccurrence|lOO_qualitativeLikelihood|Text|
|||lOO_quantitative_probability|Float|
|||lOO_quantitative_retPeriod|Float|
|||lOO_method_citationDate|Date|
|||lOO_method_citationLink|Text|
|||lOO_method_citationName|Text|
|||lOO_method_citationLevel|Text|
|||lOO_method_citationType|Text|
|magnitudeOrIntensity|LevelOrIntensity |mOI_qualitativeValue|Text|
|||mOI_quantitativeValue|Float|
|||mOI_quantitativeValue_uom|Text|
|||mOI_method_citationDate|Date|
|||mOI_method_citationLink|Text|
|||mOI_method_citationName|Text|
|||mOI_method_citationLevel|Text|
|||mOI_method_citationType|Text|
|||featureId|Long|

#### HazardArea_source

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|source|ObservedEvent|source|Long|
|||RID|Long|

#### ObservedEventL

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|nameOfEvent|CharacterString|nameOfEvent|Text|
|typeOfHazard|NaturalHazardClassification|tOH_hazardCategory|Text|
|||tOH_hazardCategory_href|Text|
|||tOH_specificHazardType|Text|
|||tOH_specificHazardType_href|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|magnitudeOrIntensity|LevelOrIntensity |mOI_qualitativeValue|Text|
|||mOI_quantitativeValue|Float|
|||mOI_quantitativeValue_uom|Text|
|||mOI_method_citationDate|Date|
|||mOI_method_citationLink|Text|
|||mOI_method_citationName|Text|
|||mOI_method_citationLevel|Text|
|||mOI_method_citationType|Text|

#### ObservedEventP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|nameOfEvent|CharacterString|nameOfEvent|Text|
|typeOfHazard|NaturalHazardClassification|tOH_hazardCategory|Text|
|||tOH_hazardCategory_href|Text|
|||tOH_specificHazardType|Text|
|||tOH_specificHazardType_href|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|magnitudeOrIntensity|LevelOrIntensity |mOI_qualitativeValue|Text|
|||mOI_quantitativeValue|Float|
|||mOI_quantitativeValue_uom|Text|
|||mOI_method_citationDate|Date|
|||mOI_method_citationLink|Text|
|||mOI_method_citationName|Text|
|||mOI_method_citationLevel|Text|
|||mOI_method_citationType|Text|

#### ObservedEventS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|nameOfEvent|CharacterString|nameOfEvent|Text|
|typeOfHazard|NaturalHazardClassification|tOH_hazardCategory|Text|
|||tOH_hazardCategory_href|Text|
|||tOH_specificHazardType|Text|
|||tOH_specificHazardType_href|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|magnitudeOrIntensity|LevelOrIntensity |mOI_qualitativeValue|Text|
|||mOI_quantitativeValue|Float|
|||mOI_quantitativeValue_uom|Text|
|||mOI_method_citationDate|Date|
|||mOI_method_citationLink|Text|
|||mOI_method_citationName|Text|
|||mOI_method_citationLevel|Text|
|||mOI_method_citationType|Text|

#### RiskZone

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|sourceOfRisk|NaturalHazardClassification |sOR_hazardCategory|Text|
|||sOR_hazardCategory_href|Text|
|||sOR_specificHazardType|Text|
|||sOR_specificHazardType_href|Text|
|source|HazardArea|source|Long|
|validityPeriod|TM_Period|validityPeriod_beginPosition|Date|
|||validityPeriod_endPosition|Date|
|levelOfRisk|LevelOrIntensity|lOR_qualitativeValue|Text|
|||lOR_quantitativeValue|Text|
|||lOR_quantitativeValue_uom|Text|
|||lOR_method_citationDate|Date|
|||lOR_method_citationLink|Text|
|||lOR_method_citationName|Text|
|||lOR_method_citationLevel|Text|
|||lOR_method_citationType|Text|

#### RiskZone_exposedElement

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|exposedElement|ExposedElement|exposedElement|Long|
|||RID|Long|
