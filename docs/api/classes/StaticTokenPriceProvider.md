# Class: StaticTokenPriceProvider

## Implements

- [`Findable`](../interfaces/Findable.md)<[`Price`](../modules.md#price)\>

## Table of contents

### Constructors

- [constructor](StaticTokenPriceProvider.md#constructor)

### Properties

- [tokenPrices](StaticTokenPriceProvider.md#tokenprices)

### Methods

- [find](StaticTokenPriceProvider.md#find)
- [findBy](StaticTokenPriceProvider.md#findby)

## Constructors

### constructor

• **new StaticTokenPriceProvider**(`tokenPrices`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `tokenPrices` | [`TokenPrices`](../modules.md#tokenprices) |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/static.ts:5](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/static.ts#L5)

## Properties

### tokenPrices

• **tokenPrices**: [`TokenPrices`](../modules.md#tokenprices)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/static.ts:4](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/static.ts#L4)

## Methods

### find

▸ **find**(`address`): `Promise`<`undefined` \| [`Price`](../modules.md#price)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |

#### Returns

`Promise`<`undefined` \| [`Price`](../modules.md#price)\>

#### Implementation of

Findable.find

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/static.ts:13](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/static.ts#L13)

___

### findBy

▸ **findBy**(`attribute`, `value`): `Promise`<`undefined` \| [`Price`](../modules.md#price)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `attribute` | `string` |
| `value` | `string` |

#### Returns

`Promise`<`undefined` \| [`Price`](../modules.md#price)\>

#### Implementation of

Findable.findBy

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/static.ts:20](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/static.ts#L20)
