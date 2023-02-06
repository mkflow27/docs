# Class: PoolsStaticRepository

## Implements

- [`Findable`](../interfaces/Findable.md)<[`Pool`](../interfaces/Pool.md), [`PoolAttribute`](../modules.md#poolattribute)\>
- [`Searchable`](../interfaces/Searchable.md)<[`Pool`](../interfaces/Pool.md)\>

## Table of contents

### Constructors

- [constructor](PoolsStaticRepository.md#constructor)

### Properties

- [pools](PoolsStaticRepository.md#pools)

### Methods

- [all](PoolsStaticRepository.md#all)
- [find](PoolsStaticRepository.md#find)
- [findBy](PoolsStaticRepository.md#findby)
- [where](PoolsStaticRepository.md#where)

## Constructors

### constructor

• **new PoolsStaticRepository**(`pools`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `pools` | [`Pool`](../interfaces/Pool.md)[] |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/static.ts:7](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/static.ts#L7)

## Properties

### pools

• `Private` **pools**: [`Pool`](../interfaces/Pool.md)[]

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/static.ts:7](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/static.ts#L7)

## Methods

### all

▸ **all**(): `Promise`<[`Pool`](../interfaces/Pool.md)[]\>

#### Returns

`Promise`<[`Pool`](../interfaces/Pool.md)[]\>

#### Implementation of

Searchable.all

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/static.ts:24](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/static.ts#L24)

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

[balancer-sdk/balancer-js/src/modules/data/pool/static.ts:9](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/static.ts#L9)

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

[balancer-sdk/balancer-js/src/modules/data/pool/static.ts:15](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/static.ts#L15)

___

### where

▸ **where**(`filter`): `Promise`<[`Pool`](../interfaces/Pool.md)[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `filter` | (`pool`: [`Pool`](../interfaces/Pool.md)) => `boolean` |

#### Returns

`Promise`<[`Pool`](../interfaces/Pool.md)[]\>

#### Implementation of

Searchable.where

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/static.ts:28](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/static.ts#L28)
