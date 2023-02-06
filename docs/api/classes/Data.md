# Class: Data

## Implements

- [`BalancerDataRepositories`](../interfaces/BalancerDataRepositories.md)

## Table of contents

### Constructors

- [constructor](Data.md#constructor)

### Properties

- [blockNumbers](Data.md#blocknumbers)
- [feeCollector](Data.md#feecollector)
- [feeDistributor](Data.md#feedistributor)
- [gaugeShares](Data.md#gaugeshares)
- [liquidityGauges](Data.md#liquiditygauges)
- [poolGauges](Data.md#poolgauges)
- [poolJoinExits](Data.md#pooljoinexits)
- [poolShares](Data.md#poolshares)
- [pools](Data.md#pools)
- [poolsOnChain](Data.md#poolsonchain)
- [protocolFees](Data.md#protocolfees)
- [tokenHistoricalPrices](Data.md#tokenhistoricalprices)
- [tokenMeta](Data.md#tokenmeta)
- [tokenPrices](Data.md#tokenprices)
- [tokenYields](Data.md#tokenyields)
- [yesterdaysPools](Data.md#yesterdayspools)

## Constructors

### constructor

• **new Data**(`networkConfig`, `provider`, `subgraphQuery?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `networkConfig` | [`BalancerNetworkConfig`](../interfaces/BalancerNetworkConfig.md) |
| `provider` | `Provider` |
| `subgraphQuery?` | [`GraphQLQuery`](../interfaces/GraphQLQuery.md) |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/index.ts:67](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/index.ts#L67)

## Properties

### blockNumbers

• **blockNumbers**: `undefined` \| [`BlockNumberRepository`](BlockNumberRepository.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/index.ts:64](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/index.ts#L64)

___

### feeCollector

• **feeCollector**: [`FeeCollectorRepository`](FeeCollectorRepository.md)

#### Implementation of

[BalancerDataRepositories](../interfaces/BalancerDataRepositories.md).[feeCollector](../interfaces/BalancerDataRepositories.md#feecollector)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/index.ts:61](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/index.ts#L61)

___

### feeDistributor

• **feeDistributor**: `undefined` \| [`FeeDistributorRepository`](FeeDistributorRepository.md)

#### Implementation of

[BalancerDataRepositories](../interfaces/BalancerDataRepositories.md).[feeDistributor](../interfaces/BalancerDataRepositories.md#feedistributor)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/index.ts:60](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/index.ts#L60)

___

### gaugeShares

• **gaugeShares**: `undefined` \| [`GaugeSharesRepository`](GaugeSharesRepository.md)

#### Implementation of

[BalancerDataRepositories](../interfaces/BalancerDataRepositories.md).[gaugeShares](../interfaces/BalancerDataRepositories.md#gaugeshares)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/index.ts:55](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/index.ts#L55)

___

### liquidityGauges

• **liquidityGauges**: `undefined` \| [`LiquidityGaugeSubgraphRPCProvider`](LiquidityGaugeSubgraphRPCProvider.md)

#### Implementation of

[BalancerDataRepositories](../interfaces/BalancerDataRepositories.md).[liquidityGauges](../interfaces/BalancerDataRepositories.md#liquiditygauges)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/index.ts:59](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/index.ts#L59)

___

### poolGauges

• **poolGauges**: `undefined` \| [`PoolGaugesRepository`](PoolGaugesRepository.md)

#### Implementation of

[BalancerDataRepositories](../interfaces/BalancerDataRepositories.md).[poolGauges](../interfaces/BalancerDataRepositories.md#poolgauges)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/index.ts:54](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/index.ts#L54)

___

### poolJoinExits

• **poolJoinExits**: [`PoolJoinExitRepository`](PoolJoinExitRepository.md)

#### Implementation of

[BalancerDataRepositories](../interfaces/BalancerDataRepositories.md).[poolJoinExits](../interfaces/BalancerDataRepositories.md#pooljoinexits)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/index.ts:65](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/index.ts#L65)

___

### poolShares

• **poolShares**: [`PoolSharesRepository`](PoolSharesRepository.md)

#### Implementation of

[BalancerDataRepositories](../interfaces/BalancerDataRepositories.md).[poolShares](../interfaces/BalancerDataRepositories.md#poolshares)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/index.ts:53](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/index.ts#L53)

___

### pools

• **pools**: [`PoolsSubgraphRepository`](PoolsSubgraphRepository.md)

#### Implementation of

[BalancerDataRepositories](../interfaces/BalancerDataRepositories.md).[pools](../interfaces/BalancerDataRepositories.md#pools)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/index.ts:50](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/index.ts#L50)

___

### poolsOnChain

• **poolsOnChain**: [`PoolsSubgraphOnChainRepository`](PoolsSubgraphOnChainRepository.md)

#### Implementation of

[BalancerDataRepositories](../interfaces/BalancerDataRepositories.md).[poolsOnChain](../interfaces/BalancerDataRepositories.md#poolsonchain)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/index.ts:51](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/index.ts#L51)

___

### protocolFees

• **protocolFees**: `undefined` \| [`ProtocolFeesProvider`](ProtocolFeesProvider.md)

#### Implementation of

[BalancerDataRepositories](../interfaces/BalancerDataRepositories.md).[protocolFees](../interfaces/BalancerDataRepositories.md#protocolfees)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/index.ts:62](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/index.ts#L62)

___

### tokenHistoricalPrices

• **tokenHistoricalPrices**: [`HistoricalPriceProvider`](HistoricalPriceProvider.md)

#### Implementation of

[BalancerDataRepositories](../interfaces/BalancerDataRepositories.md).[tokenHistoricalPrices](../interfaces/BalancerDataRepositories.md#tokenhistoricalprices)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/index.ts:57](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/index.ts#L57)

___

### tokenMeta

• **tokenMeta**: [`StaticTokenProvider`](StaticTokenProvider.md)

#### Implementation of

[BalancerDataRepositories](../interfaces/BalancerDataRepositories.md).[tokenMeta](../interfaces/BalancerDataRepositories.md#tokenmeta)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/index.ts:58](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/index.ts#L58)

___

### tokenPrices

• **tokenPrices**: [`TokenPriceProvider`](TokenPriceProvider.md)

#### Implementation of

[BalancerDataRepositories](../interfaces/BalancerDataRepositories.md).[tokenPrices](../interfaces/BalancerDataRepositories.md#tokenprices)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/index.ts:56](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/index.ts#L56)

___

### tokenYields

• **tokenYields**: [`TokenYieldsRepository`](TokenYieldsRepository.md)

#### Implementation of

[BalancerDataRepositories](../interfaces/BalancerDataRepositories.md).[tokenYields](../interfaces/BalancerDataRepositories.md#tokenyields)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/index.ts:63](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/index.ts#L63)

___

### yesterdaysPools

• **yesterdaysPools**: `undefined` \| [`PoolsSubgraphRepository`](PoolsSubgraphRepository.md)

#### Implementation of

[BalancerDataRepositories](../interfaces/BalancerDataRepositories.md).[yesterdaysPools](../interfaces/BalancerDataRepositories.md#yesterdayspools)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/index.ts:52](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/index.ts#L52)
