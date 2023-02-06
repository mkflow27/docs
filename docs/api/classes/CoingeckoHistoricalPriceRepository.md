# Class: CoingeckoHistoricalPriceRepository

Simple coingecko price source implementation. Configurable by network and token addresses.

## Implements

- [`Findable`](../interfaces/Findable.md)<[`Price`](../modules.md#price)\>

## Table of contents

### Constructors

- [constructor](CoingeckoHistoricalPriceRepository.md#constructor)

### Properties

- [chainId](CoingeckoHistoricalPriceRepository.md#chainid)
- [nativePrice](CoingeckoHistoricalPriceRepository.md#nativeprice)
- [prices](CoingeckoHistoricalPriceRepository.md#prices)
- [urlBase](CoingeckoHistoricalPriceRepository.md#urlbase)

### Methods

- [fetch](CoingeckoHistoricalPriceRepository.md#fetch)
- [find](CoingeckoHistoricalPriceRepository.md#find)
- [findBy](CoingeckoHistoricalPriceRepository.md#findby)
- [platform](CoingeckoHistoricalPriceRepository.md#platform)
- [urlRange](CoingeckoHistoricalPriceRepository.md#urlrange)

## Constructors

### constructor

• **new CoingeckoHistoricalPriceRepository**(`chainId?`)

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `chainId` | [`Network`](../enums/Network.md) | `1` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko-historical.ts:22](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko-historical.ts#L22)

## Properties

### chainId

• `Private` **chainId**: [`Network`](../enums/Network.md) = `1`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko-historical.ts:22](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko-historical.ts#L22)

___

### nativePrice

• `Optional` **nativePrice**: `Promise`<[`Price`](../modules.md#price)\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko-historical.ts:19](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko-historical.ts#L19)

___

### prices

• **prices**: [`TokenPrices`](../modules.md#tokenprices) = `{}`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko-historical.ts:18](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko-historical.ts#L18)

___

### urlBase

• **urlBase**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko-historical.ts:20](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko-historical.ts#L20)

## Methods

### fetch

▸ `Private` **fetch**(`address`, `timestamp`, `«destructured»?`): `Promise`<[`HistoricalPrices`](../modules.md#historicalprices)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `timestamp` | `number` |
| `«destructured»` | `Object` |
| › `signal?` | `AbortSignal` |

#### Returns

`Promise`<[`HistoricalPrices`](../modules.md#historicalprices)\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko-historical.ts:28](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko-historical.ts#L28)

___

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

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko-historical.ts:46](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko-historical.ts#L46)

___

### findBy

▸ **findBy**(`inputAddress`, `timestamp`): `Promise`<`undefined` \| [`Price`](../modules.md#price)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `inputAddress` | `string` |
| `timestamp` | `number` |

#### Returns

`Promise`<`undefined` \| [`Price`](../modules.md#price)\>

#### Implementation of

Findable.findBy

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko-historical.ts:50](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko-historical.ts#L50)

___

### platform

▸ `Private` **platform**(`chainId`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainId` | `number` |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko-historical.ts:62](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko-historical.ts#L62)

___

### urlRange

▸ `Private` **urlRange**(`address`, `timestamp`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `timestamp` | `number` |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko-historical.ts:80](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko-historical.ts#L80)
