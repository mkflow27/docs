# Class: PoolsBalancerAPIRepository

Access pools using the Balancer GraphQL Api.

Balancer's API URL: https://api.balancer.fi/query/

## Implements

- [`Findable`](../interfaces/Findable.md)<[`Pool`](../interfaces/Pool.md), [`PoolAttribute`](../modules.md#poolattribute)\>

## Table of contents

### Constructors

- [constructor](PoolsBalancerAPIRepository.md#constructor)

### Properties

- [client](PoolsBalancerAPIRepository.md#client)
- [nextToken](PoolsBalancerAPIRepository.md#nexttoken)
- [pools](PoolsBalancerAPIRepository.md#pools)
- [query](PoolsBalancerAPIRepository.md#query)
- [skip](PoolsBalancerAPIRepository.md#skip)

### Methods

- [fetch](PoolsBalancerAPIRepository.md#fetch)
- [fetchFromCache](PoolsBalancerAPIRepository.md#fetchfromcache)
- [find](PoolsBalancerAPIRepository.md#find)
- [findBy](PoolsBalancerAPIRepository.md#findby)
- [format](PoolsBalancerAPIRepository.md#format)

## Constructors

### constructor

• **new PoolsBalancerAPIRepository**(`options`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | `PoolsBalancerAPIOptions` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/balancer-api.ts:34](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/balancer-api.ts#L34)

## Properties

### client

• `Private` **client**: `default`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/balancer-api.ts:28](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/balancer-api.ts#L28)

___

### nextToken

• **nextToken**: `undefined` \| `string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/balancer-api.ts:31](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/balancer-api.ts#L31)

___

### pools

• **pools**: [`Pool`](../interfaces/Pool.md)[] = `[]`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/balancer-api.ts:29](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/balancer-api.ts#L29)

___

### query

• `Private` **query**: [`GraphQLQuery`](../interfaces/GraphQLQuery.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/balancer-api.ts:32](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/balancer-api.ts#L32)

___

### skip

• **skip**: `number` = `0`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/balancer-api.ts:30](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/balancer-api.ts#L30)

## Methods

### fetch

▸ **fetch**(`options?`): `Promise`<[`Pool`](../interfaces/Pool.md)[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `options?` | [`PoolsRepositoryFetchOptions`](../interfaces/PoolsRepositoryFetchOptions.md) |

#### Returns

`Promise`<[`Pool`](../interfaces/Pool.md)[]\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/balancer-api.ts:74](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/balancer-api.ts#L74)

___

### fetchFromCache

▸ **fetchFromCache**(`options?`): [`Pool`](../interfaces/Pool.md)[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `options?` | [`PoolsRepositoryFetchOptions`](../interfaces/PoolsRepositoryFetchOptions.md) |

#### Returns

[`Pool`](../interfaces/Pool.md)[]

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/balancer-api.ts:65](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/balancer-api.ts#L65)

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

[balancer-sdk/balancer-js/src/modules/data/pool/balancer-api.ts:116](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/balancer-api.ts#L116)

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

[balancer-sdk/balancer-js/src/modules/data/pool/balancer-api.ts:124](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/balancer-api.ts#L124)

___

### format

▸ `Private` **format**(`pool`): [`Pool`](../interfaces/Pool.md)

Fixes any formatting issues from the subgraph
 - GraphQL can't store a map so pool.apr.[rewardAprs/tokenAprs].breakdown
   is JSON data that needs to be parsed so they match the Pool type correctly.

#### Parameters

| Name | Type |
| :------ | :------ |
| `pool` | [`Pool`](../interfaces/Pool.md) |

#### Returns

[`Pool`](../interfaces/Pool.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/balancer-api.ts:139](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/balancer-api.ts#L139)
