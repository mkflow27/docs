# Class: HistoricalPriceProvider

## Implements

- [`Findable`](../interfaces/Findable.md)<[`Price`](../modules.md#price)\>

## Table of contents

### Constructors

- [constructor](HistoricalPriceProvider.md#constructor)

### Properties

- [aaveRates](HistoricalPriceProvider.md#aaverates)
- [coingeckoRepository](HistoricalPriceProvider.md#coingeckorepository)

### Methods

- [find](HistoricalPriceProvider.md#find)
- [findBy](HistoricalPriceProvider.md#findby)

## Constructors

### constructor

• **new HistoricalPriceProvider**(`coingeckoRepository`, `aaveRates`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `coingeckoRepository` | [`Findable`](../interfaces/Findable.md)<[`Price`](../modules.md#price), `string`, `any`\> |
| `aaveRates` | [`IAaveRates`](../interfaces/IAaveRates.md) |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/historical-price-provider.ts:5](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/historical-price-provider.ts#L5)

## Properties

### aaveRates

• `Private` **aaveRates**: [`IAaveRates`](../interfaces/IAaveRates.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/historical-price-provider.ts:7](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/historical-price-provider.ts#L7)

___

### coingeckoRepository

• `Private` **coingeckoRepository**: [`Findable`](../interfaces/Findable.md)<[`Price`](../modules.md#price), `string`, `any`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/historical-price-provider.ts:6](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/historical-price-provider.ts#L6)

## Methods

### find

▸ **find**(`address`): `Promise`<`undefined` \| [`Price`](../modules.md#price)\>

get the historical price at time of call

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `address` | `string` | the token address |

#### Returns

`Promise`<`undefined` \| [`Price`](../modules.md#price)\>

#### Implementation of

Findable.find

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/historical-price-provider.ts:15](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/historical-price-provider.ts#L15)

___

### findBy

▸ **findBy**(`address`, `timestamp`): `Promise`<`undefined` \| [`Price`](../modules.md#price)\>

get the historical price at the given timestamp.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `address` | `string` | the token address |
| `timestamp` | `number` | the UNIX timestamp |

#### Returns

`Promise`<`undefined` \| [`Price`](../modules.md#price)\>

#### Implementation of

Findable.findBy

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/historical-price-provider.ts:25](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/historical-price-provider.ts#L25)
