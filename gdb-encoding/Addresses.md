# Geodatabase Encoding Rule for INSPIRE Addresses

`Version: 0.1`
`Date: 2021-03-08`

The Simple Addresses encoding can be used as an *alternative encoding* for address data that fulfills the following requirements:

* It is sufficient to provide one `GeographicName` for all elements that use it 
* There is not more than 1 `AdminUnitName` address component per `AdministrativeUnitLevel`
* There is only a single default position per `Address` object

## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Addresses version 3.1](https://inspire.ec.europa.eu/Themes/79/2892)

## Conformance Class Core

The Addresses theme has one application schema, therefore this theme-specific encoding rule defines a single core conformance class.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Addresses conceptual model before applying the general rules of this encoding rule:
 
1. Substitute all occurences of `GeographicName` with the Simple Geographic Name through Rule `MT005(separator: '_')`.  
2. Subsitute all attributes that have a property type with a Codelist Sterotype through a inline codelist reference using `MT008()`. 
3. Inline all `addressComponents` through Rule `MT003(separator: '_', cardinality: { AdminUnitName: 6 })`, using the respective typenames to create unique property names. In addition, define that for `AdminUnitName`, six properties shall be created, one for each `AdministrativeUnitLevel`.
4. Flatten the Locator/Designator structure through application of `MT004(separator: '_', keyProperty: 'type')` (Flatten aggregated or associated components using codelist values). 
5. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` 
6. Apply Attribute shortening rule for Addresses:

    |Replace|With|
    |----|----|
    |`'locator_designator_'`|`'ld' `|
    |`'component_'`|`'' `|




#### Address

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|alternativeIdentifier|String|alternativeIdentifier|Text|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|building|bu-base:AbstractConstruction|building_href|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|locator|AddressLocator|ld_addressNumber|Text|
|||ld_addressNumberExtension|Text|
|||ld_addressNumber2ndExtension|Text|
|||ld_addressIdentifierGeneral|Text|
|||ld_unitIdentifier|Text|
|||ld_buildingIdentifier|Text|
|||ld_buildingIdentifierPrefix|Text|
|||ld_cornerAddress1stIdentifier|Text|
|||ld_cornerAddress2ndIdentifier|Text|
|||ld_entranceDoorIdentifier|Text|
|||ld_floorIdentifier|Text|
|||ld_kilometrePoint|Text|
|||ld_postalDeliveryIdentifier|Text|
|||ld_staircaseIdentifier|Text|
|||ld_unitIdentifier|Text|
|||locator_level|Text|
|||locator_level_href|Text|
|||locator_name|Text|
|parentAddress|Address|parentAddress|Long|
|||position_method|Text|
|||position_method_href|Text|
|||position_specification|Text|
|||position_specification_href|Text|
|status|StatusValue|status|Text|
|||status_href|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|component|AddressComponent|AddressAreaName|Text|
|||AdminUnitName_1stOrder|Text|
|||AdminUnitName_2ndOrder|Text|
|||AdminUnitName_3rdOrder|Text|
|||AdminUnitName_4thOrder|Text|
|||AdminUnitName_5thOrder|Text|
|||AdminUnitName_6thOrder|Text|
|||PostalDescriptor|Text|
|||ThoroughfareName|Text|
