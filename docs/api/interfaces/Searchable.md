# Interface: Searchable<T\>

## Type parameters

| Name |
| :------ |
| `T` |

## Implemented by

- [`PoolsStaticRepository`](../classes/PoolsStaticRepository.md)
- [`PoolsSubgraphOnChainRepository`](../classes/PoolsSubgraphOnChainRepository.md)
- [`PoolsSubgraphRepository`](../classes/PoolsSubgraphRepository.md)

## Table of contents

### Properties

- [all](Searchable.md#all)
- [where](Searchable.md#where)

## Properties

### all

• **all**: () => `Promise`<`T`[]\>

#### Type declaration

▸ (): `Promise`<`T`[]\>

##### Returns

`Promise`<`T`[]\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/types.ts:18](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/types.ts#L18)

___

### where

• **where**: (`filters`: (`arg`: `T`) => `boolean`) => `Promise`<`T`[]\>

#### Type declaration

▸ (`filters`): `Promise`<`T`[]\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `filters` | (`arg`: `T`) => `boolean` |

##### Returns

`Promise`<`T`[]\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/types.ts:19](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/types.ts#L19)
