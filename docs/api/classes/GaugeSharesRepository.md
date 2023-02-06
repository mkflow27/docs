# Class: GaugeSharesRepository

## Hierarchy

- `GaugesSubgraphRepository`<[`GaugeShare`](../interfaces/GaugeShare.md), [`GaugeShareAttributes`](../enums/GaugeShareAttributes.md)\>

  ↳ **`GaugeSharesRepository`**

## Table of contents

### Constructors

- [constructor](GaugeSharesRepository.md#constructor)

### Properties

- [blockHeight](GaugeSharesRepository.md#blockheight)
- [chainId](GaugeSharesRepository.md#chainid)
- [client](GaugeSharesRepository.md#client)

### Methods

- [find](GaugeSharesRepository.md#find)
- [findAllBy](GaugeSharesRepository.md#findallby)
- [findBy](GaugeSharesRepository.md#findby)
- [findByGauge](GaugeSharesRepository.md#findbygauge)
- [findByUser](GaugeSharesRepository.md#findbyuser)
- [get](GaugeSharesRepository.md#get)
- [mapType](GaugeSharesRepository.md#maptype)
- [query](GaugeSharesRepository.md#query)

## Constructors

### constructor

• **new GaugeSharesRepository**(`url`, `chainId`, `blockHeight?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |
| `chainId` | [`Network`](../enums/Network.md) |
| `blockHeight?` | () => `Promise`<`undefined` \| `number`\> |

#### Inherited from

GaugesSubgraphRepository<
  GaugeShare,
  GaugeShareAttributes
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

▸ **find**(`id`): `Promise`<`undefined` \| [`GaugeShare`](../interfaces/GaugeShare.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |

#### Returns

`Promise`<`undefined` \| [`GaugeShare`](../interfaces/GaugeShare.md)\>

#### Inherited from

GaugesSubgraphRepository.find

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts:16](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts#L16)

___

### findAllBy

▸ **findAllBy**(`attribute`, `value`, `first?`, `skip?`): `Promise`<[`GaugeShare`](../interfaces/GaugeShare.md)[]\>

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `attribute` | [`GaugeShareAttributes`](../enums/GaugeShareAttributes.md) | `undefined` |
| `value` | `string` | `undefined` |
| `first` | `number` | `1000` |
| `skip` | `number` | `0` |

#### Returns

`Promise`<[`GaugeShare`](../interfaces/GaugeShare.md)[]\>

#### Inherited from

GaugesSubgraphRepository.findAllBy

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts:24](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts#L24)

___

### findBy

▸ **findBy**(`attribute`, `value`): `Promise`<`undefined` \| [`GaugeShare`](../interfaces/GaugeShare.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `attribute` | [`GaugeShareAttributes`](../enums/GaugeShareAttributes.md) |
| `value` | `string` |

#### Returns

`Promise`<`undefined` \| [`GaugeShare`](../interfaces/GaugeShare.md)\>

#### Inherited from

GaugesSubgraphRepository.findBy

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts:20](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts#L20)

___

### findByGauge

▸ **findByGauge**(`gaugeId`, `first?`, `skip?`): `Promise`<[`GaugeShare`](../interfaces/GaugeShare.md)[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `gaugeId` | `string` |
| `first?` | `number` |
| `skip?` | `number` |

#### Returns

`Promise`<[`GaugeShare`](../interfaces/GaugeShare.md)[]\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/gauge-shares/repository.ts:51](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/gauge-shares/repository.ts#L51)

___

### findByUser

▸ **findByUser**(`userAddress`, `first?`, `skip?`): `Promise`<[`GaugeShare`](../interfaces/GaugeShare.md)[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `userAddress` | `string` |
| `first?` | `number` |
| `skip?` | `number` |

#### Returns

`Promise`<[`GaugeShare`](../interfaces/GaugeShare.md)[]\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/gauge-shares/repository.ts:38](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/gauge-shares/repository.ts#L38)

___

### get

▸ **get**(`args`): `Promise`<`undefined` \| [`GaugeShare`](../interfaces/GaugeShare.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | `any` |

#### Returns

`Promise`<`undefined` \| [`GaugeShare`](../interfaces/GaugeShare.md)\>

#### Inherited from

GaugesSubgraphRepository.get

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts:11](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts#L11)

___

### mapType

▸ **mapType**(`subgraphGaugeShare`): [`GaugeShare`](../interfaces/GaugeShare.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `subgraphGaugeShare` | `SubgraphGaugeShareFragment` |

#### Returns

[`GaugeShare`](../interfaces/GaugeShare.md)

#### Overrides

GaugesSubgraphRepository.mapType

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/gauge-shares/repository.ts:24](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/gauge-shares/repository.ts#L24)

___

### query

▸ **query**(`args`): `Promise`<[`GaugeShare`](../interfaces/GaugeShare.md)[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | `any` |

#### Returns

`Promise`<[`GaugeShare`](../interfaces/GaugeShare.md)[]\>

#### Overrides

GaugesSubgraphRepository.query

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/gauge-shares/repository.ts:14](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/gauge-shares/repository.ts#L14)
