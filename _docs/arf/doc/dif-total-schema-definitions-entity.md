# Untitled object in DIF Topology File Schema

```txt
http://turbonomic.com/dif-topology.json#/definitions/entity
```

Format for a DIF topology entity and metrics


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dif-total-schema.schema.json\*](../out/dif-total-schema.schema.json "open original schema") |

## entity Type

`object` ([Details](dif-total-schema-definitions-entity.md))

# undefined Properties

| Property                              | Type     | Required | Nullable       | Defined by                                                                                                                                                                             |
| :------------------------------------ | -------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [type](#type)                         | `string` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-entitytype.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/type")                                     |
| [uniqueId](#uniqueId)                 | `string` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-entity-properties-uniqueid.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/uniqueId")                 |
| [name](#name)                         | `string` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-entity-properties-name.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/name")                         |
| [matchIdentifiers](#matchIdentifiers) | `object` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-entity-properties-matchidentifiers.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/matchIdentifiers") |
| [hostedOn](#hostedOn)                 | `object` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-entity-properties-hostedon.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/hostedOn")                 |
| [partOf](#partOf)                     | `array`  | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-entity-properties-partof.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/partOf")                     |
| [metrics](#metrics)                   | `array`  | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-entity-properties-metrics.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/metrics")                   |

## type

Entity type


`type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-entitytype.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/type")

### type Type

`string`

### type Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                   | Explanation |
| :---------------------- | ----------- |
| `"businessApplication"` |             |
| `"businessTransaction"` |             |
| `"service"`             |             |
| `"databaseServer"`      |             |
| `"application"`         |             |

## uniqueId

Unique identifier for the entity, within the scope of the target


`uniqueId`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-entity-properties-uniqueid.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/uniqueId")

### uniqueId Type

`string`

## name

Entity name


`name`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-entity-properties-name.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/name")

### name Type

`string`

## matchIdentifiers

Attributes used to find the entity that matches this entity


`matchIdentifiers`

-   is optional
-   Type: `object` ([Details](dif-total-schema-definitions-entity-properties-matchidentifiers.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-entity-properties-matchidentifiers.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/matchIdentifiers")

### matchIdentifiers Type

`object` ([Details](dif-total-schema-definitions-entity-properties-matchidentifiers.md))

## hostedOn

Attributes used to find the entity that hosts this entity


`hostedOn`

-   is optional
-   Type: `object` ([Details](dif-total-schema-definitions-entity-properties-hostedon.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-entity-properties-hostedon.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/hostedOn")

### hostedOn Type

`object` ([Details](dif-total-schema-definitions-entity-properties-hostedon.md))

## partOf

Attributes used to find all the entities that this entity is part of


`partOf`

-   is optional
-   Type: `object[]` ([Details](dif-total-schema-definitions-entity-properties-partof-items.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-entity-properties-partof.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/partOf")

### partOf Type

`object[]` ([Details](dif-total-schema-definitions-entity-properties-partof-items.md))

## metrics

List of metrics and values for the entity


`metrics`

-   is optional
-   Type: `object[]` ([Details](dif-total-schema-definitions-metricsentry.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-entity-properties-metrics.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/metrics")

### metrics Type

`object[]` ([Details](dif-total-schema-definitions-metricsentry.md))

### metrics Constraints

**minimum number of items**: the minimum number of items for this array is: `1`
