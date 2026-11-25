# MT003: Inline associated or aggregated components using type names

> **Implementation note.** Parameters as applied in the theme encodings:
> **`property`** (required) — selector
> of the association property to inline; **`separator`** (default `_`);
> **`cardinality`** — map `{Type: n}` for numbered sub-blocks; **`discriminators`** —
> map `{Type: {values: [...]}}` for keyed sub-blocks; **`keep`** — map `{Type: "path"}`
> to inline only one value node of a component. The consumed component feature types
> are declared by the theme encoding rule (`featureTypes.consumed`).

## Category

General model simplification rules

## Description

Several INSPIRE themes, such as Transport and Addresses, use Associations to add a set of properties to a feature. An example for this is the `components` in `Address` in the *Addresses* theme. This property has a set of 1..n `AddressComponents` that together describe the actual address. In a simplified model, we want to replace this construct with a set of inlined properties. The individual components have a set of properties that make them unique - the *Type* of each property. We can thus use those Typenames to create a new set of properties from the original associated structures, like so:

- `component.ThoroughfareName`
- `component.PostalDescriptor`
- `component.AdminUnitName`
- `component.AddressAreaName`

If more than one occurrence of a specific type is present, it is differentiated by using a numeric postfix. These start with "1":

- `component.AdminUnitName_1`
- `component.AdminUnitName_2`
- `component.AdminUnitName_3`

This rule effectively denormalizes such associations. Please note that the individual properties such as `component_ThoroughfareName` are still complex; there is a need of additional rules to also simplify these.

## Original instance (example)

```xml
<ad:Address gml:id="MIG20172_example_Address">
	<ad:inspireId>...</ad:inspireId>
	<ad:position>...</ad:position>
	<ad:locator>...</ad:locator>
	<ad:component xlink:href="#ThoroughfareName_1"/>
	<ad:component xlink:href="#AddressAreaName_1"/>
	<ad:component xlink:href="#PostalDescriptor_1"/>
</ad:Address>
<!-- ... -->
<ad:ThoroughfareName gml:id="ThoroughfareName_1">
    <ad:inspireId>...</ad:inspireId>
    <ad:name>
        <ad:ThoroughfareNameValue>
            <ad:name>
                <GN:GeographicalName>
					<GN:language xsi:nil="true"/>
					...
					<GN:spelling>
						<GN:SpellingOfName>
							<GN:text>gn:language</GN:text>
						</GN:SpellingOfName>
					</GN:spelling>
					...
				</GN:GeographicalName>
            </ad:name>
        </ad:ThoroughfareNameValue>
    </ad:name>
</ad:ThoroughfareName>
<ad:AddressAreaName gml:id="AddressAreaName_1">
    <ad:inspireId>...</ad:inspireId>
    <ad:name>
        <gn:GeographicalName>
            <gn:language>ita</gn:language>
            ...
            <gn:spelling>
                <gn:SpellingOfName>
                    <gn:text>Ispra</gn:text>
                </gn:SpellingOfName>
            </gn:spelling>
            ...
        </gn:GeographicalName>
    </ad:name>
    <ad:namedPlace xsi:nil="true" nilReason="other:unpopulated"/>
</ad:AddressAreaName>
<ad:PostalDescriptor gml:id="PostalDescriptor_1">
    <ad:inspireId>...</ad:inspireId>
    <ad:postCode>21027</ad:postCode>
</ad:PostalDescriptor>
```

## Transformed instance (example)

```xml
<ads:Address gml:id="MIG20172_example_Address">
	<ads:inspireId>...</ads:inspireId>
	<ads:position>...</ads:position>
	<ads:locator>...</ads:locator>
	<ads:component_ThoroughfareName>
        <ad:ThoroughfareName gml:id="ThoroughfareName_1">
            <ad:inspireId>...</ad:inspireId>
            <ad:name>
                <ad:ThoroughfareNameValue>
                    <ad:name>
                        <GN:GeographicalName>
                            <GN:language xsi:nil="true"/>
                            ...
                            <GN:spelling>
                                <GN:SpellingOfName>
                                    <GN:text>gn:language</GN:text>
                                </GN:SpellingOfName>
                            </GN:spelling>
                            ...
                        </GN:GeographicalName>
                    </ad:name>
                </ad:ThoroughfareNameValue>
            </ad:name>
        </ad:ThoroughfareName>
    </ads:component_ThoroughfareName>
	<ads:component_AddressAreaName>
        <ad:AddressAreaName gml:id="AddressAreaName_1">
            <ad:inspireId>...</ad:inspireId>
            <ad:name>
                <gn:GeographicalName>
                    <gn:language>ita</gn:language>
                    ...
                    <gn:spelling>
                        <gn:SpellingOfName>
                            <gn:text>Ispra</gn:text>
                        </gn:SpellingOfName>
                    </gn:spelling>
                    ...
                </gn:GeographicalName>
            </ad:name>
            <ad:namedPlace xsi:nil="true" nilReason="other:unpopulated"/>
        </ad:AddressAreaName>
    </ads:component_AddressAreaName>
	<ads:component_PostalDescriptor>
        <ad:PostalDescriptor gml:id="PostalDescriptor_1">
            <ad:inspireId>...</ad:inspireId>
            <ad:postCode>21027</ad:postCode>
        </ad:PostalDescriptor>
    </ads:component_PostalDescriptor>
</ads:Address>
```

## Model transformation rule

**Parameters:**

- `separator`: The character to use to separate the original property name from the type name of the components.
- `cardinality`: An optional map with typenames and a number that indicates how many properties for a given type should be created.

Create a new property for every possible associated type, using the original property name, the separator, and the name of the element (i.e. without a ...type suffix) to build the new property name.

## Instance transformation rule

For each potential type of a value, a property is created, so instance values can be copied. Properties that are left empty after copying the source values can be removed (see example above).

## Solves usability issues

Data where key properties are in associated objects is hard to style and to filter for in most desktop GIS and web GIS software. The inlined data can be processed much easier by many tools, e.g. it can be converted to excel easily

## Known usability issues

Since this rule denormalizes components, it can increase total data volume.

## INSPIRE compliance

This rule can only be applied if there is at maximum one occurrence of each type in a set of properties, i.e. where the components are a key-value map with the keys being defined by the typenames.
