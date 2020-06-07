---
Layout: page
---
```txt
http://turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/rawData
```




| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dif-total-schema.schema.json\*](../out/dif-total-schema.schema.json "open original schema") |

## rawData Type

`object` ([Details](dif-total-schema-definitions-metricvaluewithrawdata-properties-rawdata.md))

# undefined Properties

| Property                    | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                                         |
| :-------------------------- | -------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [utilization](#utilization) | `array`  | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-rawdata-properties-utilization.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/rawData/properties/utilization") |
| [units:](#units:)           | `string` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricunit.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/rawData/properties/units:")                                                            |

## utilization




`utilization`

-   is required
-   Type: `object[]` ([Details](dif-total-schema-definitions-metricvaluewithrawdata-properties-rawdata-properties-utilization-items.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-rawdata-properties-utilization.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/rawData/properties/utilization")

### utilization Type

`object[]` ([Details](dif-total-schema-definitions-metricvaluewithrawdata-properties-rawdata-properties-utilization-items.md))

### utilization Constraints

**minimum number of items**: the minimum number of items for this array is: `1`

## units:

Units for different metrics


`units:`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricunit.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/rawData/properties/units:")

### units: Type

`string`

### units: Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value     | Explanation |
| :-------- | ----------- |
| `"count"` |             |
| `"tps"`   |             |
| `"ms"`    |             |
| `"mb"`    |             |
| `"mhz"`   |             |
| `"pct"`   |             |
