# MT015: Fan Out Feature Type By Codelist Property

> **Not yet applied.** MT015 is catalogued but not used by the theme encodings; no
> current theme fans a feature type out by a codelist value. Listed here so the
> catalogue stays complete.

## Category

Alternate Structures for specific types or type hierarchies

## Description

This rule is used to fan-out features by the value of a codelist property into separate attributes.

## Original instance (example)

```xml
	<gml:featureMember>
		<au:AdministrativeUnit>
			<au:nationalLevel xlink:href="http://inspire.ec.europa.eu/codelist/AdministrativeHierarchyLevel/1stOrder"/>
			<!-- ... -->
		</au:AdministrativeUnit>
	</gml:featureMember>
	<gml:featureMember>
		<au:AdministrativeUnit>
			<au:nationalLevel xlink:href="http://inspire.ec.europa.eu/codelist/AdministrativeHierarchyLevel/2ndOrder"/>
			<!-- ... -->
			<au:boundary xsi:nil="true"/>
		</au:AdministrativeUnit>
	</gml:featureMember>
	<gml:featureMember>
		<au:AdministrativeUnit>
			<au:nationalLevel xlink:href="http://inspire.ec.europa.eu/codelist/AdministrativeHierarchyLevel/3rdOrder"/>
			<!-- ... -->
		</au:AdministrativeUnit>
	</gml:featureMember>
```

## Transformed instance (example)

```xml
	<gml:featureMember>
		<au:AdministrativeUnit_1stOrder>
			<au:nationalLevel xlink:href="http://inspire.ec.europa.eu/codelist/AdministrativeHierarchyLevel/1stOrder"/>
			<!-- ... -->
		</au:AdministrativeUnit_1stOrder>
	</gml:featureMember>
	<gml:featureMember>
		<au:AdministrativeUnit_2ndOrder>
			<au:nationalLevel xlink:href="http://inspire.ec.europa.eu/codelist/AdministrativeHierarchyLevel/2ndOrder"/>
			<!-- ... -->
		</au:AdministrativeUnit_2ndOrder>
	</gml:featureMember>
	<gml:featureMember>
		<au:AdministrativeUnit_3rdOrder>
			<au:nationalLevel xlink:href="http://inspire.ec.europa.eu/codelist/AdministrativeHierarchyLevel/3rdOrder"/>
			<!-- ... -->
		</au:AdministrativeUnit_3rdOrder>
	</gml:featureMember>


``` 

## Model transformation rule

Create a copy of the original feature class for each codelist value. Add the value CodelistValue as a Suffix.

## Instance transformation rule

- Copy the features to a feature class depending on the property that was used for the fan-out.

## Solves usability issues

None

## Known usability issues

Long Codelists can resolve in a big number of extra Feature Classes.

## INSPIRE compliance

No issues.

## Notes

- Not part of the original INSPIRE MIF 2017.2 catalogue (MT001–MT009); added in this project.
