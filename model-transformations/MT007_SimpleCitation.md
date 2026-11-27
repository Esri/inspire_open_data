# MT007: Simplified Citation

> **Implementation note.** As applied in the theme encodings, the rule
> collapses a citation to five flat fields — `<prop>_citationDate`, `_citationLink`,
> `_citationName`, `_citationLevel`, `_citationType` (MT019 may shorten the prefix).
> Parameters: **`types`** — extra data-type names treated as citations;
> **`properties`** — property names to treat as citations (needed for by-reference
> citations that carry no inline citation type, e.g. `legalFoundationDocument`);
> **`levelAsCodelist`** — encode `citationLevel` as a value + `_href` codelist pair
> (default: a plain value).

## Category

Alternate Structures for specific types or type hierarchies

## Description

Citations are another element type that is used in many different places throughout the INSPIRE data specifications. ISO 19115 defines `CI_Citation`, which has a very deep structure that tend to bury key information, creating a lot of overhead. INSPIRE introduced two base types to simplify citations, `LegislationCitation` and `DocumentCitation`. However, in many places, `CI_Citation` is in use. This rule proposes a simplified alternative representation for `CI_Citation`. For consistency, it can also be used as a substitute to `LegislationCitation` and `DocumentCitation` when no external register is available.

The simplified citation is based on a link to an external publication and adds minimal information with five properties:

- citationDate
- citationLink
- citationName
- citationLevel
- citationType

Each of these properties maps directly to an existing property of the original citation types. The `citationType` property can be used to indicate what kind of citation is represented by this object; its values can be taken from the original type name, or can be based on a codelist.

## Original instance (example)

```xml
<am:ManagementRestrictionOrRegulationZone>
  <!-- ... -->
  <am:legalBasis
    xlink:href="http://www.retsinformation.dk/eli/lta/2017/122"
    xlink:title="Bekendtgørelse af lov om skove">
    <base2:LegislationCitation>
      <base2:name>Bekendtgørelse af lov om skove</base2:name>
      <base2:shortName>LBK nr 122 af 26/01/2017</base2:shortName>
      <base2:date>
        <gmd:CI_Date>
          <gmd:date>
            <gco:Date>2017-01-26</gco:Date>
          </gmd:date>
          <gmd:dateType>
            <gmd:CI_DateTypeCode
              codeListValue="creation"
              codeList="http://standards.iso.org/ittf/PubliclyAvailableStandards/ISO_19139_Schemas/resources/codelist/ML_gmxCodelists.xml#CI_DateTypeCode" />
          </gmd:dateType>
        </gmd:CI_Date>
      </base2:date>
      <base2:link>http://www.retsinformation.dk/eli/lta/2017/122</base2:link>
      <base2:level xlink:href="http://inspire.ec.europa.eu/codelist/LegislationLevelValue/national" xlink:title="national" />
    </base2:LegislationCitation>
  </am:legalBasis>
  <!-- ... -->
</am:ManagementRestrictionOrRegulationZone>
```

## Transformed instance (example)

```xml
<ems:EnvironmentalMonitoringFacility>
  <!-- ... -->
  <ems:legalBackground>
    <simple:SimpleCitation>
      <simple:name>Bekendtgørelse af lov om skove</simple:name>
      <simple:type>LegislationCitation</simple:type>
      <simple:date>2017-01-26</simple:date>
      <simple:link>http://www.retsinformation.dk/eli/lta/2017/122</simple:link>
      <simple:level xlink:href="http://inspire.ec.europa.eu/codelist/LegislationLevelValue/national" xlink:title="national" />
    </simple:SimpleCitation>
  </ems:legalBackground>
  <!-- ... -->
</ems:EnvironmentalMonitoringFacility>
```

## Model transformation rule

Substitute existing `LegislationCitation` and `CI_Citation` types with this SimpleCitation type.

## Instance transformation rule

- Copy the value of `base2:date` (`gmd:CI_Date`) to the property `simple:date`.
- Copy the value of `base2:name` to the property `simple:name`.
- Copy the value of `base2:link` to the property `simple:link`.
- Copy the value(s) of `base2:level` to the property `simple:level`. Note that only one link may be present in the data.
- Insert the element name `LegislationCitation` into the property `simple:type`.

## Solves usability issues

The transformed data structure can easily be edited, filtered and symbolized in desktop GIS and web GIS software. This transformation also reduces data volume.

## Known usability issues

None.

## INSPIRE compliance

This rule works only with one external link, and it removes finer-grained information about dates. Beyond name, date, link, level and type, the source citation types (`LegislationCitation` / `DocumentCitation` / `CI_Citation`) carry further attributes (e.g. shortName, identifiers, additional dates such as `dateEnteredIntoForce`, responsibleParty) that the five SimpleCitation fields do not retain. The simplified form is therefore a conformant INSPIRE encoding *on its own* only where those attributes are void for the dataset (or homogeneous and documented in metadata); otherwise it is conformant only as an *additional* encoding alongside the default GML. It can be combined with the [Property Composition to Association](./MT006_PropertyCompositionToAssociation.md) rule to add more information from an external register.

## Notes

 * None.
