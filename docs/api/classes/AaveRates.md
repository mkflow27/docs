# Class: AaveRates

## Implements

- [`IAaveRates`](../interfaces/IAaveRates.md)

## Table of contents

### Constructors

- [constructor](AaveRates.md#constructor)

### Properties

- [multicall](AaveRates.md#multicall)
- [network](AaveRates.md#network)
- [rates](AaveRates.md#rates)

### Methods

- [fetch](AaveRates.md#fetch)
- [getRate](AaveRates.md#getrate)

## Constructors

### constructor

• **new AaveRates**(`multicallAddress`, `provider`, `network`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `multicallAddress` | `string` |
| `provider` | `Provider` |
| `network` | [`Network`](../enums/Network.md) |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/aave-rates.ts:21](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/aave-rates.ts#L21)

## Properties

### multicall

• **multicall**: `Contract`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/aave-rates.ts:18](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/aave-rates.ts#L18)

___

### network

• `Private` **network**: [`Network`](../enums/Network.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/aave-rates.ts:24](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/aave-rates.ts#L24)

___

### rates

• `Optional` **rates**: `Promise`<{ `[wrappedATokenAddress: string]`: `number`;  }\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/aave-rates.ts:19](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/aave-rates.ts#L19)

## Methods

### fetch

▸ `Private` **fetch**(`network`): `Promise`<{ `[wrappedATokenAddress: string]`: `number`;  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `network` | [`MAINNET`](../enums/Network.md#mainnet) \| [`POLYGON`](../enums/Network.md#polygon) |

#### Returns

`Promise`<{ `[wrappedATokenAddress: string]`: `number`;  }\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/aave-rates.ts:29](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/aave-rates.ts#L29)

___

### getRate

▸ **getRate**(`wrappedAToken`): `Promise`<`number`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `wrappedAToken` | `string` |

#### Returns

`Promise`<`number`\>

#### Implementation of

IAaveRates.getRate

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/aave-rates.ts:49](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/aave-rates.ts#L49)
