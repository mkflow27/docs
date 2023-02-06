# Class: TokenPriceProvider

## Implements

- [`Findable`](../interfaces/Findable.md)<[`Price`](../modules.md#price)\>

## Table of contents

### Constructors

- [constructor](TokenPriceProvider.md#constructor)

### Properties

- [aaveRates](TokenPriceProvider.md#aaverates)
- [coingeckoRepository](TokenPriceProvider.md#coingeckorepository)
- [subgraphRepository](TokenPriceProvider.md#subgraphrepository)

### Methods

- [find](TokenPriceProvider.md#find)
- [findBy](TokenPriceProvider.md#findby)

## Constructors

### constructor

• **new TokenPriceProvider**(`coingeckoRepository`, `subgraphRepository`, `aaveRates`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `coingeckoRepository` | [`Findable`](../interfaces/Findable.md)<[`Price`](../modules.md#price), `string`, `any`\> |
| `subgraphRepository` | [`Findable`](../interfaces/Findable.md)<[`Price`](../modules.md#price), `string`, `any`\> |
| `aaveRates` | [`IAaveRates`](../interfaces/IAaveRates.md) |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/provider.ts:5](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/provider.ts#L5)

## Properties

### aaveRates

• `Private` **aaveRates**: [`IAaveRates`](../interfaces/IAaveRates.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/provider.ts:8](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/provider.ts#L8)

___

### coingeckoRepository

• `Private` **coingeckoRepository**: [`Findable`](../interfaces/Findable.md)<[`Price`](../modules.md#price), `string`, `any`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/provider.ts:6](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/provider.ts#L6)

___

### subgraphRepository

• `Private` **subgraphRepository**: [`Findable`](../interfaces/Findable.md)<[`Price`](../modules.md#price), `string`, `any`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/provider.ts:7](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/provider.ts#L7)

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

[balancer-sdk/balancer-js/src/modules/data/token-prices/provider.ts:11](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/provider.ts#L11)

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

[balancer-sdk/balancer-js/src/modules/data/token-prices/provider.ts:37](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/provider.ts#L37)
