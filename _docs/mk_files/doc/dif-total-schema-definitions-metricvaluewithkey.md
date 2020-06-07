# Untitled object in DIF Topology File Schema

```txt
http://turbonomic.com/dif-topology.json#/definitions/_kpi/properties/kpi/items
```




| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dif-total-schema.schema.json\*](../out/dif-total-schema.schema.json "open original schema") |

## items Type

`object` ([Details](dif-total-schema-definitions-metricvaluewithkey.md))

# undefined Properties

| Property                    | Type     | Required | Nullable       | Defined by                                                                                                                                                                                           |
| :-------------------------- | -------- | -------- | -------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [description](#description) | `string` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithkey-properties-description.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/description") |
| [key](#key)                 | `string` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithkey-properties-key.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/key")                 |
| [average](#average)         | `number` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithkey-properties-average.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/average")         |
| [capacity](#capacity)       | `number` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithkey-properties-capacity.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/capacity")       |
| [unit](#unit)               | `string` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricunit.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/unit")                                       |

## description




`description`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithkey-properties-description.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/description")

### description Type

`string`

## key




`key`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithkey-properties-key.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/key")

### key Type

`string`

## average




`average`

-   is required
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithkey-properties-average.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/average")

### average Type

`number`

## capacity




`capacity`

-   is optional
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithkey-properties-capacity.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/capacity")

### capacity Type

`number`

## unit

Units for different metrics


`unit`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricunit.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/unit")

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
