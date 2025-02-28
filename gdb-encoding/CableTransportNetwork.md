# Geodatabase Encoding Rule for INSPIRE Cable Transport Network

`Version: 1.0`
`Date: 2025-01-19`

The Simple Cable Transport Network encoding can be used as an *alternative encoding* for Cable Transport Network data that fulfills the following requirements:

* There is no NetworkProperty for any Object in the data. 
* There is no `inNetwork` relation for any Object in the data. 
* There is no `CablewayLinkSequence` or `CablewayLinkSet` in the data. 



## Normative References

* [INSPIRE UML-to-Geodatabase encoding rule version 0.2](GeodatabaseEncoding.md)
* [Data Specification - INSPIRE Transport Networks version 3.3.0](https://github.com/INSPIRE-MIF/technical-guidelines/tree/main/data/tn)

## Conformance Class Cable Transport Network

The Transport Networks theme has five application schemas. This application schema-specific encoding rule defines a conformance class for the application schema Cable Transport Network.

### Model Transformation

This section describes which transformation rules with which parameters are applied to the Cable Transport Network conceptual model before applying the general rules of this encoding rule:
 
1. Substitute all attributes that have a property type with a Codelist Stereotype through a inline codelist reference using `MT008()`. 
2. Substitute all occurrences of `GeographicName` with the Simple Geographic Name through Rule `MT005(separator: '_')`.
3. Apply the General Flattening rule to simplify the remaining properties: `MT001(separator: '_')`.
4. `spokeStart` and `spokeEnd` on `CablewayNode` can be derived as the inverse properties of `startNode` and `endNode` from `CablewayLink`.




#### CablewayLink

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|fictitious|fictitious|fictitious|Long|
|geographicalName|geographicalName|geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
|cablewayType|CablewayTypeValue|cablewayType_href|Text|
|||cablewayType|Text|

#### CablewayNode

|Name|Type|Simplified Name|GDB Type|
|------|------|------|------|
|||featureId|Long|
|beginLifespanVersion|DateTime|beginLifespanVersion|Date|
|inspireId|Identifier|inspireId_localId|Text|
|||inspireId_namespace|Text|
|||inspireId_versionId|Text|
|endLifespanVersion|DateTime|endLifespanVersion|Date|
|geographicalName||geographicalName_language|Text|
|||geographicalName_name|Text|
|validFrom|DateTime|validFrom|Date|
|validTo|DateTime|validTo|Date|
