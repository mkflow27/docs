# Class: Liquidity

## Table of contents

### Constructors

- [constructor](Liquidity.md#constructor)

### Properties

- [pools](Liquidity.md#pools)
- [tokenPrices](Liquidity.md#tokenprices)

### Methods

- [getLiquidity](Liquidity.md#getliquidity)

## Constructors

### constructor

• **new Liquidity**(`pools`, `tokenPrices`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `pools` | [`Findable`](../interfaces/Findable.md)<[`Pool`](../interfaces/Pool.md), [`PoolAttribute`](../modules.md#poolattribute), `any`\> |
| `tokenPrices` | [`Findable`](../interfaces/Findable.md)<[`Price`](../modules.md#price), `string`, `any`\> |

#### Defined in

[balancer-sdk/balancer-js/src/modules/liquidity/liquidity.module.ts:15](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/liquidity/liquidity.module.ts#L15)

## Properties

### pools

• `Private` **pools**: [`Findable`](../interfaces/Findable.md)<[`Pool`](../interfaces/Pool.md), [`PoolAttribute`](../modules.md#poolattribute), `any`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/liquidity/liquidity.module.ts:16](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/liquidity/liquidity.module.ts#L16)

___

### tokenPrices

• `Private` **tokenPrices**: [`Findable`](../interfaces/Findable.md)<[`Price`](../modules.md#price), `string`, `any`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/liquidity/liquidity.module.ts:17](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/liquidity/liquidity.module.ts#L17)

## Methods

### getLiquidity

▸ **getLiquidity**(`pool`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `pool` | [`Pool`](../interfaces/Pool.md) |

#### Returns

`Promise`<`string`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/liquidity/liquidity.module.ts:20](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/liquidity/liquidity.module.ts#L20)
