# Untitled object in DIF Topology File Schema

```txt
http://turbonomic.com/dif-topology.json#/definitions/metricsEntry/oneOf/10
```

Specification for DB Memory metrics


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dif-total-schema.schema.json\*](../out/dif-total-schema.schema.json "open original schema") |

## 10 Type

`object` ([Details](dif-total-schema-definitions-_dbmem.md))

# undefined Properties

| Property        | Type    | Required | Nullable       | Defined by                                                                                                                                                        |
| :-------------- | ------- | -------- | -------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [dbMem](#dbMem) | `array` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-_dbmem-properties-dbmem.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_dbMem/properties/dbMem") |

## dbMem




`dbMem`

-   is required
-   Type: `object[]` ([Details](dif-total-schema-definitions-metricvalue.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-_dbmem-properties-dbmem.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_dbMem/properties/dbMem")

### dbMem Type

`object[]` ([Details](dif-total-schema-definitions-metricvalue.md))

### dbMem Constraints

**minimum number of items**: the minimum number of items for this array is: `1`

**unique items**: all items in this array must be unique. Duplicates are not allowed.
