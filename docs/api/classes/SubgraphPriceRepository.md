# Class: SubgraphPriceRepository

## Implements

- [`Findable`](../interfaces/Findable.md)<[`Price`](../modules.md#price)\>

## Table of contents

### Constructors

- [constructor](SubgraphPriceRepository.md#constructor)

### Properties

- [chainId](SubgraphPriceRepository.md#chainid)
- [debouncer](SubgraphPriceRepository.md#debouncer)
- [prices](SubgraphPriceRepository.md#prices)
- [subgraphUrl](SubgraphPriceRepository.md#subgraphurl)

### Methods

- [fetch](SubgraphPriceRepository.md#fetch)
- [find](SubgraphPriceRepository.md#find)
- [findBy](SubgraphPriceRepository.md#findby)

## Constructors

### constructor

• **new SubgraphPriceRepository**(`subgraphUrl`, `chainId?`)

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `subgraphUrl` | `string` | `undefined` |
| `chainId` | [`Network`](../enums/Network.md) | `1` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/subgraph.ts:21](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/subgraph.ts#L21)

## Properties

### chainId

• `Private` **chainId**: [`Network`](../enums/Network.md) = `1`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/subgraph.ts:21](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/subgraph.ts#L21)

___

### debouncer

• **debouncer**: [`Debouncer`](Debouncer.md)<[`TokenPrices`](../modules.md#tokenprices), `string`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/subgraph.ts:19](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/subgraph.ts#L19)

___

### prices

• **prices**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: `Promise`<[`Price`](../modules.md#price)\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/subgraph.ts:18](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/subgraph.ts#L18)

___

### subgraphUrl

• `Private` **subgraphUrl**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-prices/subgraph.ts:21](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/subgraph.ts#L21)

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

[balancer-sdk/balancer-js/src/modules/data/token-prices/subgraph.ts:28](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/subgraph.ts#L28)

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

[balancer-sdk/balancer-js/src/modules/data/token-prices/subgraph.ts:67](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/subgraph.ts#L67)

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

[balancer-sdk/balancer-js/src/modules/data/token-prices/subgraph.ts:78](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-prices/subgraph.ts#L78)
