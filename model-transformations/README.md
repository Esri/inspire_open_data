# Model Transformations

## Introduction

This catalogue builds on the [TransformationRules](https://github.com/INSPIRE-MIF/2017.2/blob/master/model-transformations/TransformationRules.md)
developed under [MIF action 2017.2](https://github.com/INSPIRE-MIF/2017.2) and adds further
rules needed for streamlined encodings of INSPIRE data.

The rules are **target-neutral**: the same rule set underlies both the
**file-geodatabase (GDB)** encoding and the **GeoJSON** encoding. A single rule run produces
a simplified, encoding-independent model, which a serializer target then renders to a
geodatabase or to GeoJSON (RFC 7946) with JSON Schema. The rules were originally developed
for the ESRI file-geodatabase encoding and have since been generalized to serve both targets.

These methods reduce complexity in encoded INSPIRE data — e.g. by flattening nested
structures, resolving indirect references, restricting geometry to simple types, extracting
high-cardinality properties into tables, and substituting complex types (`GeographicalName`,
`CI_Citation`, `TM_Period`, …) with simpler ones. The substitute types are added to the theme
namespaces under draft schemas (`https://inspire.ec.europa.eu/draft-schemas/`).

An alternate encoding may refer to any number of these model transformation rules in its
conformance classes; each rule has a unique identifier. For an alternate encoding to be the
sole encoding, there must be no information loss for the particular data set in question.

**Provenance.** MT001–MT009 are the [2017.2](https://github.com/INSPIRE-MIF/2017.2/tree/master/model-transformations)
base rules and are reused unchanged. MT010 and above are added in this project.

## Requirements for Model Transformations

Each model transformation is described using these properties:

- Name
- Unique Identifier
- Description
- Original vs. Transformed UML Model, where applicable
- Original instance in default encoding
- Transformed instance in default encoding, where applicable
- Model Transformation Rule
- Instance Transformation Rule
- Solved Data Usability issues
- Open/new Data Usability issues
- INSPIRE compliance conditions and reversability
- Examples of use
- Additional notes and enhancements

## Catalogue of simplifying Model Transformations

### MT001: General Flattening

[General Flattening of nested structures](./MT001_GeneralFlattening.md)

### MT002: Extract Primitive Array

[Extract Primitive Array](./MT002_ExtractPrimitiveArray.md)

### MT003: Inline associated or aggregated components using type names

[Association/Aggregation to Composition with Hard Typing](./MT003_AssociatedComponentsHardType.md)

### MT004: Flatten aggregated or associated components using codelist values

[Association/Aggregation to Composition with Soft Typing](./MT004_AssociatedComponentsSoftType.md)

### MT005: Simplified Geographical Name

[Simple Geographic Name](./MT005_SimpleGeographicName.md) — collapses a `GeographicalName`
to a single name value; optional `language` (keep a `<name>_language` companion — subsumes
the former standalone name+language rule) and `nameLeaf` (`<name>_name`).

### MT006: Restriction of property encoding options to only by-reference

[Property Composition to Association](./MT006_PropertyCompositionToAssociation.md)

### MT007: Simplified Citation

[Simple Citation](./MT007_SimpleCitation.md)

### MT008: Simplified Codelist Reference

[Simple Codelist Reference](./MT008_SimpleCodelistReference.md)

### MT009: Simplified Period

[Simple Period](./MT009_SimplePeriod.md)

### MT010: Simplified PT_FreeText

[Simple Free Text](./MT010_SimplePT_FreeText.md)

### MT011: High Cardinality Properties to Extra Tables

[High Cardinality Properties to Extra Tables](./MT011_HighCardinalityPropertiesToExtraTables.md)

### MT012: Limit number of High Cardinality Objects

[Limit Multiplicity for High Cardinality Properties](./MT012_LimitMultiplicityForHighCardinalityProperties.md)

### MT013: Represent n:m Relationships in Table

[Represent n:m Relationships in Table](./MT013_RepresentNtoMRelationshipsInTable.md)

### MT014: One Feature Class Per Geometry Type

[One Feature Class Per Geometry Type](./MT014_OneFeatureClassPerGeometryType.md)

### MT015: Fan Out Feature Type By Codelist Property

[Fan Out Feature Type By Codelist Property](./MT015_FanOutFeatureTypeByCodelistProperty.md)

### MT016: Denormalize Relationship

[Denormalize Relationship](./MT016_DenormalizeRelationship.md)

### MT017: Simplified Category

[Simplified Category](./MT017_SimpleCategory.md)

### MT018: Limit Multiplicity by Fixed Cardinality

[Limit Multiplicity by Fixed Cardinality](./MT018_LimitMultiplicityByFixedCardinality.md)

### MT019: Shorten Attribute Names

[Shorten Attribute Names](./MT019_ShortenAttributeNames.md)

### MT020: Feature Reference to Long Foreign Key

[Feature Reference to Foreign Key](./MT020_FeatureReferenceToForeignKey.md)

### MT021: Simplified Contact

[Simplified Contact](./MT021_SimpleContact.md)

### MT022: Restrict Union Members

[Restrict Union Members](./MT022_RestrictUnionMembers.md)

### MT023: Simplified Resolution

[Simplified Resolution](./MT023_SimpleResolution.md)

### MT024: Simplified Dimension

[Simplified Dimension](./MT024_SimpleDimension.md)

### MT025: Simplified RelatedParty

[Simplified RelatedParty](./MT025_SimpleRelatedParty.md)

### MT026: Denormalize Attribute From Related Feature

[Denormalize Attribute](./MT026_DenormalizeAttribute.md)

### MT027: Extract Secondary Geometry To Feature Class

[Extract Secondary Geometry](./MT027_ExtractSecondaryGeometry.md) — moves a feature type's
second geometry (e.g. `CadastralParcel.referencePoint`) into its own spatial child feature
class (`RID` FK + geometry), since a feature class holds only one geometry.
