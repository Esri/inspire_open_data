# INSPIRE UML-to-Geodatabase encoding rule

`Version: 0.1`
`Date: 2021-03-01`

## Table of Contents

* [Preface](#preface)
* [Introduction](#introduction)
* [Scope](#scope)
    * Use Cases
	* Themes
    * Technical Issues
    * Technical Limitations
	* Cross-cutting INSPIRE requirements
* [Normative References](#normative-references)
* [Terms and Definitions](#terms-and-definitions)
* [Schema Conversion Rules](#schema-conversion-rules)
    * Types
    * Properties
    * Associations
* [Instance Encoding Rules](#instance-encoding-rules)
    * Requirements and Recommendations
    * Mapping from Conceptual Model to GeoJSON Logical Model
    * Alternative Coordinate Reference Systems
    * Identifiers
* [INSPIRE Theme Encoding Rules](#inspire-theme-encoding-rules)

[comment]: <>  (## Preface)

[comment]: <>  (todo)



## Introduction

This section describes what this document contains and what the high-level objective of this encoding is.

ESRI Geodatabase (GDB) is a format designed for geospatial data. It provides data structures such as feature datasets, feature classes, and associated tables. The database can be stored in a folder based structure (File Geodatabase) or in Spatial Relational Database (Enterprise Geodatabase).  

Within INSPIRE, this encoding rule can used be to encode data from several themes, with a focus on usability of the data in GIS desktop and web clients such as ArcPro, ArcMap, ArcGIS Online, QGIS, FME, and hale studio. It can serve as an *Alternative Encoding* that can be used instead of the default encoding for data, where there is no information loss. In other cases, this Geodatabase encoding may serve as an *Additional Encoding* only.

## Scope

This sections describes the scope of the INSPIRE UML-to-Geodatabase encoding rule. Geodatabase is not equally well suited for all themes and use cases.

### Use Cases

This encoding rule specifically addresses data usability in web and desktop client software, such as ArcGIS Pro, ArcMap, ArcGIS Online, and QGIS. It optimizes usage of INSPIRE data for mapping and geoprocessing in such applications.

The encoding rule is developed with the Internet Engineering Task Force (IETF) [GeoJSON](https://geojson.org) and the Open Web Foundation [GeoServices](http://geoservices.github.io) specifications in mind, for which it can be used in web and desktop client software, such as ArcGIS Pro, ArcMap, ArcGIS Online, and QGIS. 

The encoding rule is also developed with the [OGC API Features standard] (https://www.ogc.org/standards/ogcapi-features) in mind, for which it should provide a storage format that can be used in applications like ArcGIS Online to enable data excahnge via OGC API-Features based on the Geodatabase. 

### Coverage of INSPIRE Themes

For each Application Schema to be covered, a specific Geodatabase Encoding Rule is provided. 
Currently these Application Schemas are covered:

* [`Addresses`](Addresses.md)
* [`AdministrativeAndSocialGovernmentalServices`](AdministrativeAndSocialGovernmentalServices.md)
* [`AdministrativeUnits`](AdministrativeUnits.md)
* [`AreaManagementRestrictionAndRegulationZones`](AreaManagementRestrictionAndRegulationZones.md)
* [`Buildings2D`](Buildings2D.md)
* [`Buildings3D`](Buildings3D.md)
* [`EnvironmentalManagementFacilities`](EnvironmentalManagementFacilities.md)
* [`ExistingLandUse`](ExistingLandUse.md)
* [`NaturalRiskZones`](NaturalRiskZones.md)
* [`PlannedLandUse`](PlannedLandUse.md)
* [`ProtectedSites`](ProtectedSites.md)
* [`SampledLandUse`](SampledLandUse.md)



### Technical Issues

This Encoding Rule addresses specific technical issues that have been problematic when using the default encoding:

* Most GIS software cannot fully make use of non-simple attributes and nested structures for styling, processing and filtering;
* Multiple values per (complex) properties cannot be used fully in ArcGIS and other GIS tools;
* References to other features often cannot be resolved by GIS tools; Propertes of referenced features cannot be used in styling or for filtering;
* Abstract geometry types for an object mean that a wide range of different geometries can be used for any single feature class;
* Mixed geometry types in a FeatureCollection are usually not supported.

### Technical Limitations

In some cases such as the handling of high-cardinality properties, this encoding rule makes a trade-off, so not all issues are resolved. Implementers can apply additional model and instance transformation rules to make adjustments for specific data sets and environments.

The Geodatabase format has limited support for coverage/raster data, therefore this encoding rule cannot be used for those types of data.

### INSPIRE Requirements for Encoding Rules

The Implementing Rules (IRs) on interoperability of spatial data sets and services (Commission Regulation (EU) No 1089/2010) lay down the following requirements for encoding rules:

> **Article 7 -- Encoding**
>
> 1. Every encoding rule used to encode spatial data shall conform to EN ISO 19118. In particular, it shall specify schema
> conversion rules for all spatial object types and all attributes and association roles and the output data structure used. 
> 2. Every encoding rule used to encode spatial data shall be made available.

*To Do: Doesit matter that GDB is not utf-8 encoded?* *To Do: REVIEW THIS XX*

D2.7 specifies more detailed requirements and recommendations for encoding rules. The following list lists the requirements from that document and shows which ones are also met in this encoding rule:

> * Requirement 12: ... documents shall be required to be encoded using UTF-8 as character encoding.

D2.7 also contains a relevant recommendation:

> * Recommendation 3: Encoding rules should be based on international, preferably open, standards.

## Normative References

This section contains references to standards documents and related resources.

[comment]: <>  (*To Do: Good Reference for the GDB format* *To Do: REVIEW THIS XX*)

* [Sustainability of Digital Formats: Planning for Library of Congress Collections – ESRI Geodatabase XML](https://www.loc.gov/preservation/digital/formats/fdd/fdd000295.shtml)
* [GeoJSON - IETF RFC 7946](https://tools.ietf.org/html/rfc7946)
* [INSPIRE Drafting Team Data Specifications. D2.7: Guidelines for the encoding of spatial data, Version 3.3](http://inspire.ec.europa.eu/documents/guidelines-encoding-spatial-data)

## Terms and Definitions

Terms and Definitions can be found in the [Glossary](Glossary.md) document.

## Schema Conversion Rules

INSPIRE defines the conceptual model using UML.

In this Encoding Rule, we take a two-step approach, where we apply model transformations on the level of the conceptual model. This model can then be encoded in Geodatabase using the general schema and instance conversion rules laid out in the next sections.

### Types

#### Feature types 

All types that have the stereotype `<<featureType>>` are converted to Geodatabase feature classes if the type has a geometry. If the type has no geometry it is converted to a table. The typenames remain as they are. 

Where a class has one attribute with a geometry type, this attribute will be mapped to the geometry of the feature class, while all other properties will be mapped to attributes of the same feature class. Where a class has more than one Geometry property, a theme-specific profile has to define which geometry property is the "default" geometry that should be mapped to as the geometry of the feature class. Additional geometry properties can be mapped to additional feature classes.  

#### Data Types

All data types are mapped to JSON objects, where properties of the type are directly added to the root object. Their typenames remain as they are.

#### ISO 19103 - Basic types

All property types are transformed to the simple types that JSON knows about: Number, String, Boolean and Object. The exact mapping from the UML model to the JSON datatypes is outlined in the following table:

| UML Model property type | Geodatabase datatype | Conversion Notes | 
| ------ | ----- | ----- |
| CharacterString | Text |  |
| LocalisedCharacterString | Text | `LanguageCode` is added as a separate property. |
| Boolean | Short Integer |  |
| Integer | Long |  |
| Real | Double |  |
| Decimal | Double |  |
| DateTime | Date | The string must follow the ISO 8601 format, including timezone information (e.g. `2008-10-31T15:07:38-05:00`). |
| Date | Date | The string most follow the format `yyyy-mm-dd`. |
| Length | Double | `uom` is added as a separate property. |
| Measure | Double | `uom` is added as a separate property. |
| URI | string |  |
| URL | string |  |

Any other UML Model property type are to be mapped to `Text`, with specific rules being defined on a case-by-case basis in each theme profile.

#### ISO 19107 - Geometry types

ISO 19107 defines a set of Geometry types, which need to be mapped to the types available in Geodatabase. 

NOTE Not all types can be mapped to Geodatabase; if a data set requires such a type, it cannot use this encoding rule as an Alternative Encoding rule.

| ISO 19107 type | Geodatabase datatype | Conversion Notes | 
| ------ | ----- | ----- |
| GM_Aggregate      | not supported | Limitations apply as to which types in the collection can be included. |
| GM_Curve          | Line | In GML, Curves can also be nonlinear segments or arcs. |
| GM_MultiCurve     | Line | In GML, Curves can also be nonlinear segments or arcs. |
| GM_MultiPoint     | MultiPoint |  |
| GM_MultiPrimitive | not supported | `GM_MultiPrimitive` is an abstract type. |
| GM_MultiSurface   | Polygon |  |
| GM_Object         | Any Geodatabase Geometry type | `GM_Object` is an abstract type, any Geodatabase geometry can be used. |
| GM_Point          | Point |  |
| GM_PolyhedralSurface | Multipatch | At this point, this specification does not support 3D meshes. |
| GM_Primitive      | Any GeoJSON Geometry type | `GM_Primitive` is an abstract type, any Geodatabase geometry can be used. |
| GM_Surface        | Polygon | A `GM_Surface` can have many SurfacePatches, it is thus mapped to MultiPolygon. |
| GM_Tin            | not supported | A TIN without triangulation could be converted to a MultiPoint object. |
| GM_Triangle       | Multipatch | At this point, this specification does not support triangles. |

#### ISO 19108 - Temporal types

For types from ISO 19108 used in INSPIRE schemas, suitable mappings need to be found on a case-by-case basis. The default should be to use the [Simple Period](/model-transformations/SimplePeriod.md) substitution rule.

#### ISO 19115 - Metadata types

For types from ISO 19115 used in INSPIRE schemas, suitable mappings need to be found on a case-by-case basis. For `CI_Citation`, the [Simple Citation](/model-transformations/SimpleCitation.md) substitution rule can be applied.

#### Abstract Types as property types

Where an abstract type with multiple concrete sub-types is used as a property type, a suitable choice of a concrete subtype should be made on a case-by-case basis. As an example, limiting the potential geometry types in this way can make processing easier.

#### Union Types

A `union` represents a choice between multiple properties with potentially different value types, such as in the AreaOfResponsibilityType, where there are options such as `areaOfResponsibilityByAdministrativeUnit` and `areaOfResponsibilityByNamedPlace`. The multiplicity of these options may also differ.

For Union Types used in INSPIRE models, suitable mappings need to be found on a case-by-case basis.

#### Enumerations and Code Lists

No mapping for code lists and enumerations is required. Their values shall be identified by (ideally resolvable) HTTP URIs.

NOTE The INSPIRE Registry can provide the JSON representation of the code list and its entries.

### Properties

Property names remain as they are.

*To Do: REVIEW THIS XX*
If a property has a cardinality > 1, a suitable mapping needs to be found on a case-by-case basis. There is a [model transformation rule](/model-transformations/ExtraTablesMultiplicity.md) that describes how an extra table/featurclass can be used if the number of occurences of such a property can be very high. 

Properties that represent values from code lists are encoded using the `SimpleCodelistReference` [rule described here](/model-transformations/SimpleCodelistReference.md).

NOTE Namespace prefixes, as used in the default encoding, are not used in the Geodatabase encoding rule.

#### Properties with a `uom` attribute

The unit of measurement attribute (`uom`) on any property `x` has to be retained. It is transformed to a new property of the type with the name `x_uom`.

#### Voidable

The stereotype `<<voidable>>` is not converted. If a property has no value, it may be dropped.

### Association Roles

Association roles are retained as they are, if they are not transformed using a profile-specific rule, such as [Inline associated or aggregated components using type names](../model-transformation/AssociatedComponentsHardType).

## Instance Encoding Rules

This section describes how the encoding is derived from the converted conceptual model, and describes which common rules have to be applied for this encoding rule.

### Character Encoding
*To Do: REVIEW THIS XX*
The character encoding of all data encoding in Geodatabase shall be UTF-8.

### Coordinate Reference Systems 

The geodatabase format supports all mandated coordinate systems. As INSPIRE mandates the use of the European Terrestrial Reference System 1989 (ETRS89, see [Requirement 1](https://inspire.ec.europa.eu/reports/ImplementingRules/DataSpecifications/INSPIRE_Specification_CRS_v2.0.pdf)) for the areas within the geographical scope of ETRS89 we encourage ETRS89 to be used.

### nilReason information

In the Geodatabase encoding rule, `nilReason` information shall not be maintained per feature, but rather in the dataset metadata. Properties that have `nil` values shall thus be ignored in the encoding process.

NOTE If, for any dataset, there is specific `nilReason` information per feature, then Geodatabase cannot serve as an alternative encoding rule for that dataset

### Identifiers

A spatial object encoded using the default encoding rule may have several properties that identify it:

* `gml:id`: This property with the `ID` property type is not present in the conceptual model, but mandatory for any spatial object encoded in GML. It represents a technical identifier that is unique within a document and can serve as the target of an anchor/reference.
* `gml:identifier`: This property with the `gml:CodeWithAuthorityType` property type is not present in the conceptual model, but inherited from the `AbstractGML` type. It represents an identifier that is unique within the codeSpace given and serves as the external identifier of the object.
* `inspireId:` This property with the type `IdentifierPropertyType` defines a unique, persistent domain identifier for the spatial object within the INSPIRE infrastructure.

These properties are mapped to the encoded Geodatabase object as follows:

| Default Encoding property | Property Type | Geodatabase Property | Property Type | Conversion Notes | 
| ------ | ----- | ----- | ----- | ----- |
| `gml:id` | ID | `featureId` | integer | new technical identifier, that replaces the string based gml:id |
| `gml:identifier` | CodeWithAuthorityType | `identifier` | string | Can be omitted if empty in the source object. |
| `base:inspireId` | IdentifierPropertyType | `inspireId_localid` | string |  |
|  |  | `inspireId_namespace` | string |  |
|  |  | `inspireId_versionId` | string | Can be omitted if empty in the source object. |

## INSPIRE Theme Encoding Rules

This document does not contain specific rules for each INSPIRE theme. These are maintained in separate documents to facilitate loosely coupled development cycles and groups.

Each of the theme-specific Encoding Rules defines at least one conformance class. Any conformance class in a theme Encoding Rule may define a number of Model Transformation rules that need to be applied before the encoding process. These transformations are documented in the [Model Transformation Rules](../model-transformations/TransformationRules.md) paper. They serve the purpose of adapting the conceptual model (UML) to better match the logical model of the target platform.
