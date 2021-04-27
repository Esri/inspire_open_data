# Model Transformations GDB

## Introduction

This document uses the [TransformationRules](`https://github.com/INSPIRE-MIF/2017.2/blob/master/model-transformations/TransformationRules.md`) developed under [MIF action 2017.2](`https://github.com/INSPIRE-MIF/2017.2`) and adds additional rules to meet the requiements of a transformation to file geodatabase.  

These Rules were used to create the alternative encodings for ESRI Geodatabase under [Model Transformations](./TransformationRules.md) The intent of this document is to describe multiple model transformation methods. These methods reduce complexity in encoded INSPIRE data, e.g. by reducing levels of aggregation, indirect referencing, using simple geometries and flattening structures such as arrays. As with alternate encodings, they have different objectives and scopes. A rule may be used with any number of encodings, including the default encoding, if applicable.

An Alternate encoding may refer to any number of such model transformation rules in its conformance classes. For this purpose, each model transformation rules receives a unique identifier. For an Alternate encoding to be the sole encoding, there may not be any information loss for the particular data set in question.

## Requirements for Model Transformations

We describe each Model Transformation by using these properties:

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
- Examples of use (Links to issues in the 2017.2 repository)
- Additional notes and enhancements

## Catalogue of simplifying Model Transformations

This section contains a selection of examples for model transformations we have identified so far. 

The catalogue also contains several substitution rules, where existing types such as `GeographicName` are replaced with less complex types. These types are added to the theme namespaces under draft schemas  (`https://inspire.ec.europa.eu/draft-schemas/`).

### MT001: Flattening of nested structures

[General Flattening of nested structures](./GeneralFlattening.md)

### MT002: Extract Primitive Arrays

[Extract Primitive Array](./ExtractPrimitiveArray.md)

### MT003: Association/Aggregation to Composition with Hard Typing

[Association/Aggregation to Composition with Hard Typing](./AssociatedComponentsHardType.md)

### MT004: Association/Aggregation to Composition with Soft Typing

[Association/Aggregation to Composition with Soft Typing](./AssociatedComponentsSoftType.md)

### MT006: Property Composition to Association

[Property Composition to Association](./PropertyCompositionToAssociation.md)


### MT005: Simple Geographic Name

[Simple Geographic Name](./SimpleGeographicName.md)

### MT007: Simple Citation

[Simple Citation](./SimpleCitation.md)

### MT008: Simple Codelist Reference

[Simple Codelist Reference](./SimpleCodelistReference.md)

### MT009: Simple Period

[Simple Period](./SimplePeriod.md)

### MT010: Simple Free Text

[Simple Free Text](./SimplePT_FreeText.md)

### MT011: Simple TM_Period

[Simple TM_Period](./SimpleTM_Period.md)

### MT012: Simple Related Party

[Simple RelatedParty](./SimpleRelatedParty.md)

### MT013: Homogeneous Geometry

[Homogeneous Geometry](./HomogeneousGeometry.md)

### MT014: One To Many Relationships As Extra Table

[One To Many Relationships As Extra Table](./OneToManyRelationshipsAsExtraTable.md)


### MT015: Many To Many Relationships As Link Table

[One To Many Relationships As Extra Table](./ManyToManyRelationshipsAsLinkTable.md)
