# Geodatabase Encoding Rule for INSPIRE Soil

`Version: 1.0`
`Date: 2025-09-01`

The Simple Soil encoding can be used as an *alternative encoding* for Soil data that fulfills the following requirements:

* There is not Coverage data.
* There is no `SoilDerivedObject`
* There is no `soilProfileObservation` per `SoilProfile`
* There is no `WRBSoilName` per `SoilProfile`
* There is no `profileElementObservation` per `ProfileElement`
* There is no `soilDerivedObjectObservation` per `SoilDerivedObject`
* There is no `FAOHorizonSubordinate` per `FAOHorizonNotation`
* There is not more than 2 `otherSoilName` per `SoilProfile`
* There is not more than 1 `isDerivedFrom` per `DerivedSoilProfile`
* `SoilSite` has a Surface or MultiSurface geometry.






## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Soil version 3.2.0](https://github.com/INSPIRE-MIF/technical-guidelines/tree/main/data/so)

## Conformance Class Core

The Soil theme has one application schema, therefore this theme-specific encoding rule defines a single core conformance class.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Soil conceptual model before applying the general rules of this encoding rule:
 
1. Substitute all attributes that have a property type with a Codelist Stereotype through an inline codelist reference using `MT008()`. 
2. `SoilSite.isObservedOnLocation` is modeled as the inverse of `SoilPlot.locatedOn`
`ObservedSoilProfile.isDescribedBy` and `DerivedSoilProfile.isDescribedBy` is modeled as the inverse of `ProfileElement.isPartOf`
3. Apply the SimplePeriod rule `MT009()`.
4. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
5. Limit the Multiplicity for `otherSoilName` for `SoilProfile` to 1 through Rule `MT012(2)`
6. Limit the Multiplicity for `isDerivedFrom` for `DerivedSoilProfile` to 1 through Rule `MT012(1)`



#### DerivedSoilProfile

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|localIdentifier||localIdentifier|Text|
|||oSN_1_soilName_href|Text|
|||oSN_1_soilName|Text|
|||oSN_1_isOriginalClassification|Short|
|||oSN_2_soilName_href|Text|
|||oSN_2_soilName|Text|
|||oSN_2_isOriginalClassification|Short|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|||isDerivedFrom|Text|

#### ObservedSoilProfile

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|localIdentifier||localIdentifier|Text|
|||oSN_1_soilName_href|Text|
|||oSN_1_soilName|Text|
|otherSoilName{}.OtherSoilNameType.isOriginalClassification||oSN_1_isOriginalClassification|Short|
|||oSN_2_soilName_href|Text|
|||oSN_2_soilName|Text|
|otherSoilName{}.OtherSoilNameType.isOriginalClassification||oSN_2_isOriginalClassification|Short|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|||location|Long|

#### SoilBody

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|soilBodyLabel||soilBodyLabel|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|

#### SoilBody_isDescribed

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||RID|Long|
|||isDescribedBy|Long|

#### SoilHorizon

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|||pSF_1_fractionContent|Float|
|||pSF_1_fraction_upperValue|Float|
|||pSF_1_fraction_lowerValue|Float|
|||pSF_2_fractionContent|Float|
|||pSF_2_fraction_upperValue|Float|
|||pSF_2_fraction_lowerValue|Float|
|||pSF_3_fractionContent|Float|
|||pSF_3_fraction_upperValue|Float|
|||pSF_3_fraction_lowerValue|Float|
|||elementDepthRange_upperValue|Float|
|||elementDepthRange_lowerValue|Float|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|||isPartOf_href|Long|
|FAOHorizonNotation.FAOHorizonNotationType.FAOHorizonDiscontinuity||FAOHN_FAOHorizonDiscontinuity|Long|
|||FAOHN_FAOHorizonMaster_href|Text|
|||FAOHN_FAOHorizonMaster|Text|
|||FAOHN_FAOPrime_href|Text|
|||FAOHN_FAOPrime|Text|
|FAOHorizonNotation.FAOHorizonNotationType.FAOHorizonVertical||FAOHN_FAOHorizonVertical|Long|
|FAOHorizonNotation.FAOHorizonNotationType.isOriginalClassification||FAOHN_isOriginalClassification|Short|
|||oHN_1_horizonNotation_href|Text|
|||oHN_1_horizonNotation|Text|
|||oHN_1_isOriginalClassification|Short|
|||oHN_2_horizonNotation_href|Text|
|||oHN_2_horizonNotation|Text|
|||oHN_2_isOriginalClassification|Short|

#### SoilLayer

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|||pSF_1_fractionContent|Float|
|||pSF_1_fraction_upperValue|Float|
|||pSF_1_fraction_lowerValue|Float|
|||pSF_2_fractionContent|Float|
|||pSF_2_fraction_upperValue|Float|
|||pSF_2_fraction_lowerValue|Float|
|||pSF_3_fractionContent|Float|
|||pSF_3_fraction_upperValue|Float|
|||pSF_3_fraction_lowerValue|Float|
|||elementDepthRange_upperValue|Float|
|||elementDepthRange_lowerValue|Float|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|||isPartOf|Long|
|||layerType_href|Text|
|||layerType|Text|
|||layerRockType_1_href|Text|
|||layerRockType_1|Text|
|||layerRockType_2_href|Text|
|||layerRockType_2|Text|
|||layerRockType_3_href|Text|
|||layerRockType_3|Text|
|||layerGenesisProcess_href|Text|
|||layerGenesisProcess|Text|
|||layerGenesisEnvironment_href|Text|
|||layerGenesisEnvironment|Text|
|||layerGenesisProcessState_href|Text|
|||layerGenesisProcessState|Text|

#### SoilPlot

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|soilPlotLocation||soilPlotLocation|Text|
|||soilPlotType_href|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|||observedProfile_href|Text|
|||locatedOn_href|Text|

#### SoilSite

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|||soilInvestigationPurpose|Text|
|||soilInvestigationPurpose_href|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
