# Class: LiquidityGaugesMulticallRepository

A lot of code to get liquidity gauge state via RPC multicall.
TODO: reseach helper contracts or extend subgraph

## Table of contents

### Constructors

- [constructor](LiquidityGaugesMulticallRepository.md#constructor)

### Properties

- [chainId](LiquidityGaugesMulticallRepository.md#chainid)
- [multicall](LiquidityGaugesMulticallRepository.md#multicall)

### Methods

- [getRewardCounts](LiquidityGaugesMulticallRepository.md#getrewardcounts)
- [getRewardData](LiquidityGaugesMulticallRepository.md#getrewarddata)
- [getRewardTokens](LiquidityGaugesMulticallRepository.md#getrewardtokens)
- [getTotalSupplies](LiquidityGaugesMulticallRepository.md#gettotalsupplies)
- [getWorkingSupplies](LiquidityGaugesMulticallRepository.md#getworkingsupplies)

## Constructors

### constructor

• **new LiquidityGaugesMulticallRepository**(`multicallAddress`, `chainId`, `provider`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `multicallAddress` | `string` |
| `chainId` | [`Network`](../enums/Network.md) |
| `provider` | `Provider` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/multicall.ts:34](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/multicall.ts#L34)

## Properties

### chainId

• `Private` **chainId**: [`Network`](../enums/Network.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/multicall.ts:36](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/multicall.ts#L36)

___

### multicall

• **multicall**: `Contract`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/multicall.ts:32](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/multicall.ts#L32)

## Methods

### getRewardCounts

▸ **getRewardCounts**(`gaugeAddresses`): `Promise`<{ `[gaugeAddress: string]`: `number`;  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `gaugeAddresses` | `string`[] |

#### Returns

`Promise`<{ `[gaugeAddress: string]`: `number`;  }\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/multicall.ts:86](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/multicall.ts#L86)

___

### getRewardData

▸ **getRewardData**(`gaugeAddresses`, `passingRewardTokens?`): `Promise`<{ `[gaugeAddress: string]`: { `[rewardTokenAddress: string]`: [`RewardData`](../interfaces/RewardData.md);  };  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `gaugeAddresses` | `string`[] |
| `passingRewardTokens?` | `Object` |

#### Returns

`Promise`<{ `[gaugeAddress: string]`: { `[rewardTokenAddress: string]`: [`RewardData`](../interfaces/RewardData.md);  };  }\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/multicall.ts:167](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/multicall.ts#L167)

___

### getRewardTokens

▸ **getRewardTokens**(`gaugeAddresses`, `passingRewardCounts?`): `Promise`<{ `[gaugeAddress: string]`: `string`[];  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `gaugeAddresses` | `string`[] |
| `passingRewardCounts?` | `Object` |

#### Returns

`Promise`<{ `[gaugeAddress: string]`: `string`[];  }\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/multicall.ts:119](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/multicall.ts#L119)

___

### getTotalSupplies

▸ **getTotalSupplies**(`gaugeAddresses`): `Promise`<{ `[gaugeAddress: string]`: `number`;  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `gaugeAddresses` | `string`[] |

#### Returns

`Promise`<{ `[gaugeAddress: string]`: `number`;  }\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/multicall.ts:42](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/multicall.ts#L42)

___

### getWorkingSupplies

▸ **getWorkingSupplies**(`gaugeAddresses`): `Promise`<{ `[gaugeAddress: string]`: `number`;  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `gaugeAddresses` | `string`[] |

#### Returns

`Promise`<{ `[gaugeAddress: string]`: `number`;  }\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/liquidity-gauges/multicall.ts:64](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/liquidity-gauges/multicall.ts#L64)
