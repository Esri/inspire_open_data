# MT010: Simplified PT_FreeText

> **Implementation note.** As applied in the theme encodings, the rule
> runs **unconditionally on every theme** as a base normalization (a no-op where there
> is no free text): it collapses each `PT_FreeText` / `LocalisedCharacterString` to a
> single Text value plus a `<prop>_locale` companion. Optional parameter
> **`keepLocale`** (default true) — set false to drop the `_locale` companion.

## Category

Alternate Structures for specific types or type hierarchies

## Description

`PT_FreeText` is used to provide textual information in different locales using textGroups. These text groups use LocalisedCharacterString to provide information in different languages. The number of text groups is not limited by the data model. This creates a complex structure that is in many cases not necessary making it harder to create and to process.

This rule proposes a simplified alternative representation:

## Original instance (example)

```xml
<us-emf:EnvironmentalManagementFacility gml:id="id153d54f4-076e-4166-a30c-78e29f2f23ec">
			<!-- ... -->
      <us-emf:facilityDescription>
        <gmd:PT_FreeText>
					<gmd:textGroup>
						  <gmd:LocalisedCharacterString locale="de_DE">Beschreibung der Aktivität</gmd:LocalisedCharacterString>
					</gmd:textGroup>
					<gmd:textGroup>
						  <gmd:LocalisedCharacterString locale="en_EN">Description of activity</gmd:LocalisedCharacterString>
					</gmd:textGroup>
				</gmd:PT_FreeText>
      </us-emf:facilityDescription>
		<!-- ... -->
</us-emf:EnvironmentalManagementFacility>

```

## Transformed instance (example)

```xml
<us-emfs:EnvironmentalManagementFacility gml:id="id153d54f4-076e-4166-a30c-78e29f2f23ec">
			<!-- ... -->
      <us-emfs:facilityDescription>
      	  <gmd:LocalisedCharacterString locale="de_DE">Beschreibung der Aktivität</gmd:LocalisedCharacterString>
				  <gmd:LocalisedCharacterString locale="en_EN">Description of activity</gmd:LocalisedCharacterString>
      </us-emfs:facilityDescription>
		<!-- ... -->
</us-emfs:EnvironmentalManagementFacility>
```

## Model transformation rule

Substitute existing `PT_FreeText` types with this SimplePT_FreeText type.

## Instance transformation rule

- Copy the value of `gmd:LocalisedCharacterString` to the property `gmd:LocalisedCharacterString`.
- Copy the value of `gmd:LocalisedCharacterString.locale` to the property `gmd:LocalisedCharacterString.locale`.

## Solves usability issues

The transformed data structure can easily be edited, filtered and symbolized in desktop GIS and web GIS software.

## Known usability issues

None.

## INSPIRE compliance

Fully compliant.

## Notes

- Not part of the original INSPIRE MIF 2017.2 catalogue (MT001–MT009); added in this project.
