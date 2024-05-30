#Population Distribution - demography

<br />
<strong>Geodatabase Documentation</strong>
<hr />
<strong>Date: </strong>20240530100000.000000<br />
<hr />
<p><strong>Summary Information and Links</strong><br /><br />
  <a href="#FeatureDatasets">0 Feature Datasets and 1 Feature Classes</a><br />
  No Topology Datasets<br />
  No Geometric Networks<br />
  No Rasters<br />
  <a href="#ObjectClasses">0 Tables (Object Classes)</a><br />
  <a href="#RelationshipClasses">0 Relationship Classes</a><br />
  <a href="#Domains">5 Domains</a><br />
</p>
<hr />
<p><a name="FeatureDatasets" /><strong>Feature Datasets and Child Classes</strong></p><a name="Raster" />
<p><strong>Rasters</strong></p><br />
<hr /><a name="ObjectClasses" />
<p><strong>Workspace-Level Tables and Feature Classes</strong></p>

<a href="#FeatureClassAddress">PopulationDistribution - FeatureClass</a><br />

<p /><br />
<hr /><a name="RelationshipClasses" />
<p><strong>Relationship Classes</strong></p>
<p />
<hr /><br />

<a name="Domains" />
<p><strong>Domains</strong></p>
<a href="#DomainStatusValue">StatusValue</a><br />
<a href="#DomainGeometrySpecificationValue">GeometrySpecificationValue</a><br />
<a href="#DomainGeometryMethodValue">GeometryMethodValue</a><br /><a
  href="#DomainLocatorLevelValue">LocatorLevelValue</a><br />
<p>
  <hr /><br /><a name="FeatureClassAddress" />
<p><strong>PopulationDistribution - FeatureClass</strong></p>
<p>
<table width="100%" style="border-color: white">
  <tbody>
    <tr>
      <td width="12%" style="border-color: white"><strong>Name</strong></td>
      <td width="*" style="border-color: white">PopulationDistribution</td>
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
      <td width="*" style="border-color: white">PopulationDistribution</td>
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
      <td width="*" style="border-color: white">PopulationDistribution</td>
    </tr>
  </tbody>
</table><br />
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
      <td width="8%" />
      <td width="8%"><a href="#Domain" /></td>
      <td width="8%" />
      <td width="8%">true</td>
      <td />
      <td />
    </tr>
    <tr>
      <td width="8%">SHAPE</td>
      <td width="8%">Geometry</td>
      <td width="3%">0</td>
      <td width="8%">SHAPE</td>
      <td width="8%" />
      <td width="8%"><a href="#Domain" /></td>
      <td width="8%" />
      <td width="8%">true</td>
      <td />
      <td />
    </tr>
    <tr>
      <td width="8%">AgeBy5Years</td>
      <td width="8%">Integer</td>
      <td width="3%">4</td>
      <td width="8%">AgeBy5Years</td>
      <td width="8%">Age by 5 years</td>
      <td width="8%"><a href="#Domain" /></td>
      <td width="8%" />
      <td width="8%">true</td>
      <td />
      <td />
    </tr>
    <tr>
      <td width="8%">AgeBy5Years_herf</td>
      <td width="8%">String</td>
      <td width="3%">254</td>
      <td width="8%">AgeBy5Years_herf</td>
      <td width="8%">URI from the INSPIRE code list register - AgeBy5Years - https://inspire.ec.europa.eu/codelist/ClassificationTypeValue/ageBy5Years</td>
      <td width="8%"><a href="#AgeBy5Years" >AgeBy5Years</a></td>
      <td width="8%" />
      <td width="8%">true</td>
      <td />
      <td />
    </tr>
    <tr>
      <td width="8%">AgeByYear</td>
      <td width="8%">Integer</td>
      <td width="3%">4</td>
      <td width="8%">AgeByYear</td>
      <td width="8%">Age by year</td>
      <td width="8%"><a href="#Domain" /></td>
      <td width="8%" />
      <td width="8%">true</td>
      <td />
      <td />
    </tr>
    <tr>
      <td width="8%">AgeByYear_herf</td>
      <td width="8%">String</td>
      <td width="3%">254</td>
      <td width="8%">AgeByYear_herf</td>
      <td width="8%">URI from the INSPIRE code list register - AgeByYearValue - https://inspire.ec.europa.eu/codelist/ClassificationTypeValue/ageByYear</td>
      <td width="8%"><a href="#AgeByYear" >AgeByYear</a></td>
      <td width="8%" />
      <td width="8%">true</td>
      <td />
      <td />
    </tr>
        <tr>
      <td width="8%">AgeGroup</td>
      <td width="8%">Integer</td>
      <td width="3%">4</td>
      <td width="8%">AgeGroup</td>
      <td width="8%">Age group</td>
      <td width="8%"><a href="#Domain" /></td>
      <td width="8%" />
      <td width="8%">true</td>
      <td />
      <td />
    </tr>
    <tr>
      <td width="8%">AgeGroup_herf</td>
      <td width="8%">String</td>
      <td width="3%">254</td>
      <td width="8%">AgeGroup_herf</td>
      <td width="8%">URI from the INSPIRE code list register - AgeGroupValue - http://inspire.ec.europa.eu/codeList/AgeGroupValue</td>
      <td width="8%"><a href="#AgeGroupValue" >AgeGroupValue</a></td>
      <td width="8%" />
      <td width="8%">true</td>
      <td />
      <td />
        <tr>
      <td width="8%">Gender</td>
      <td width="8%">Integer</td>
      <td width="3%">4</td>
      <td width="8%">Gender</td>
      <td width="8%">Age by group</td>
      <td width="8%"><a href="#Domain" /></td>
      <td width="8%" />
      <td width="8%">true</td>
      <td />
      <td />
    </tr>
    </tr>
    <tr>
      <td width="8%">Gender_herf</td>
      <td width="8%">String</td>
      <td width="3%">254</td>
      <td width="8%">Gender_herf</td>
      <td width="8%">URI from the INSPIRE code list register - Gender - https://inspire.ec.europa.eu/codelist/ClassificationTypeValue/gender</td>
      <td width="8%"><a href="#Gender" >Gender</a></td>
      <td width="8%" />
      <td width="8%">true</td>
      <td />
      <td />
    </tr>
    <tr>
      <td width="8%">NACE</td>
      <td width="8%">string</td>
      <td width="3%">256</td>
      <td width="8%">NACE</td>
      <td width="8%">
The economic activity classification NACE Version 2 (Classification of Economic Activities in the European Community).</td>
      <td width="8%"><a href="#Domain" /></td>
      <td width="8%" />
      <td width="8%">true</td>
      <td />
      <td />
    </tr>
    <tr>
      <td width="8%">NACE_href</td>
      <td width="8%">String</td>
      <td width="3%">254</td>
      <td width="8%">NACE_href</td>
      <td width="8%">URI from the INSPIRE code list register - NACE - https://inspire.ec.europa.eu/codelist/ClassificationTypeValue/Nace2</td>
      <td width="8%"><a href="#Domain" />NACE</td>
      <td width="8%" />
      <td width="8%">true</td>
      <td />
      <td />
    </tr>
    <tr>
      <td width="8%">Dimensions</td>
      <td width="8%">integer</td>
      <td width="3%">4</td>
      <td width="8%">Dimentions</td>
      <td width="8%">The identification of what the piece of datum refers to in terms of geographic location or individual characteristics.</td>
      <td width="8%"><a href="#Domain" /></td>
      <td width="8%" />
      <td width="8%">true</td>
      <td />
      <td />
    </tr>
    <tr>
      <td width="8%">SpecialValue</td>
      <td width="8%">string</td>
      <td width="3%">256</td>
      <td width="8%">SpecialValue</td>
      <td width="8%">Special Value</td>
      <td width="8%"><a href="#Domain" /></td>
      <td width="8%" />
      <td width="8%">true</td>
      <td />
      <td />
    </tr>
    <tr>
      <td width="8%">SpecialValue_href</td>
      <td width="8%">String</td>
      <td width="3%">254</td>
      <td width="8%">SpecialValue_href</td>
      <td width="8%">URI from the INSPIRE code list register - SpecialValue - http://inspire.ec.europa.eu/codeList/SpecialValue</td>
      <td width="8%"><a href="#Domain" /></td>
      <td width="8%" />
      <td width="8%">true</td>
      <td />
      <td />
    </tr>
    <tr>
      <td width="8%">StatisticalValue</td>
      <td width="8%">string</td>
      <td width="3%">256</td>
      <td width="8%">StatisticalValue</td>
      <td width="8%">
Statistical Value/td>
      <td width="8%"><a href="#Domain" /></td>
      <td width="8%" />
      <td width="8%">true</td>
      <td />
      <td />
    </tr>
    <tr>
      <td width="8%">StatisticalValue_href</td>
      <td width="8%">String</td>
      <td width="3%">254</td>
      <td width="8%">StatisticalValue_href</td>
      <td width="8%">URI from the INSPIRE code list register - StatisticalValue - http://inspire.ec.europa.eu/codeList/StatisticsMeasurementMethodValue</td>
      <td width="8%"><a href="#Domain" /></td>
      <td width="8%" />
      <td width="8%">true</td>
      <td />
      <td />
    </tr>
    <tr>
      <td width="8%">StatisticalMeasurement</td>
      <td width="8%">string</td>
      <td width="3%">256</td>
      <td width="8%">StatisticalMeasurement</td>
      <td width="8%">Statistics measurement method value</td>
      <td width="8%"><a href="#Domain" /></td>
      <td width="8%" />
      <td width="8%">true</td>
      <td />
      <td />
    </tr>
    <tr>
      <td width="8%">StatisticalMeasurement_href</td>
      <td width="8%">String</td>
      <td width="3%">254</td>
      <td width="8%">StatisticalMeasurement_href</td>
      <td width="8%">URI from the INSPIRE code list register - StatisticalMeasurement - http://inspire.ec.europa.eu/codeList/StatisticsMeasurementMethodValue</td>
      <td width="8%"><a href="#Domain" /></td>
      <td width="8%" />
      <td width="8%">true</td>
      <td />
      <td />
    </tr>
  </tbody>
</table>
</p>
</p>
<p>
  <hr /><a name="AgeBy5Years" />
<p><strong>AgeBy5Years - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
  <tbody>
    <tr>
      <td width="12%" style="border-color: white"><strong>DomainName</strong></td>
      <td width="*" style="border-color: white">AgeBy5Years</td>
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
</table><br />
<table width="100%">
  <tbody>
    <tr style="border-width:0px"><strong>
        <td width="10%" style="border-width:0px"><strong>Code</strong></td>
      </strong>
      <td width="20%" style="border-width:0px"><strong>Name</strong></td>
    </tr>
    <tr>
    <tr>
      <td width="20%">0-5</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/0-5</td>
    </tr>
    <tr>
      <td width="20%">5-10</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/5-10</td>
    </tr>
        <tr>
      <td width="20%">10-15</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/10-15</td>
    </tr>
        <tr>
      <td width="20%">15-20</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/15-20</td>
    </tr>
        <tr>
      <td width="20%">20-25</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/20-25</td>
    </tr>
        <tr>
      <td width="20%">25-30</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/25-30</td>
    </tr>
        <tr>
      <td width="20%">30-35</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/30-35</td>
    </tr>
        <tr>
      <td width="20%">35-40</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/35-40</td>
    </tr>
        <tr>
      <td width="20%">40-45</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/40-45</td>
    </tr>
        <tr>
      <td width="20%">45-50</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/45-50</td>
    </tr>
        <tr>
      <td width="20%">50-55</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/50-55</td>
    </tr>
        <tr>
      <td width="20%">55-60</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/55-60</td>
    </tr>
        <tr>
      <td width="20%">60-65</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/60-65</td>
    </tr>
        <tr>
      <td width="20%">65-70</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/65-70</td>
    </tr>
        <tr>
      <td width="20%">70-75</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/70-75</td>
    </tr>
        <tr>
      <td width="20%">75-80</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/75-80</td>
    </tr>
        <tr>
      <td width="20%">80-85</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/80-85</td>
    </tr>
        <tr>
      <td width="20%">85-90</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/85-90</td>
    </tr>
        <tr>
      <td width="20%">90-95</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/90-95</td>
    </tr>
        <tr>
      <td width="20%">95-100</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeBy5YearsValue/95-100</td>
    </tr>
    
  </tbody>
</table>
</p>
</p>
<p>
  <hr /><a name="AgeByYear" />
<p><strong>AgeByYear - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
  <tbody>
    <tr>
      <td width="12%" style="border-color: white"><strong>DomainName</strong></td>
      <td width="*" style="border-color: white">AgeByYear</td>
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
</table><br />
<table width="100%">
  <tbody>
    <tr style="border-width:0px"><strong>
        <td width="10%" style="border-width:0px"><strong>Code</strong></td>
      </strong>
      <td width="20%" style="border-width:0px"><strong>Name</strong></td>
    </tr>
      <tr><td width="20%">0-1</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/0-1</td></tr>
      <tr><td width="20%">1-2</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/1-2</td></tr>
      <tr><td width="20%">2-3</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/2-3</td></tr>
      <tr><td width="20%">3-4</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/3-4</td></tr>
      <tr><td width="20%">4-5</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/4-5</td></tr>
      <tr><td width="20%">5-6</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/5-6</td></tr>
      <tr><td width="20%">6-7</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/6-7</td></tr>
      <tr><td width="20%">7-8</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/7-8</td></tr>
      <tr><td width="20%">8-9</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/8-9</td></tr>
      <tr><td width="20%">9-10</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/9-10</td></tr>
      <tr><td width="20%">10-11</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/10-11</td></tr>
      <tr><td width="20%">11-12</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/11-12</td></tr>
      <tr><td width="20%">12-13</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/12-13</td></tr>
      <tr><td width="20%">13-14</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/13-14</td></tr>
      <tr><td width="20%">14-15</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/14-15</td></tr>
      <tr><td width="20%">15-16</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/15-16</td></tr>
      <tr><td width="20%">16-17</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/16-17</td></tr>
      <tr><td width="20%">17-18</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/17-18</td></tr>
      <tr><td width="20%">18-19</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/18-19</td></tr>
      <tr><td width="20%">19-20</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/19-20</td></tr>
      <tr><td width="20%">20-21</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/20-21</td></tr>
      <tr><td width="20%">21-22</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/21-22</td></tr>
      <tr><td width="20%">22-23</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/22-23</td></tr>
      <tr><td width="20%">23-24</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/23-24</td></tr>
      <tr><td width="20%">24-25</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/24-25</td></tr>
      <tr><td width="20%">25-26</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/25-26</td></tr>
      <tr><td width="20%">26-27</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/26-27</td></tr>
      <tr><td width="20%">27-28</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/27-28</td></tr>
      <tr><td width="20%">28-29</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/28-29</td></tr>
      <tr><td width="20%">29-30</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/29-30</td></tr>
      <tr><td width="20%">30-31</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/30-31</td></tr>
      <tr><td width="20%">31-32</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/31-32</td></tr>
      <tr><td width="20%">32-33</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/32-33</td></tr>
      <tr><td width="20%">33-34</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/33-34</td></tr>
      <tr><td width="20%">34-35</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/34-35</td></tr>
      <tr><td width="20%">35-36</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/35-36</td></tr>
      <tr><td width="20%">36-37</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/36-37</td></tr>
      <tr><td width="20%">37-38</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/37-38</td></tr>
      <tr><td width="20%">38-39</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/38-39</td></tr>
      <tr><td width="20%">39-40</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/39-40</td></tr>
      <tr><td width="20%">40-41</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/40-41</td></tr>
      <tr><td width="20%">41-42</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/41-42</td></tr>
      <tr><td width="20%">42-43</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/42-43</td></tr>
      <tr><td width="20%">43-44</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/43-44</td></tr>
      <tr><td width="20%">44-45</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/44-45</td></tr>
      <tr><td width="20%">45-46</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/45-46</td></tr>
      <tr><td width="20%">46-47</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/46-47</td></tr>
      <tr><td width="20%">47-48</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/47-48</td></tr>
      <tr><td width="20%">48-49</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/48-49</td></tr>
      <tr><td width="20%">49-50</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/49-50</td></tr>
      <tr><td width="20%">50-51</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/50-51</td></tr>
      <tr><td width="20%">51-52</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/51-52</td></tr>
      <tr><td width="20%">52-53</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/52-53</td></tr>
      <tr><td width="20%">53-54</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/53-54</td></tr>
      <tr><td width="20%">54-55</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/54-55</td></tr>
      <tr><td width="20%">55-56</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/55-56</td></tr>
      <tr><td width="20%">56-57</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/56-57</td></tr>
      <tr><td width="20%">57-58</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/57-58</td></tr>
      <tr><td width="20%">58-59</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/58-59</td></tr>
      <tr><td width="20%">59-60</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/59-60</td></tr>
      <tr><td width="20%">60-61</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/60-61</td></tr>
      <tr><td width="20%">61-62</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/61-62</td></tr>
      <tr><td width="20%">62-63</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/62-63</td></tr>
      <tr><td width="20%">63-64</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/63-64</td></tr>
      <tr><td width="20%">64-65</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/64-65</td></tr>
      <tr><td width="20%">65-66</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/65-66</td></tr>
      <tr><td width="20%">66-67</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/66-67</td></tr>
      <tr><td width="20%">67-68</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/67-68</td></tr>
      <tr><td width="20%">68-69</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/68-69</td></tr>
      <tr><td width="20%">69-70</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/69-70</td></tr>
      <tr><td width="20%">70-71</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/70-71</td></tr>
      <tr><td width="20%">71-72</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/71-72</td></tr>
      <tr><td width="20%">72-73</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/72-73</td></tr>
      <tr><td width="20%">73-74</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/73-74</td></tr>
      <tr><td width="20%">74-75</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/74-75</td></tr>
      <tr><td width="20%">75-76</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/75-76</td></tr>
      <tr><td width="20%">76-77</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/76-77</td></tr>
      <tr><td width="20%">77-78</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/77-78</td></tr>
      <tr><td width="20%">78-79</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/78-79</td></tr>
      <tr><td width="20%">79-80</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/79-80</td></tr>
      <tr><td width="20%">80-81</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/80-81</td></tr>
      <tr><td width="20%">81-82</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/81-82</td></tr>
      <tr><td width="20%">82-83</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/82-83</td></tr>
      <tr><td width="20%">83-84</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/83-84</td></tr>
      <tr><td width="20%">84-85</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/84-85</td></tr>
      <tr><td width="20%">85-86</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/85-86</td></tr>
      <tr><td width="20%">86-87</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/86-87</td></tr>
      <tr><td width="20%">87-88</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/87-88</td></tr>
      <tr><td width="20%">88-89</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/88-89</td></tr>
      <tr><td width="20%">89-90</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/89-90</td></tr>
      <tr><td width="20%">90-91</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/90-91</td></tr>
      <tr><td width="20%">91-92</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/91-92</td></tr>
      <tr><td width="20%">92-93</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/92-93</td></tr>
      <tr><td width="20%">93-94</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/93-94</td></tr>
      <tr><td width="20%">94-95</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/94-95</td></tr>
      <tr><td width="20%">95-96</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/95-96</td></tr>
      <tr><td width="20%">96-97</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/96-97</td></tr>
      <tr><td width="20%">97-98</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/97-98</td></tr>
      <tr><td width="20%">98-99</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/98-99</td></tr>
      <tr><td width="20%">99-100</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/99-100</td></tr>
      <tr><td width="20%">100+</td><td width="20%">http://inspire.ec.europa.eu/codelist/AgeByYearValue/100+</td></tr>
    </tr>
    
  </tbody>
</table>
</p>
<p>
  <hr /><a name="AgeGroupValue" />
<p><strong>AgeGroupValue - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
  <tbody>
    <tr>
      <td width="12%" style="border-color: white"><strong>DomainName</strong></td>
      <td width="*" style="border-color: white">AgeGroupValue</td>
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
</table><br />
<table width="100%">
  <tbody>
    <tr style="border-width:0px"><strong>
        <td width="10%" style="border-width:0px"><strong>Code</strong></td>
      </strong>
      <td width="20%" style="border-width:0px"><strong>Name</strong></td>
    </tr>
    <tr>
    <tr>
      <td width="20%">0_15</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeGroupValue/0_15</td>
    </tr>
    <tr>
      <td width="20%">15_65</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeGroupValue/15_65</td>
    </tr>
    <tr>
      <td width="20%">65+</td>
      <td width="20%">http://inspire.ec.europa.eu/codelist/AgeGroupValue/65+</td>
    </tr>
    </tr>
  </tbody>
</table>
</p>
</p>
<p>
  <hr /><a name="Gender" />
<p><strong>Gender - Domain</strong></p>
<p>
<table width="100%" style="border-color: white">
  <tbody>
    <tr>
      <td width="12%" style="border-color: white"><strong>DomainName</strong></td>
      <td width="*" style="border-color: white">Gender</td>
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
</table><br />
<table width="100%">
  <tbody>
    <tr style="border-width:0px"><strong>
        <td width="10%" style="border-width:0px"><strong>Code</strong></td>
      </strong>
      <td width="20%" style="border-width:0px"><strong>Name</strong></td>
    </tr>
    <tr>
    <tr>
      <td width="20%">male</td>
      <td width="20%">male</td>
    </tr>
    <tr>
      <td width="20%">female</td>
      <td width="20%">female</td>
    </tr>
    <tr>
      <td width="20%">unknown</td>
      <td width="20%">unknown</td>
    </tr>
    </tr>
  </tbody>
</table>
</p>
</p>
