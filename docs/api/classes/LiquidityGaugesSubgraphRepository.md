# Class: LiquidityGaugesSubgraphRepository

Access liquidity gauges indexed by subgraph.
Because we have ~100 gauges to save on repeated http calls we cache all results as `gauges` on an instance.
Balancer's subgraph URL: https://thegraph.com/hosted-service/subgraph/balancer-labs/balancer-gauges

## Implements

- [`Findable`](../interfaces/Findable.md)<`SubgraphLiquidityGauge`\>

## Table of contents

### Constructors

- [constructor](LiquidityGaugesSubgraphRepository.md#constructor)

### Properties

- [client](LiquidityGaugesSubgraphRepository.md#client)
- [gauges](LiquidityGaugesSubgraphRepository.md#gauges)

### Methods

- [fetch](LiquidityGaugesSubgraphRepository.md#fetch)
- [find](LiquidityGaugesSubgraphRepository.md#find)
- [findBy](LiquidityGaugesSubgraphRepository.md#findby)

## Constructors

### constructor

• **new LiquidityGaugesSubgraphRepository**(`url`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/subgraph.ts:19](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/subgraph.ts#L19)

## Properties

### client

• `Private` **client**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `GaugeShare` | (`variables`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `id`: `string`  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`GaugeShareQuery`\> |
| `GaugeShares` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`GaugeShare_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`GaugeShare_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`GaugeSharesQuery`\> |
| `LiquidityGauges` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`LiquidityGauge_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`LiquidityGauge_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`LiquidityGaugesQuery`\> |
| `PoolGauges` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`Pool_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`Pool_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolGaugesQuery`\> |
| `Pools` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`Pool_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`Pool_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolsQuery`\> |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/subgraph.ts:16](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/subgraph.ts#L16)

___

### gauges

• **gauges**: `LiquidityGauge`[] = `[]`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/subgraph.ts:17](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/subgraph.ts#L17)

## Methods

### fetch

▸ **fetch**(): `Promise`<`LiquidityGauge`[]\>

#### Returns

`Promise`<`LiquidityGauge`[]\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/subgraph.ts:23](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/subgraph.ts#L23)

___

### find

▸ **find**(`id`): `Promise`<`undefined` \| `LiquidityGauge`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |

#### Returns

`Promise`<`undefined` \| `LiquidityGauge`\>

#### Implementation of

Findable.find

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/subgraph.ts:38](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/subgraph.ts#L38)

___

### findBy

▸ **findBy**(`param`, `value`): `Promise`<`undefined` \| `LiquidityGauge`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `param` | `string` |
| `value` | `string` |

#### Returns

`Promise`<`undefined` \| `LiquidityGauge`\>

#### Implementation of

Findable.findBy

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/subgraph.ts:46](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/subgraph.ts#L46)
