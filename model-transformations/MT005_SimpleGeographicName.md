# MT005: Simplified Geographical Name

> **Implementation note.** `MT005` as applied in the theme encodings differs from the
> original MIG description below: instead of one field per language (`name_deu`/`name_eng`), it
> collapses each `GeographicalName` to **one Text name value** (dropping nativeness,
> nameStatus, spelling, pronunciation, grammatical*, and by default language).
> Optional parameters:
> - `language: true` — also keep a single `<name>_language` companion. **This
>   subsumes the former standalone *SimpleGeographicNamePlusLanguage* rule**, which was
>   merged into MT005; the ~10 themes that used it now use `MT005` with `language: true`.
> - `nameLeaf: true` — carry the value in a `name` child so flattening yields
>   `<property>_name` (the published Esri form) instead of `<property>`.

## Category

Alternate Structures for specific types or type hierarchies

## Description

Geographical Names are re-used throughout more than 20 INSPIRE themes overall, ranging from Cadastral Parcels and Addresses to Statistical Units. For many existing data sets, the `GeographicalName` type is overspecified, with very little information being unique to each instance. For cases where only minimal information on names is available, this simplified structure can be used. One key use case that is quite frequent however is to have names in more than one language. There are multiple official languages in more than half of the countries affected by INSPIRE.

The simplified name consists of one property per language, which will contain the `spelling.text` subproperty value of the original property:

- `name_deu`
- `name_fra`

For other properties of the original `GeographicalName`, such as `nameStatus` and `nativeness`, defaults may be documented in the dataset metadata.

## Original instance (example)

```xml
<gn:NamedPlace gml:id="MIG20172_example_NamedPlace">
	<gn:beginLifespanVersion xsi:nil="true"/>
	<gn:geometry>
		<gml:Point gml:id="_d7180a8f-a590-44da-8b45-41d96d5cba5e" srsName="http://www.opengis.net/def/crs/EPSG/0/25832" srsDimension="2">
		<gml:pos>471979.2568 5564594.2444</gml:pos>
		</gml:Point>
	</gn:geometry>
	<gn:inspireId>
		<base:Identifier>
			<base:localId>NamedPlace_Example</base:localId>
			<base:namespace>https://www.examples.eu/</base:namespace>
		</base:Identifier>
	</gn:inspireId>
	<gn:localType xsi:nil="true"/>
	<gn:name>
		<gn:GeographicalName>
			<gn:language>deu</gn:language>
			<gn:nativeness xsi:nil="true"/>
			<gn:nameStatus xsi:nil="true"/>
			<gn:sourceOfName xsi:nil="true"/>
			<gn:pronunciation xsi:nil="true"/>
			<gn:spelling>
				<gn:SpellingOfName>
				<gn:text>München</gn:text>
				<gn:script xsi:nil="true"/>
				</gn:SpellingOfName>
			</gn:spelling>
		</gn:GeographicalName>
	</gn:name>
	<gn:name>
		<gn:GeographicalName>
			<gn:language>eng</gn:language>
			<gn:nativeness xsi:nil="true"/>
			<gn:nameStatus xsi:nil="true"/>
			<gn:sourceOfName xsi:nil="true"/>
			<gn:pronunciation xsi:nil="true"/>
			<gn:spelling>
				<gn:SpellingOfName>
				<gn:text>Munich</gn:text>
				<gn:script xsi:nil="true"/>
				</gn:SpellingOfName>
			</gn:spelling>
		</gn:GeographicalName>
	</gn:name>
	<gn:type xsi:nil="true"/>
</gn:NamedPlace>
```

## Transformed instance (example)

```xml
<gns:NamedPlace gml:id="MIG20172_example_NamedPlace">
	<gns:beginLifespanVersion xsi:nil="true"/>
	<gns:geometry>
		<gml:Point gml:id="_d7180a8f-a590-44da-8b45-41d96d5cba5e" srsName="http://www.opengis.net/def/crs/EPSG/0/25832" srsDimension="2">
		<gml:pos>471979.2568 5564594.2444</gml:pos>
		</gml:Point>
	</gns:geometry>
	<gns:inspireId>
		<base:Identifier>
			<base:localId>NamedPlace_Example</base:localId>
			<base:namespace>https://www.examples.eu/</base:namespace>
		</base:Identifier>
	</gns:inspireId>
	<gns:localType xsi:nil="true"/>
	<gns:name_deu>München</gns:name_deu>
	<gns:name_eng>Munich</gns:name_eng>
	<gns:type xsi:nil="true"/>
</gns:NamedPlace>
```

## Model transformation rule

**Parameters:**

- `separator`: The character to use to separate the original property name from the ISO 693-3 or ISO 693-5 language codes.
- `languageCodes`: A List of ISO 693-3 or ISO 693-5 codes for which to create the specific properties.

Create a new property for every language given as a parameter. Give each property as name the concatenation of "name", the value of the separator parameter and the ISO 693-3 or ISO 693-5 code of the language.

## Instance transformation rule

Copy the value of the `spelling.text` to the new property.

## Solves usability issues

The transformed data structure can easily be edited, filtered and symbolized in desktop GIS and web GIS software. This transformation also reduced data volume significantly in datasets that use in-place encoding of `GeographicalNames`.

## Known usability issues

None.

## INSPIRE compliance

This rule discards individual metadata about geographical names, such as the name status and its nativeness. If this information is homogeneous, it should be documented in the dataset metadata. If it is heterogeneous, this transformation will result in a loss of information.

**Reversibility (as applied here).** Beyond the MIG rule, `MT005` as applied in the theme encodings reduces each feature to a **single** name value and, unless `language` is set, drops the language as well as any additional name variants. It is a conformant INSPIRE encoding *on its own* only where the feature carries a single name and the dropped attributes (language, nameStatus, nativeness, sourceOfName, pronunciation, spelling metadata, additional names) are void — or homogeneous and documented in the dataset metadata, so the default encoding is recoverable. Otherwise it is conformant only as an *additional* encoding alongside the default GML.

## Notes

- This rule may be enhanced by storing additional properties that were present on the original name in "subfields" such as `name.deu.nativeness`.
