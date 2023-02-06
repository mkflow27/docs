# Class: Relayer

## Table of contents

### Constructors

- [constructor](Relayer.md#constructor)

### Properties

- [swaps](Relayer.md#swaps)
- [CHAINED\_REFERENCE\_READONLY\_PREFIX](Relayer.md#chained-reference-readonly-prefix)
- [CHAINED\_REFERENCE\_TEMP\_PREFIX](Relayer.md#chained-reference-temp-prefix)

### Methods

- [encodeSwapUnwrap](Relayer.md#encodeswapunwrap)
- [exitPoolAndBatchSwap](Relayer.md#exitpoolandbatchswap)
- [fetchPools](Relayer.md#fetchpools)
- [getPools](Relayer.md#getpools)
- [swapUnwrapAaveStaticExactIn](Relayer.md#swapunwrapaavestaticexactin)
- [swapUnwrapAaveStaticExactOut](Relayer.md#swapunwrapaavestaticexactout)
- [constructExitCall](Relayer.md#constructexitcall)
- [constructJoinCall](Relayer.md#constructjoincall)
- [encodeApproveVault](Relayer.md#encodeapprovevault)
- [encodeBatchSwap](Relayer.md#encodebatchswap)
- [encodeExitPool](Relayer.md#encodeexitpool)
- [encodeGaugeDeposit](Relayer.md#encodegaugedeposit)
- [encodeGaugeWithdraw](Relayer.md#encodegaugewithdraw)
- [encodeJoinPool](Relayer.md#encodejoinpool)
- [encodePeekChainedReferenceValue](Relayer.md#encodepeekchainedreferencevalue)
- [encodeSetRelayerApproval](Relayer.md#encodesetrelayerapproval)
- [encodeUnwrapAaveStaticToken](Relayer.md#encodeunwrapaavestatictoken)
- [encodeWrapAaveDynamicToken](Relayer.md#encodewrapaavedynamictoken)
- [fromChainedReference](Relayer.md#fromchainedreference)
- [isChainedReference](Relayer.md#ischainedreference)
- [signRelayerApproval](Relayer.md#signrelayerapproval)
- [toChainedReference](Relayer.md#tochainedreference)

## Constructors

### constructor

• **new Relayer**(`swapsOrConfig`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapsOrConfig` | [`BalancerSdkConfig`](../interfaces/BalancerSdkConfig.md) \| [`Swaps`](Swaps.md) |

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:47](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L47)

## Properties

### swaps

• `Private` `Readonly` **swaps**: [`Swaps`](Swaps.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:42](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L42)

___

### CHAINED\_REFERENCE\_READONLY\_PREFIX

▪ `Static` **CHAINED\_REFERENCE\_READONLY\_PREFIX**: `string` = `'ba11'`

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:45](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L45)

___

### CHAINED\_REFERENCE\_TEMP\_PREFIX

▪ `Static` **CHAINED\_REFERENCE\_TEMP\_PREFIX**: `string` = `'ba10'`

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:44](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L44)

## Methods

### encodeSwapUnwrap

▸ **encodeSwapUnwrap**(`wrappedTokens`, `swapType`, `swaps`, `assets`, `funds`, `limits`): `string`[]

Creates encoded multicalls using swap outputs as input amounts for token unwrap.

#### Parameters

| Name | Type |
| :------ | :------ |
| `wrappedTokens` | `string`[] |
| `swapType` | [`SwapType`](../enums/SwapType.md) |
| `swaps` | [`BatchSwapStep`](../modules.md#batchswapstep)[] |
| `assets` | `string`[] |
| `funds` | [`FundManagement`](../modules.md#fundmanagement) |
| `limits` | `BigNumberish`[] |

#### Returns

`string`[]

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:580](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L580)

___

### exitPoolAndBatchSwap

▸ **exitPoolAndBatchSwap**(`params`): `Promise`<[`TransactionData`](../interfaces/TransactionData.md)\>

exitPoolAndBatchSwap Chains poolExit with batchSwap to final tokens.

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | [`ExitAndBatchSwapInput`](../interfaces/ExitAndBatchSwapInput.md) |

#### Returns

`Promise`<[`TransactionData`](../interfaces/TransactionData.md)\>

Transaction data with calldata. Outputs.amountsOut has amounts of finalTokensOut returned.

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:298](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L298)

___

### fetchPools

▸ **fetchPools**(): `Promise`<`boolean`\>

fetchPools saves updated pools data to SOR internal onChainBalanceCache.

#### Returns

`Promise`<`boolean`\>

Boolean indicating whether pools data was fetched correctly (true) or not (false).

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:276](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L276)

___

### getPools

▸ **getPools**(): [`SubgraphPoolBase`](../interfaces/SubgraphPoolBase.md)[]

#### Returns

[`SubgraphPoolBase`](../interfaces/SubgraphPoolBase.md)[]

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:280](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L280)

___

### swapUnwrapAaveStaticExactIn

▸ **swapUnwrapAaveStaticExactIn**(`tokensIn`, `aaveStaticTokens`, `amountsIn`, `rates`, `funds`, `slippage`, `fetchPools?`): `Promise`<[`TransactionData`](../interfaces/TransactionData.md)\>

swapUnwrapAaveStaticExactIn Finds swaps for tokenIn>wrapped Aave static tokens and chains with unwrap to underlying stable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tokensIn` | `string`[] | array to token addresses for swapping as tokens in. |
| `aaveStaticTokens` | `string`[] | array contains the addresses of the Aave static tokens that tokenIn will be swapped to. These will be unwrapped. |
| `amountsIn` | `string`[] | amounts to be swapped for each token in. |
| `rates` | `string`[] | The rate used to convert wrappedToken to underlying. |
| `funds` | [`FundManagement`](../modules.md#fundmanagement) | Funding info for swap. Note - recipient should be relayer and sender should be caller. |
| `slippage` | `string` | Slippage to be applied to swap section. i.e. 5%=50000000000000000. |
| `fetchPools` | [`FetchPoolsInput`](../interfaces/FetchPoolsInput.md) | Set whether SOR will fetch updated pool info. |

#### Returns

`Promise`<[`TransactionData`](../interfaces/TransactionData.md)\>

Transaction data with calldata. Outputs.amountsOut has final amounts out of unwrapped tokens.

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:426](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L426)

___

### swapUnwrapAaveStaticExactOut

▸ **swapUnwrapAaveStaticExactOut**(`tokensIn`, `aaveStaticTokens`, `amountsUnwrapped`, `rates`, `funds`, `slippage`, `fetchPools?`): `Promise`<[`TransactionData`](../interfaces/TransactionData.md)\>

swapUnwrapAaveStaticExactOut Finds swaps for tokenIn>wrapped Aave static tokens and chains with unwrap to underlying stable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tokensIn` | `string`[] | array to token addresses for swapping as tokens in. |
| `aaveStaticTokens` | `string`[] | array contains the addresses of the Aave static tokens that tokenIn will be swapped to. These will be unwrapped. |
| `amountsUnwrapped` | `string`[] | amounts of unwrapped tokens out. |
| `rates` | `string`[] | The rate used to convert wrappedToken to underlying. |
| `funds` | [`FundManagement`](../modules.md#fundmanagement) | Funding info for swap. Note - recipient should be relayer and sender should be caller. |
| `slippage` | `string` | Slippage to be applied to swap section. i.e. 5%=50000000000000000. |
| `fetchPools` | [`FetchPoolsInput`](../interfaces/FetchPoolsInput.md) | Set whether SOR will fetch updated pool info. |

#### Returns

`Promise`<[`TransactionData`](../interfaces/TransactionData.md)\>

Transaction data with calldata. Outputs.amountsIn has the amounts of tokensIn.

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:505](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L505)

___

### constructExitCall

▸ `Static` **constructExitCall**(`params`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | [`ExitPoolData`](../modules.md#exitpooldata) |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:202](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L202)

___

### constructJoinCall

▸ `Static` **constructJoinCall**(`params`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | [`JoinPoolData`](../modules.md#joinpooldata) |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:235](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L235)

___

### encodeApproveVault

▸ `Static` **encodeApproveVault**(`tokenAddress`, `maxAmount`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `tokenAddress` | `string` |
| `maxAmount` | `string` |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:69](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L69)

___

### encodeBatchSwap

▸ `Static` **encodeBatchSwap**(`params`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | [`EncodeBatchSwapInput`](../interfaces/EncodeBatchSwapInput.md) |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:116](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L116)

___

### encodeExitPool

▸ `Static` **encodeExitPool**(`params`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | [`EncodeExitPoolInput`](../interfaces/EncodeExitPoolInput.md) |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:129](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L129)

___

### encodeGaugeDeposit

▸ `Static` **encodeGaugeDeposit**(`gaugeAddress`, `sender`, `recipient`, `amount`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `gaugeAddress` | `string` |
| `sender` | `string` |
| `recipient` | `string` |
| `amount` | `string` |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:102](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L102)

___

### encodeGaugeWithdraw

▸ `Static` **encodeGaugeWithdraw**(`gaugeAddress`, `sender`, `recipient`, `amount`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `gaugeAddress` | `string` |
| `sender` | `string` |
| `recipient` | `string` |
| `amount` | `string` |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:88](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L88)

___

### encodeJoinPool

▸ `Static` **encodeJoinPool**(`params`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | [`EncodeJoinPoolInput`](../interfaces/EncodeJoinPoolInput.md) |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:140](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L140)

___

### encodePeekChainedReferenceValue

▸ `Static` **encodePeekChainedReferenceValue**(`reference`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `reference` | `BigNumberish` |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:178](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L178)

___

### encodeSetRelayerApproval

▸ `Static` **encodeSetRelayerApproval**(`relayerAdress`, `approved`, `authorisation`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `relayerAdress` | `string` |
| `approved` | `boolean` |
| `authorisation` | `string` |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:76](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L76)

___

### encodeUnwrapAaveStaticToken

▸ `Static` **encodeUnwrapAaveStaticToken**(`params`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | [`EncodeUnwrapAaveStaticTokenInput`](../interfaces/EncodeUnwrapAaveStaticTokenInput.md) |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:165](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L165)

___

### encodeWrapAaveDynamicToken

▸ `Static` **encodeWrapAaveDynamicToken**(`params`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | [`EncodeWrapAaveDynamicTokenInput`](../interfaces/EncodeWrapAaveDynamicTokenInput.md) |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:152](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L152)

___

### fromChainedReference

▸ `Static` **fromChainedReference**(`ref`, `isTemporary?`): `BigNumber`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `ref` | `string` | `undefined` |
| `isTemporary` | `boolean` | `true` |

#### Returns

`BigNumber`

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:193](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L193)

___

### isChainedReference

▸ `Static` **isChainedReference**(`amount`): `boolean`

Returns true if `amount` is not actually an amount, but rather a chained reference.

#### Parameters

| Name | Type |
| :------ | :------ |
| `amount` | `string` |

#### Returns

`boolean`

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:58](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L58)

___

### signRelayerApproval

▸ `Static` **signRelayerApproval**(`relayerAddress`, `signerAddress`, `signer`, `vault`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `relayerAddress` | `string` |
| `signerAddress` | `string` |
| `signer` | `JsonRpcSigner` |
| `vault` | `Vault` |

#### Returns

`Promise`<`string`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:634](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L634)

___

### toChainedReference

▸ `Static` **toChainedReference**(`key`, `isTemporary?`): `BigNumber`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `key` | `BigNumberish` | `undefined` |
| `isTemporary` | `boolean` | `true` |

#### Returns

`BigNumber`

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/relayer.module.ts:184](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/relayer.module.ts#L184)
