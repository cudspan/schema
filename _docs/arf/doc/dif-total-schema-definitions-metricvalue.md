# Untitled object in DIF Topology File Schema

```txt
http://turbonomic.com/dif-topology.json#/definitions/_dbMem/properties/dbMem/items
```




| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dif-total-schema.schema.json\*](../out/dif-total-schema.schema.json "open original schema") |

## items Type

`object` ([Details](dif-total-schema-definitions-metricvalue.md))

# undefined Properties

| Property              | Type     | Required | Nullable       | Defined by                                                                                                                                                                       |
| :-------------------- | -------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [average](#average)   | `number` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvalue-properties-average.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/average")   |
| [min](#min)           | `number` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvalue-properties-min.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/min")           |
| [max](#max)           | `number` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvalue-properties-max.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/max")           |
| [capacity](#capacity) | `number` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvalue-properties-capacity.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/capacity") |
| [unit](#unit)         | `string` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricunit.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/unit")                          |

## average




`average`

-   is required
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvalue-properties-average.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/average")

### average Type

`number`

## min




`min`

-   is optional
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvalue-properties-min.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/min")

### min Type

`number`

## max




`max`

-   is optional
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvalue-properties-max.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/max")

### max Type

`number`

## capacity




`capacity`

-   is optional
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvalue-properties-capacity.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/capacity")

### capacity Type

`number`

## unit

Units for different metrics


`unit`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricunit.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/unit")

### unit Type

`string`

### unit Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value     | Explanation |
| :-------- | ----------- |
| `"count"` |             |
| `"tps"`   |             |
| `"ms"`    |             |
| `"mb"`    |             |
| `"mhz"`   |             |
| `"pct"`   |             |
