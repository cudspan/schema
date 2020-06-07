---
Layout: page
---
```txt
http://turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/unit
```

Units for different metrics


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dif-total-schema.schema.json\*](../out/dif-total-schema.schema.json "open original schema") |

## unit Type

`string`

## unit Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value     | Explanation |
| :-------- | ----------- |
| `"count"` |             |
| `"tps"`   |             |
| `"ms"`    |             |
| `"mb"`    |             |
| `"mhz"`   |             |
| `"pct"`   |             |
