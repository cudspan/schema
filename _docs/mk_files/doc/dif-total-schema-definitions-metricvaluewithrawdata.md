# Untitled object in DIF Topology File Schema

```txt
http://turbonomic.com/dif-topology.json#/definitions/_memory/properties/memory
```




| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dif-total-schema.schema.json\*](../out/dif-total-schema.schema.json "open original schema") |

## memory Type

`object` ([Details](dif-total-schema-definitions-metricvaluewithrawdata.md))

# undefined Properties

| Property              | Type     | Required | Nullable       | Defined by                                                                                                                                                                                             |
| :-------------------- | -------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [average](#average)   | `number` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-average.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/average")   |
| [min](#min)           | `number` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-min.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/min")           |
| [max](#max)           | `number` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-max.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/max")           |
| [capacity](#capacity) | `number` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-capacity.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/capacity") |
| [unit](#unit)         | `string` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricunit.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/unit")                                     |
| [rawData](#rawData)   | `object` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-rawdata.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/rawData")   |

## average




`average`

-   is required
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-average.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/average")

### average Type

`number`

## min




`min`

-   is optional
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-min.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/min")

### min Type

`number`

## max




`max`

-   is optional
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-max.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/max")

### max Type

`number`

## capacity




`capacity`

-   is optional
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-capacity.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/capacity")

### capacity Type

`number`

## unit

Units for different metrics


`unit`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricunit.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/unit")

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

## rawData




`rawData`

-   is optional
-   Type: `object` ([Details](dif-total-schema-definitions-metricvaluewithrawdata-properties-rawdata.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-rawdata.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/rawData")

### rawData Type

`object` ([Details](dif-total-schema-definitions-metricvaluewithrawdata-properties-rawdata.md))
