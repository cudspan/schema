# Untitled object in DIF Topology File Schema

```txt
http://turbonomic.com/dif-topology.json#/definitions/metricsEntry/oneOf/5
```

Specification for the custom metrics


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dif-total-schema.schema.json\*](../out/dif-total-schema.schema.json "open original schema") |

## 5 Type

`object` ([Details](dif-total-schema-definitions-_kpi.md))

# undefined Properties

| Property    | Type    | Required | Nullable       | Defined by                                                                                                                                                |
| :---------- | ------- | -------- | -------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [kpi](#kpi) | `array` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-_kpi-properties-kpi.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_kpi/properties/kpi") |

## kpi




`kpi`

-   is required
-   Type: `object[]` ([Details](dif-total-schema-definitions-metricvaluewithkey.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-_kpi-properties-kpi.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_kpi/properties/kpi")

### kpi Type

`object[]` ([Details](dif-total-schema-definitions-metricvaluewithkey.md))

### kpi Constraints

**minimum number of items**: the minimum number of items for this array is: `1`

**unique items**: all items in this array must be unique. Duplicates are not allowed.
