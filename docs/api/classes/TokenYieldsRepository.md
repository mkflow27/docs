# Class: TokenYieldsRepository

## Implements

- [`Findable`](../interfaces/Findable.md)<`number`\>

## Table of contents

### Constructors

- [constructor](TokenYieldsRepository.md#constructor)

### Properties

- [network](TokenYieldsRepository.md#network)
- [sources](TokenYieldsRepository.md#sources)
- [yields](TokenYieldsRepository.md#yields)

### Methods

- [fetch](TokenYieldsRepository.md#fetch)
- [find](TokenYieldsRepository.md#find)
- [findBy](TokenYieldsRepository.md#findby)

## Constructors

### constructor

• **new TokenYieldsRepository**(`network`, `sources?`)

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `network` | [`Network`](../enums/Network.md) | `undefined` |
| `sources` | `Object` | `yieldSourceMap` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-yields/repository.ts:42](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-yields/repository.ts#L42)

## Properties

### network

• `Private` **network**: [`Network`](../enums/Network.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-yields/repository.ts:42](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-yields/repository.ts#L42)

___

### sources

• `Private` **sources**: `Object` = `yieldSourceMap`

#### Index signature

▪ [address: `string`]: [`AprFetcher`](../interfaces/AprFetcher.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-yields/repository.ts:42](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-yields/repository.ts#L42)

___

### yields

• `Private` **yields**: `Object` = `{}`

#### Index signature

▪ [address: `string`]: `number`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-yields/repository.ts:40](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-yields/repository.ts#L40)

## Methods

### fetch

▸ **fetch**(`address`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |

#### Returns

`Promise`<`void`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-yields/repository.ts:44](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-yields/repository.ts#L44)

___

### find

▸ **find**(`address`): `Promise`<`undefined` \| `number`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |

#### Returns

`Promise`<`undefined` \| `number`\>

#### Implementation of

Findable.find

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-yields/repository.ts:52](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-yields/repository.ts#L52)

___

### findBy

▸ **findBy**(`attribute`, `value`): `Promise`<`undefined` \| `number`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `attribute` | `string` |
| `value` | `string` |

#### Returns

`Promise`<`undefined` \| `number`\>

#### Implementation of

Findable.findBy

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-yields/repository.ts:64](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-yields/repository.ts#L64)
