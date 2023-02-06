# Class: PoolsSubgraphOnChainRepository

Access pools using generated subgraph client and multicall.

## Implements

- [`Findable`](../interfaces/Findable.md)<[`Pool`](../interfaces/Pool.md), [`PoolAttribute`](../modules.md#poolattribute)\>
- [`Searchable`](../interfaces/Searchable.md)<[`Pool`](../interfaces/Pool.md)\>

## Table of contents

### Constructors

- [constructor](PoolsSubgraphOnChainRepository.md#constructor)

### Properties

- [multicall](PoolsSubgraphOnChainRepository.md#multicall)
- [pools](PoolsSubgraphOnChainRepository.md#pools)
- [poolsSubgraph](PoolsSubgraphOnChainRepository.md#poolssubgraph)
- [provider](PoolsSubgraphOnChainRepository.md#provider)
- [skip](PoolsSubgraphOnChainRepository.md#skip)
- [vault](PoolsSubgraphOnChainRepository.md#vault)

### Methods

- [all](PoolsSubgraphOnChainRepository.md#all)
- [fetch](PoolsSubgraphOnChainRepository.md#fetch)
- [fetchDefault](PoolsSubgraphOnChainRepository.md#fetchdefault)
- [find](PoolsSubgraphOnChainRepository.md#find)
- [findBy](PoolsSubgraphOnChainRepository.md#findby)
- [where](PoolsSubgraphOnChainRepository.md#where)

## Constructors

### constructor

• **new PoolsSubgraphOnChainRepository**(`options`)

Repository using multicall to get onchain data.

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | `PoolsSubgraphOnChainRepositoryOptions` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraphOnChain.ts:41](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraphOnChain.ts#L41)

## Properties

### multicall

• `Private` **multicall**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraphOnChain.ts:28](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraphOnChain.ts#L28)

___

### pools

• `Private` `Optional` **pools**: `Promise`<[`Pool`](../interfaces/Pool.md)[]\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraphOnChain.ts:27](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraphOnChain.ts#L27)

___

### poolsSubgraph

• `Private` **poolsSubgraph**: [`PoolsSubgraphRepository`](PoolsSubgraphRepository.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraphOnChain.ts:25](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraphOnChain.ts#L25)

___

### provider

• `Private` **provider**: `Provider`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraphOnChain.ts:26](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraphOnChain.ts#L26)

___

### skip

• **skip**: `number` = `0`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraphOnChain.ts:30](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraphOnChain.ts#L30)

___

### vault

• `Private` **vault**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraphOnChain.ts:29](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraphOnChain.ts#L29)

## Methods

### all

▸ **all**(): `Promise`<[`Pool`](../interfaces/Pool.md)[]\>

#### Returns

`Promise`<[`Pool`](../interfaces/Pool.md)[]\>

#### Implementation of

Searchable.all

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraphOnChain.ts:98](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraphOnChain.ts#L98)

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

[balancer-sdk/balancer-js/src/modules/data/pool/subgraphOnChain.ts:75](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraphOnChain.ts#L75)

___

### fetchDefault

▸ `Private` **fetchDefault**(): `Promise`<[`Pool`](../interfaces/Pool.md)[]\>

We need a list of all the pools, for calculating APRs (nested pools), and for SOR (path finding).
All the pools are fetched on page load and cachced for speedy lookups.

#### Returns

`Promise`<[`Pool`](../interfaces/Pool.md)[]\>

Promise resolving to pools list

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraphOnChain.ts:59](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraphOnChain.ts#L59)

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

[balancer-sdk/balancer-js/src/modules/data/pool/subgraphOnChain.ts:86](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraphOnChain.ts#L86)

___

### findBy

▸ **findBy**(`param`, `value`): `Promise`<`undefined` \| [`Pool`](../interfaces/Pool.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `param` | [`PoolAttribute`](../modules.md#poolattribute) |
| `value` | `string` |

#### Returns

`Promise`<`undefined` \| [`Pool`](../interfaces/Pool.md)\>

#### Implementation of

Findable.findBy

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraphOnChain.ts:90](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraphOnChain.ts#L90)

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

[balancer-sdk/balancer-js/src/modules/data/pool/subgraphOnChain.ts:105](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraphOnChain.ts#L105)
