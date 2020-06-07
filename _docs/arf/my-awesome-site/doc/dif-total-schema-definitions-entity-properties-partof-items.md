---
Layout: page
---
```txt
http://turbonomic.com/dif-topology.json#/definitions/entity/properties/partOf/items
```




| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dif-total-schema.schema.json\*](../out/dif-total-schema.schema.json "open original schema") |

## items Type

`object` ([Details](dif-total-schema-definitions-entity-properties-partof-items.md))

# undefined Properties

| Property              | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                             |
| :-------------------- | -------- | -------- | -------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [entity](#entity)     | `string` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-entitytype.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/partOf/items/properties/entity")                                           |
| [uniqueId](#uniqueId) | `string` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-entity-properties-partof-items-properties-uniqueid.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/partOf/items/properties/uniqueId") |

## entity

Entity type


`entity`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-entitytype.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/partOf/items/properties/entity")

### entity Type

`string`

### entity Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                   | Explanation |
| :---------------------- | ----------- |
| `"businessApplication"` |             |
| `"businessTransaction"` |             |
| `"service"`             |             |
| `"databaseServer"`      |             |
| `"application"`         |             |

## uniqueId

Unique identifier for the parent entity within the scope of this target


`uniqueId`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-entity-properties-partof-items-properties-uniqueid.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/partOf/items/properties/uniqueId")

### uniqueId Type

`string`
