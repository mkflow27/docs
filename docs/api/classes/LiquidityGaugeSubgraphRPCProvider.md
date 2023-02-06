# Class: LiquidityGaugeSubgraphRPCProvider

## Implements

- [`Findable`](../interfaces/Findable.md)<[`LiquidityGauge`](../interfaces/LiquidityGauge.md)\>

## Table of contents

### Constructors

- [constructor](LiquidityGaugeSubgraphRPCProvider.md#constructor)

### Properties

- [chainId](LiquidityGaugeSubgraphRPCProvider.md#chainid)
- [gaugeController](LiquidityGaugeSubgraphRPCProvider.md#gaugecontroller)
- [gauges](LiquidityGaugeSubgraphRPCProvider.md#gauges)
- [multicall](LiquidityGaugeSubgraphRPCProvider.md#multicall)
- [relativeWeights](LiquidityGaugeSubgraphRPCProvider.md#relativeweights)
- [rewardData](LiquidityGaugeSubgraphRPCProvider.md#rewarddata)
- [subgraph](LiquidityGaugeSubgraphRPCProvider.md#subgraph)
- [workingSupplies](LiquidityGaugeSubgraphRPCProvider.md#workingsupplies)

### Methods

- [compose](LiquidityGaugeSubgraphRPCProvider.md#compose)
- [fetch](LiquidityGaugeSubgraphRPCProvider.md#fetch)
- [find](LiquidityGaugeSubgraphRPCProvider.md#find)
- [findBy](LiquidityGaugeSubgraphRPCProvider.md#findby)

## Constructors

### constructor

• **new LiquidityGaugeSubgraphRPCProvider**(`subgraphUrl`, `multicallAddress`, `gaugeControllerAddress`, `chainId`, `provider`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `subgraphUrl` | `string` |
| `multicallAddress` | `string` |
| `gaugeControllerAddress` | `string` |
| `chainId` | [`Network`](../enums/Network.md) |
| `provider` | `Provider` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/provider.ts:39](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/provider.ts#L39)

## Properties

### chainId

• `Private` **chainId**: [`Network`](../enums/Network.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/provider.ts:43](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/provider.ts#L43)

___

### gaugeController

• `Optional` **gaugeController**: [`GaugeControllerMulticallRepository`](GaugeControllerMulticallRepository.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/provider.ts:29](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/provider.ts#L29)

___

### gauges

• `Optional` **gauges**: `Promise`<[`LiquidityGauge`](../interfaces/LiquidityGauge.md)[]\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/provider.ts:37](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/provider.ts#L37)

___

### multicall

• **multicall**: [`LiquidityGaugesMulticallRepository`](LiquidityGaugesMulticallRepository.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/provider.ts:30](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/provider.ts#L30)

___

### relativeWeights

• **relativeWeights**: `Object` = `{}`

#### Index signature

▪ [gaugeAddress: `string`]: `number`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/provider.ts:33](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/provider.ts#L33)

___

### rewardData

• **rewardData**: `Object` = `{}`

#### Index signature

▪ [gaugeAddress: `string`]: { `[tokenAddress: string]`: [`RewardData`](../interfaces/RewardData.md);  }

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/provider.ts:34](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/provider.ts#L34)

___

### subgraph

• **subgraph**: [`LiquidityGaugesSubgraphRepository`](LiquidityGaugesSubgraphRepository.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/provider.ts:31](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/provider.ts#L31)

___

### workingSupplies

• **workingSupplies**: `Object` = `{}`

#### Index signature

▪ [gaugeAddress: `string`]: `number`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/provider.ts:32](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/provider.ts#L32)

## Methods

### compose

▸ `Private` **compose**(`subgraphGauge`): `Object`

#### Parameters

| Name | Type |
| :------ | :------ |
| `subgraphGauge` | `LiquidityGauge` |

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `id` | `string` |
| `name` | `string` |
| `poolAddress` | `string` |
| `poolId` | `undefined` \| `Maybe`<`string`\> |
| `relativeWeight` | `number` |
| `rewardTokens` | { `[tokenAddress: string]`: [`RewardData`](../interfaces/RewardData.md);  } |
| `totalSupply` | `number` |
| `workingSupply` | `number` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/provider.ts:147](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/provider.ts#L147)

___

### fetch

▸ **fetch**(): `Promise`<[`LiquidityGauge`](../interfaces/LiquidityGauge.md)[]\>

#### Returns

`Promise`<[`LiquidityGauge`](../interfaces/LiquidityGauge.md)[]\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/provider.ts:61](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/provider.ts#L61)

___

### find

▸ **find**(`id`): `Promise`<`undefined` \| [`LiquidityGauge`](../interfaces/LiquidityGauge.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |

#### Returns

`Promise`<`undefined` \| [`LiquidityGauge`](../interfaces/LiquidityGauge.md)\>

#### Implementation of

Findable.find

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/provider.ts:115](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/provider.ts#L115)

___

### findBy

▸ **findBy**(`attribute`, `value`): `Promise`<`undefined` \| [`LiquidityGauge`](../interfaces/LiquidityGauge.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `attribute` | `string` |
| `value` | `string` |

#### Returns

`Promise`<`undefined` \| [`LiquidityGauge`](../interfaces/LiquidityGauge.md)\>

#### Implementation of

Findable.findBy

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/provider.ts:123](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/provider.ts#L123)
