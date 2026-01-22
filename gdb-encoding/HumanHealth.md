# Geodatabase Encoding Rule for INSPIRE Human Health

`Version: 1.0`
`Date: 2025-09-29`

The Human Health encoding can be used as an *alternative encoding* for Human Health data that fulfills the following requirements:

* There is not more than 3 `diseaseMeasure` per `Disease`






## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Human Health version 4.0.0](https://github.com/INSPIRE-MIF/technical-guidelines/tree/main/data/hh)

## Conformance Class Core

The Human Health theme has one application schema, therefore this theme-specific encoding rule defines a single core conformance class.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Human Health conceptual model before applying the general rules of this encoding rule:
 
1. Substitute all attributes that have a property type with a Codelist Stereotype through an inline codelist reference using `MT008()`. 
2. Apply the SimplePeriod rule `MT009()`.
3. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
4. Limit the Multiplicity for `diseaseMeasure` for `Disease` to 3 through Rule `MT012(3)`
5. Apply Attribute shortening rule for Biomarker:

    |Replace|With|
    |----|----|
    |`'biomarkerStatisticalParameter_'`|`'bSP_' `|
    
    

    


#### Biomarker

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||aggregationUnit_href|Text|
|||biomarkerName_chemical_href|Text|
|||biomarkerName_chemical|Text|
|||biomarkerName_matrix_href|Text|
|||biomarkerName_matrix|Text|
|BiomarkerStatisticalParameterType||bSP_geometricMean|Float|
|||bSP_geometricMean_uom|Text|
|||bSP_CI95ofGM|Float|
|||bSP_CI95ofGM_uom|Text|
|||bSP_P50|Float|
|||bSP_P50_uom|Text|
|||bSP_P90|Float|
|||bSP_P90_uom|Text|
|||bSP_P95|Float|
|||bSP_P95_uom|Text|
|||bSP_CI95ofP95|Float|
|||bSP_CI95ofP95_uom|Text|
|||bSP_maximum|Float|
|||bSP_maximum_uom|Text|
|||bSP_numberOfPartecipants|Long|
|||bSP_pinLOD|Float|
|||bSP_LOQ|Float|
|ReferencePeriodType||referencePeriod_startDate|Date|
|||referencePeriod_endDate|Date|
|AgeRangeType||ageRange_startAge_month|Long|
|||ageRange_startAge_week|Long|
|||ageRange_startAge_year|Long|
|||ageRange_range_month|Long|
|||ageRange_range_week|Long|
|||ageRange_range_year|Long|
|||gender_href|Text|
|||gender|Text|
|BiomarkerThematicMetadata||refersTo_studyType|Text|
|||refersTo_areaType|Text|
|||refersTo_specificSubPopulation|Text|
|||refersTo_meanAge_month|Long|
|||refersTo_meanAge_week|Long|
|||refersTo_meanAge_year|Long|

#### Disease

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||aggregationUnit_href|Text|
|AgeRangeType||ageRange_startAge_month|Long|
|||ageRange_startAge_week|Long|
|||ageRange_startAge_year|Long|
|||ageRange_range_month|Long|
|||ageRange_range_week|Long|
|||ageRange_range_year|Long|
|DiseaseMeasure||diseaseMeasure_1_type_href|Text|
|DiseaseMeasure||diseaseMeasure_1_type|Text|
|||diseaseMeasure_1_value|Float|
|DiseaseMeasure||diseaseMeasure_2_type_href|Text|
|DiseaseMeasure||diseaseMeasure_2_type|Text|
|||diseaseMeasure_2_value|Float|
|DiseaseMeasure||diseaseMeasure_3_type_href|Text|
|DiseaseMeasure||diseaseMeasure_3_type|Text|
|||diseaseMeasure_3_value|Float|
|||gender_href|Text|
|||gender|Text|
|ReferencePeriodType||referencePeriod_startDate|Date|
|||referencePeriod_endDate|Date|
|||pathology_href|Text|
|||pathology|Text|
|||COD_href|Text|
|||COD|Text|

#### EnvHealthDeterminantConcentrationMeasureP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||type_href|Text|
|||type|Text|
|||measureTime_beginPosition|Date|
|||measureTime_endPosition|Date|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|measure||measure|Float|
|||measure_uom|Text|
|||category_href|Text|
|||category|Text|
|||component_href|Text|
|||component|Text|
|||media_href|Text|
|||media|Text|

#### EnvHealthDeterminantConcentrationMeasureS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||type_href|Text|
|||type|Text|
|||measureTime_beginPosition|Date|
|||measureTime_endPosition|Date|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|measure||measure|Float|
|||measure_uom|Text|
|||category_href|Text|
|||category|Text|
|||component_href|Text|
|||component|Text|
|||media_href|Text|
|||media|Text|

#### EnvHealthDeterminantMeasureP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||type_href|Text|
|||type|Text|
|||measureTime_beginPosition|Date|
|||measureTime_endPosition|Date|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|measure||measure|Float|
|measure.uom||measure_uom|Text|
|||category_href|Text|
|||category|Text|

#### EnvHealthDeterminantMeasureS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||type_href|Text|
|||type|Text|
|||measureTime_beginPosition|Date|
|||measureTime_endPosition|Date|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|measure||measure|Float|
|measure.uom||measure_uom|Text|
|||category_href|Text|
|||category|Text|

#### EnvHealthDeterminantNoiseMeasureP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||type_href|Text|
|||type|Text|
|||measureTime_beginPosition|Date|
|||measureTime_endPosition|Date|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|measure||measure|Float|
|||measure_uom|Text|
|||category_href|Text|
|||category|Text|
|||source_href|Text|
|||source|Text|

#### EnvHealthDeterminantNoiseMeasureS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||type_href|Text|
|||type|Text|
|||measureTime_beginPosition|Date|
|||measureTime_endPosition|Date|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|measure||measure|Float|
|||measure_uom|Text|
|||category_href|Text|
|||category|Text|
|||source_href|Text|
|||source|Text|

#### EnvHealthDeterminantStatisticalData

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||aggregationUnit_href|Text|
|||statisticalMethod_href|Text|
|||statisticalMethod|Text|
|||type_href|Text|
|||type|Text|
|measure||measure|Float|
|measure.uom||measure_uom|Text|

#### GeneralHealthStatistics

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||aggregationUnit_href|Text|
|AgeRangeType||ageRange_startAge_month|Long|
|||ageRange_startAge_week|Long|
|||ageRange_startAge_year|Long|
|||ageRange_range_month|Long|
|||ageRange_range_week|Long|
|||ageRange_range_year|Long|
|||gender_href|Text|
|||gender|Text|
|||generalHealthName_href|Text|
|||generalHealthName|Text|
|generalHealthValue||generalHealthValue|Float|
|ReferencePeriodType||referencePeriod_startDate|Date|
|||referencePeriod_endDate|Date|

#### HealthServicesStatistic

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|||aggregationUnit_href|Text|
|||healthServiceType_href|Text|
|||healthServiceType|Text|
|healthServiceValue||healthServiceValue|Float|
|ReferencePeriodType||referencePeriod_startDate|Date|
|||referencePeriod_endDate|Date|
