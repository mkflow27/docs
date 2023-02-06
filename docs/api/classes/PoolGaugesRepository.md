# Class: PoolGaugesRepository

## Hierarchy

- `GaugesSubgraphRepository`<[`PoolGauges`](../interfaces/PoolGauges.md), [`PoolGaugesAttributes`](../enums/PoolGaugesAttributes.md)\>

  ↳ **`PoolGaugesRepository`**

## Table of contents

### Constructors

- [constructor](PoolGaugesRepository.md#constructor)

### Properties

- [blockHeight](PoolGaugesRepository.md#blockheight)
- [chainId](PoolGaugesRepository.md#chainid)
- [client](PoolGaugesRepository.md#client)

### Methods

- [find](PoolGaugesRepository.md#find)
- [findAllBy](PoolGaugesRepository.md#findallby)
- [findBy](PoolGaugesRepository.md#findby)
- [get](PoolGaugesRepository.md#get)
- [mapType](PoolGaugesRepository.md#maptype)
- [query](PoolGaugesRepository.md#query)

## Constructors

### constructor

• **new PoolGaugesRepository**(`url`, `chainId`, `blockHeight?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |
| `chainId` | [`Network`](../enums/Network.md) |
| `blockHeight?` | () => `Promise`<`undefined` \| `number`\> |

#### Inherited from

GaugesSubgraphRepository<
  PoolGauges,
  PoolGaugesAttributes
\>.constructor

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/gauges-subgraph-repository.ts:11](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/gauges-subgraph-repository.ts#L11)

## Properties

### blockHeight

• `Protected` `Optional` **blockHeight**: () => `Promise`<`undefined` \| `number`\>

#### Type declaration

▸ (): `Promise`<`undefined` \| `number`\>

##### Returns

`Promise`<`undefined` \| `number`\>

#### Inherited from

GaugesSubgraphRepository.blockHeight

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/gauges-subgraph-repository.ts:14](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/gauges-subgraph-repository.ts#L14)

___

### chainId

• `Protected` **chainId**: [`Network`](../enums/Network.md)

#### Inherited from

GaugesSubgraphRepository.chainId

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/gauges-subgraph-repository.ts:13](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/gauges-subgraph-repository.ts#L13)

___

### client

• `Protected` **client**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `GaugeShare` | (`variables`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `id`: `string`  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`GaugeShareQuery`\> |
| `GaugeShares` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`GaugeShare_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`GaugeShare_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`GaugeSharesQuery`\> |
| `LiquidityGauges` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`LiquidityGauge_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`LiquidityGauge_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`LiquidityGaugesQuery`\> |
| `PoolGauges` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`Pool_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`Pool_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolGaugesQuery`\> |
| `Pools` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`Pool_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`Pool_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolsQuery`\> |

#### Inherited from

GaugesSubgraphRepository.client

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/gauges-subgraph-repository.ts:9](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/gauges-subgraph-repository.ts#L9)

## Methods

### find

▸ **find**(`id`): `Promise`<`undefined` \| [`PoolGauges`](../interfaces/PoolGauges.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |

#### Returns

`Promise`<`undefined` \| [`PoolGauges`](../interfaces/PoolGauges.md)\>

#### Inherited from

GaugesSubgraphRepository.find

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts:16](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts#L16)

___

### findAllBy

▸ **findAllBy**(`attribute`, `value`, `first?`, `skip?`): `Promise`<[`PoolGauges`](../interfaces/PoolGauges.md)[]\>

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `attribute` | [`PoolGaugesAttributes`](../enums/PoolGaugesAttributes.md) | `undefined` |
| `value` | `string` | `undefined` |
| `first` | `number` | `1000` |
| `skip` | `number` | `0` |

#### Returns

`Promise`<[`PoolGauges`](../interfaces/PoolGauges.md)[]\>

#### Inherited from

GaugesSubgraphRepository.findAllBy

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts:24](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts#L24)

___

### findBy

▸ **findBy**(`attribute`, `value`): `Promise`<`undefined` \| [`PoolGauges`](../interfaces/PoolGauges.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `attribute` | [`PoolGaugesAttributes`](../enums/PoolGaugesAttributes.md) |
| `value` | `string` |

#### Returns

`Promise`<`undefined` \| [`PoolGauges`](../interfaces/PoolGauges.md)\>

#### Inherited from

GaugesSubgraphRepository.findBy

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts:20](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts#L20)

___

### get

▸ **get**(`args`): `Promise`<`undefined` \| [`PoolGauges`](../interfaces/PoolGauges.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | `any` |

#### Returns

`Promise`<`undefined` \| [`PoolGauges`](../interfaces/PoolGauges.md)\>

#### Inherited from

GaugesSubgraphRepository.get

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts:11](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts#L11)

___

### mapType

▸ **mapType**(`fragment`): [`PoolGauges`](../interfaces/PoolGauges.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `fragment` | `any` |

#### Returns

[`PoolGauges`](../interfaces/PoolGauges.md)

#### Overrides

GaugesSubgraphRepository.mapType

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool-gauges/repository.ts:17](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool-gauges/repository.ts#L17)

___

### query

▸ **query**(`args`): `Promise`<[`PoolGauges`](../interfaces/PoolGauges.md)[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | `any` |

#### Returns

`Promise`<[`PoolGauges`](../interfaces/PoolGauges.md)[]\>

#### Overrides

GaugesSubgraphRepository.query

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool-gauges/repository.ts:9](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool-gauges/repository.ts#L9)
