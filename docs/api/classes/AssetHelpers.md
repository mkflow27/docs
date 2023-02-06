# Class: AssetHelpers

## Table of contents

### Constructors

- [constructor](AssetHelpers.md#constructor)

### Properties

- [ETH](AssetHelpers.md#eth)
- [WETH](AssetHelpers.md#weth)

### Methods

- [isETH](AssetHelpers.md#iseth)
- [isWETH](AssetHelpers.md#isweth)
- [sortTokens](AssetHelpers.md#sorttokens)
- [translateToERC20](AssetHelpers.md#translatetoerc20)
- [isEqual](AssetHelpers.md#isequal)

## Constructors

### constructor

• **new AssetHelpers**(`wethAddress`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `wethAddress` | `string` |

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/assetHelpers.ts:15](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/assetHelpers.ts#L15)

## Properties

### ETH

• `Readonly` **ETH**: `string` = `AddressZero`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/assetHelpers.ts:12](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/assetHelpers.ts#L12)

___

### WETH

• `Readonly` **WETH**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/assetHelpers.ts:13](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/assetHelpers.ts#L13)

## Methods

### isETH

▸ **isETH**(`token`): `boolean`

Tests whether `token` is ETH (represented by `0x0000...0000`).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `token` | `string` | the address of the asset to be checked |

#### Returns

`boolean`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/assetHelpers.ts:27](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/assetHelpers.ts#L27)

___

### isWETH

▸ **isWETH**(`token`): `boolean`

Tests whether `token` is WETH.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `token` | `string` | the address of the asset to be checked |

#### Returns

`boolean`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/assetHelpers.ts:34](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/assetHelpers.ts#L34)

___

### sortTokens

▸ **sortTokens**(`tokens`, `...others`): [`string`[], ...unknown[][]]

Sorts an array of token addresses into ascending order to match the format expected by the Vault.

Passing additional arrays will result in each being sorted to maintain relative ordering to token addresses.

The zero address (representing ETH) is sorted as if it were the WETH address.
This matches the behaviour expected by the Vault when receiving an array of addresses.

**`Example`**

```ts
const [tokens] = sortTokens([tokenB, tokenC, tokenA])
const [tokens, weights] = sortTokens([tokenB, tokenC, tokenA], [weightB, weightC, weightA])
// where tokens = [tokenA, tokenB, tokenC], weights = [weightA, weightB, weightC]
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tokens` | `string`[] | an array of token addresses to be sorted in ascending order |
| `...others` | `unknown`[][] | a set of arrays to be sorted in the same order as the tokens, e.g. token weights or asset manager addresses |

#### Returns

[`string`[], ...unknown[][]]

an array of the form `[tokens, ...others]` where each subarray has been sorted to maintain its ordering relative to `tokens`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/assetHelpers.ts:63](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/assetHelpers.ts#L63)

___

### translateToERC20

▸ **translateToERC20**(`token`): `string`

Converts an asset to the equivalent ERC20 address.

For ERC20s this will return the passed address but passing ETH (`0x0000...0000`) will return the WETH address

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `token` | `string` | the address of the asset to be translated to an equivalent ERC20 |

#### Returns

`string`

the address of translated ERC20 asset

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/assetHelpers.ts:43](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/assetHelpers.ts#L43)

___

### isEqual

▸ `Static` **isEqual**(`addressA`, `addressB`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `addressA` | `string` |
| `addressB` | `string` |

#### Returns

`boolean`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/assetHelpers.ts:19](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/assetHelpers.ts#L19)
