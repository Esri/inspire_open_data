# Geodatabase Encoding Rule for INSPIRE EnergyResourcesVector

`Version: 1.0`
`Date: 2025-08-11`

The Simple Energy Resources Vector encoding can be used as an *alternative encoding* for Energy Resources Vector data that fulfills the following requirements:

* There is not Coverage data.
* There is not more than 1 `reportingAuthority` per `FossilFuelResource` and `RenewableAndWasteResource`
* There is not more than 1 `exploitationPeriod` per `FossilFuelResource` and `RenewableAndWasteResource`
* There is not more than 1 `resourceName` per `FossilFuelResource` and `RenewableAndWasteResource`
* There is not more than 1 `quantity amount` per `FossilFuelResource_type`
* There is not more than 1 `quantity dateOfDetermination` per `FossilFuelResource_type`
* There is not more than 1 `quantity resourceClass` per `FossilFuelResource_type`


## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Natural Risk Zones version 3.0.0](https://github.com/INSPIRE-MIF/technical-guidelines/tree/main/data/er)

## Conformance Class Core

The Energy Resources theme has three application schema. This application schema-specific encoding rule defines a single conformance class for the application schema Energy Resources Vector.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Energy Resources Vector conceptual model before applying the general rules of this encoding rule:
 
1. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. 
2. Apply the Simplified Geographical Name rule `MT005()`.
3. Apply the SimplePeriod rule `MT009()`.
4. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
5. Limit the Multiplicity for `reportingAuthority` for `FossilFuelResource` and `RenewableAndWasteResource`to 1 through Rule `MT012(1)`
6. Limit the Multiplicity for `exploitationPeriod` for `FossilFuelResource` and `RenewableAndWasteResource`to 1 through Rule `MT012(1)`
7. Limit the Multiplicity for `resourceName` for `FossilFuelResource` and `RenewableAndWasteResource`to 1 through Rule `MT012(1)`
8. Limit the Multiplicity for `quantity amount` for `FossilFuelResource_type` to 1 through Rule `MT012(1)`
9. Limit the Multiplicity for `quantity dateOfDetermination` for `FossilFuelResource_type` to 1 through Rule `MT012(1)`
10. Limit the Multiplicity for `quantity resourceClass` for `FossilFuelResource_type` to 1 through Rule `MT012(1)`
11. Apply the Simplified Codelist Reference rule `MT008()`.
12. Apply Attribute shortening rule for FossilFuelResource:

    |Replace|With|
    |----|----|
    |`'reportingAuthority_'`|`'repAuthority__' `|
    |`'resourceName_'`|`'resName_' `|
    |`'ClassificationAndQuantificationFramework'`|`'cqFramework' `|
    |`'exploitationPeriod_'`|`'expPeriod_' `|
    |`'verticalExtent_'`|`'vertExt_' `|

13. Apply Attribute shortening rule for RenewableAndWasteResource:

    |Replace|With|
    |----|----|
    |`'reportingAuthority_'`|`'repAuthority__' `|
    |`'resourceName_'`|`'resName_' `|
    |`'ClassificationAndQuantificationFramework'`|`'cqFramework' `|
    |`'exploitationPeriod_'`|`'expPeriod_' `|
    |`'verticalExtent_'`|`'vertExt_' `|

14. Apply Attribute shortening rule for FossilFuelResource_type:

    |Replace|With|
    |----|----|
    |`'resource_calorificValue_calorificRange'`|`'res_calRange_' `|
    |`'resource_calorificValue_calorificScalar'`|`'res_calScalar_' `|
    |`'resource_quantity_'`|`'res_quant_' `|
    |`'resource_quantity_resourceClass_'`|`'res_quant_resourceClass' `|
    |`'resource_typeOfResource_'`|`'res_typeOfResource' `|
  

    
#### FossilFuelResourceL

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|reportingAuthority|reportingAuthority|repAuthority_contact|Text|
|||repAuthority_individualName|Text|
|||repAuthority_organisationName|Text|
|||repAuthority_positionName|Text|
|||repAuthority_role|Text|
|resourceName|resourceName|resName|Text|
|||resName_lang|Text|
|ClassificationAndQuantificationFramework|ClassificationAndQuantificationFramework|cqFramework|Text|
|||cqFramework_href|Text|
|exploitationPeriod|DateTime|expPeriod_beginTime|Date|
|||expPeriod_endTimeTime|Date|
|verticalExtent|VerticalExtentType|vertExt_lowerBound|Float|
|||vertExt_upperBound|Float|
|||vertExt_scalar|Float|
|||vertExt_Reference|Text|
|||vertExt_Reference_href|Text|
|dateOfDiscovery|DateTime|dateOfDiscovery|Date|

#### FossilFuelResourceP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|reportingAuthority|reportingAuthority|repAuthority_contact|Text|
|||repAuthority_individualName|Text|
|||repAuthority_organisationName|Text|
|||repAuthority_positionName|Text|
|||repAuthority_role|Text|
|resourceName|resourceName|resName|Text|
|||resName_lang|Text|
|ClassificationAndQuantificationFramework|ClassificationAndQuantificationFramework|cqFramework|Text|
|||cqFramework_href|Text|
|exploitationPeriod|DateTime|expPeriod_beginTime|Date|
|||expPeriod_endTimeTime|Date|
|verticalExtent|VerticalExtentType|vertExt_lowerBound|Float|
|||vertExt_upperBound|Float|
|||vertExt_scalar|Float|
|||vertExt_Reference|Text|
|||vertExt_Reference_href|Text|
|dateOfDiscovery|DateTime|dateOfDiscovery|Date|

#### FossilFuelResourceS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|reportingAuthority|reportingAuthority|repAuthority_contact|Text|
|||repAuthority_individualName|Text|
|||repAuthority_organisationName|Text|
|||repAuthority_positionName|Text|
|||repAuthority_role|Text|
|resourceName|resourceName|resName|Text|
|||resName_lang|Text|
|ClassificationAndQuantificationFramework|ClassificationAndQuantificationFramework|cqFramework|Text|
|||cqFramework_href|Text|
|exploitationPeriod|DateTime|expPeriod_beginTime|Date|
|||expPeriod_endTimeTime|Date|
|verticalExtent|VerticalExtentType|vertExt_lowerBound|Float|
|||vertExt_upperBound|Float|
|||vertExt_scalar|Float|
|||vertExt_Reference|Text|
|||vertExt_Reference_href|Text|
|dateOfDiscovery|DateTime|dateOfDiscovery|Date|

#### RenewableAndWasteResourceL

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|reportingAuthority|reportingAuthority|repAuthority_contact|Text|
|||repAuthority_individualName|Text|
|||repAuthority_organisationName|Text|
|||repAuthority_positionName|Text|
|||repAuthority_role|Text|
|resourceName|resourceName|resName|Text|
|||resName_lang|Text|
|ClassificationAndQuantificationFramework|ClassificationAndQuantificationFramework|cqFramework|Text|
|||cqFramework_href|Text|
|exploitationPeriod|DateTime|expPeriod_beginTime|Date|
|||expPeriod_endTimeTime|Date|
|verticalExtent|VerticalExtentType|vertExt_lowerBound|Float|
|||vertExt_upperBound|Float|
|||vertExt_scalar|Float|
|||vertExt_Reference|Text|
|||vertExt_Reference_href|Text|
|dateOfDetermination|DateTime|dateOfDiscovery|Date|
|Capacity|Float|capacity|Float|
|||capacity_uom|Text|
|typeOfResource|RenewableAndWasteValue|typeOfResource|Text|
|||typeOfResource_href|Text|

#### RenewableAndWasteResourceP

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|reportingAuthority|reportingAuthority|repAuthority_contact|Text|
|||repAuthority_individualName|Text|
|||repAuthority_organisationName|Text|
|||repAuthority_positionName|Text|
|||repAuthority_role|Text|
|resourceName|resourceName|resName|Text|
|||resName_lang|Text|
|ClassificationAndQuantificationFramework|ClassificationAndQuantificationFramework|cqFramework|Text|
|||cqFramework_href|Text|
|exploitationPeriod|DateTime|expPeriod_beginTime|Date|
|||expPeriod_endTimeTime|Date|
|verticalExtent|VerticalExtentType|vertExt_lowerBound|Float|
|||vertExt_upperBound|Float|
|||vertExt_scalar|Float|
|||vertExt_Reference|Text|
|||vertExt_Reference_href|Text|
|dateOfDetermination|DateTime|dateOfDiscovery|Date|
|Capacity|Float|capacity|Float|
|||capacity_uom|Text|
|typeOfResource|RenewableAndWasteValue|typeOfResource|Text|
|||typeOfResource_href|Text|

#### RenewableAndWasteResourceS

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|reportingAuthority|reportingAuthority|repAuthority_contact|Text|
|||repAuthority_individualName|Text|
|||repAuthority_organisationName|Text|
|||repAuthority_positionName|Text|
|||repAuthority_role|Text|
|resourceName|resourceName|resName|Text|
|||resName_lang|Text|
|ClassificationAndQuantificationFramework|ClassificationAndQuantificationFramework|cqFramework|Text|
|||cqFramework_href|Text|
|exploitationPeriod|DateTime|expPeriod_beginTime|Date|
|||expPeriod_endTimeTime|Date|
|verticalExtent|VerticalExtentType|vertExt_lowerBound|Float|
|||vertExt_upperBound|Float|
|||vertExt_scalar|Float|
|||vertExt_Reference|Text|
|||vertExt_Reference_href|Text|
|dateOfDetermination|DateTime|dateOfDiscovery|Date|
|Capacity|Float|capacity|Float|
|||capacity_uom|Text|
|typeOfResource|RenewableAndWasteValue|typeOfResource|Text|
|||typeOfResource_href|Text|


#### FossilFuelResource_type

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
inspireId|Identifier|featureId|Long|
|calorificValue|CalorificValueType|res_calRange_lower|Float|
|||res_calRange_lower_uom|Text|
|||res_calRange_upper|Float|
|||res_calRange_upper_uom|Text|
|||res_calScalar|Float|
|||res_calScalar_uom|Text|
|quantity|FossilFuelMeasure|res_quant_amount|Float|
|||res_quant_amount_uom|Text|
|||res_quant_dateOfDeterm|Date|
|resourceClass|FossilFuelClassValue|res_quant_resourceClass|Text|
|||res_quant_resourceClass_href|Text|
|typeOfResource|FossilFuelValue|res_typeOfResource|Text|
|||res_typeOfResource_href|Text|
|||RID|Long|

#### RelFossilFuelResourceL_Resource_type

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|FossilFuelResourceType|FossilFuelResourceType|featureId|Long|
|||RID|Long|

#### RelFossilFuelResourceP_Resource_type

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|FossilFuelResourceType|FossilFuelResourceType|featureId|Long|
|||RID|Long|

#### RelFossilFuelResourceS_Resource_type

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|FossilFuelResourceType|FossilFuelResourceType|featureId|Long|
|||RID|Long|
