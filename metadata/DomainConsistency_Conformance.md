DRAFT - Template metadata for fGDB templates
- [x] TO DO: suggest conformity explanation
- [ ] TO DO: create template MD for fGDB
- [ ] TO DO: create version of template MD to distrtibute with demo data

## Conformity explanation statement
INSPIRE Metadata must contain an explanation of conformance. The metadata ConformanceResult is used to gather metrics for INSPIRE reporting. To convey that Alternative Encoding are used to meet INSPIRE requirements for encoding rules per Article 7, this guidance document proposes the following conformity explanation statement for use in the data set **Metadata Quality Report for Domain Consistency**:

> "1. The Implementing Rules on interoperability of spatial data sets and services (Commission Regulation (EU) No 1089/2010) lays down the following requirements for encoding rules: Article 7 -- Encoding | Every encoding rule used to encode spatial data shall conform to EN ISO 19118. In particular, it shall specify schema conversion rules for all spatial object types and all attributes and association roles and the output data structure used. Every encoding rule used to encode spatial data shall be made available. D2.7 specifies more detailed requirements and recommendations for encoding rules. The following list lists the requirements from that document and shows which ones are also met in this encoding rule: Requirement 12: ... documents shall be required to be encoded using UTF-8 as character encoding. D2.7 also contains a relevant recommendation: Recommendation  3: Encoding rules should be based on international, preferably open, standards | INSPIRE Action 2017.2 Alternative Encoding set the pattern for conformity of spatial data sets and services per Article 7; Data herein use ‘Streamlined INSPIRE Esri GDB Alternative Encoding’; every encoding rule used is available at https://github.com/ArcGIS/Inspire_Open_Data | 
> 2. Conformity of network services (i.e., Download and View Services) per Action 2019.2: ‘Improving accessibility of data sets through network services’ - Simplification of data-service linkages; and per Action 2018.1: ‘Streamlining the monitoring and reporting for 2019’ identification of the type of network services may be based on the definition of the service access points as defined in data set metadata"

### Where the statement is used
Item metadata can be edited in the ArcGIS Online Metadata editor. This example shows how the statement would appear in the resulting INSPIRE XML metadata:
```
<gmd:report>
  <gmd:DQ_DomainConsistency>
    <gmd:result>
      <gmd:DQ_ConformanceResult>
      ...
        <gmd:explanation>
<gco:CharacterString>1. Conformity of spatial data sets and services per INSPIRE Action 2017.2 Alternative Encoding - The Implementing Rules on interoperability of spatial data sets and services (Commission Regulation (EU) No 1089/2010) lays down the following requirements for encoding rules: Article 7 -- Encoding | Every encoding rule used to encode spatial data shall conform to EN ISO 19118. In particular, it shall specify schema conversion rules for all spatial object types and all attributes and association roles and the output data structure used. Every encoding rule used to encode spatial data shall be made available. D2.7 specifies more detailed requirements and recommendations for encoding rules. The following list lists the requirements from that document and shows which ones are also met in this encoding rule: Requirement 12: ... documents shall be required to be encoded using UTF-8 as character encoding. D2.7 also contains a relevant recommendation: Recommendation 3: Encoding rules should be based on international, preferably open, standards | Data herein use ‘Streamlined INSPIRE Esri GDB Alternative Encoding’; every encoding rule used is available at https://github.com/ArcGIS/Inspire_Open_Data | 2. Conformity of network services (i.e., Download and View Services) per Action 2019.2: ‘Improving accessibility of data sets through network services’ - Simplification of data-service linkages; and per Action 2018.1: ‘Streamlining the monitoring and reporting for 2019’ identification of the type of network services may be based on the definition of the service access points as defined in data set metadata</gco:CharacterString>
        </gmd:explanation>
```
## Guidance for data providers regarding conformance
Data providers are responsible for the conformance of their data to INSPIRE Implementing Rules on interoperability of spatial data sets and services (Commission Regulation (EU) No 1089/2010). ArcGIS INSPIRE Open Data enables the creation of spatial data sets and services using Alternative Encoding rules for Esri GDB. The following guidance can help you determine conformance:

- IF you load your source data into the target fGDB template and complete the necessary INSPIRE attributes,
- AND confirm there is no loss of data using Alternative Encoding when compared with using the INSPIRE default complex GML encoding,
- AND publish a Feature Layer and a Tile Layer from your hosted Feature Layer to automatically generate the INSPIRE Download and View Services,
- AND update the dataset and services metadata with Additional Distributions and pass the INSPIRE Reference Validator,
- THEN the spatial data sets and services provided can be considered confomant to the Alternative Encosing per the conformance explanation statement.

Finally, share your INSPIRE spatial data sets and services using Hub Open Data to fulfill your obligations under the PSI-2/Open Data Directive.

## Learn how
Ready to learn how? ArcGIS INSPIRE Open Data is a freely available solution to use with ArcGIS. Step-by-step tutorials are available to guide you through the process [Follow the Learn Path](https://linktoLearnPath)
