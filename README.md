# Streamlined INSPIRE Esri GDB - Alternative Encodings 
This is a repository for streamlined INSPIRE Esri Geodatabase (GDB) encodings documented according to INSPIRE Implementing Rules (IRs) [Article 7 -- Encodings](#inspire-requirements-for-encoding-rules). This repository provides access to:
* streamlined fGDB templates and hosted Feature layer templates
* publicly available encoding rules used to encode spatial data and that explain how (and/or under which conditions) the encoding meets the requirements of the IRs
* examples

Importantly, data provided in streamlined INSPIRE Esri GDBs can be used as an alternative to (i.e., instead of) the default complex INSPIRE GML encoding, or in addition to the default encoding.

## Why would you want to use alternative encodings? 
For many use cases, streamlined INSPIRE data are easier to create, use, and share. The default encoding for INSPIRE is highly structured complex GML. It is widely recognized that due to complex data structures the consumption of INSPIRE data is not easy.[[1]](#referencees) By applying Alternative Encoding rules, the complex data structures are simplified and flattened, resulting in streamlined INSPIRE data (also referred to as simplified INSPIRE data). Streamlined INSPIRE data have great potential to improve interoperablity and ease of use within mainstream ICT and GIS applications.

INSPIRE Action 2017.2 maintenance and implementation work programme [[2]](#referencees) laid the groundwork for Alternative Encoding by defining documentation templates and providing guidance and examples for developing alternative encodings. 

### This body of work
During action 2017.2, proposals for alternative encodings rules were collected through an open call on the MIG collaboration platform and prioritised by Member State representatives in a survey. The results of the survey clearly showed support for GeoJSON as a possible alternative encoding. In addition, also simplified GML, database formats (geopackage, PostGIS, ESRI Geodatabase (GDB)) and linked data had significant support.[[3]](#referencees)

This body of work addresses the support for using ESRI Geodatabase (GDB) and contributes to the larger body of work on INSPIRE alternative encodings.[[4]](#referencees)

Why fGDB... benefits and target use case... easy to use and share... for example, make it easy to share on the web as feature layers, GeoJSON, shapefile, GeoPackage, and more...

The INSPIRE-MIF Repository for action 2017.2 on alternative encoings can be found [here](https://github.com/INSPIRE-MIF/2017.2), including [template for Alternative Encodings for INSPIRE Data](https://github.com/INSPIRE-MIF/2017.2/blob/master/template/template.md) used herein. The glossary for terms can be found [here](https://github.com/INSPIRE-MIF/2017.2/blob/master/glossary.md).

## INSPIRE Requirements for Encoding Rules
The Implementing Rules on interoperability of spatial data sets and services (Commission Regulation (EU) No 1089/2010) lays down the following requirements for encoding rules:

**Article 7 -- Encoding**
> Every encoding rule used to encode spatial data shall conform to EN ISO 19118. *In particular, it shall specify schema conversion rules for all spatial object types and all attributes and association roles and the output data structure used.
> Every encoding rule used to encode spatial data shall be made available.*

**D2.7** specifies more detailed requirements and recommendations for encoding rules. The following list lists the requirements from that document and shows which ones are also met in this encoding rule:
> Requirement 12: ... documents shall be required to be encoded using UTF-8 as character encoding.

**D2.7** also contains a relevant recommendation:
> Recommendation 3: Encoding rules should be based on international, preferably open, standards.

The important thing is that a complete mapping from the UML conceptual model to the encoding used and made public, as is done in this repository.

## Is the Default INSPIRE GML Encoding Still Required?

Data provided through INSPIRE Alternative Encoding can be used *instead of* the default complex INSPIRE GML encoding, or *in addition to* the default encoding.

It depends on the source data whether an encoding can be considered alternative (or just additional). The default encoding is **not required**, so long as the simplification rules do not lead to information loss from the source data set *as compared with using the ddefault encoding.* If the simplification rules lead to information loss from the source data set, it should be considered an "additional encoding" and the default INSPIRE GML encoding should still be used.
  
The alternative encoding should not be used to omit attributes or object types that exist in the source data.

## References
[1] INSPIRE action 2017.2 on Alternative Encodings https://inspire.ec.europa.eu/sites/default/files/inspire_alternative_encodings.pdf

[2] Action 2017.2 on alternative encodings for INSPIRE data (completed) https://webgate.ec.europa.eu/fpfis/wikis/pages/viewpage.action?pageId=277742184

[3] https://github.com/INSPIRE-MIF/2017.2/blob/master/GeoJSON/geojson-encoding-rule.md

[4] Github Action 2017.2 working space https://github.com/INSPIRE-MIF/2017.2


