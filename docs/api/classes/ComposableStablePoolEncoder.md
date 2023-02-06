# Class: ComposableStablePoolEncoder

## Table of contents

### Constructors

- [constructor](ComposableStablePoolEncoder.md#constructor)

### Methods

- [exitBPTInForExactTokensOut](ComposableStablePoolEncoder.md#exitbptinforexacttokensout)
- [exitExactBPTInForOneTokenOut](ComposableStablePoolEncoder.md#exitexactbptinforonetokenout)
- [joinCollectProtocolFees](ComposableStablePoolEncoder.md#joincollectprotocolfees)
- [joinExactTokensInForBPTOut](ComposableStablePoolEncoder.md#joinexacttokensinforbptout)
- [joinInit](ComposableStablePoolEncoder.md#joininit)
- [joinTokenInForExactBPTOut](ComposableStablePoolEncoder.md#jointokeninforexactbptout)

## Constructors

### constructor

• `Private` **new ComposableStablePoolEncoder**()

Cannot be constructed.

#### Defined in

[balancer-sdk/balancer-js/src/pool-composable-stable/encoder.ts:20](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-composable-stable/encoder.ts#L20)

## Methods

### exitBPTInForExactTokensOut

▸ `Static` **exitBPTInForExactTokensOut**(`amountsOut`, `maxBPTAmountIn`): `string`

Encodes the userData parameter for exiting a ComposableStablePool by removing exact amounts of tokens

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `amountsOut` | `BigNumberish`[] | the amounts of each token to be withdrawn from the pool |
| `maxBPTAmountIn` | `BigNumberish` | the minimum acceptable BPT to burn in return for withdrawn tokens |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-composable-stable/encoder.ts:102](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-composable-stable/encoder.ts#L102)

___

### exitExactBPTInForOneTokenOut

▸ `Static` **exitExactBPTInForOneTokenOut**(`bptAmountIn`, `exitTokenIndex`): `string`

Encodes the userData parameter for exiting a ComposableStablePool by removing a single token in return for an exact amount of BPT

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bptAmountIn` | `BigNumberish` | the amount of BPT to be burned |
| `exitTokenIndex` | `number` | - |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-composable-stable/encoder.ts:84](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-composable-stable/encoder.ts#L84)

___

### joinCollectProtocolFees

▸ `Static` **joinCollectProtocolFees**(): `string`

Encodes the userData parameter for collecting protocol fees for StablePhantomPool

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-composable-stable/encoder.ts:37](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-composable-stable/encoder.ts#L37)

___

### joinExactTokensInForBPTOut

▸ `Static` **joinExactTokensInForBPTOut**(`amountsIn`, `minimumBPT`): `string`

Encodes the userData parameter for joining a ComposableStablePool with exact token inputs

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `amountsIn` | `BigNumberish`[] | the amounts each of token to deposit in the pool as liquidity |
| `minimumBPT` | `BigNumberish` | the minimum acceptable BPT to receive in return for deposited tokens |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-composable-stable/encoder.ts:48](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-composable-stable/encoder.ts#L48)

___

### joinInit

▸ `Static` **joinInit**(`amountsIn`): `string`

Encodes the userData parameter for providing the initial liquidity to a ComposableStablePool

#### Parameters

| Name | Type |
| :------ | :------ |
| `amountsIn` | `BigNumberish`[] |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-composable-stable/encoder.ts:28](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-composable-stable/encoder.ts#L28)

___

### joinTokenInForExactBPTOut

▸ `Static` **joinTokenInForExactBPTOut**(`bptAmountOut`, `enterTokenIndex`): `string`

Encodes the userData parameter for joining a ComposableStablePool with to receive an exact amount of BPT

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bptAmountOut` | `BigNumberish` | the amount of BPT to be minted |
| `enterTokenIndex` | `number` | the index of the token to be provided as liquidity |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-composable-stable/encoder.ts:66](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-composable-stable/encoder.ts#L66)
