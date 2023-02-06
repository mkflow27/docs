# Class: WeightedPoolEncoder

## Table of contents

### Constructors

- [constructor](WeightedPoolEncoder.md#constructor)

### Methods

- [exitBPTInForExactTokensOut](WeightedPoolEncoder.md#exitbptinforexacttokensout)
- [exitExactBPTInForOneTokenOut](WeightedPoolEncoder.md#exitexactbptinforonetokenout)
- [exitExactBPTInForTokensOut](WeightedPoolEncoder.md#exitexactbptinfortokensout)
- [joinAllTokensInForExactBPTOut](WeightedPoolEncoder.md#joinalltokensinforexactbptout)
- [joinExactTokensInForBPTOut](WeightedPoolEncoder.md#joinexacttokensinforbptout)
- [joinInit](WeightedPoolEncoder.md#joininit)
- [joinTokenInForExactBPTOut](WeightedPoolEncoder.md#jointokeninforexactbptout)

## Constructors

### constructor

• `Private` **new WeightedPoolEncoder**()

Cannot be constructed.

#### Defined in

[balancer-sdk/balancer-js/src/pool-weighted/encoder.ts:22](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-weighted/encoder.ts#L22)

## Methods

### exitBPTInForExactTokensOut

▸ `Static` **exitBPTInForExactTokensOut**(`amountsOut`, `maxBPTAmountIn`): `string`

Encodes the userData parameter for exiting a WeightedPool by removing exact amounts of tokens

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `amountsOut` | `BigNumberish`[] | the amounts of each token to be withdrawn from the pool |
| `maxBPTAmountIn` | `BigNumberish` | the minimum acceptable BPT to burn in return for withdrawn tokens |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-weighted/encoder.ts:111](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-weighted/encoder.ts#L111)

___

### exitExactBPTInForOneTokenOut

▸ `Static` **exitExactBPTInForOneTokenOut**(`bptAmountIn`, `exitTokenIndex`): `string`

Encodes the userData parameter for exiting a WeightedPool by removing a single token in return for an exact amount of BPT

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bptAmountIn` | `BigNumberish` | the amount of BPT to be burned |
| `exitTokenIndex` | `number` | - |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-weighted/encoder.ts:83](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-weighted/encoder.ts#L83)

___

### exitExactBPTInForTokensOut

▸ `Static` **exitExactBPTInForTokensOut**(`bptAmountIn`): `string`

Encodes the userData parameter for exiting a WeightedPool by removing tokens in return for an exact amount of BPT

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bptAmountIn` | `BigNumberish` | the amount of BPT to be burned |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-weighted/encoder.ts:100](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-weighted/encoder.ts#L100)

___

### joinAllTokensInForExactBPTOut

▸ `Static` **joinAllTokensInForExactBPTOut**(`bptAmountOut`): `string`

Encodes the userData parameter for joining a WeightedPool proportionally to receive an exact amount of BPT

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bptAmountOut` | `BigNumberish` | the amount of BPT to be minted |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-weighted/encoder.ts:72](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-weighted/encoder.ts#L72)

___

### joinExactTokensInForBPTOut

▸ `Static` **joinExactTokensInForBPTOut**(`amountsIn`, `minimumBPT`): `string`

Encodes the userData parameter for joining a WeightedPool with exact token inputs

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `amountsIn` | `BigNumberish`[] | the amounts each of token to deposit in the pool as liquidity |
| `minimumBPT` | `BigNumberish` | the minimum acceptable BPT to receive in return for deposited tokens |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-weighted/encoder.ts:41](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-weighted/encoder.ts#L41)

___

### joinInit

▸ `Static` **joinInit**(`amountsIn`): `string`

Encodes the userData parameter for providing the initial liquidity to a WeightedPool

#### Parameters

| Name | Type |
| :------ | :------ |
| `amountsIn` | `BigNumberish`[] |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-weighted/encoder.ts:30](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-weighted/encoder.ts#L30)

___

### joinTokenInForExactBPTOut

▸ `Static` **joinTokenInForExactBPTOut**(`bptAmountOut`, `enterTokenIndex`): `string`

Encodes the userData parameter for joining a WeightedPool with a single token to receive an exact amount of BPT

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bptAmountOut` | `BigNumberish` | the amount of BPT to be minted |
| `enterTokenIndex` | `number` | the index of the token to be provided as liquidity |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/pool-weighted/encoder.ts:55](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-weighted/encoder.ts#L55)
