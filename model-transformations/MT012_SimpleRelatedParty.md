## MT012: Simplified Period

<table>
<tr>
<td>Category</td>
<td>Alternate Structures for specific types or type hierarchies</td>
</tr>
<tr>
<td>Description</td>
<td><p>XML has primitive types for times and dates that are well supported through most software. In INSPIRE and the related ISO standards, a more powerful but also highly complex model is available that allows to precisely specify time-related information. This model allows any subtype of <code>AbstractTimeObject</code>, which can include <code>TimeEdge</code>, <code>TimeInstant</code>, <code>TimeNode</code> and <code>TimePeriods</code>. In several themes, such as EMF, other types buld on top of this model, such as <code>ef:OperationalActivityPeriod</code>. Alltogether, this means that relatively important information tends to be nested very deep in a structure, making it harder to create and to process.</p> 
<p>Within this rule, we substitute these complex structures through a very simple structure with just two properties:</p>
<ul>
    <li>beginPosition</li>
    <li>endPosition</li>
</ul>
<p>Both of these are to use teh same definitions for these two properties as in the original structure. Note that the <code>endPosition</code> is optional, so the simple type can also be used for periods that haven't ended yet.</p>
</td>
</tr>
<tr>
<td>Original instance in default encoding:</td>
<td>

```xml
<ef:EnvironmentalMonitoringFacility>
  <!-- ... -->
  <ef:operationalActivityPeriod>
      <ef:OperationalActivityPeriod gml:id="Piezometre.OperationalActivityPeriod.2.06512X0037-STREMY">
          <ef:activityTime>
              <gml:TimePeriod gml:id="TimePeriod.2.225196">
                  <gml:beginPosition>1977-10-08T23:00:00Z</gml:beginPosition>
                  <gml:endPosition>2014-10-14T06:00:00Z</gml:endPosition>
              </gml:TimePeriod>
          </ef:activityTime>
      </ef:OperationalActivityPeriod>
  </ef:operationalActivityPeriod>
  <!-- ... -->
</ef:EnvironmentalMonitoringFacility>
```
   
</td>
</tr>
<tr>
<td>Transformed instance in default encoding:</td>
<td>

```xml
<efs:EnvironmentalMonitoringFacility>
  <!-- ... -->
  <efs:operationalActivityPeriod>
      <simple:SimplePeriod>
        <gml:beginPosition>1977-10-08T23:00:00Z</gml:beginPosition>
        <gml:endPosition>2014-10-14T06:00:00Z</gml:endPosition>
      </simple:SimplePeriod>
  </efs:operationalActivityPeriod>
  <!-- ... -->
</efs:EnvironmentalMonitoringFacility>
``` 

</td>
</tr>
<tr>
<td>Model transformation rule: </td>
<td>
    <p>Parameters:</p> 
    <ul>
      <li><code>type</code>: The type to be substituted, e.g. <code>OperationalActivityPeriod</code>.</li>
    </ul>
    <p>Substitute existing type as indicated by the <code>type</code> parameter with this <code>SimplePeriod</code> type.</p>
</td>
</tr>
<tr>
<td>Instance transformation rule:</td>
<td>
	<ul>
		<li>Copy the value of <code>gml:beginPosition</code> to the property <code>gml:beginPosition</code>.</li>
		<li>Copy the value of <code>gml:endPosition</code> to the property <code>gml:endPosition</code>.</li>
	</ul>
</td>
</tr>
<tr>
<td>Solves usability issues:</td>
<td>The transformed data structure can easily be edited, filtered and symbolized in desktop GIS and web GIS software. This transformation also reduces data volume in datasets.</td>
</tr>
<tr>
<td>Known usability issues:</td>
<td>None.</td>
</tr>
<tr>
<td>INSPIRE Compliance:</td>
<td>This rule works only with one external link, and it removed finer grained information about dates. It can be combined with the [Property Composition to Association](./PropertyCompositiontoAssociation.md) rule to add more information from an external register.</td>
</tr>
</table>

Notes:

 * None.
