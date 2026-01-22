
#HabitatsAndBiotopes


<br/>
<strong>Geodatabase Documentation</strong>
<hr/>
<strong>Date: </strong>20251120120738.9636533<br/>
<hr/>
<p><strong>Summary Information and Links</strong><br/><br/><a href="#FeatureDatasets">0 Feature Datasets and 3
Feature Classes</a><br/>No Topology Datasets<br/>No Geometric Networks<br/>No Rasters<br/><a href="#ObjectClasses">0 Tables (Object Classes)</a><br/><a href="#RelationshipClasses">0 Relationship
Classes</a><br/><a href="#Domains">6 Domains</a><br/></p>
<hr/>
<p><a name="FeatureDatasets"/><strong>Feature Datasets and Child Classes</strong></p><a name="Raster"/>
<p><strong>Rasters</strong></p><br/>
<hr/><a name="ObjectClasses"/>
<p><strong>Workspace-Level Tables and Feature Classes</strong></p>
    <a href="#FeatureClassHabitatL">HabitatL - FeatureClass</a><br/><a href="#FeatureClassHabitatP">HabitatP - FeatureClass</a><br/><a href="#FeatureClassHabitatS">HabitatS - FeatureClass</a><br/>
<p/><br/>
<hr/><a name="RelationshipClasses"/>
<p><strong>Relationship Classes</strong></p><p/>
<hr/><br/><a name="Domains"/>
<p><strong>Domains</strong></p>
   <a href="#DomainQualifierLocalNameValue">QualifierLocalNameValue</a><br/><a href="#DomainQualifierLocalNameValue_value">QualifierLocalNameValue_value</a><br/><a href="#DomainReferenceHabitatTypeSchemeValue">ReferenceHabitatTypeSchemeValue</a><br/><a href="#DomainReferenceHabitatTypeSchemeValue_value">ReferenceHabitatTypeSchemeValue_value</a><br/><a href="#DomainReferenceSpeciesSchemeValue">ReferenceSpeciesSchemeValue</a><br/><a href="#DomainReferenceSpeciesSchemeValue_value">ReferenceSpeciesSchemeValue_value</a><br/>
    <p><hr/><br/><a name="FeatureClassHabitatL"/>
<p><strong>HabitatL - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">HabitatL</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>ShapeType</strong></td>
<td width="*" style="border-color: white">Polyline</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FeatureType</strong></td>
<td width="*" style="border-color: white">Simple</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">HabitatL</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>HasM</strong></td>
<td width="*" style="border-color: white">false</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>HasZ</strong></td>
<td width="*" style="border-color: white">false</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>HasAttachments</strong></td>
<td width="*" style="border-color: white">false</td>
</tr>
</tbody>
</table>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Description</strong></td>
<td width="*" style="border-color: white">HabitatL</td>
</tr>
</tbody>
</table><br/>
<table width="100%">
<tbody>
<tr style="border:0px">
<td width="8%" style="border:0px"><strong>Field</strong></td>
<td width="8%" style="border:0px"><strong>DataType</strong></td>
<td width="5%" style="border:0px"><strong>Length</strong></td>
<td width="8%" style="border:0px"><strong>AliasName</strong></td>
<td width="8%" style="border:0px"><strong>Description</strong></td>
<td width="8%" style="border:0px"><strong>Domain</strong></td>
<td width="8%" style="border:0px"><strong>DefaultValue</strong></td>
<td width="8%" style="border:0px"><strong>IsNullable</strong></td>
<td width="5%" style="border:0px"><strong>Precision</strong></td>
<td width="5%" style="border:0px"><strong>Scale</strong></td>
</tr>
<tr>
<td width="8%">OBJECTID</td>
<td width="8%">OID</td>
<td width="3%">4</td>
<td width="8%">OBJECTID</td>
<td width="8%"/>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">SHAPE</td>
<td width="8%">Geometry</td>
<td width="3%">0</td>
<td width="8%">SHAPE</td>
<td width="8%"/>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">featureId</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">featureId</td>
<td width="8%">A local identifier, assigned by the data provider. The local identifier is unique within the namespace, that is no other spatial object carries the same unique identifier.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_areaCovered</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">h_areaCovered</td>
<td width="8%">(habitat.HabitatTypeCoverType.areaCovered): The area covered by a certain habitat type within the provided geometry of the habitat spatial object. The surface area should be expressed in square meters.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_areaCovered_uom</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_areaCovered_uom</td>
<td width="8%">(habitat.HabitatTypeCoverType.areaCovered.uom): Units used for measuring area in this measure.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_l_localName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_l_localName</td>
<td width="8%">(habitat.HabitatTypeCoverType.localHabitatName.LocalNameType.localName): Name according to a local classification scheme.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_l_localNameCode</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_l_localNameCode</td>
<td width="8%">(habitat.HabitatTypeCoverType.localHabitatName.LocalNameType.localNameCode): Natural language name according to a local classification scheme.</td>
<td width="8%"><a href="#DomainLocalNameCodeValue_value">LocalNameCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_l_localNameCode_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_l_localNameCode_href</td>
<td width="8%">URI from the INSPIRE code list register - LocalNameCodeValue <a href="https://inspire.ec.europa.eu/codelist/LocalNameCodeValue">https://inspire.ec.europa.eu/codelist/LocalNameCodeValue</a></td>
<td width="8%"><a href="#DomainLocalNameCodeValue">LocalNameCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_l_localScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_l_localScheme</td>
<td width="8%">(habitat.HabitatTypeCoverType.localHabitatName.LocalNameType.localScheme): Uniform resource identifier of a local classification scheme. Classification scheme, which is used locally and contains all classification types, their codes and/or  very often their names in natural language.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_l_qualifierLocalName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_l_qualifierLocalName</td>
<td width="8%">(habitat.HabitatTypeCoverType.localHabitatName.LocalNameType.qualifierLocalName): The relation between the local name and the corresponding name in the Pan-European schema. EXAMPLE The local habitat type can be conceptually the same as the related Pan-European habitat type, the relationship then is called “congruent”   or  the local habitat type may be a subtype of the Pan-European habitat type, therefore the relationship should be "includedIn", etc.</td>
<td width="8%"><a href="#DomainQualifierLocalNameValue_value">QualifierLocalNameValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_l_qualifierLocalName_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_l_qualifierLocalName_href</td>
<td width="8%">URI from the INSPIRE code list register - QualifierLocalNameValue <a href="https://inspire.ec.europa.eu/codelist/QualifierLocalNameValue">https://inspire.ec.europa.eu/codelist/QualifierLocalNameValue</a></td>
<td width="8%"><a href="#DomainQualifierLocalNameValue">QualifierLocalNameValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_lengthCovered</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">h_lengthCovered</td>
<td width="8%">(habitat.HabitatTypeCoverType.lengthCovered): The length covered by a certain habitat type within the provided geometry of the habitat spatial object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_lengthCovered_uom</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_lengthCovered_uom</td>
<td width="8%">(habitat.HabitatTypeCoverType.lengthCovered.uom): Units used for measuring length in this measure.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_rHabitatTypeId</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_rHabitatTypeId</td>
<td width="8%">(habitat.HabitatTypeCoverType.referenceHabitatTypeId): Habitat type unique identifier (code) according to one Pan-European classification scheme. EXAMPLE "1110", "40C0", "95A0", etc., if the referenceHabitatScheme is "habitatsDirective", or "A1.111", "A1.1121", "G1.1111", "X34", etc., if the ReferenceHabitatScheme is "eunis"</td>
<td width="8%"><a href="#DomainReferenceHabitatTypeCodeValue_value">ReferenceHabitatTypeCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_rHabitatTypeId_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_rHabitatTypeId_href</td>
<td width="8%">URI from the INSPIRE code list register - ReferenceHabitatTypeCodeValue <a href="https://inspire.ec.europa.eu/codelist/ReferenceHabitatTypeCodeValue">https://inspire.ec.europa.eu/codelist/ReferenceHabitatTypeCodeValue</a></td>
<td width="8%"><a href="#DomainReferenceHabitatTypeCodeValue">ReferenceHabitatTypeCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_rHabitatTypeName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_rHabitatTypeName</td>
<td width="8%">(habitat.HabitatTypeCoverType.referenceHabitatTypeName): Name of a habitat type according to one Pan-European classification scheme. In the given Pan-European habitat classification systems, the habitat types can be identified by both: a short "identifier" (code)  and  a name in natural language, which is meant in this attribute. EXAMPLE Habitats Directive habitat type 3260 (code) "Floating vegetation of Ranunculus" or "Chenopodietum rubri of submountainous rivers" (name).</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_rHabitatTypeScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_rHabitatTypeScheme</td>
<td width="8%">(habitat.HabitatTypeCoverType.referenceHabitatTypeScheme): One of the Pan-European classification schemes, that are widely used in Europe. The list includes at least the classification of the natural habitat types of community interest listed in Annex I of the Habitats Directive, as well as the hierarchic classification of the habitat types of interest for biodiversity and nature protection listed in the EUNIS database, which is maintained by the EEA.</td>
<td width="8%"><a href="#DomainReferenceHabitatTypeSchemeValue_value">ReferenceHabitatTypeSchemeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_rHabitatTypeScheme_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_rHabitatTypeScheme_href</td>
<td width="8%">URI from the INSPIRE code list register - ReferenceHabitatTypeSchemeValue <a href="https://inspire.ec.europa.eu/codelist/ReferenceHabitatTypeSchemeValue">https://inspire.ec.europa.eu/codelist/ReferenceHabitatTypeSchemeValue</a></td>
<td width="8%"><a href="#DomainReferenceHabitatTypeSchemeValue">ReferenceHabitatTypeSchemeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_volumeCovered</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">h_volumeCovered</td>
<td width="8%">(habitat.HabitatTypeCoverType.volumeCovered): The volume covered by a certain habitat type within the provided geometry of the habitat spatial object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_volumeCovered_uom</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_volumeCovered_uom</td>
<td width="8%">(habitat.HabitatTypeCoverType.volumeCovered.uom): Units used for measuring volume in this measure.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_l_localName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_l_localName</td>
<td width="8%">(habitatSpecies.HabitatSpeciesType.localSpeciesName.LocalNameType.localName): Name according to a local classification scheme.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_l_localNameCode</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_l_localNameCode</td>
<td width="8%">(habitatSpecies.HabitatSpeciesType.localSpeciesName.LocalNameType.localNameCode): Natural language name according to a local classification scheme.</td>
<td width="8%"><a href="#DomainLocalNameCodeValue_value">LocalNameCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_l_localNameCode_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_l_localNameCode_href</td>
<td width="8%">URI from the INSPIRE code list register - LocalNameCodeValue <a href="https://inspire.ec.europa.eu/codelist/LocalNameCodeValue">https://inspire.ec.europa.eu/codelist/LocalNameCodeValue</a></td>
<td width="8%"><a href="#DomainLocalNameCodeValue">LocalNameCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_l_localScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_l_localScheme</td>
<td width="8%">(habitatSpecies.HabitatSpeciesType.localSpeciesName.LocalNameType.localScheme): Uniform resource identifier of a local classification scheme. Classification scheme, which is used locally and contains all classification types, their codes and/or  very often their names in natural language.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_l_qualifierLocalName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_l_qualifierLocalName</td>
<td width="8%">(habitatSpecies.HabitatSpeciesType.localSpeciesName.LocalNameType.qualifierLocalName): The relation between the local name and the corresponding name in the Pan-European schema. EXAMPLE The local habitat type can be conceptually the same as the related Pan-European habitat type, the relationship then is called “congruent”   or  the local habitat type may be a subtype of the Pan-European habitat type, therefore the relationship should be "includedIn", etc.</td>
<td width="8%"><a href="#DomainQualifierLocalNameValue_value">QualifierLocalNameValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_l_qualifierLocalName_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_l_qualifierLocalName_href</td>
<td width="8%">URI from the INSPIRE code list register - QualifierLocalNameValue <a href="https://inspire.ec.europa.eu/codelist/QualifierLocalNameValue">https://inspire.ec.europa.eu/codelist/QualifierLocalNameValue</a></td>
<td width="8%"><a href="#DomainQualifierLocalNameValue">QualifierLocalNameValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_rSpeciesId</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_rSpeciesId</td>
<td width="8%">(habitatSpecies.HabitatSpeciesType.referenceSpeciesId): Identifier of one of the reference lists given by the referenceSpeciesScheme.</td>
<td width="8%"><a href="#DomainReferenceSpeciesCodeValue_value">ReferenceSpeciesCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_rSpeciesId_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_rSpeciesId_href</td>
<td width="8%">URI from the INSPIRE code list register - ReferenceSpeciesCodeValue <a href="https://inspire.ec.europa.eu/codelist/ReferenceSpeciesCodeValue">https://inspire.ec.europa.eu/codelist/ReferenceSpeciesCodeValue</a></td>
<td width="8%"><a href="#DomainReferenceSpeciesCodeValue">ReferenceSpeciesCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_rSpeciesScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_rSpeciesScheme</td>
<td width="8%">(habitatSpecies.HabitatSpeciesType.referenceSpeciesScheme): Reference list defining a nomenclatural and taxonomical standard to which all local species names and taxonomic concepts shall be mapped to. Closed codelist of accepted PAN-european taxonomical reference lists defining the nomenclature and taxonomical concept of a given species name. This must not be regarded as the ultimate taxonomic truth: this will always change. It serves as a definition of a taxonomic concept described by systematic and synonym relations where other names and there inherent taxonomic concepts can be mapped to. The code list comprises of Eu-Nomen, EUNIS and Natura2000. In these sources harmonized species GUIDs and names are maintained by institutions with an assignment outside INSPIRE and the species names are to be retrieved through webservices using GUIDs. Only one of these list must be used for one taxon. The priority is as follows: 1) EU-Nomen, 2) EUNIS, 3) NatureDirectives. This implies: if a taxon is listed in EU-Nomen, this reference must be used as first choice. If it is not listed in EU-Nomen, the second choice is EUNIS, if not in EUNIS, NatureDirectives can be used.</td>
<td width="8%"><a href="#DomainReferenceSpeciesSchemeValue_value">ReferenceSpeciesSchemeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_rSpeciesScheme_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_rSpeciesScheme_href</td>
<td width="8%">URI from the INSPIRE code list register - ReferenceSpeciesSchemeValue <a href="https://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue">https://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue</a></td>
<td width="8%"><a href="#DomainReferenceSpeciesSchemeValue">ReferenceSpeciesSchemeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hVeg_localName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hVeg_localName</td>
<td width="8%">(habitatVegetation.HabitatVegetationType.localVegetationName.LocalNameType.localName): Name according to a local classification scheme.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hVeg_localNameCode</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hVeg_localNameCode</td>
<td width="8%">(habitatVegetation.HabitatVegetationType.localVegetationName.LocalNameType.localNameCode): Natural language name according to a local classification scheme.</td>
<td width="8%"><a href="#DomainLocalNameCodeValue_value">LocalNameCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hVeg_localNameCode_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hVeg_localNameCode_href</td>
<td width="8%">URI from the INSPIRE code list register - LocalNameCodeValue <a href="https://inspire.ec.europa.eu/codelist/LocalNameCodeValue">https://inspire.ec.europa.eu/codelist/LocalNameCodeValue</a></td>
<td width="8%"><a href="#DomainLocalNameCodeValue">LocalNameCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hVeg_localScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hVeg_localScheme</td>
<td width="8%">(habitatVegetation.HabitatVegetationType.localVegetationName.LocalNameType.localScheme): Uniform resource identifier of a local classification scheme. Classification scheme, which is used locally and contains all classification types, their codes and/or  very often their names in natural language.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hVeg_qualifierLocalName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hVeg_qualifierLocalName</td>
<td width="8%">(habitatVegetation.HabitatVegetationType.localVegetationName.LocalNameType.qualifierLocalName): The relation between the local name and the corresponding name in the Pan-European schema. EXAMPLE The local habitat type can be conceptually the same as the related Pan-European habitat type, the relationship then is called “congruent”   or  the local habitat type may be a subtype of the Pan-European habitat type, therefore the relationship should be "includedIn", etc.</td>
<td width="8%"><a href="#DomainQualifierLocalNameValue_value">QualifierLocalNameValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hVeg_qualifierLocalName_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hVeg_qualifierLocalName_href</td>
<td width="8%">URI from the INSPIRE code list register - QualifierLocalNameValue <a href="https://inspire.ec.europa.eu/codelist/QualifierLocalNameValue">https://inspire.ec.europa.eu/codelist/QualifierLocalNameValue</a></td>
<td width="8%"><a href="#DomainQualifierLocalNameValue">QualifierLocalNameValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inspireId_localId</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">inspireId_localId</td>
<td width="8%">A local identifier, assigned by the data provider. The local identifier is unique within the namespace, that is no other spatial object carries the same unique identifier.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inspireId_namespace</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">inspireId_namespace</td>
<td width="8%">Namespace uniquely identifying the data source of the spatial object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inspireId_versionId</td>
<td width="8%">String</td>
<td width="3%">25</td>
<td width="8%">inspireId_versionId</td>
<td width="8%">The identifier of the particular version of the spatial object, with a maximum length of 25 characters. If the specification of a spatial object type with an external object identifier includes life-cycle information, the version identifier is used to distinguish between the different versions of a spatial object. Within the set of all versions of a spatial object, the version identifier is unique</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">SHAPE_Length</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">SHAPE_Length</td>
<td width="8%"/>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p></p><p><hr/><br/><a name="FeatureClassHabitatP"/>
<p><strong>HabitatP - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">HabitatP</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>ShapeType</strong></td>
<td width="*" style="border-color: white">Point</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FeatureType</strong></td>
<td width="*" style="border-color: white">Simple</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">HabitatP</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>HasM</strong></td>
<td width="*" style="border-color: white">false</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>HasZ</strong></td>
<td width="*" style="border-color: white">false</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>HasAttachments</strong></td>
<td width="*" style="border-color: white">false</td>
</tr>
</tbody>
</table>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Description</strong></td>
<td width="*" style="border-color: white">HabitatP</td>
</tr>
</tbody>
</table><br/>
<table width="100%">
<tbody>
<tr style="border:0px">
<td width="8%" style="border:0px"><strong>Field</strong></td>
<td width="8%" style="border:0px"><strong>DataType</strong></td>
<td width="5%" style="border:0px"><strong>Length</strong></td>
<td width="8%" style="border:0px"><strong>AliasName</strong></td>
<td width="8%" style="border:0px"><strong>Description</strong></td>
<td width="8%" style="border:0px"><strong>Domain</strong></td>
<td width="8%" style="border:0px"><strong>DefaultValue</strong></td>
<td width="8%" style="border:0px"><strong>IsNullable</strong></td>
<td width="5%" style="border:0px"><strong>Precision</strong></td>
<td width="5%" style="border:0px"><strong>Scale</strong></td>
</tr>
<tr>
<td width="8%">OBJECTID</td>
<td width="8%">OID</td>
<td width="3%">4</td>
<td width="8%">OBJECTID</td>
<td width="8%"/>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">SHAPE</td>
<td width="8%">Geometry</td>
<td width="3%">0</td>
<td width="8%">SHAPE</td>
<td width="8%"/>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">featureId</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">featureId</td>
<td width="8%">A local identifier, assigned by the data provider. The local identifier is unique within the namespace, that is no other spatial object carries the same unique identifier.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_areaCovered</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">h_areaCovered</td>
<td width="8%">(habitat.HabitatTypeCoverType.areaCovered): The area covered by a certain habitat type within the provided geometry of the habitat spatial object. The surface area should be expressed in square meters.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_areaCovered_uom</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_areaCovered_uom</td>
<td width="8%">(habitat.HabitatTypeCoverType.areaCovered.uom): Units used for measuring area in this measure.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_l_localName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_l_localName</td>
<td width="8%">(habitat.HabitatTypeCoverType.localHabitatName.LocalNameType.localName): Name according to a local classification scheme.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_l_localNameCode</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_l_localNameCode</td>
<td width="8%">(habitat.HabitatTypeCoverType.localHabitatName.LocalNameType.localNameCode): Natural language name according to a local classification scheme.</td>
<td width="8%"><a href="#DomainLocalNameCodeValue_value">LocalNameCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_l_localNameCode_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_l_localNameCode_href</td>
<td width="8%">URI from the INSPIRE code list register - LocalNameCodeValue <a href="https://inspire.ec.europa.eu/codelist/LocalNameCodeValue">https://inspire.ec.europa.eu/codelist/LocalNameCodeValue</a></td>
<td width="8%"><a href="#DomainLocalNameCodeValue">LocalNameCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_l_localScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_l_localScheme</td>
<td width="8%">(habitat.HabitatTypeCoverType.localHabitatName.LocalNameType.localScheme): Uniform resource identifier of a local classification scheme. Classification scheme, which is used locally and contains all classification types, their codes and/or  very often their names in natural language.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_l_qualifierLocalName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_l_qualifierLocalName</td>
<td width="8%">(habitat.HabitatTypeCoverType.localHabitatName.LocalNameType.qualifierLocalName): The relation between the local name and the corresponding name in the Pan-European schema. EXAMPLE The local habitat type can be conceptually the same as the related Pan-European habitat type, the relationship then is called “congruent”   or  the local habitat type may be a subtype of the Pan-European habitat type, therefore the relationship should be "includedIn", etc.</td>
<td width="8%"><a href="#DomainQualifierLocalNameValue_value">QualifierLocalNameValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_l_qualifierLocalName_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_l_qualifierLocalName_href</td>
<td width="8%">URI from the INSPIRE code list register - QualifierLocalNameValue <a href="https://inspire.ec.europa.eu/codelist/QualifierLocalNameValue">https://inspire.ec.europa.eu/codelist/QualifierLocalNameValue</a></td>
<td width="8%"><a href="#DomainQualifierLocalNameValue">QualifierLocalNameValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_lengthCovered</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">h_lengthCovered</td>
<td width="8%">(habitat.HabitatTypeCoverType.lengthCovered): The length covered by a certain habitat type within the provided geometry of the habitat spatial object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_lengthCovered_uom</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_lengthCovered_uom</td>
<td width="8%">(habitat.HabitatTypeCoverType.lengthCovered.uom): Units used for measuring length in this measure.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_rHabitatTypeId</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_rHabitatTypeId</td>
<td width="8%">(habitat.HabitatTypeCoverType.referenceHabitatTypeId): Habitat type unique identifier (code) according to one Pan-European classification scheme. EXAMPLE "1110", "40C0", "95A0", etc., if the referenceHabitatScheme is "habitatsDirective", or "A1.111", "A1.1121", "G1.1111", "X34", etc., if the ReferenceHabitatScheme is "eunis"</td>
<td width="8%"><a href="#DomainReferenceHabitatTypeCodeValue_value">ReferenceHabitatTypeCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_rHabitatTypeId_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_rHabitatTypeId_href</td>
<td width="8%">URI from the INSPIRE code list register - ReferenceHabitatTypeCodeValue <a href="https://inspire.ec.europa.eu/codelist/ReferenceHabitatTypeCodeValue">https://inspire.ec.europa.eu/codelist/ReferenceHabitatTypeCodeValue</a></td>
<td width="8%"><a href="#DomainReferenceHabitatTypeCodeValue">ReferenceHabitatTypeCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_rHabitatTypeName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_rHabitatTypeName</td>
<td width="8%">(habitat.HabitatTypeCoverType.referenceHabitatTypeName): Name of a habitat type according to one Pan-European classification scheme. In the given Pan-European habitat classification systems, the habitat types can be identified by both: a short "identifier" (code)  and  a name in natural language, which is meant in this attribute. EXAMPLE Habitats Directive habitat type 3260 (code) "Floating vegetation of Ranunculus" or "Chenopodietum rubri of submountainous rivers" (name).</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_rHabitatTypeScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_rHabitatTypeScheme</td>
<td width="8%">(habitat.HabitatTypeCoverType.referenceHabitatTypeScheme): One of the Pan-European classification schemes, that are widely used in Europe. The list includes at least the classification of the natural habitat types of community interest listed in Annex I of the Habitats Directive, as well as the hierarchic classification of the habitat types of interest for biodiversity and nature protection listed in the EUNIS database, which is maintained by the EEA.</td>
<td width="8%"><a href="#DomainReferenceHabitatTypeSchemeValue_value">ReferenceHabitatTypeSchemeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_rHabitatTypeScheme_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_rHabitatTypeScheme_href</td>
<td width="8%">URI from the INSPIRE code list register - ReferenceHabitatTypeSchemeValue <a href="https://inspire.ec.europa.eu/codelist/ReferenceHabitatTypeSchemeValue">https://inspire.ec.europa.eu/codelist/ReferenceHabitatTypeSchemeValue</a></td>
<td width="8%"><a href="#DomainReferenceHabitatTypeSchemeValue">ReferenceHabitatTypeSchemeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_volumeCovered</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">h_volumeCovered</td>
<td width="8%">(habitat.HabitatTypeCoverType.volumeCovered): The volume covered by a certain habitat type within the provided geometry of the habitat spatial object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_volumeCovered_uom</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_volumeCovered_uom</td>
<td width="8%">(habitat.HabitatTypeCoverType.volumeCovered.uom): Units used for measuring volume in this measure.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_l_localName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_l_localName</td>
<td width="8%">(habitatSpecies.HabitatSpeciesType.localSpeciesName.LocalNameType.localName): Name according to a local classification scheme.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_l_localNameCode</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_l_localNameCode</td>
<td width="8%">(habitatSpecies.HabitatSpeciesType.localSpeciesName.LocalNameType.localNameCode): Natural language name according to a local classification scheme.</td>
<td width="8%"><a href="#DomainLocalNameCodeValue_value">LocalNameCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_l_localNameCode_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_l_localNameCode_href</td>
<td width="8%">URI from the INSPIRE code list register - LocalNameCodeValue <a href="https://inspire.ec.europa.eu/codelist/LocalNameCodeValue">https://inspire.ec.europa.eu/codelist/LocalNameCodeValue</a></td>
<td width="8%"><a href="#DomainLocalNameCodeValue">LocalNameCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_l_localScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_l_localScheme</td>
<td width="8%">(habitatSpecies.HabitatSpeciesType.localSpeciesName.LocalNameType.localScheme): Uniform resource identifier of a local classification scheme. Classification scheme, which is used locally and contains all classification types, their codes and/or  very often their names in natural language.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_l_qualifierLocalName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_l_qualifierLocalName</td>
<td width="8%">(habitatSpecies.HabitatSpeciesType.localSpeciesName.LocalNameType.qualifierLocalName): The relation between the local name and the corresponding name in the Pan-European schema. EXAMPLE The local habitat type can be conceptually the same as the related Pan-European habitat type, the relationship then is called “congruent”   or  the local habitat type may be a subtype of the Pan-European habitat type, therefore the relationship should be "includedIn", etc.</td>
<td width="8%"><a href="#DomainQualifierLocalNameValue_value">QualifierLocalNameValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_l_qualifierLocalName_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_l_qualifierLocalName_href</td>
<td width="8%">URI from the INSPIRE code list register - QualifierLocalNameValue <a href="https://inspire.ec.europa.eu/codelist/QualifierLocalNameValue">https://inspire.ec.europa.eu/codelist/QualifierLocalNameValue</a></td>
<td width="8%"><a href="#DomainQualifierLocalNameValue">QualifierLocalNameValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_rSpeciesId</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_rSpeciesId</td>
<td width="8%">(habitatSpecies.HabitatSpeciesType.referenceSpeciesId): Identifier of one of the reference lists given by the referenceSpeciesScheme.</td>
<td width="8%"><a href="#DomainReferenceSpeciesCodeValue_value">ReferenceSpeciesCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_rSpeciesId_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_rSpeciesId_href</td>
<td width="8%">URI from the INSPIRE code list register - ReferenceSpeciesCodeValue <a href="https://inspire.ec.europa.eu/codelist/ReferenceSpeciesCodeValue">https://inspire.ec.europa.eu/codelist/ReferenceSpeciesCodeValue</a></td>
<td width="8%"><a href="#DomainReferenceSpeciesCodeValue">ReferenceSpeciesCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_rSpeciesScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_rSpeciesScheme</td>
<td width="8%">(habitatSpecies.HabitatSpeciesType.referenceSpeciesScheme): Reference list defining a nomenclatural and taxonomical standard to which all local species names and taxonomic concepts shall be mapped to. Closed codelist of accepted PAN-european taxonomical reference lists defining the nomenclature and taxonomical concept of a given species name. This must not be regarded as the ultimate taxonomic truth: this will always change. It serves as a definition of a taxonomic concept described by systematic and synonym relations where other names and there inherent taxonomic concepts can be mapped to. The code list comprises of Eu-Nomen, EUNIS and Natura2000. In these sources harmonized species GUIDs and names are maintained by institutions with an assignment outside INSPIRE and the species names are to be retrieved through webservices using GUIDs. Only one of these list must be used for one taxon. The priority is as follows: 1) EU-Nomen, 2) EUNIS, 3) NatureDirectives. This implies: if a taxon is listed in EU-Nomen, this reference must be used as first choice. If it is not listed in EU-Nomen, the second choice is EUNIS, if not in EUNIS, NatureDirectives can be used.</td>
<td width="8%"><a href="#DomainReferenceSpeciesSchemeValue_value">ReferenceSpeciesSchemeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_rSpeciesScheme_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_rSpeciesScheme_href</td>
<td width="8%">URI from the INSPIRE code list register - ReferenceSpeciesSchemeValue <a href="https://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue">https://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue</a></td>
<td width="8%"><a href="#DomainReferenceSpeciesSchemeValue">ReferenceSpeciesSchemeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hVeg_localName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hVeg_localName</td>
<td width="8%">(habitatVegetation.HabitatVegetationType.localVegetationName.LocalNameType.localName): Name according to a local classification scheme.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hVeg_localNameCode</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hVeg_localNameCode</td>
<td width="8%">(habitatVegetation.HabitatVegetationType.localVegetationName.LocalNameType.localNameCode): Natural language name according to a local classification scheme.</td>
<td width="8%"><a href="#DomainLocalNameCodeValue_value">LocalNameCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hVeg_localNameCode_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hVeg_localNameCode_href</td>
<td width="8%">URI from the INSPIRE code list register - LocalNameCodeValue <a href="https://inspire.ec.europa.eu/codelist/LocalNameCodeValue">https://inspire.ec.europa.eu/codelist/LocalNameCodeValue</a></td>
<td width="8%"><a href="#DomainLocalNameCodeValue">LocalNameCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hVeg_localScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hVeg_localScheme</td>
<td width="8%">(habitatVegetation.HabitatVegetationType.localVegetationName.LocalNameType.localScheme): Uniform resource identifier of a local classification scheme. Classification scheme, which is used locally and contains all classification types, their codes and/or  very often their names in natural language.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hVeg_qualifierLocalName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hVeg_qualifierLocalName</td>
<td width="8%">(habitatVegetation.HabitatVegetationType.localVegetationName.LocalNameType.qualifierLocalName): The relation between the local name and the corresponding name in the Pan-European schema. EXAMPLE The local habitat type can be conceptually the same as the related Pan-European habitat type, the relationship then is called “congruent”   or  the local habitat type may be a subtype of the Pan-European habitat type, therefore the relationship should be "includedIn", etc.</td>
<td width="8%"><a href="#DomainQualifierLocalNameValue_value">QualifierLocalNameValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hVeg_qualifierLocalName_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hVeg_qualifierLocalName_href</td>
<td width="8%">URI from the INSPIRE code list register - QualifierLocalNameValue <a href="https://inspire.ec.europa.eu/codelist/QualifierLocalNameValue">https://inspire.ec.europa.eu/codelist/QualifierLocalNameValue</a></td>
<td width="8%"><a href="#DomainQualifierLocalNameValue">QualifierLocalNameValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inspireId_localId</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">inspireId_localId</td>
<td width="8%">A local identifier, assigned by the data provider. The local identifier is unique within the namespace, that is no other spatial object carries the same unique identifier.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inspireId_namespace</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">inspireId_namespace</td>
<td width="8%">Namespace uniquely identifying the data source of the spatial object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inspireId_versionId</td>
<td width="8%">String</td>
<td width="3%">25</td>
<td width="8%">inspireId_versionId</td>
<td width="8%">The identifier of the particular version of the spatial object, with a maximum length of 25 characters. If the specification of a spatial object type with an external object identifier includes life-cycle information, the version identifier is used to distinguish between the different versions of a spatial object. Within the set of all versions of a spatial object, the version identifier is unique</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p></p><p><hr/><br/><a name="FeatureClassHabitatS"/>
<p><strong>HabitatS - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Name</strong></td>
<td width="*" style="border-color: white">HabitatS</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>ShapeType</strong></td>
<td width="*" style="border-color: white">Polygon</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FeatureType</strong></td>
<td width="*" style="border-color: white">Simple</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>AliasName</strong></td>
<td width="*" style="border-color: white">HabitatS</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>HasM</strong></td>
<td width="*" style="border-color: white">false</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>HasZ</strong></td>
<td width="*" style="border-color: white">false</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>HasAttachments</strong></td>
<td width="*" style="border-color: white">false</td>
</tr>
</tbody>
</table>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>Description</strong></td>
<td width="*" style="border-color: white">HabitatS</td>
</tr>
</tbody>
</table><br/>
<table width="100%">
<tbody>
<tr style="border:0px">
<td width="8%" style="border:0px"><strong>Field</strong></td>
<td width="8%" style="border:0px"><strong>DataType</strong></td>
<td width="5%" style="border:0px"><strong>Length</strong></td>
<td width="8%" style="border:0px"><strong>AliasName</strong></td>
<td width="8%" style="border:0px"><strong>Description</strong></td>
<td width="8%" style="border:0px"><strong>Domain</strong></td>
<td width="8%" style="border:0px"><strong>DefaultValue</strong></td>
<td width="8%" style="border:0px"><strong>IsNullable</strong></td>
<td width="5%" style="border:0px"><strong>Precision</strong></td>
<td width="5%" style="border:0px"><strong>Scale</strong></td>
</tr>
<tr>
<td width="8%">OBJECTID</td>
<td width="8%">OID</td>
<td width="3%">4</td>
<td width="8%">OBJECTID</td>
<td width="8%"/>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">SHAPE</td>
<td width="8%">Geometry</td>
<td width="3%">0</td>
<td width="8%">SHAPE</td>
<td width="8%"/>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">featureId</td>
<td width="8%">Integer</td>
<td width="3%">4</td>
<td width="8%">featureId</td>
<td width="8%">A local identifier, assigned by the data provider. The local identifier is unique within the namespace, that is no other spatial object carries the same unique identifier.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_areaCovered</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">h_areaCovered</td>
<td width="8%">(habitat.HabitatTypeCoverType.areaCovered): The area covered by a certain habitat type within the provided geometry of the habitat spatial object. The surface area should be expressed in square meters.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_areaCovered_uom</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_areaCovered_uom</td>
<td width="8%">(habitat.HabitatTypeCoverType.areaCovered.uom): Units used for measuring area in this measure.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_l_localName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_l_localName</td>
<td width="8%">(habitat.HabitatTypeCoverType.localHabitatName.LocalNameType.localName): Name according to a local classification scheme.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_l_localNameCode</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_l_localNameCode</td>
<td width="8%">(habitat.HabitatTypeCoverType.localHabitatName.LocalNameType.localNameCode): Natural language name according to a local classification scheme.</td>
<td width="8%"><a href="#DomainLocalNameCodeValue_value">LocalNameCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_l_localNameCode_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_l_localNameCode_href</td>
<td width="8%">URI from the INSPIRE code list register - LocalNameCodeValue <a href="https://inspire.ec.europa.eu/codelist/LocalNameCodeValue">https://inspire.ec.europa.eu/codelist/LocalNameCodeValue</a></td>
<td width="8%"><a href="#DomainLocalNameCodeValue">LocalNameCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_l_localScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_l_localScheme</td>
<td width="8%">(habitat.HabitatTypeCoverType.localHabitatName.LocalNameType.localScheme): Uniform resource identifier of a local classification scheme. Classification scheme, which is used locally and contains all classification types, their codes and/or  very often their names in natural language.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_l_qualifierLocalName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_l_qualifierLocalName</td>
<td width="8%">(habitat.HabitatTypeCoverType.localHabitatName.LocalNameType.qualifierLocalName): The relation between the local name and the corresponding name in the Pan-European schema. EXAMPLE The local habitat type can be conceptually the same as the related Pan-European habitat type, the relationship then is called “congruent”   or  the local habitat type may be a subtype of the Pan-European habitat type, therefore the relationship should be "includedIn", etc.</td>
<td width="8%"><a href="#DomainQualifierLocalNameValue_value">QualifierLocalNameValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_l_qualifierLocalName_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_l_qualifierLocalName_href</td>
<td width="8%">URI from the INSPIRE code list register - QualifierLocalNameValue <a href="https://inspire.ec.europa.eu/codelist/QualifierLocalNameValue">https://inspire.ec.europa.eu/codelist/QualifierLocalNameValue</a></td>
<td width="8%"><a href="#DomainQualifierLocalNameValue">QualifierLocalNameValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_lengthCovered</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">h_lengthCovered</td>
<td width="8%">(habitat.HabitatTypeCoverType.lengthCovered): The length covered by a certain habitat type within the provided geometry of the habitat spatial object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_lengthCovered_uom</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_lengthCovered_uom</td>
<td width="8%">(habitat.HabitatTypeCoverType.lengthCovered.uom): Units used for measuring length in this measure.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_rHabitatTypeId</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_rHabitatTypeId</td>
<td width="8%">(habitat.HabitatTypeCoverType.referenceHabitatTypeId): Habitat type unique identifier (code) according to one Pan-European classification scheme. EXAMPLE "1110", "40C0", "95A0", etc., if the referenceHabitatScheme is "habitatsDirective", or "A1.111", "A1.1121", "G1.1111", "X34", etc., if the ReferenceHabitatScheme is "eunis"</td>
<td width="8%"><a href="#DomainReferenceHabitatTypeCodeValue_value">ReferenceHabitatTypeCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_rHabitatTypeId_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_rHabitatTypeId_href</td>
<td width="8%">URI from the INSPIRE code list register - ReferenceHabitatTypeCodeValue <a href="https://inspire.ec.europa.eu/codelist/ReferenceHabitatTypeCodeValue">https://inspire.ec.europa.eu/codelist/ReferenceHabitatTypeCodeValue</a></td>
<td width="8%"><a href="#DomainReferenceHabitatTypeCodeValue">ReferenceHabitatTypeCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_rHabitatTypeName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_rHabitatTypeName</td>
<td width="8%">(habitat.HabitatTypeCoverType.referenceHabitatTypeName): Name of a habitat type according to one Pan-European classification scheme. In the given Pan-European habitat classification systems, the habitat types can be identified by both: a short "identifier" (code)  and  a name in natural language, which is meant in this attribute. EXAMPLE Habitats Directive habitat type 3260 (code) "Floating vegetation of Ranunculus" or "Chenopodietum rubri of submountainous rivers" (name).</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_rHabitatTypeScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_rHabitatTypeScheme</td>
<td width="8%">(habitat.HabitatTypeCoverType.referenceHabitatTypeScheme): One of the Pan-European classification schemes, that are widely used in Europe. The list includes at least the classification of the natural habitat types of community interest listed in Annex I of the Habitats Directive, as well as the hierarchic classification of the habitat types of interest for biodiversity and nature protection listed in the EUNIS database, which is maintained by the EEA.</td>
<td width="8%"><a href="#DomainReferenceHabitatTypeSchemeValue_value">ReferenceHabitatTypeSchemeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_rHabitatTypeScheme_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_rHabitatTypeScheme_href</td>
<td width="8%">URI from the INSPIRE code list register - ReferenceHabitatTypeSchemeValue <a href="https://inspire.ec.europa.eu/codelist/ReferenceHabitatTypeSchemeValue">https://inspire.ec.europa.eu/codelist/ReferenceHabitatTypeSchemeValue</a></td>
<td width="8%"><a href="#DomainReferenceHabitatTypeSchemeValue">ReferenceHabitatTypeSchemeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_volumeCovered</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">h_volumeCovered</td>
<td width="8%">(habitat.HabitatTypeCoverType.volumeCovered): The volume covered by a certain habitat type within the provided geometry of the habitat spatial object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">h_volumeCovered_uom</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">h_volumeCovered_uom</td>
<td width="8%">(habitat.HabitatTypeCoverType.volumeCovered.uom): Units used for measuring volume in this measure.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_l_localName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_l_localName</td>
<td width="8%">(habitatSpecies.HabitatSpeciesType.localSpeciesName.LocalNameType.localName): Name according to a local classification scheme.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_l_localNameCode</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_l_localNameCode</td>
<td width="8%">(habitatSpecies.HabitatSpeciesType.localSpeciesName.LocalNameType.localNameCode): Natural language name according to a local classification scheme.</td>
<td width="8%"><a href="#DomainLocalNameCodeValue_value">LocalNameCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_l_localNameCode_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_l_localNameCode_href</td>
<td width="8%">URI from the INSPIRE code list register - LocalNameCodeValue <a href="https://inspire.ec.europa.eu/codelist/LocalNameCodeValue">https://inspire.ec.europa.eu/codelist/LocalNameCodeValue</a></td>
<td width="8%"><a href="#DomainLocalNameCodeValue">LocalNameCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_l_localScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_l_localScheme</td>
<td width="8%">(habitatSpecies.HabitatSpeciesType.localSpeciesName.LocalNameType.localScheme): Uniform resource identifier of a local classification scheme. Classification scheme, which is used locally and contains all classification types, their codes and/or  very often their names in natural language.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_l_qualifierLocalName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_l_qualifierLocalName</td>
<td width="8%">(habitatSpecies.HabitatSpeciesType.localSpeciesName.LocalNameType.qualifierLocalName): The relation between the local name and the corresponding name in the Pan-European schema. EXAMPLE The local habitat type can be conceptually the same as the related Pan-European habitat type, the relationship then is called “congruent”   or  the local habitat type may be a subtype of the Pan-European habitat type, therefore the relationship should be "includedIn", etc.</td>
<td width="8%"><a href="#DomainQualifierLocalNameValue_value">QualifierLocalNameValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_l_qualifierLocalName_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_l_qualifierLocalName_href</td>
<td width="8%">URI from the INSPIRE code list register - QualifierLocalNameValue <a href="https://inspire.ec.europa.eu/codelist/QualifierLocalNameValue">https://inspire.ec.europa.eu/codelist/QualifierLocalNameValue</a></td>
<td width="8%"><a href="#DomainQualifierLocalNameValue">QualifierLocalNameValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_rSpeciesId</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_rSpeciesId</td>
<td width="8%">(habitatSpecies.HabitatSpeciesType.referenceSpeciesId): Identifier of one of the reference lists given by the referenceSpeciesScheme.</td>
<td width="8%"><a href="#DomainReferenceSpeciesCodeValue_value">ReferenceSpeciesCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_rSpeciesId_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_rSpeciesId_href</td>
<td width="8%">URI from the INSPIRE code list register - ReferenceSpeciesCodeValue <a href="https://inspire.ec.europa.eu/codelist/ReferenceSpeciesCodeValue">https://inspire.ec.europa.eu/codelist/ReferenceSpeciesCodeValue</a></td>
<td width="8%"><a href="#DomainReferenceSpeciesCodeValue">ReferenceSpeciesCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_rSpeciesScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_rSpeciesScheme</td>
<td width="8%">(habitatSpecies.HabitatSpeciesType.referenceSpeciesScheme): Reference list defining a nomenclatural and taxonomical standard to which all local species names and taxonomic concepts shall be mapped to. Closed codelist of accepted PAN-european taxonomical reference lists defining the nomenclature and taxonomical concept of a given species name. This must not be regarded as the ultimate taxonomic truth: this will always change. It serves as a definition of a taxonomic concept described by systematic and synonym relations where other names and there inherent taxonomic concepts can be mapped to. The code list comprises of Eu-Nomen, EUNIS and Natura2000. In these sources harmonized species GUIDs and names are maintained by institutions with an assignment outside INSPIRE and the species names are to be retrieved through webservices using GUIDs. Only one of these list must be used for one taxon. The priority is as follows: 1) EU-Nomen, 2) EUNIS, 3) NatureDirectives. This implies: if a taxon is listed in EU-Nomen, this reference must be used as first choice. If it is not listed in EU-Nomen, the second choice is EUNIS, if not in EUNIS, NatureDirectives can be used.</td>
<td width="8%"><a href="#DomainReferenceSpeciesSchemeValue_value">ReferenceSpeciesSchemeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hS_rSpeciesScheme_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hS_rSpeciesScheme_href</td>
<td width="8%">URI from the INSPIRE code list register - ReferenceSpeciesSchemeValue <a href="https://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue">https://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue</a></td>
<td width="8%"><a href="#DomainReferenceSpeciesSchemeValue">ReferenceSpeciesSchemeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hVeg_localName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hVeg_localName</td>
<td width="8%">(habitatVegetation.HabitatVegetationType.localVegetationName.LocalNameType.localName): Name according to a local classification scheme.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hVeg_localNameCode</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hVeg_localNameCode</td>
<td width="8%">(habitatVegetation.HabitatVegetationType.localVegetationName.LocalNameType.localNameCode): Natural language name according to a local classification scheme.</td>
<td width="8%"><a href="#DomainLocalNameCodeValue_value">LocalNameCodeValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hVeg_localNameCode_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hVeg_localNameCode_href</td>
<td width="8%">URI from the INSPIRE code list register - LocalNameCodeValue <a href="https://inspire.ec.europa.eu/codelist/LocalNameCodeValue">https://inspire.ec.europa.eu/codelist/LocalNameCodeValue</a></td>
<td width="8%"><a href="#DomainLocalNameCodeValue">LocalNameCodeValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hVeg_localScheme</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hVeg_localScheme</td>
<td width="8%">(habitatVegetation.HabitatVegetationType.localVegetationName.LocalNameType.localScheme): Uniform resource identifier of a local classification scheme. Classification scheme, which is used locally and contains all classification types, their codes and/or  very often their names in natural language.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hVeg_qualifierLocalName</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hVeg_qualifierLocalName</td>
<td width="8%">(habitatVegetation.HabitatVegetationType.localVegetationName.LocalNameType.qualifierLocalName): The relation between the local name and the corresponding name in the Pan-European schema. EXAMPLE The local habitat type can be conceptually the same as the related Pan-European habitat type, the relationship then is called “congruent”   or  the local habitat type may be a subtype of the Pan-European habitat type, therefore the relationship should be "includedIn", etc.</td>
<td width="8%"><a href="#DomainQualifierLocalNameValue_value">QualifierLocalNameValue_value</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">hVeg_qualifierLocalName_href</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">hVeg_qualifierLocalName_href</td>
<td width="8%">URI from the INSPIRE code list register - QualifierLocalNameValue <a href="https://inspire.ec.europa.eu/codelist/QualifierLocalNameValue">https://inspire.ec.europa.eu/codelist/QualifierLocalNameValue</a></td>
<td width="8%"><a href="#DomainQualifierLocalNameValue">QualifierLocalNameValue</a></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inspireId_localId</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">inspireId_localId</td>
<td width="8%">A local identifier, assigned by the data provider. The local identifier is unique within the namespace, that is no other spatial object carries the same unique identifier.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inspireId_namespace</td>
<td width="8%">String</td>
<td width="3%">254</td>
<td width="8%">inspireId_namespace</td>
<td width="8%">Namespace uniquely identifying the data source of the spatial object.</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">inspireId_versionId</td>
<td width="8%">String</td>
<td width="3%">25</td>
<td width="8%">inspireId_versionId</td>
<td width="8%">The identifier of the particular version of the spatial object, with a maximum length of 25 characters. If the specification of a spatial object type with an external object identifier includes life-cycle information, the version identifier is used to distinguish between the different versions of a spatial object. Within the set of all versions of a spatial object, the version identifier is unique</td>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">SHAPE_Length</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">SHAPE_Length</td>
<td width="8%"/>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr><tr>
<td width="8%">SHAPE_Area</td>
<td width="8%">Double</td>
<td width="3%">8</td>
<td width="8%">SHAPE_Area</td>
<td width="8%"/>
<td width="8%"><a href="#Domain"/></td>
<td width="8%"/>
<td width="8%">true</td>
<td/>
<td/>
</tr>
</tbody>
</table>
</p></p>
    <p>
    <hr/><a name="DomainQualifierLocalNameValue"/>
<p><strong>QualifierLocalNameValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">QualifierLocalNameValue</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FieldType</strong></td>
<td width="*" style="border-color: white">String</td>
</tr>
<tr>
<td width="20%" style="border-color: white"><strong>Domain Type</strong></td>
<td width="*%" style="border-color: white">CodedValue</td>
</tr>
</tbody>
</table><br/>
<table width="100%">
<tbody>
<tr style="border-width:0px"><strong>
<td width="10%" style="border-width:0px"><strong>Code</strong></td>
</strong>
<td width="20%" style="border-width:0px"><strong>Name</strong></td>
</tr>
<tr>
<tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierLocalNameValue/congruent</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierLocalNameValue/congruent</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierLocalNameValue/excludes</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierLocalNameValue/excludes</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierLocalNameValue/includedIn</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierLocalNameValue/includedIn</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierLocalNameValue/includes</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierLocalNameValue/includes</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierLocalNameValue/overlaps</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/QualifierLocalNameValue/overlaps</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainQualifierLocalNameValue_value"/>
<p><strong>QualifierLocalNameValue_value - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">QualifierLocalNameValue_value</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FieldType</strong></td>
<td width="*" style="border-color: white">String</td>
</tr>
<tr>
<td width="20%" style="border-color: white"><strong>Domain Type</strong></td>
<td width="*%" style="border-color: white">CodedValue</td>
</tr>
</tbody>
</table><br/>
<table width="100%">
<tbody>
<tr style="border-width:0px"><strong>
<td width="10%" style="border-width:0px"><strong>Code</strong></td>
</strong>
<td width="20%" style="border-width:0px"><strong>Name</strong></td>
</tr>
<tr>
<tr>
<td width="20%">congruent</td>
<td width="20%">congruent</td>
</tr><tr>
<td width="20%">excludes</td>
<td width="20%">excludes</td>
</tr><tr>
<td width="20%">includedIn</td>
<td width="20%">includedIn</td>
</tr><tr>
<td width="20%">includes</td>
<td width="20%">includes</td>
</tr><tr>
<td width="20%">overlaps</td>
<td width="20%">overlaps</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainReferenceHabitatTypeSchemeValue"/>
<p><strong>ReferenceHabitatTypeSchemeValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">ReferenceHabitatTypeSchemeValue</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FieldType</strong></td>
<td width="*" style="border-color: white">String</td>
</tr>
<tr>
<td width="20%" style="border-color: white"><strong>Domain Type</strong></td>
<td width="*%" style="border-color: white">CodedValue</td>
</tr>
</tbody>
</table><br/>
<table width="100%">
<tbody>
<tr style="border-width:0px"><strong>
<td width="10%" style="border-width:0px"><strong>Code</strong></td>
</strong>
<td width="20%" style="border-width:0px"><strong>Name</strong></td>
</tr>
<tr>
<tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ReferenceHabitatTypeSchemeValue/eunis</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ReferenceHabitatTypeSchemeValue/eunis</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ReferenceHabitatTypeSchemeValue/habitatsDirective</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ReferenceHabitatTypeSchemeValue/habitatsDirective</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ReferenceHabitatTypeSchemeValue/marineStrategyFrameworkDirective</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ReferenceHabitatTypeSchemeValue/marineStrategyFrameworkDirective</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainReferenceHabitatTypeSchemeValue_value"/>
<p><strong>ReferenceHabitatTypeSchemeValue_value - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">ReferenceHabitatTypeSchemeValue_value</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FieldType</strong></td>
<td width="*" style="border-color: white">String</td>
</tr>
<tr>
<td width="20%" style="border-color: white"><strong>Domain Type</strong></td>
<td width="*%" style="border-color: white">CodedValue</td>
</tr>
</tbody>
</table><br/>
<table width="100%">
<tbody>
<tr style="border-width:0px"><strong>
<td width="10%" style="border-width:0px"><strong>Code</strong></td>
</strong>
<td width="20%" style="border-width:0px"><strong>Name</strong></td>
</tr>
<tr>
<tr>
<td width="20%">eunis</td>
<td width="20%">eunis</td>
</tr><tr>
<td width="20%">habitatsDirective</td>
<td width="20%">habitatsDirective</td>
</tr><tr>
<td width="20%">marineStrategyFrameworkDirective</td>
<td width="20%">marineStrategyFrameworkDirective</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainReferenceSpeciesSchemeValue"/>
<p><strong>ReferenceSpeciesSchemeValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">ReferenceSpeciesSchemeValue</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FieldType</strong></td>
<td width="*" style="border-color: white">String</td>
</tr>
<tr>
<td width="20%" style="border-color: white"><strong>Domain Type</strong></td>
<td width="*%" style="border-color: white">CodedValue</td>
</tr>
</tbody>
</table><br/>
<table width="100%">
<tbody>
<tr style="border-width:0px"><strong>
<td width="10%" style="border-width:0px"><strong>Code</strong></td>
</strong>
<td width="20%" style="border-width:0px"><strong>Name</strong></td>
</tr>
<tr>
<tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue/eunomen</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue/eunomen</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue/eunis</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue/eunis</td>
</tr><tr>
<td width="20%">http://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue/natureDirectives</td>
<td width="20%">http://inspire.ec.europa.eu/codelist/ReferenceSpeciesSchemeValue/natureDirectives</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p><p>
    <hr/><a name="DomainReferenceSpeciesSchemeValue_value"/>
<p><strong>ReferenceSpeciesSchemeValue_value - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
<tbody>
<tr>
<td width="12%" style="border-color: white"><strong>DomainName</strong></td>
<td width="*" style="border-color: white">ReferenceSpeciesSchemeValue_value</td>
</tr>
<tr>
<td width="12%" style="border-color: white"><strong>FieldType</strong></td>
<td width="*" style="border-color: white">String</td>
</tr>
<tr>
<td width="20%" style="border-color: white"><strong>Domain Type</strong></td>
<td width="*%" style="border-color: white">CodedValue</td>
</tr>
</tbody>
</table><br/>
<table width="100%">
<tbody>
<tr style="border-width:0px"><strong>
<td width="10%" style="border-width:0px"><strong>Code</strong></td>
</strong>
<td width="20%" style="border-width:0px"><strong>Name</strong></td>
</tr>
<tr>
<tr>
<td width="20%">eunomen</td>
<td width="20%">eunomen</td>
</tr><tr>
<td width="20%">eunis</td>
<td width="20%">eunis</td>
</tr><tr>
<td width="20%">natureDirectives</td>
<td width="20%">natureDirectives</td>
</tr>
</tr>
</tbody>
</table>
</p>
</p>
