# Class: PoolsFallbackRepository

The fallback provider takes multiple PoolRepository's in an array and uses them in order
falling back to the next one if a request times out.

This is useful for using the Balancer API while being able to fall back to the graph if it is down
to ensure Balancer is maximally decentralized.

## Implements

- [`Findable`](../interfaces/Findable.md)<[`Pool`](../interfaces/Pool.md), [`PoolAttribute`](../modules.md#poolattribute)\>

## Table of contents

### Constructors

- [constructor](PoolsFallbackRepository.md#constructor)

### Properties

- [currentProviderIdx](PoolsFallbackRepository.md#currentprovideridx)
- [providers](PoolsFallbackRepository.md#providers)
- [timeout](PoolsFallbackRepository.md#timeout)

### Accessors

- [currentProvider](PoolsFallbackRepository.md#currentprovider)

### Methods

- [fallbackQuery](PoolsFallbackRepository.md#fallbackquery)
- [fetch](PoolsFallbackRepository.md#fetch)
- [find](PoolsFallbackRepository.md#find)
- [findBy](PoolsFallbackRepository.md#findby)

## Constructors

### constructor

• **new PoolsFallbackRepository**(`providers`, `options?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `providers` | [`PoolRepository`](../interfaces/PoolRepository.md)[] |
| `options` | [`PoolsFallbackRepositoryOptions`](../interfaces/PoolsFallbackRepositoryOptions.md) |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/fallback.ts:21](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/fallback.ts#L21)

## Properties

### currentProviderIdx

• **currentProviderIdx**: `number`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/fallback.ts:18](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/fallback.ts#L18)

___

### providers

• `Private` `Readonly` **providers**: [`PoolRepository`](../interfaces/PoolRepository.md)[]

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/fallback.ts:22](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/fallback.ts#L22)

___

### timeout

• **timeout**: `number`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/fallback.ts:19](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/fallback.ts#L19)

## Accessors

### currentProvider

• `get` **currentProvider**(): `undefined` \| [`PoolRepository`](../interfaces/PoolRepository.md)

#### Returns

`undefined` \| [`PoolRepository`](../interfaces/PoolRepository.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/fallback.ts:33](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/fallback.ts#L33)

## Methods

### fallbackQuery

▸ **fallbackQuery**(`func`, `args`): `Promise`<`any`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `func` | `string` |
| `args` | `unknown`[] |

#### Returns

`Promise`<`any`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/fallback.ts:56](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/fallback.ts#L56)

___

### fetch

▸ **fetch**(`options?`): `Promise`<[`Pool`](../interfaces/Pool.md)[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `options?` | [`PoolsRepositoryFetchOptions`](../interfaces/PoolsRepositoryFetchOptions.md) |

#### Returns

`Promise`<[`Pool`](../interfaces/Pool.md)[]\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/fallback.ts:29](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/fallback.ts#L29)

___

### find

▸ **find**(`id`): `Promise`<`undefined` \| [`Pool`](../interfaces/Pool.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |

#### Returns

`Promise`<`undefined` \| [`Pool`](../interfaces/Pool.md)\>

#### Implementation of

Findable.find

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/fallback.ts:44](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/fallback.ts#L44)

___

### findBy

▸ **findBy**(`attribute`, `value`): `Promise`<`undefined` \| [`Pool`](../interfaces/Pool.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `attribute` | [`PoolAttribute`](../modules.md#poolattribute) |
| `value` | `string` |

#### Returns

`Promise`<`undefined` \| [`Pool`](../interfaces/Pool.md)\>

#### Implementation of

Findable.findBy

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/fallback.ts:48](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/fallback.ts#L48)
