---
Layout: page
---
```txt
http://turbonomic.com/dif-topology.json
```

Format for a DIF topology


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                 |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------------ |
| Can be instantiated | Yes        | Unknown status | No           | Forbidden         | Allowed               | none                | [dif-total-schema.schema.json](../out/dif-total-schema.schema.json "open original schema") |

## DIF Topology File Type

`object` ([DIF Topology File](dif-total-schema.md))

# DIF Topology File Properties

| Property                  | Type      | Required | Nullable       | Defined by                                                                                                                           |
| :------------------------ | --------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------------------------------- |
| [version](#version)       | `string`  | Required | cannot be null | [DIF Topology File](dif-total-schema-properties-version.md "http&#x3A;//turbonomic.com/dif-topology.json#/properties/version")       |
| [updateTime](#updateTime) | `integer` | Required | cannot be null | [DIF Topology File](dif-total-schema-properties-updatetime.md "http&#x3A;//turbonomic.com/dif-topology.json#/properties/updateTime") |
| [topology](#topology)     | `array`   | Required | cannot be null | [DIF Topology File](dif-total-schema-properties-topology.md "http&#x3A;//turbonomic.com/dif-topology.json#/properties/topology")     |

## version




`version`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-properties-version.md "http&#x3A;//turbonomic.com/dif-topology.json#/properties/version")

### version Type

`string`

## updateTime

Epoch timestamp for when files are generated


`updateTime`

-   is required
-   Type: `integer`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-properties-updatetime.md "http&#x3A;//turbonomic.com/dif-topology.json#/properties/updateTime")

### updateTime Type

`integer`

## topology

List of topology entities WOOF <h1>LINK BELOW</h1><p>This is more text! <a href='http://www.cudspan.net'>CLICK ME</a></p>


`topology`

-   is required
-   Type: `object[]` ([Details](dif-total-schema-definitions-entity.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-properties-topology.md "http&#x3A;//turbonomic.com/dif-topology.json#/properties/topology")

### topology Type

`object[]` ([Details](dif-total-schema-definitions-entity.md))

### topology Constraints

**minimum number of items**: the minimum number of items for this array is: `1`

# DIF Topology File Definitions

## Definitions group entityType

Reference this group by using

```json
{"$ref":"http://turbonomic.com/dif-topology.json#/definitions/entityType"}
```

| Property | Type | Required | Nullable | Defined by |
| :------- | ---- | -------- | -------- | :--------- |

## Definitions group hostEntityType

Reference this group by using

```json
{"$ref":"http://turbonomic.com/dif-topology.json#/definitions/hostEntityType"}
```

| Property | Type | Required | Nullable | Defined by |
| :------- | ---- | -------- | -------- | :--------- |

## Definitions group metricUnit

Reference this group by using

```json
{"$ref":"http://turbonomic.com/dif-topology.json#/definitions/metricUnit"}
```

| Property | Type | Required | Nullable | Defined by |
| :------- | ---- | -------- | -------- | :--------- |

## Definitions group metricValue

Reference this group by using

```json
{"$ref":"http://turbonomic.com/dif-topology.json#/definitions/metricValue"}
```

| Property              | Type     | Required | Nullable       | Defined by                                                                                                                                                                       |
| :-------------------- | -------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [average](#average)   | `number` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvalue-properties-average.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/average")   |
| [min](#min)           | `number` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvalue-properties-min.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/min")           |
| [max](#max)           | `number` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvalue-properties-max.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/max")           |
| [capacity](#capacity) | `number` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvalue-properties-capacity.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/capacity") |
| [unit](#unit)         | `string` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvalue-properties-unit.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/unit")         |

### average




`average`

-   is required
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvalue-properties-average.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/average")

#### average Type

`number`

### min




`min`

-   is optional
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvalue-properties-min.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/min")

#### min Type

`number`

### max




`max`

-   is optional
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvalue-properties-max.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/max")

#### max Type

`number`

### capacity




`capacity`

-   is optional
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvalue-properties-capacity.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/capacity")

#### capacity Type

`number`

### unit

Units for different metrics


`unit`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvalue-properties-unit.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValue/properties/unit")

#### unit Type

`string`

#### unit Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value     | Explanation |
| :-------- | ----------- |
| `"count"` |             |
| `"tps"`   |             |
| `"ms"`    |             |
| `"mb"`    |             |
| `"mhz"`   |             |
| `"pct"`   |             |

## Definitions group metricsEntry

Reference this group by using

```json
{"$ref":"http://turbonomic.com/dif-topology.json#/definitions/metricsEntry"}
```

| Property | Type | Required | Nullable | Defined by |
| :------- | ---- | -------- | -------- | :--------- |

## Definitions group \_responseTime

Reference this group by using

```json
{"$ref":"http://turbonomic.com/dif-topology.json#/definitions/_responseTime"}
```

| Property                      | Type     | Required | Nullable       | Defined by                                                                                                                                                          |
| :---------------------------- | -------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [responseTime](#responseTime) | `object` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvalue.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_responseTime/properties/responseTime") |

### responseTime




`responseTime`

-   is required
-   Type: `object` ([Details](dif-total-schema-definitions-metricvalue.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvalue.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_responseTime/properties/responseTime")

#### responseTime Type

`object` ([Details](dif-total-schema-definitions-metricvalue.md))

## Definitions group \_transaction

Reference this group by using

```json
{"$ref":"http://turbonomic.com/dif-topology.json#/definitions/_transaction"}
```

| Property                    | Type     | Required | Nullable       | Defined by                                                                                                                                                        |
| :-------------------------- | -------- | -------- | -------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [transaction](#transaction) | `object` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvalue.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_transaction/properties/transaction") |

### transaction




`transaction`

-   is required
-   Type: `object` ([Details](dif-total-schema-definitions-metricvalue.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvalue.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_transaction/properties/transaction")

#### transaction Type

`object` ([Details](dif-total-schema-definitions-metricvalue.md))

## Definitions group \_connections

Reference this group by using

```json
{"$ref":"http://turbonomic.com/dif-topology.json#/definitions/_connections"}
```

| Property                    | Type     | Required | Nullable       | Defined by                                                                                                                                                        |
| :-------------------------- | -------- | -------- | -------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [connections](#connections) | `object` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvalue.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_connections/properties/connections") |

### connections




`connections`

-   is required
-   Type: `object` ([Details](dif-total-schema-definitions-metricvalue.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvalue.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_connections/properties/connections")

#### connections Type

`object` ([Details](dif-total-schema-definitions-metricvalue.md))

## Definitions group \_heap

Reference this group by using

```json
{"$ref":"http://turbonomic.com/dif-topology.json#/definitions/_heap"}
```

| Property      | Type     | Required | Nullable       | Defined by                                                                                                                                          |
| :------------ | -------- | -------- | -------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------- |
| [heap](#heap) | `object` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvalue.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_heap/properties/heap") |

### heap




`heap`

-   is required
-   Type: `object` ([Details](dif-total-schema-definitions-metricvalue.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvalue.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_heap/properties/heap")

#### heap Type

`object` ([Details](dif-total-schema-definitions-metricvalue.md))

## Definitions group \_collectionTime

Reference this group by using

```json
{"$ref":"http://turbonomic.com/dif-topology.json#/definitions/_collectionTime"}
```

| Property                          | Type     | Required | Nullable       | Defined by                                                                                                                                                              |
| :-------------------------------- | -------- | -------- | -------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [collectionTime](#collectionTime) | `object` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvalue.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_collectionTime/properties/collectionTime") |

### collectionTime




`collectionTime`

-   is required
-   Type: `object` ([Details](dif-total-schema-definitions-metricvalue.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvalue.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_collectionTime/properties/collectionTime")

#### collectionTime Type

`object` ([Details](dif-total-schema-definitions-metricvalue.md))

## Definitions group \_threads

Reference this group by using

```json
{"$ref":"http://turbonomic.com/dif-topology.json#/definitions/_threads"}
```

| Property            | Type    | Required | Nullable       | Defined by                                                                                                                                                                |
| :------------------ | ------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [threads](#threads) | `array` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-_threads-properties-threads.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_threads/properties/threads") |

### threads




`threads`

-   is required
-   Type: `object[]` ([Details](dif-total-schema-definitions-metricvalue.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-_threads-properties-threads.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_threads/properties/threads")

#### threads Type

`object[]` ([Details](dif-total-schema-definitions-metricvalue.md))

#### threads Constraints

**minimum number of items**: the minimum number of items for this array is: `1`

**unique items**: all items in this array must be unique. Duplicates are not allowed.

## Definitions group \_cacheHitRate

Reference this group by using

```json
{"$ref":"http://turbonomic.com/dif-topology.json#/definitions/_cacheHitRate"}
```

| Property                      | Type    | Required | Nullable       | Defined by                                                                                                                                                                                    |
| :---------------------------- | ------- | -------- | -------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [cacheHitRate](#cacheHitRate) | `array` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-_cachehitrate-properties-cachehitrate.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_cacheHitRate/properties/cacheHitRate") |

### cacheHitRate




`cacheHitRate`

-   is required
-   Type: `object[]` ([Details](dif-total-schema-definitions-metricvalue.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-_cachehitrate-properties-cachehitrate.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_cacheHitRate/properties/cacheHitRate")

#### cacheHitRate Type

`object[]` ([Details](dif-total-schema-definitions-metricvalue.md))

#### cacheHitRate Constraints

**minimum number of items**: the minimum number of items for this array is: `1`

**unique items**: all items in this array must be unique. Duplicates are not allowed.

## Definitions group \_dbMem

Reference this group by using

```json
{"$ref":"http://turbonomic.com/dif-topology.json#/definitions/_dbMem"}
```

| Property        | Type    | Required | Nullable       | Defined by                                                                                                                                                        |
| :-------------- | ------- | -------- | -------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [dbMem](#dbMem) | `array` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-_dbmem-properties-dbmem.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_dbMem/properties/dbMem") |

### dbMem




`dbMem`

-   is required
-   Type: `object[]` ([Details](dif-total-schema-definitions-metricvalue.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-_dbmem-properties-dbmem.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_dbMem/properties/dbMem")

#### dbMem Type

`object[]` ([Details](dif-total-schema-definitions-metricvalue.md))

#### dbMem Constraints

**minimum number of items**: the minimum number of items for this array is: `1`

**unique items**: all items in this array must be unique. Duplicates are not allowed.

## Definitions group \_cpu

Reference this group by using

```json
{"$ref":"http://turbonomic.com/dif-topology.json#/definitions/_cpu"}
```

| Property    | Type     | Required | Nullable       | Defined by                                                                                                                                                   |
| :---------- | -------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [cpu](#cpu) | `object` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_cpu/properties/cpu") |

### cpu




`cpu`

-   is required
-   Type: `object` ([Details](dif-total-schema-definitions-metricvaluewithrawdata.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_cpu/properties/cpu")

#### cpu Type

`object` ([Details](dif-total-schema-definitions-metricvaluewithrawdata.md))

## Definitions group \_memory

Reference this group by using

```json
{"$ref":"http://turbonomic.com/dif-topology.json#/definitions/_memory"}
```

| Property          | Type     | Required | Nullable       | Defined by                                                                                                                                                         |
| :---------------- | -------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [memory](#memory) | `object` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_memory/properties/memory") |

### memory




`memory`

-   is required
-   Type: `object` ([Details](dif-total-schema-definitions-metricvaluewithrawdata.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_memory/properties/memory")

#### memory Type

`object` ([Details](dif-total-schema-definitions-metricvaluewithrawdata.md))

## Definitions group \_kpi

Reference this group by using

```json
{"$ref":"http://turbonomic.com/dif-topology.json#/definitions/_kpi"}
```

| Property    | Type    | Required | Nullable       | Defined by                                                                                                                                                |
| :---------- | ------- | -------- | -------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [kpi](#kpi) | `array` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-_kpi-properties-kpi.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_kpi/properties/kpi") |

### kpi




`kpi`

-   is required
-   Type: `object[]` ([Details](dif-total-schema-definitions-metricvaluewithkey.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-_kpi-properties-kpi.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/\_kpi/properties/kpi")

#### kpi Type

`object[]` ([Details](dif-total-schema-definitions-metricvaluewithkey.md))

#### kpi Constraints

**minimum number of items**: the minimum number of items for this array is: `1`

**unique items**: all items in this array must be unique. Duplicates are not allowed.

## Definitions group metricValueWithKey

Reference this group by using

```json
{"$ref":"http://turbonomic.com/dif-topology.json#/definitions/metricValueWithKey"}
```

| Property                    | Type     | Required | Nullable       | Defined by                                                                                                                                                                                           |
| :-------------------------- | -------- | -------- | -------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [description](#description) | `string` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithkey-properties-description.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/description") |
| [key](#key)                 | `string` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithkey-properties-key.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/key")                 |
| [average](#average)         | `number` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithkey-properties-average.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/average")         |
| [capacity](#capacity)       | `number` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithkey-properties-capacity.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/capacity")       |
| [unit](#unit)               | `string` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithkey-properties-unit.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/unit")               |

### description




`description`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithkey-properties-description.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/description")

#### description Type

`string`

### key




`key`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithkey-properties-key.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/key")

#### key Type

`string`

### average




`average`

-   is required
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithkey-properties-average.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/average")

#### average Type

`number`

### capacity




`capacity`

-   is optional
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithkey-properties-capacity.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/capacity")

#### capacity Type

`number`

### unit

Units for different metrics


`unit`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithkey-properties-unit.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithKey/properties/unit")

#### unit Type

`string`

#### unit Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value     | Explanation |
| :-------- | ----------- |
| `"count"` |             |
| `"tps"`   |             |
| `"ms"`    |             |
| `"mb"`    |             |
| `"mhz"`   |             |
| `"pct"`   |             |

## Definitions group metricValueWithRawData

Reference this group by using

```json
{"$ref":"http://turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData"}
```

| Property              | Type     | Required | Nullable       | Defined by                                                                                                                                                                                             |
| :-------------------- | -------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [average](#average)   | `number` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-average.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/average")   |
| [min](#min)           | `number` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-min.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/min")           |
| [max](#max)           | `number` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-max.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/max")           |
| [capacity](#capacity) | `number` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-capacity.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/capacity") |
| [unit](#unit)         | `string` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-unit.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/unit")         |
| [rawData](#rawData)   | `object` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-rawdata.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/rawData")   |

### average




`average`

-   is required
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-average.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/average")

#### average Type

`number`

### min




`min`

-   is optional
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-min.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/min")

#### min Type

`number`

### max




`max`

-   is optional
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-max.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/max")

#### max Type

`number`

### capacity




`capacity`

-   is optional
-   Type: `number`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-capacity.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/capacity")

#### capacity Type

`number`

### unit

Units for different metrics


`unit`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-unit.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/unit")

#### unit Type

`string`

#### unit Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value     | Explanation |
| :-------- | ----------- |
| `"count"` |             |
| `"tps"`   |             |
| `"ms"`    |             |
| `"mb"`    |             |
| `"mhz"`   |             |
| `"pct"`   |             |

### rawData




`rawData`

-   is optional
-   Type: `object` ([Details](dif-total-schema-definitions-metricvaluewithrawdata-properties-rawdata.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-metricvaluewithrawdata-properties-rawdata.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/metricValueWithRawData/properties/rawData")

#### rawData Type

`object` ([Details](dif-total-schema-definitions-metricvaluewithrawdata-properties-rawdata.md))

## Definitions group entity

Reference this group by using

```json
{"$ref":"http://turbonomic.com/dif-topology.json#/definitions/entity"}
```

| Property                              | Type     | Required | Nullable       | Defined by                                                                                                                                                                             |
| :------------------------------------ | -------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [type](#type)                         | `string` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-entity-properties-type.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/type")                         |
| [uniqueId](#uniqueId)                 | `string` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-entity-properties-uniqueid.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/uniqueId")                 |
| [name](#name)                         | `string` | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-entity-properties-name.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/name")                         |
| [matchIdentifiers](#matchIdentifiers) | `object` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-entity-properties-matchidentifiers.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/matchIdentifiers") |
| [hostedOn](#hostedOn)                 | `object` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-entity-properties-hostedon.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/hostedOn")                 |
| [partOf](#partOf)                     | `array`  | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-entity-properties-partof.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/partOf")                     |
| [metrics](#metrics)                   | `array`  | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-entity-properties-metrics.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/metrics")                   |

### type

Entity type


`type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-entity-properties-type.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/type")

#### type Type

`string`

#### type Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                   | Explanation |
| :---------------------- | ----------- |
| `"businessApplication"` |             |
| `"businessTransaction"` |             |
| `"service"`             |             |
| `"databaseServer"`      |             |
| `"application"`         |             |

### uniqueId

Unique identifier for the entity, within the scope of the target


`uniqueId`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-entity-properties-uniqueid.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/uniqueId")

#### uniqueId Type

`string`

### name

Entity name


`name`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-entity-properties-name.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/name")

#### name Type

`string`

### matchIdentifiers

Attributes used to find the entity that matches this entity


`matchIdentifiers`

-   is optional
-   Type: `object` ([Details](dif-total-schema-definitions-entity-properties-matchidentifiers.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-entity-properties-matchidentifiers.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/matchIdentifiers")

#### matchIdentifiers Type

`object` ([Details](dif-total-schema-definitions-entity-properties-matchidentifiers.md))

### hostedOn

Attributes used to find the entity that hosts this entity


`hostedOn`

-   is optional
-   Type: `object` ([Details](dif-total-schema-definitions-entity-properties-hostedon.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-entity-properties-hostedon.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/hostedOn")

#### hostedOn Type

`object` ([Details](dif-total-schema-definitions-entity-properties-hostedon.md))

### partOf

Attributes used to find all the entities that this entity is part of


`partOf`

-   is optional
-   Type: `object[]` ([Details](dif-total-schema-definitions-entity-properties-partof-items.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-entity-properties-partof.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/partOf")

#### partOf Type

`object[]` ([Details](dif-total-schema-definitions-entity-properties-partof-items.md))

### metrics

List of metrics and values for the entity


`metrics`

-   is optional
-   Type: `object[]` ([Details](dif-total-schema-definitions-metricsentry.md))
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-entity-properties-metrics.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/metrics")

#### metrics Type

`object[]` ([Details](dif-total-schema-definitions-metricsentry.md))

#### metrics Constraints

**minimum number of items**: the minimum number of items for this array is: `1`
