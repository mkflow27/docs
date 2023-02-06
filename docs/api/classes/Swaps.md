# Class: Swaps

## Table of contents

### Constructors

- [constructor](Swaps.md#constructor)

### Properties

- [chainId](Swaps.md#chainid)
- [sor](Swaps.md#sor)
- [vaultContract](Swaps.md#vaultcontract)

### Methods

- [buildSwap](Swaps.md#buildswap)
- [fetchPools](Swaps.md#fetchpools)
- [findRouteGivenIn](Swaps.md#findroutegivenin)
- [findRouteGivenOut](Swaps.md#findroutegivenout)
- [getPools](Swaps.md#getpools)
- [getSorSwap](Swaps.md#getsorswap)
- [queryBatchSwap](Swaps.md#querybatchswap)
- [queryBatchSwapWithSor](Swaps.md#querybatchswapwithsor)
- [querySimpleFlashSwap](Swaps.md#querysimpleflashswap)
- [encodeBatchSwap](Swaps.md#encodebatchswap)
- [encodeSimpleFlashSwap](Swaps.md#encodesimpleflashswap)
- [getLimitsForSlippage](Swaps.md#getlimitsforslippage)

## Constructors

### constructor

• **new Swaps**(`sorOrConfig`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `sorOrConfig` | [`BalancerSdkConfig`](../interfaces/BalancerSdkConfig.md) \| [`SOR`](SOR.md) |

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/swaps.module.ts:40](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/swaps.module.ts#L40)

## Properties

### chainId

• **chainId**: `number`

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/swaps.module.ts:36](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/swaps.module.ts#L36)

___

### sor

• `Readonly` **sor**: [`SOR`](SOR.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/swaps.module.ts:35](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/swaps.module.ts#L35)

___

### vaultContract

• **vaultContract**: `Vault`

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/swaps.module.ts:37](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/swaps.module.ts#L37)

## Methods

### buildSwap

▸ **buildSwap**(`BuildTransactionParameters`): [`SwapAttributes`](../interfaces/SwapAttributes.md)

Uses SOR to find optimal route for a trading pair and amount

#### Parameters

| Name | Type |
| :------ | :------ |
| `BuildTransactionParameters` | [`BuildTransactionParameters`](../interfaces/BuildTransactionParameters.md) |

#### Returns

[`SwapAttributes`](../interfaces/SwapAttributes.md)

transaction request ready to send with signer.sendTransaction

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/swaps.module.ts:142](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/swaps.module.ts#L142)

___

### fetchPools

▸ **fetchPools**(): `Promise`<`boolean`\>

fetchPools saves updated pools data to SOR internal onChainBalanceCache.

#### Returns

`Promise`<`boolean`\>

Boolean indicating whether pools data was fetched correctly (true) or not (false).

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/swaps.module.ts:229](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/swaps.module.ts#L229)

___

### findRouteGivenIn

▸ **findRouteGivenIn**(`FindRouteParameters`): `Promise`<[`SwapInfo`](../interfaces/SwapInfo.md)\>

Uses SOR to find optimal route for a trading pair and amount

#### Parameters

| Name | Type |
| :------ | :------ |
| `FindRouteParameters` | [`FindRouteParameters`](../interfaces/FindRouteParameters.md) |

#### Returns

`Promise`<[`SwapInfo`](../interfaces/SwapInfo.md)\>

Best trade route information

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/swaps.module.ts:88](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/swaps.module.ts#L88)

___

### findRouteGivenOut

▸ **findRouteGivenOut**(`FindRouteParameters`): `Promise`<[`SwapInfo`](../interfaces/SwapInfo.md)\>

Uses SOR to find optimal route for a trading pair and amount

#### Parameters

| Name | Type |
| :------ | :------ |
| `FindRouteParameters` | [`FindRouteParameters`](../interfaces/FindRouteParameters.md) |

#### Returns

`Promise`<[`SwapInfo`](../interfaces/SwapInfo.md)\>

Best trade route information

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/swaps.module.ts:112](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/swaps.module.ts#L112)

___

### getPools

▸ **getPools**(): [`SubgraphPoolBase`](../interfaces/SubgraphPoolBase.md)[]

#### Returns

[`SubgraphPoolBase`](../interfaces/SubgraphPoolBase.md)[]

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/swaps.module.ts:233](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/swaps.module.ts#L233)

___

### getSorSwap

▸ **getSorSwap**(`swapInput`): `Promise`<[`SwapInfo`](../interfaces/SwapInfo.md)\>

Use SOR to get swapInfo for tokenIn<>tokenOut.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `swapInput` | [`SwapInput`](../interfaces/SwapInput.md) | Swap information used for querying using SOR. |

#### Returns

`Promise`<[`SwapInfo`](../interfaces/SwapInfo.md)\>

SOR swap info.

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/swaps.module.ts:313](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/swaps.module.ts#L313)

___

### queryBatchSwap

▸ **queryBatchSwap**(`batchSwap`): `Promise`<`string`[]\>

queryBatchSwap simulates a call to `batchSwap`, returning an array of Vault asset deltas.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `batchSwap` | `Pick`<[`BatchSwap`](../modules.md#batchswap), ``"kind"`` \| ``"assets"`` \| ``"swaps"``\> | BatchSwap information used for query. |

#### Returns

`Promise`<`string`[]\>

Returns an array with the net Vault asset balance deltas. Positive amounts represent tokens (or ETH) sent to the
Vault, and negative amounts represent tokens (or ETH) sent by the Vault. Each delta corresponds to the asset at
the same index in the `assets` array.

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/swaps.module.ts:247](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/swaps.module.ts#L247)

___

### queryBatchSwapWithSor

▸ **queryBatchSwapWithSor**(`queryWithSor`): `Promise`<[`QueryWithSorOutput`](../interfaces/QueryWithSorOutput.md)\>

Uses SOR to create and query a batchSwap.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `queryWithSor` | [`QueryWithSorInput`](../interfaces/QueryWithSorInput.md) | Swap information used for querying using SOR. |

#### Returns

`Promise`<[`QueryWithSorOutput`](../interfaces/QueryWithSorOutput.md)\>

Returns amount of tokens swaps along with swap and asset info that can be submitted to a batchSwap call.

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/swaps.module.ts:268](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/swaps.module.ts#L268)

___

### querySimpleFlashSwap

▸ **querySimpleFlashSwap**(`params`): `Promise`<[`QuerySimpleFlashSwapResponse`](../interfaces/QuerySimpleFlashSwapResponse.md)\>

Simple interface to test if a simple flash swap is valid and see potential profits.

A "simple" flash swap is an arbitrage executed with only two tokens and two pools,
swapping in the first pool and then back in the second pool for a profit. For more
complex flash swaps, you will have to use the batch swap method.

Learn more: A [Flash Swap](https://dev.balancer.fi/resources/swaps/flash-swaps).

_NB: This method doesn't execute a flashSwap

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `params` | `Omit`<[`QuerySimpleFlashSwapParameters`](../interfaces/QuerySimpleFlashSwapParameters.md), ``"vaultContract"``\> | BatchSwap information used for query. |

#### Returns

`Promise`<[`QuerySimpleFlashSwapResponse`](../interfaces/QuerySimpleFlashSwapResponse.md)\>

Returns an ethersjs transaction response

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/swaps.module.ts:295](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/swaps.module.ts#L295)

___

### encodeBatchSwap

▸ `Static` **encodeBatchSwap**(`batchSwap`): `string`

Encode batchSwap in an ABI byte string

[See method for a batchSwap](https://dev.balancer.fi/references/contracts/apis/the-vault#batch-swaps).

_NB: This method doesn't execute a batchSwap -- it returns an [ABI byte string](https://docs.soliditylang.org/en/latest/abi-spec.html)
containing the data of the function call on a contract, which can then be sent to the network to be executed.
(ex. [sendTransaction](https://web3js.readthedocs.io/en/v1.2.11/web3-eth.html#sendtransaction)).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `batchSwap` | [`BatchSwap`](../modules.md#batchswap) | BatchSwap information used for query. |

#### Returns

`string`

encodedBatchSwapData - Returns an ABI byte string containing the data of the function call on a contract

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/swaps.module.ts:188](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/swaps.module.ts#L188)

___

### encodeSimpleFlashSwap

▸ `Static` **encodeSimpleFlashSwap**(`params`): `string`

Encode simple flash swap into a ABI byte string

A "simple" flash swap is an arbitrage executed with only two tokens and two pools,
swapping in the first pool and then back in the second pool for a profit. For more
complex flash swaps, you will have to use the batch swap method.

Learn more: A [Flash Swap](https://dev.balancer.fi/resources/swaps/flash-swaps).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `params` | [`SimpleFlashSwapParameters`](../interfaces/SimpleFlashSwapParameters.md) | BatchSwap information used for query. |

#### Returns

`string`

encodedBatchSwapData - Returns an ABI byte string containing the data of the function call on a contract

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/swaps.module.ts:217](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/swaps.module.ts#L217)

___

### getLimitsForSlippage

▸ `Static` **getLimitsForSlippage**(`tokensIn`, `tokensOut`, `swapType`, `deltas`, `assets`, `slippage`): `string`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `tokensIn` | `string`[] |
| `tokensOut` | `string`[] |
| `swapType` | [`SwapType`](../enums/SwapType.md) |
| `deltas` | `string`[] |
| `assets` | `string`[] |
| `slippage` | `string` |

#### Returns

`string`[]

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/swaps.module.ts:56](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/swaps.module.ts#L56)
