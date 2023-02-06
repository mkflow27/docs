# Interface: BalancerDataRepositories

## Implemented by

- [`Data`](../classes/Data.md)

## Table of contents

### Properties

- [feeCollector](BalancerDataRepositories.md#feecollector)
- [feeDistributor](BalancerDataRepositories.md#feedistributor)
- [gaugeShares](BalancerDataRepositories.md#gaugeshares)
- [liquidityGauges](BalancerDataRepositories.md#liquiditygauges)
- [poolGauges](BalancerDataRepositories.md#poolgauges)
- [poolJoinExits](BalancerDataRepositories.md#pooljoinexits)
- [poolShares](BalancerDataRepositories.md#poolshares)
- [pools](BalancerDataRepositories.md#pools)
- [poolsOnChain](BalancerDataRepositories.md#poolsonchain)
- [protocolFees](BalancerDataRepositories.md#protocolfees)
- [tokenHistoricalPrices](BalancerDataRepositories.md#tokenhistoricalprices)
- [tokenMeta](BalancerDataRepositories.md#tokenmeta)
- [tokenPrices](BalancerDataRepositories.md#tokenprices)
- [tokenYields](BalancerDataRepositories.md#tokenyields)
- [yesterdaysPools](BalancerDataRepositories.md#yesterdayspools)

## Properties

### feeCollector

• **feeCollector**: [`Findable`](Findable.md)<`number`, `string`, `any`\>

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:116](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L116)

___

### feeDistributor

• `Optional` **feeDistributor**: [`BaseFeeDistributor`](BaseFeeDistributor.md)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:115](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L115)

___

### gaugeShares

• `Optional` **gaugeShares**: [`GaugeSharesRepository`](../classes/GaugeSharesRepository.md)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:122](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L122)

___

### liquidityGauges

• `Optional` **liquidityGauges**: [`Findable`](Findable.md)<[`LiquidityGauge`](LiquidityGauge.md), `string`, `any`\>

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:114](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L114)

___

### poolGauges

• `Optional` **poolGauges**: [`PoolGaugesRepository`](../classes/PoolGaugesRepository.md)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:120](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L120)

___

### poolJoinExits

• **poolJoinExits**: [`PoolJoinExitRepository`](../classes/PoolJoinExitRepository.md)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:121](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L121)

___

### poolShares

• **poolShares**: [`PoolSharesRepository`](../classes/PoolSharesRepository.md)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:119](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L119)

___

### pools

• **pools**: [`Findable`](Findable.md)<[`Pool`](Pool.md), [`PoolAttribute`](../modules.md#poolattribute), `any`\> & [`Searchable`](Searchable.md)<[`Pool`](Pool.md)\>

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:108](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L108)

___

### poolsOnChain

• **poolsOnChain**: [`Findable`](Findable.md)<[`Pool`](Pool.md), [`PoolAttribute`](../modules.md#poolattribute), `any`\> & [`Searchable`](Searchable.md)<[`Pool`](Pool.md)\>

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:109](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L109)

___

### protocolFees

• `Optional` **protocolFees**: [`ProtocolFeesProvider`](../classes/ProtocolFeesProvider.md)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:117](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L117)

___

### tokenHistoricalPrices

• **tokenHistoricalPrices**: [`Findable`](Findable.md)<[`Price`](../modules.md#price), `string`, `any`\>

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:112](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L112)

___

### tokenMeta

• **tokenMeta**: [`Findable`](Findable.md)<[`Token`](Token.md), [`TokenAttribute`](../modules.md#tokenattribute), `any`\>

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:113](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L113)

___

### tokenPrices

• **tokenPrices**: [`Findable`](Findable.md)<[`Price`](../modules.md#price), `string`, `any`\>

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:111](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L111)

___

### tokenYields

• **tokenYields**: [`Findable`](Findable.md)<`number`, `string`, `any`\>

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:118](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L118)

___

### yesterdaysPools

• `Optional` **yesterdaysPools**: [`Findable`](Findable.md)<[`Pool`](Pool.md), [`PoolAttribute`](../modules.md#poolattribute), `any`\> & [`Searchable`](Searchable.md)<[`Pool`](Pool.md)\>

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:110](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L110)
