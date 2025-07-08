# Geodatabase Encoding Rule for INSPIRE Air Transport Network

`Version: 0.5`
`Date: 2025-02-28`

The Simple Air Transport Network encoding can be used as an *alternative encoding* for AirTransportNetwork data that fulfills the following requirements:

* There is no NetworkProperty in the data. 
* There is no `inNetwork` relation for any Object in the data. 
* There is no `AirwayLinkSequence`, `AirRoute`, `ApronArea`, `DesignatedPoint`, `ProcedureLink` , `InstrumentApproachProcedure`, `Navaid`, `StandardInstrumentArrival`, `StandardInstrumentDeparture`, `TouchDownLiftOff` or `AirwayLinkSet` in the data. 



## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Transport Networks version 3.3.0](https://github.com/INSPIRE-MIF/technical-guidelines/tree/main/data/tn)

## Conformance Class Air Transport Network

The Transport Networks theme has five application schemas. This application schema-specific encoding rule defines a conformance class for the application schema Air Transport Network.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Air Transport Network conceptual model before applying the general rules of this encoding rule:
 
1. Substitute all attributes that have a property type with a Codelist Sterotype through an inline codelist reference using `MT008()`. 
2. Substitute all occurences of `GeographicName` with the Simple Geographic Name through Rule `MT005(separator: '_')`.
3. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')` .
4. `spokeStart` and `spokeEnd` on `AerodromeNode`, `RunwayCentrelinePoint` , `TouchDownLiftOff` and `DesignatedPoint` can be derived as the inverse properties of `startNode` and `endNode` from `AirRouteLink`.




#### AerodromeArea

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|geographicalName|GeographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|

#### AerodromeNode

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|geographicalName|GeographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|significantPoint|Boolean|significantPoint|Short|
|designatorIATA|CharacterString|designatorIATA|Text|
|locationIndicatorICAO|CharacterString|locationIndicatorICAO|Text|

#### AirRouteLink

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|fictitious|Boolean|fictitious|Long|
|endNode|AirNode|endNode|Long|
|startNode|AirNode|startNode|Long|
|geographicalName|GeographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|airRouteLinkClass|AirRouteLinkClassValue|airRouteLinkClass_href|Text|
|||airRouteLinkClass|Text|

#### AirspaceArea

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|geographicalName|GeographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|AirspaceAreaType|AirspaceAreaTypeValue|AirspaceAreaType_href|Text|
|||AirspaceAreaType|Text|

#### RunwayArea

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|geographicalName|GeographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|designator|CharacterString|designator|Text|
||RunwayTypeValue|runwayType_href|Text|
|||runwayType|Text|

#### RunwayCentrelinePoint

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|geographicalName|GeographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|significantPoint|Boolean|significantPoint|Short|
|pointRole|PointRoleValue|pointRole_href|Text|
|||pointRole|Text|

#### TaxiwayArea

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|geographicalName|GeographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|designator|CharacterString|designator|Text|

#### TouchDownLiftOff

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|geographicalName|GeographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|significantPoint|Boolean|significantPoint|Short|
|designator|CharacterString|designator|Text|
