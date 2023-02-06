# Interface: Findable<T, P, V\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | `T` |
| `P` | `string` |
| `V` | `any` |

## Implemented by

- [`BlockNumberRepository`](../classes/BlockNumberRepository.md)
- [`CoingeckoHistoricalPriceRepository`](../classes/CoingeckoHistoricalPriceRepository.md)
- [`CoingeckoPriceRepository`](../classes/CoingeckoPriceRepository.md)
- [`FeeCollectorRepository`](../classes/FeeCollectorRepository.md)
- [`HistoricalPriceProvider`](../classes/HistoricalPriceProvider.md)
- [`LiquidityGaugeSubgraphRPCProvider`](../classes/LiquidityGaugeSubgraphRPCProvider.md)
- [`LiquidityGaugesSubgraphRepository`](../classes/LiquidityGaugesSubgraphRepository.md)
- [`Pools`](../classes/Pools.md)
- [`PoolsBalancerAPIRepository`](../classes/PoolsBalancerAPIRepository.md)
- [`PoolsFallbackRepository`](../classes/PoolsFallbackRepository.md)
- [`PoolsStaticRepository`](../classes/PoolsStaticRepository.md)
- [`PoolsSubgraphOnChainRepository`](../classes/PoolsSubgraphOnChainRepository.md)
- [`PoolsSubgraphRepository`](../classes/PoolsSubgraphRepository.md)
- [`StaticTokenPriceProvider`](../classes/StaticTokenPriceProvider.md)
- [`StaticTokenProvider`](../classes/StaticTokenProvider.md)
- [`SubgraphPriceRepository`](../classes/SubgraphPriceRepository.md)
- [`TokenPriceProvider`](../classes/TokenPriceProvider.md)
- [`TokenYieldsRepository`](../classes/TokenYieldsRepository.md)

## Table of contents

### Properties

- [find](Findable.md#find)
- [findBy](Findable.md#findby)

## Properties

### find

• **find**: (`id`: `string`) => `Promise`<`undefined` \| `T`\>

#### Type declaration

▸ (`id`): `Promise`<`undefined` \| `T`\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |

##### Returns

`Promise`<`undefined` \| `T`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/types.ts:13](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/types.ts#L13)

___

### findBy

• **findBy**: (`attribute`: `P`, `value`: `V`) => `Promise`<`undefined` \| `T`\>

#### Type declaration

▸ (`attribute`, `value`): `Promise`<`undefined` \| `T`\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `attribute` | `P` |
| `value` | `V` |

##### Returns

`Promise`<`undefined` \| `T`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/types.ts:14](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/types.ts#L14)
