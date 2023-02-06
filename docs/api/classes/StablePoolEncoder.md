# Class: StablePoolEncoder

## Table of contents

### Constructors

- [constructor](StablePoolEncoder.md#constructor)

### Methods

- [exitBPTInForExactTokensOut](StablePoolEncoder.md#exitbptinforexacttokensout)
- [exitExactBPTInForOneTokenOut](StablePoolEncoder.md#exitexactbptinforonetokenout)
- [exitExactBPTInForTokensOut](StablePoolEncoder.md#exitexactbptinfortokensout)
- [joinCollectProtocolFees](StablePoolEncoder.md#joincollectprotocolfees)
- [joinExactTokensInForBPTOut](StablePoolEncoder.md#joinexacttokensinforbptout)
- [joinInit](StablePoolEncoder.md#joininit)
- [joinTokenInForExactBPTOut](StablePoolEncoder.md#jointokeninforexactbptout)

## Constructors

### constructor

• `Private` **new StablePoolEncoder**()

Cannot be constructed.

#### Defined in

[balancer-sdk/balancer-js/src/pool-stable/encoder.ts:25](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-stable/encoder.ts#L25)

## Methods

### exitBPTInForExactTokensOut

▸ `Static` **exitBPTInForExactTokensOut**(`amountsOut`, `maxBPTAmountIn`): `string`

Encodes the userData parameter for exiting a StablePool by removing exact amounts of tokens

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `amountsOut` | `BigNumberish`[] | the amounts of each token to be withdrawn from the pool |
| `maxBPTAmountIn` | `BigNumberish` | the minimum acceptable BPT to burn in return for withdrawn tokens |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-stable/encoder.ts:113](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-stable/encoder.ts#L113)

___

### exitExactBPTInForOneTokenOut

▸ `Static` **exitExactBPTInForOneTokenOut**(`bptAmountIn`, `exitTokenIndex`): `string`

Encodes the userData parameter for exiting a StablePool by removing a single token in return for an exact amount of BPT

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bptAmountIn` | `BigNumberish` | the amount of BPT to be burned |
| `exitTokenIndex` | `number` | - |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-stable/encoder.ts:85](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-stable/encoder.ts#L85)

___

### exitExactBPTInForTokensOut

▸ `Static` **exitExactBPTInForTokensOut**(`bptAmountIn`): `string`

Encodes the userData parameter for exiting a StablePool by removing tokens in return for an exact amount of BPT

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bptAmountIn` | `BigNumberish` | the amount of BPT to be burned |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-stable/encoder.ts:102](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-stable/encoder.ts#L102)

___

### joinCollectProtocolFees

▸ `Static` **joinCollectProtocolFees**(): `string`

Encodes the userData parameter for collecting protocol fees for StablePhantomPool

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-stable/encoder.ts:42](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-stable/encoder.ts#L42)

___

### joinExactTokensInForBPTOut

▸ `Static` **joinExactTokensInForBPTOut**(`amountsIn`, `minimumBPT`): `string`

Encodes the userData parameter for joining a StablePool with exact token inputs

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `amountsIn` | `BigNumberish`[] | the amounts each of token to deposit in the pool as liquidity |
| `minimumBPT` | `BigNumberish` | the minimum acceptable BPT to receive in return for deposited tokens |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-stable/encoder.ts:53](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-stable/encoder.ts#L53)

___

### joinInit

▸ `Static` **joinInit**(`amountsIn`): `string`

Encodes the userData parameter for providing the initial liquidity to a StablePool

#### Parameters

| Name | Type |
| :------ | :------ |
| `amountsIn` | `BigNumberish`[] |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-stable/encoder.ts:33](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-stable/encoder.ts#L33)

___

### joinTokenInForExactBPTOut

▸ `Static` **joinTokenInForExactBPTOut**(`bptAmountOut`, `enterTokenIndex`): `string`

Encodes the userData parameter for joining a StablePool with to receive an exact amount of BPT

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bptAmountOut` | `BigNumberish` | the amount of BPT to be minted |
| `enterTokenIndex` | `number` | the index of the token to be provided as liquidity |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-stable/encoder.ts:67](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-stable/encoder.ts#L67)
