# Class: Pools

Controller / use-case layer for interacting with pools data.

## Implements

- [`Findable`](../interfaces/Findable.md)<[`PoolWithMethods`](../interfaces/PoolWithMethods.md)\>

## Table of contents

### Constructors

- [constructor](Pools.md#constructor)

### Properties

- [aprService](Pools.md#aprservice)
- [emissionsService](Pools.md#emissionsservice)
- [exitService](Pools.md#exitservice)
- [feesService](Pools.md#feesservice)
- [impermanentLossService](Pools.md#impermanentlossservice)
- [joinService](Pools.md#joinservice)
- [liquidityService](Pools.md#liquidityservice)
- [networkConfig](Pools.md#networkconfig)
- [poolFactory](Pools.md#poolfactory)
- [proportionalAmounts](Pools.md#proportionalamounts)
- [repositories](Pools.md#repositories)
- [volumeService](Pools.md#volumeservice)

### Methods

- [all](Pools.md#all)
- [apr](Pools.md#apr)
- [dataSource](Pools.md#datasource)
- [fees](Pools.md#fees)
- [find](Pools.md#find)
- [findBy](Pools.md#findby)
- [generalisedExit](Pools.md#generalisedexit)
- [generalisedJoin](Pools.md#generalisedjoin)
- [impermanentLoss](Pools.md#impermanentloss)
- [liquidity](Pools.md#liquidity)
- [volume](Pools.md#volume)
- [where](Pools.md#where)
- [wrap](Pools.md#wrap)

## Constructors

### constructor

• **new Pools**(`networkConfig`, `repositories`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `networkConfig` | [`BalancerNetworkConfig`](../interfaces/BalancerNetworkConfig.md) |
| `repositories` | [`BalancerDataRepositories`](../interfaces/BalancerDataRepositories.md) |

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:45](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L45)

## Properties

### aprService

• **aprService**: `PoolApr`

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:34](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L34)

___

### emissionsService

• **emissionsService**: `undefined` \| `EmissionsService`

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:42](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L42)

___

### exitService

• **exitService**: `Exit`

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:37](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L37)

___

### feesService

• **feesService**: `PoolFees`

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:38](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L38)

___

### impermanentLossService

• **impermanentLossService**: `ImpermanentLossService`

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:41](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L41)

___

### joinService

• **joinService**: `Join`

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:36](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L36)

___

### liquidityService

• **liquidityService**: [`Liquidity`](Liquidity.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:35](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L35)

___

### networkConfig

• `Private` **networkConfig**: [`BalancerNetworkConfig`](../interfaces/BalancerNetworkConfig.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:46](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L46)

___

### poolFactory

• **poolFactory**: `PoolFactory__factory`

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:40](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L40)

___

### proportionalAmounts

• **proportionalAmounts**: (`pool`: { `id`: `string` ; `tokens`: { `address`: `string` ; `balance`: `string` ; `decimals?`: `number`  }[]  }, `token`: `string`, `amount`: `string`) => { `amounts`: `string`[] ; `tokens`: `string`[]  }

#### Type declaration

▸ (`pool`, `token`, `amount`): `Object`

Calculates the proportional amounts of tokens in relation to a given token and amount.
Useful for calculating the amounts of tokens to be sent to a pool when joining or swapping.
When using proportional amounts to join a pool the price impact will be minimal.

**`Example`**

```ts
const pool = {
  id: '0x0000',
  tokens: [
    { address: '0x1234', balance: '10' },
    { address: '0x5678', balance: '20' }
  ]
}

const { tokens, amounts } = proportionalAmounts(pool, '0x1234', '1000000000000000000')
```

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pool` | `Object` | Pool object |
| `pool.id` | `string` | - |
| `pool.tokens` | { `address`: `string` ; `balance`: `string` ; `decimals?`: `number`  }[] | - |
| `token` | `string` | Token address in relation to which the amounts are calculated |
| `amount` | `string` | Amount of token |

##### Returns

`Object`

Object with tokens and amounts

| Name | Type |
| :------ | :------ |
| `amounts` | `string`[] |
| `tokens` | `string`[] |

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:43](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L43)

___

### repositories

• `Private` **repositories**: [`BalancerDataRepositories`](../interfaces/BalancerDataRepositories.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:47](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L47)

___

### volumeService

• **volumeService**: `PoolVolume`

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:39](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L39)

## Methods

### all

▸ **all**(): `Promise`<[`PoolWithMethods`](../interfaces/PoolWithMethods.md)[]\>

#### Returns

`Promise`<[`PoolWithMethods`](../interfaces/PoolWithMethods.md)[]\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:380](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L380)

___

### apr

▸ **apr**(`pool`): `Promise`<[`AprBreakdown`](../interfaces/AprBreakdown.md)\>

Calculates APR on any pool data

#### Parameters

| Name | Type |
| :------ | :------ |
| `pool` | [`Pool`](../interfaces/Pool.md) |

#### Returns

`Promise`<[`AprBreakdown`](../interfaces/AprBreakdown.md)\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:91](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L91)

___

### dataSource

▸ **dataSource**(): [`Findable`](../interfaces/Findable.md)<[`Pool`](../interfaces/Pool.md), [`PoolAttribute`](../modules.md#poolattribute), `any`\> & [`Searchable`](../interfaces/Searchable.md)<[`Pool`](../interfaces/Pool.md)\>

#### Returns

[`Findable`](../interfaces/Findable.md)<[`Pool`](../interfaces/Pool.md), [`PoolAttribute`](../modules.md#poolattribute), `any`\> & [`Searchable`](../interfaces/Searchable.md)<[`Pool`](../interfaces/Pool.md)\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:80](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L80)

___

### fees

▸ **fees**(`pool`): `Promise`<`number`\>

Calculates total fees for the pool in the last 24 hours

#### Parameters

| Name | Type |
| :------ | :------ |
| `pool` | [`Pool`](../interfaces/Pool.md) |

#### Returns

`Promise`<`number`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:193](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L193)

___

### find

▸ **find**(`id`): `Promise`<`undefined` \| [`PoolWithMethods`](../interfaces/PoolWithMethods.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |

#### Returns

`Promise`<`undefined` \| [`PoolWithMethods`](../interfaces/PoolWithMethods.md)\>

#### Implementation of

Findable.find

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:357](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L357)

___

### findBy

▸ **findBy**(`param`, `value`): `Promise`<`undefined` \| [`PoolWithMethods`](../interfaces/PoolWithMethods.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `param` | `string` |
| `value` | `string` |

#### Returns

`Promise`<`undefined` \| [`PoolWithMethods`](../interfaces/PoolWithMethods.md)\>

#### Implementation of

Findable.findBy

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:364](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L364)

___

### generalisedExit

▸ **generalisedExit**(`poolId`, `amount`, `userAddress`, `slippage`, `authorisation?`): `Promise`<{ `callData`: `string` ; `expectedAmountsOut`: `string`[] ; `minAmountsOut`: `string`[] ; `priceImpact`: `string` ; `to`: `string` ; `tokensOut`: `string`[]  }\>

Builds generalised exit transaction

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `poolId` | `string` | Pool id |
| `amount` | `string` | Token amount in EVM scale |
| `userAddress` | `string` | User address |
| `slippage` | `string` | Maximum slippage tolerance in bps i.e. 50 = 0.5%. |
| `authorisation?` | `string` | Optional auhtorisation call to be added to the chained transaction |

#### Returns

`Promise`<{ `callData`: `string` ; `expectedAmountsOut`: `string`[] ; `minAmountsOut`: `string`[] ; `priceImpact`: `string` ; `to`: `string` ; `tokensOut`: `string`[]  }\>

transaction data ready to be sent to the network along with tokens, min and expected amounts out.

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:164](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L164)

___

### generalisedJoin

▸ **generalisedJoin**(`poolId`, `tokens`, `amounts`, `userAddress`, `wrapMainTokens`, `slippage`, `authorisation?`): `Promise`<{ `callData`: `string` ; `expectedOut`: `string` ; `minOut`: `string` ; `priceImpact`: `string` ; `to`: `string`  }\>

Builds generalised join transaction

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `poolId` | `string` | Pool id |
| `tokens` | `string`[] | Token addresses |
| `amounts` | `string`[] | Token amounts in EVM scale |
| `userAddress` | `string` | User address |
| `wrapMainTokens` | `boolean` | Indicates whether main tokens should be wrapped before being used |
| `slippage` | `string` | Maximum slippage tolerance in bps i.e. 50 = 0.5%. |
| `authorisation?` | `string` | Optional auhtorisation call to be added to the chained transaction |

#### Returns

`Promise`<{ `callData`: `string` ; `expectedOut`: `string` ; `minOut`: `string` ; `priceImpact`: `string` ; `to`: `string`  }\>

transaction data ready to be sent to the network along with min and expected BPT amounts out.

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:128](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L128)

___

### impermanentLoss

▸ **impermanentLoss**(`timestamp`, `pool`): `Promise`<`number`\>

Calculates Impermanent Loss on any pool data

#### Parameters

| Name | Type |
| :------ | :------ |
| `timestamp` | `number` |
| `pool` | [`Pool`](../interfaces/Pool.md) |

#### Returns

`Promise`<`number`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:102](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L102)

___

### liquidity

▸ **liquidity**(`pool`): `Promise`<`string`\>

Calculates total liquidity of the pool

#### Parameters

| Name | Type |
| :------ | :------ |
| `pool` | [`Pool`](../interfaces/Pool.md) |

#### Returns

`Promise`<`string`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:112](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L112)

___

### volume

▸ **volume**(`pool`): `Promise`<`number`\>

Calculates total volume of the pool in the last 24 hours

#### Parameters

| Name | Type |
| :------ | :------ |
| `pool` | [`Pool`](../interfaces/Pool.md) |

#### Returns

`Promise`<`number`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:203](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L203)

___

### where

▸ **where**(`filter`): `Promise`<[`PoolWithMethods`](../interfaces/PoolWithMethods.md)[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `filter` | (`pool`: [`Pool`](../interfaces/Pool.md)) => `boolean` |

#### Returns

`Promise`<[`PoolWithMethods`](../interfaces/PoolWithMethods.md)[]\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:389](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L389)

___

### wrap

▸ `Static` **wrap**(`pool`, `networkConfig`): [`PoolWithMethods`](../interfaces/PoolWithMethods.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `pool` | [`Pool`](../interfaces/Pool.md) |
| `networkConfig` | [`BalancerNetworkConfig`](../interfaces/BalancerNetworkConfig.md) |

#### Returns

[`PoolWithMethods`](../interfaces/PoolWithMethods.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/index.ts:207](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/index.ts#L207)
