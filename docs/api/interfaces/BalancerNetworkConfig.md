# Interface: BalancerNetworkConfig

## Table of contents

### Properties

- [addresses](BalancerNetworkConfig.md#addresses)
- [chainId](BalancerNetworkConfig.md#chainid)
- [pools](BalancerNetworkConfig.md#pools)
- [poolsToIgnore](BalancerNetworkConfig.md#poolstoignore)
- [sorConnectingTokens](BalancerNetworkConfig.md#sorconnectingtokens)
- [tenderly](BalancerNetworkConfig.md#tenderly)
- [urls](BalancerNetworkConfig.md#urls)

## Properties

### addresses

• **addresses**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `contracts` | [`ContractAddresses`](ContractAddresses.md) |
| `tokens` | { `bal?`: `string` ; `bbaUsd?`: `string` ; `lbpRaisingTokens?`: `string`[] ; `stETH?`: `string` ; `veBal?`: `string` ; `wrappedNativeAsset`: `string` ; `wstETH?`: `string`  } |
| `tokens.bal?` | `string` |
| `tokens.bbaUsd?` | `string` |
| `tokens.lbpRaisingTokens?` | `string`[] |
| `tokens.stETH?` | `string` |
| `tokens.veBal?` | `string` |
| `tokens.wrappedNativeAsset` | `string` |
| `tokens.wstETH?` | `string` |

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:82](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L82)

___

### chainId

• **chainId**: [`Network`](../enums/Network.md)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:81](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L81)

___

### pools

• **pools**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `wETHwstETH?` | [`PoolReference`](../modules.md#poolreference) |

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:100](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L100)

___

### poolsToIgnore

• `Optional` **poolsToIgnore**: `string`[]

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:103](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L103)

___

### sorConnectingTokens

• `Optional` **sorConnectingTokens**: { `address`: `string` ; `symbol`: `string`  }[]

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:104](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L104)

___

### tenderly

• `Optional` **tenderly**: [`BalancerTenderlyConfig`](BalancerTenderlyConfig.md)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:94](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L94)

___

### urls

• **urls**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `blockNumberSubgraph?` | `string` |
| `gaugesSubgraph?` | `string` |
| `subgraph` | `string` |

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:95](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L95)
