# Class: CoingeckoPriceRepository

Simple coingecko price source implementation. Configurable by network and token addresses.

## Implements

- [`Findable`](../interfaces/Findable.md)<[`Price`](../modules.md#price)\>

## Table of contents

### Constructors

- [constructor](CoingeckoPriceRepository.md#constructor)

### Properties

- [baseTokenAddresses](CoingeckoPriceRepository.md#basetokenaddresses)
- [chainId](CoingeckoPriceRepository.md#chainid)
- [debouncer](CoingeckoPriceRepository.md#debouncer)
- [nativePrice](CoingeckoPriceRepository.md#nativeprice)
- [prices](CoingeckoPriceRepository.md#prices)
- [urlBase](CoingeckoPriceRepository.md#urlbase)

### Methods

- [fetch](CoingeckoPriceRepository.md#fetch)
- [fetchNative](CoingeckoPriceRepository.md#fetchnative)
- [find](CoingeckoPriceRepository.md#find)
- [findBy](CoingeckoPriceRepository.md#findby)
- [platform](CoingeckoPriceRepository.md#platform)
- [url](CoingeckoPriceRepository.md#url)

## Constructors

### constructor

• **new CoingeckoPriceRepository**(`tokenAddresses`, `chainId?`)

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `tokenAddresses` | `string`[] | `undefined` |
| `chainId` | [`Network`](../enums/Network.md) | `1` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko.ts:17](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko.ts#L17)

## Properties

### baseTokenAddresses

• **baseTokenAddresses**: `string`[]

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko.ts:14](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko.ts#L14)

___

### chainId

• `Private` **chainId**: [`Network`](../enums/Network.md) = `1`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko.ts:17](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko.ts#L17)

___

### debouncer

• **debouncer**: [`Debouncer`](Debouncer.md)<[`TokenPrices`](../modules.md#tokenprices), `string`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko.ts:15](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko.ts#L15)

___

### nativePrice

• `Optional` **nativePrice**: `Promise`<[`Price`](../modules.md#price)\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko.ts:12](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko.ts#L12)

___

### prices

• **prices**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: `Promise`<[`Price`](../modules.md#price)\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko.ts:11](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko.ts#L11)

___

### urlBase

• **urlBase**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko.ts:13](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko.ts#L13)

## Methods

### fetch

▸ `Private` **fetch**(`addresses`, `«destructured»?`): `Promise`<[`TokenPrices`](../modules.md#tokenprices)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `addresses` | `string`[] |
| `«destructured»` | `Object` |
| › `signal?` | `AbortSignal` |

#### Returns

`Promise`<[`TokenPrices`](../modules.md#tokenprices)\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko.ts:28](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko.ts#L28)

___

### fetchNative

▸ `Private` **fetchNative**(`«destructured»?`): `Promise`<[`Price`](../modules.md#price)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `«destructured»` | `Object` |
| › `signal?` | `AbortSignal` |

#### Returns

`Promise`<[`Price`](../modules.md#price)\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko.ts:43](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko.ts#L43)

___

### find

▸ **find**(`inputAddress`): `Promise`<`undefined` \| [`Price`](../modules.md#price)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `inputAddress` | `string` |

#### Returns

`Promise`<`undefined` \| [`Price`](../modules.md#price)\>

#### Implementation of

Findable.find

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko.ts:68](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko.ts#L68)

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

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko.ts:99](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko.ts#L99)

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

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko.ts:107](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko.ts#L107)

___

### url

▸ `Private` **url**(`addresses`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `addresses` | `string`[] |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/coingecko.ts:125](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/coingecko.ts#L125)
