# MT014: One Feature Class Per Geometry Type

> **Implementation note.** As applied in the theme encodings, the rule
> takes **`geometryTypes`** — a subset of
> `Point` | `Line` | `Surface`. The feature type is fanned out into one feature class
> per listed geometry, suffixed `P` / `L` / `S` (e.g. `…ZoneP` / `…ZoneL` / `…ZoneS`).

## Category

Alternate Structures for specific types or type hierarchies

## Description

The encoding in GML allows mixing geometry properties with different data types in the same file/structure. This is not possible in some GIS Databases. Therefore with this rule one Feature Class per geometry type is used to separate heterogeneous geometry types into tables. A suffix is used to indicate which type of Geometry is stored in each table. **P** for Point geometries, **L** for Line and **S** for Area geometries.

## Original instance (example)

```xml
	<gml:featureMember>
		<am:ManagementRestrictionOrRegulationZone>
			<am:geometry>
				<gml:Point ...>
					<!-- ... -->
				</gml:Point>
			</am:geometry>
			<!-- ... -->
		</am:ManagementRestrictionOrRegulationZone>
	</gml:featureMember>
	<gml:featureMember>
		<am:ManagementRestrictionOrRegulationZone>
			<am:geometry>
				<gml:LineString ...>
					<!-- ... -->
				</gml:LineString>
			</am:geometry>
			<!-- ... -->
		</am:ManagementRestrictionOrRegulationZone>
	</gml:featureMember>
	<gml:featureMember>
		<am:ManagementRestrictionOrRegulationZone >
			<gml:MultiSurface>
				<!-- ... -->
			</gml:MultiSurface>
		</am:ManagementRestrictionOrRegulationZone>
		<!-- ... -->
	</gml:featureMember>
```

## Transformed instance (example)

```xml
<gml:featureMember>
		<ams:ManagementRestrictionOrRegulationZoneP>
			<ams:geometry>
				<gml:Point ...>
					<!-- ... -->
				</gml:Point>
			</ams:geometry>
			<!-- ... -->
		</ams:ManagementRestrictionOrRegulationZoneP>
	</gml:featureMember>
	<gml:featureMember>
		<ams:ManagementRestrictionOrRegulationZoneL>
			<ams:geometry>
				<gml:LineString ...>
					<!-- ... -->
				</gml:LineString>
			</ams:geometry>
			<!-- ... -->
		</ams:ManagementRestrictionOrRegulationZoneL>
	</gml:featureMember>
	<gml:featureMember>
		<ams:ManagementRestrictionOrRegulationZoneS>
			<gml:MultiSurface>
				<!-- ... -->
			</gml:MultiSurface>
		</ams:ManagementRestrictionOrRegulationZoneS>
		<!-- ... -->
	</gml:featureMember>


``` 

## Model transformation rule

Store each object in table according to its geometry type.

## Instance transformation rule

- If the geometry is a point geometry copy the object into the FeatureClass ending with P
- If the geometry is a line geometry copy the object into the FeatureClass ending with L.
- If the geometry is an area geometry copy the object into the FeatureClass ending with S.

## Solves usability issues

The transformed data structure can easily be read and edited in desktop GIS and web GIS software.

## Known usability issues

There are at maximum 3 instead of one table in the target structure.

## INSPIRE compliance

No issues.

## Notes

- Not part of the original INSPIRE MIF 2017.2 catalogue (MT001–MT009); added in this project.
