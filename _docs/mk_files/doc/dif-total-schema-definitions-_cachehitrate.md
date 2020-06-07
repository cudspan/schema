# Untitled object in DIF Topology File Schema

```txt
http://turbonomic.com/dif-topology.json#/definitions/metricsEntry/oneOf/9
```

Specification for DB Cache Hit Rate metrics


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dif-total-schema.schema.json\*](../out/dif-total-schema.schema.json "open original schema") |

## 9 Type

`object` ([Details](dif-total-schema-definitions-_cachehitrate.md))

# undefined Properties

| Property                      | Type    | Required | Nullable       | Defined by                                                                                                                                                                                    |
| :---------------------------- | ------- | -------- | -------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [cacheHitRate](#cacheHitRate) | `array` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-_cachehitrate-properties-cachehitrate.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_cacheHitRate/properties/cacheHitRate") |

## cacheHitRate




`cacheHitRate`

-   is required
-   Type: `object[]` ([Details](dif-total-schema-definitions-metricvalue.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-_cachehitrate-properties-cachehitrate.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_cacheHitRate/properties/cacheHitRate")

### cacheHitRate Type

`object[]` ([Details](dif-total-schema-definitions-metricvalue.md))

### cacheHitRate Constraints

**minimum number of items**: the minimum number of items for this array is: `1`

**unique items**: all items in this array must be unique. Duplicates are not allowed.
