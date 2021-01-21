# Streamlined INSPIRE Esri GDB Alternative Encodings
This is a repository for streamlined INSPIRE Esri Geodatabase (GDB) encodings documented according to INSPIRE Implementing Rules [Article 7 -- Encodings](#art7). This repository provides access to streamlined fGDB templates, publicly available encoding rules used to encode spatial data, and examples.

## What is Alternative Encoding?
Streamlined (also referred to as simplified) INSPIRE data, enabled by Implementing Rules on interoperability of spatial data sets and services (Commission Regulation (EU) No 1089/2010, improve interoperablity and ease of use for INSPIRE data within mainstream GIS.

### This body of work
Proposals for alternative encodings rules were collected through an open call on the MIG collaboration platform and prioritised by Member State representatives in a survey. The results of the survey clearly showed support for GeoJSON as a possible alternative encoding. In addition, also simplified GML, database formats (geopackage, PostGIS, ESRI Geodatabase (GDB)) and linked data had significant support.

This body of work supports alternative encodings using Esri GDB and contributes to a larger body of work on INSPIRE alternative encodings.

The INSPIRE-MIF Repository for action 2017.2 on alternative encoings can be found [here](https://github.com/INSPIRE-MIF/2017.2), including [template for Alternative Encodings for INSPIRE Data](https://github.com/INSPIRE-MIF/2017.2/blob/master/template/template.md) used herein. The glossary for terms can be found [here](https://github.com/INSPIRE-MIF/2017.2/blob/master/glossary.md).

## INSPIRE Requirements for Encoding Rules
The Implementing Rules on interoperability of spatial data sets and services (Commission Regulation (EU) No 1089/2010) lays down the following requirements for encoding rules:

[**Article 7 -- Encoding**](#art7)
> Every encoding rule used to encode spatial data shall conform to EN ISO 19118. *In particular, it shall specify schema conversion rules for all spatial object types and all attributes and association roles and the output data structure used.
> Every encoding rule used to encode spatial data shall be made available.*

**D2.7** specifies more detailed requirements and recommendations for encoding rules. The following list lists the requirements from that document and shows which ones are also met in this encoding rule:
> Requirement 12: ... documents shall be required to be encoded using UTF-8 as character encoding.

**D2.7** also contains a relevant recommendation:
> Recommendation 3: Encoding rules should be based on international, preferably open, standards.
