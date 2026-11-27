# MT009: Simplified Period

> **Implementation note.** As applied in the theme encodings, the rule
> collapses a period property to two datetime leaves, `<prop>_beginPosition` /
> `<prop>_endPosition`. It matches a property whose data type is a period type
> (`OperationalActivityPeriod`, `TM_Period`, or a `gml:TimePeriod` wrapper) or any
> type listed in the optional **`types`** parameter; a `gml:TimePeriod` wrapper is
> detected automatically.

## Category

Alternate Structures for specific types or type hierarchies

## Description

XML has primitive types for times and dates that are well supported through most software. In INSPIRE and the related ISO standards, a more powerful but also highly complex model is available that allows to precisely specify time-related information. This model allows any subtype of `AbstractTimeObject`, which can include `TimeEdge`, `TimeInstant`, `TimeNode` and `TimePeriods`. In several themes, such as EMF, other types build on top of this model, such as `ef:OperationalActivityPeriod`. Altogether, this means that relatively important information tends to be nested very deep in a structure, making it harder to create and to process.

Within this rule, we substitute these complex structures through a very simple structure with just two properties:

- beginPosition
- endPosition

Both of these are to use the same definitions for these two properties as in the original structure. Note that the `endPosition` is optional, so the simple type can also be used for periods that haven't ended yet.

## Original instance (example)

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

## Transformed instance (example)

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

## Model transformation rule

**Parameters:**

- `type`: The type to be substituted, e.g. `OperationalActivityPeriod`.

Substitute existing type as indicated by the `type` parameter with this `SimplePeriod` type.

## Instance transformation rule

- Copy the value of `gml:beginPosition` to the property `gml:beginPosition`.
- Copy the value of `gml:endPosition` to the property `gml:endPosition`.

## Solves usability issues

The transformed data structure can easily be edited, filtered and symbolized in desktop GIS and web GIS software. This transformation also reduces data volume in datasets.

## Known usability issues

None.

## INSPIRE compliance

This rule keeps only the begin and end positions and discards the richer temporal model (other `AbstractTimeObject` subtypes, indeterminate positions, calendar/reference-system detail). It is compliant where the period is a simple begin/end interval; time information expressed only through the fuller model is lost. Where that fuller information is present, the simplified form is conformant only as an *additional* encoding alongside the default GML.

## Notes

 * None.
