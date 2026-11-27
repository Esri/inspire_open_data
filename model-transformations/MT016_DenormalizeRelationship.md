# MT016: Denormalize Relationship

## Category

General model simplification rules

## Description

A bidirectional association in the INSPIRE model is navigable from both ends, but
one end is merely the **inverse** of the other and carries no independent
information — it can always be reconstructed from the forward side. This rule
**denormalizes** such an association by dropping the inverse (back-reference)
property and keeping only the forward association. For example, a network `Node`
carries `spokeStart`/`spokeEnd` that are just the inverse of a `Link`'s
`startNode`/`endNode`; the published field lists store only the link's forward
references and omit the node-side spokes. Removing the redundant inverse avoids a
second copy of the same relationship and keeps the encoded feature type lean.

A 1:n association may instead be denormalized the other way: drop the n-valued
forward property on the *one* side and place a single Long featureId **FK on the
many side**, so the relationship needs no extra relation table. When that FK is
not navigable in the source model it is **materialized** (opt-in via
`materialize`). Example: `Holding.contains` (1:n to `Site`) is dropped and a
single `Site.holding` FK is added on `Site`. (When the many-side FK already
exists in the source — as the transport `startNode`/`endNode` — only the inverse
is dropped and no materialization is needed.)

## Original instance (example)

```xml
<tn-w:WaterwayLink gml:id="Link_1">
  <tn:startNode xlink:href="#Node_1"/>
  <tn:endNode   xlink:href="#Node_2"/>
</tn-w:WaterwayLink>

<tn-w:WaterwayNode gml:id="Node_1">
  <tn:spokeStart xlink:href="#Link_1"/>   <!-- inverse of WaterwayLink.startNode -->
</tn-w:WaterwayNode>
```

## Transformed instance (example)

```xml
<tn-w:WaterwayLink gml:id="Link_1">
  <tn:startNode xlink:href="#Node_1"/>
  <tn:endNode   xlink:href="#Node_2"/>
</tn-w:WaterwayLink>

<tn-w:WaterwayNode gml:id="Node_1"/>       <!-- spokeStart/spokeEnd dropped -->
```

## Model transformation rule

**Parameters:**

- `inverses` (required): a list of `{ path, inverseOf }`-style objects, each with:
  - `path` (required): `<FeatureType>/<property>` — the inverse property to drop;
    applied only when the processed feature type matches the first path segment.
  - `inverseOf`: `<FeatureType>/<property>` naming the other end. Informative for
    a plain drop; with `materialize` it is the FK to create on the many side.
  - `materialize` (optional, default false): also add `inverseOf` as a single
    Long featureId FK on its feature type when it does not already exist (the
    inverse of the dropped 1:n forward association).

Drop each named `path` property from its feature type's structure before the
general flattening (`MT001`). A path that matches nothing is reported as a warning.
With `materialize`, additionally create the `inverseOf` FK on the many side.

## Instance transformation rule

Discard the inverse references at the node/source end. No values are copied; the
relationship remains fully recoverable by reading the retained forward association
(the link's `startNode`/`endNode`).

## Solves usability issues

- Removes a redundant second representation of the same relationship.
- Produces smaller, clearer feature types with a single, canonical navigation
  direction.

## Known usability issues

- The relationship is then navigable only from the forward end; a reverse lookup
  requires a query/join instead of a stored back-reference.

## INSPIRE compliance

Compliant: no information is lost — the dropped inverse end is derivable from the
retained forward association.

## Notes

- Used by the Transport Network themes to drop `spokeStart`/`spokeEnd` on the
  network node types (inverse of the link's `startNode`/`endNode`), and by
  AgriculturalAndAquacultureFacilities with `materialize` to turn `Holding.contains`
  (1:n) into the `Site.holding` FK on the many side.
- Not part of the original INSPIRE MIF 2017.2 catalogue (MT001–MT009); added in this project.
