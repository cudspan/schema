# Untitled object in DIF Topology File Schema

```txt
http://turbonomic.com/dif-topology.json#/definitions/entity/properties/hostedOn
```

Attributes used to find the entity that hosts this entity


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                   |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dif-total-schema.schema.json\*](../out/dif-total-schema.schema.json "open original schema") |

## hostedOn Type

`object` ([Details](dif-total-schema-definitions-entity-properties-hostedon.md))

# undefined Properties

| Property                | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                       |
| :---------------------- | -------- | -------- | -------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [hostType](#hostType)   | `array`  | Required | cannot be null | [DIF Topology File](dif-total-schema-definitions-entity-properties-hostedon-properties-hosttype.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/hostedOn/properties/hostType")   |
| [hostUuid](#hostUuid)   | `string` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-entity-properties-hostedon-properties-hostuuid.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/hostedOn/properties/hostUuid")   |
| [ipAddress](#ipAddress) | `string` | Optional | cannot be null | [DIF Topology File](dif-total-schema-definitions-entity-properties-hostedon-properties-ipaddress.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/hostedOn/properties/ipAddress") |

## hostType

List of entity types of the possible underlying host entity. The order in which the entity types is specified is used to find the host entity.


`hostType`

-   is required
-   Type: `string[]`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-entity-properties-hostedon-properties-hosttype.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/hostedOn/properties/hostType")

### hostType Type

`string[]`

## hostUuid

Unique identifier for the host entity


`hostUuid`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-entity-properties-hostedon-properties-hostuuid.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/hostedOn/properties/hostUuid")

### hostUuid Type

`string`

## ipAddress

IP Address of the host entity


`ipAddress`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [DIF Topology File](dif-total-schema-definitions-entity-properties-hostedon-properties-ipaddress.md "http&#x3A;//turbonomic.com/dif-topology.json#/definitions/entity/properties/hostedOn/properties/ipAddress")

### ipAddress Type

`string`
