# MT012: Limit number of High Cardinality Objects

> **Implementation note.** As applied in the theme encodings, the rule
> takes **`limits`** — a list of `{path, number}` (path = selector). `number == 1`
> keeps the single occurrence under its own name; `number > 1` replicates the field(s)
> as `<name>_1 … <name>_N`. It runs on the tree before MT001 (for `number == 1`) or on
> the flattened field list after MT001 (for `number > 1`).

## Category

Alternate Structures for specific types or type hierarchies

## Description

Providing a data structure for high cardinality objects can be solved by creating extra tables. However these extra tables make it sometimes harder to access the information and in almost all cases the multiplicity required to store real data is much lower. In these cases we limit the maximum of a multiplicity to a fixed value. This increases the usability of the data and reduces the number of tables necessary to store the information, while still supporting most real world scenarios.

## Original instance (example)

```xml
<au:AdministrativeUnit>
<!-- ... -->
  <au:nationalLevelName>
    <gmd:LocalisedCharacterString>Name 1</gmd:LocalisedCharacterString>
  </au:nationalLevelName>
  <au:nationalLevelName>
    <gmd:LocalisedCharacterString>Name 2</gmd:LocalisedCharacterString>
  </au:nationalLevelName>
  <au:nationalLevelName>
    <gmd:LocalisedCharacterString>Name 3</gmd:LocalisedCharacterString>
  </au:nationalLevelName>
<!-- ... -->
</au:AdministrativeUnit>
  
```

## Transformed instance (example)

```xml
<aus:AdministrativeUnit>
<!-- ... -->
  <au:nationalLevelName_1>
    <gmd:LocalisedCharacterString>Name 1</gmd:LocalisedCharacterString>
  </au:nationalLevelName_1>
  <au:nationalLevelName_2>
    <gmd:LocalisedCharacterString>Name 2</gmd:LocalisedCharacterString>
  </au:nationalLevelName_2>
  <au:nationalLevelName_3>
    <gmd:LocalisedCharacterString>Name 3</gmd:LocalisedCharacterString>
  </au:nationalLevelName_3>
<!-- ... -->
</aus:AdministrativeUnit>


```

## Model transformation rule

**Parameters:**

- `number`: The number to which this cardinality is limited by the rule

Depending on the value of number limit a selected property occurrence.

## Instance transformation rule

- Copy the value of `property` to the same property with a number according to its position in the source data.

## Solves usability issues

The transformed data structure can easily be read and edited in desktop GIS and web GIS software. This transformation also reduces data volume.

## Known usability issues

Depending on the number of fields chosen there might be too many or not enough fields in the database.

## INSPIRE compliance

If the cardinality of a property in the source data is higher than the number selected for this rule there might be information loss.

## Notes

- Not part of the original INSPIRE MIF 2017.2 catalogue (MT001–MT009); added in this project.
