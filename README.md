# Streamlined INSPIRE Esri GDB - Alternative Encodings 
This is a repository for streamlined INSPIRE Esri Geodatabase (GDB) encodings documented according to INSPIRE Implementing Rules (IRs) [Article 7 -- Encodings](#inspire-requirements-for-encoding-rules). This repository provides access to:

* publicly available encoding rules used to encode spatial data and that explain how (and under which conditions) the encoding meets the requirements of the IRs
* streamlined fGDB templates
* live [ArcGIS INSPIRE Open Data](https://arcgis-inspire-esri.opendata.arcgis.com/) demonstration Hub

Importantly, data provided in streamlined INSPIRE Esri GDBs can be used as an alternative to (i.e., instead of) the default complex INSPIRE GML encoding or in addition to the default encoding.

## Why would you want to use alternative encodings? 
For many use cases, streamlined INSPIRE data are easier to create, use, and share. The default encoding for INSPIRE is highly structured complex GML. It is widely recognized that due to complex data structures, the consumption of INSPIRE data is not easy.[[1]](#references) By applying Alternative Encoding rules, the complex data structures are simplified and flattened, resulting in streamlined INSPIRE data (also referred to as simplified INSPIRE data). Streamlined INSPIRE data have great potential to improve interoperability and ease of use within mainstream ICT and GIS applications.

INSPIRE Action 2017.2 Maintenance and Implementation Group (MIG) work programme [[2]](#referencees) laid the groundwork for Alternative Encoding by defining documentation templates and providing guidance and examples for developing alternative encodings. 

### This body of work
During action 2017.2, proposals for alternative encodings rules were collected through an open call on the MIG collaboration platform and prioritised by Member State representatives in a survey. The results of the survey clearly showed support for GeoJSON as a possible alternative encoding. In addition, simplified GML, database formats (GeoPackage, PostGIS, ESRI Geodatabase (GDB)), and linked data also had significant support.[[3]](#referencees)

This body of work addresses the proposed support for using ESRI Geodatabase (GDB) and contributes to the larger body of work on INSPIRE alternative encodings.[[4]](#referencees)

It references the INSPIRE-MIF Repository for [Action 2017.2 on alternative encodings](https://github.com/INSPIRE-MIF/2017.2), including the [template for Alternative Encodings for INSPIRE Data](https://github.com/INSPIRE-MIF/2017.2/blob/master/template/template.md) and the [glossary of terms](https://github.com/INSPIRE-MIF/2017.2/blob/master/glossary.md).

### Why GDB? 
In today's IT environment, users expect to share multiple representations and service interfaces (APIs) of the same data resource to target different users and use cases. ArcGIS makes interoperability easy through the application of international open standards and open specifications. With ArcGIS, your GDB data are easily published as GeoServices REST and shared as GeoJSON, CSV, KML, Shapefile, and fGDB. Optional additional distributions including OGC WMTS and OGC API-Features provide your INSPIRE View and Download services.

The geodatabase (GDB) is a "container" used to hold a collection of datasets. File Geodatabase (fGDB) is a subtype of GDB stored as folders in a file system. fGDB uses an efficient data structure for high performance and scalability. By default, fGDB files can grow to 1 TB, which can be changed to 4 or 256 TB using a configuration keyword.

#### fGDB Links
* [Streamlined INSPIRE GDB Templates](https://arcgis-inspire-esri.opendata.arcgis.com/pages/resources) following Alternative Encoding rules documented herein
* Additional resources about File Geodatabase
   * Learn more [about fGDB](https://pro.arcgis.com/en/pro-app/latest/help/data/geodatabases/overview/types-of-geodatabases.htm)
   * [ESRI File Geodatabase API](https://github.com/Esri/file-geodatabase-api)
   * GDAL documentation for Vector drivers » [ESRI File Geodatabase (FileGDB)](https://gdal.org/drivers/vector/filegdb.html)
   * [Working with File Geodatabases (.GBD) using QGIS and GDAL](https://gis.ucla.edu/node/53), UCLA Geospatial (2015)

## INSPIRE Requirements for Encoding Rules
The Implementing Rules on interoperability of spatial data sets and services (Commission Regulation (EU) No 1089/2010) lays down the following requirements for encoding rules:

**Article 7 -- Encoding**
> Every encoding rule used to encode spatial data shall conform to EN ISO 19118. *In particular, it shall specify schema conversion rules for all spatial object types and all attributes and association roles and the output data structure used.
> Every encoding rule used to encode spatial data shall be made available.*

**D2.7** specifies more detailed requirements and recommendations for encoding rules. The following list lists the requirements from that document and shows which ones are also met in this encoding rule:
> Requirement 12: ... documents shall be required to be encoded using UTF-8 as character encoding.

**D2.7** also contains a relevant recommendation:
> Recommendation 3: Encoding rules should be based on international, preferably open, standards.

The important thing is a complete mapping from the UML conceptual model to the encoding used and made public, as is done in this repository.

## Is the Default INSPIRE GML Encoding Still Required?
Data provided through INSPIRE Alternative Encoding can be used *instead of* the default complex INSPIRE GML encoding, or *in addition to* the default encoding.

It depends on the source data whether an encoding can be considered an alternative (or just additional). The default encoding is **not required**, so long as the simplification rules do not lead to information loss from the source data set *as compared with using the default encoding.* If the simplification rules lead to information loss from the source data set, it should be considered an "additional encoding," and the default INSPIRE GML encoding should still be used.
  
Alternative encoding should not be used to omit attributes or object types that exist in the source data.

## References
[1] INSPIRE action 2017.2 on Alternative Encodings https://inspire.ec.europa.eu/sites/default/files/inspire_alternative_encodings.pdf

[2] Action 2017.2 on alternative encodings for INSPIRE data (completed) https://webgate.ec.europa.eu/fpfis/wikis/pages/viewpage.action?pageId=277742184

[3] https://github.com/INSPIRE-MIF/2017.2/blob/master/GeoJSON/geojson-encoding-rule.md

[4] Github Action 2017.2 working space https://github.com/INSPIRE-MIF/2017.2

## Join the Esri Community
[INSPIRE Esri Community](https://community.esri.com/t5/inspire/ct-p/inspire)

## Contributing
Esri welcomes contributions from anyone and everyone. Please see our [guidelines for contributing](https://github.com/esri/contributing).

## Licensing
Copyright 2021 Esri

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

A copy of the license is available in the repository's [license.txt]( https://github.com/ArcGIS/inspire_open_data/blob/main/license.txt) file.
