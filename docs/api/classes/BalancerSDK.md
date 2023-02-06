# Class: BalancerSDK

Balancer SDK

**`Param`**

SDK configuration

## Implements

- [`BalancerSDKRoot`](../interfaces/BalancerSDKRoot.md)

## Table of contents

### Constructors

- [constructor](BalancerSDK.md#constructor)

### Properties

- [balancerContracts](BalancerSDK.md#balancercontracts)
- [config](BalancerSDK.md#config)
- [data](BalancerSDK.md#data)
- [networkConfig](BalancerSDK.md#networkconfig)
- [pools](BalancerSDK.md#pools)
- [pricing](BalancerSDK.md#pricing)
- [provider](BalancerSDK.md#provider)
- [relayer](BalancerSDK.md#relayer)
- [sor](BalancerSDK.md#sor)
- [subgraph](BalancerSDK.md#subgraph)
- [swaps](BalancerSDK.md#swaps)
- [zaps](BalancerSDK.md#zaps)

### Accessors

- [contracts](BalancerSDK.md#contracts)
- [rpcProvider](BalancerSDK.md#rpcprovider)

## Constructors

### constructor

• **new BalancerSDK**(`config`, `sor?`, `subgraph?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `config` | [`BalancerSdkConfig`](../interfaces/BalancerSdkConfig.md) |
| `sor` | [`Sor`](Sor-1.md) |
| `subgraph` | [`Subgraph`](Subgraph.md) |

#### Defined in

[balancer-sdk/balancer-js/src/modules/sdk.module.ts:44](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sdk.module.ts#L44)

## Properties

### balancerContracts

• **balancerContracts**: `Contracts`

#### Defined in

[balancer-sdk/balancer-js/src/modules/sdk.module.ts:39](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sdk.module.ts#L39)

___

### config

• **config**: [`BalancerSdkConfig`](../interfaces/BalancerSdkConfig.md)

#### Implementation of

[BalancerSDKRoot](../interfaces/BalancerSDKRoot.md).[config](../interfaces/BalancerSDKRoot.md#config)

#### Defined in

[balancer-sdk/balancer-js/src/modules/sdk.module.ts:45](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sdk.module.ts#L45)

___

### data

• `Readonly` **data**: [`Data`](Data.md)

#### Implementation of

[BalancerSDKRoot](../interfaces/BalancerSDKRoot.md).[data](../interfaces/BalancerSDKRoot.md#data)

#### Defined in

[balancer-sdk/balancer-js/src/modules/sdk.module.ts:38](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sdk.module.ts#L38)

___

### networkConfig

• `Readonly` **networkConfig**: [`BalancerNetworkConfig`](../interfaces/BalancerNetworkConfig.md)

#### Implementation of

[BalancerSDKRoot](../interfaces/BalancerSDKRoot.md).[networkConfig](../interfaces/BalancerSDKRoot.md#networkconfig)

#### Defined in

[balancer-sdk/balancer-js/src/modules/sdk.module.ts:41](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sdk.module.ts#L41)

___

### pools

• `Readonly` **pools**: [`Pools`](Pools.md)

#### Implementation of

[BalancerSDKRoot](../interfaces/BalancerSDKRoot.md).[pools](../interfaces/BalancerSDKRoot.md#pools)

#### Defined in

[balancer-sdk/balancer-js/src/modules/sdk.module.ts:37](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sdk.module.ts#L37)

___

### pricing

• `Readonly` **pricing**: `Pricing`

#### Defined in

[balancer-sdk/balancer-js/src/modules/sdk.module.ts:36](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sdk.module.ts#L36)

___

### provider

• `Readonly` **provider**: `Provider`

#### Defined in

[balancer-sdk/balancer-js/src/modules/sdk.module.ts:42](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sdk.module.ts#L42)

___

### relayer

• `Readonly` **relayer**: [`Relayer`](Relayer.md)

#### Implementation of

[BalancerSDKRoot](../interfaces/BalancerSDKRoot.md).[relayer](../interfaces/BalancerSDKRoot.md#relayer)

#### Defined in

[balancer-sdk/balancer-js/src/modules/sdk.module.ts:35](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sdk.module.ts#L35)

___

### sor

• **sor**: [`Sor`](Sor-1.md)

#### Implementation of

[BalancerSDKRoot](../interfaces/BalancerSDKRoot.md).[sor](../interfaces/BalancerSDKRoot.md#sor)

#### Defined in

[balancer-sdk/balancer-js/src/modules/sdk.module.ts:46](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sdk.module.ts#L46)

___

### subgraph

• **subgraph**: [`Subgraph`](Subgraph.md)

#### Implementation of

[BalancerSDKRoot](../interfaces/BalancerSDKRoot.md).[subgraph](../interfaces/BalancerSDKRoot.md#subgraph)

#### Defined in

[balancer-sdk/balancer-js/src/modules/sdk.module.ts:47](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sdk.module.ts#L47)

___

### swaps

• `Readonly` **swaps**: [`Swaps`](Swaps.md)

#### Implementation of

[BalancerSDKRoot](../interfaces/BalancerSDKRoot.md).[swaps](../interfaces/BalancerSDKRoot.md#swaps)

#### Defined in

[balancer-sdk/balancer-js/src/modules/sdk.module.ts:34](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sdk.module.ts#L34)

___

### zaps

• **zaps**: `Zaps`

#### Defined in

[balancer-sdk/balancer-js/src/modules/sdk.module.ts:40](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sdk.module.ts#L40)

## Accessors

### contracts

• `get` **contracts**(): `ContractInstances`

Expose balancer contracts, e.g. Vault, LidoRelayer.

#### Returns

`ContractInstances`

#### Defined in

[balancer-sdk/balancer-js/src/modules/sdk.module.ts:76](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sdk.module.ts#L76)

___

### rpcProvider

• `get` **rpcProvider**(): `Provider`

#### Returns

`Provider`

#### Implementation of

[BalancerSDKRoot](../interfaces/BalancerSDKRoot.md).[rpcProvider](../interfaces/BalancerSDKRoot.md#rpcprovider)

#### Defined in

[balancer-sdk/balancer-js/src/modules/sdk.module.ts:69](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sdk.module.ts#L69)
