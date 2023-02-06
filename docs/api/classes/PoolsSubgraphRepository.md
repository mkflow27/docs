# Class: PoolsSubgraphRepository

Access pools using generated subgraph client.

Balancer's subgraph URL: https://thegraph.com/hosted-service/subgraph/balancer-labs/balancer-v2

## Implements

- [`Findable`](../interfaces/Findable.md)<[`Pool`](../interfaces/Pool.md), [`PoolAttribute`](../modules.md#poolattribute)\>
- [`Searchable`](../interfaces/Searchable.md)<[`Pool`](../interfaces/Pool.md)\>

## Table of contents

### Constructors

- [constructor](PoolsSubgraphRepository.md#constructor)

### Properties

- [blockHeight](PoolsSubgraphRepository.md#blockheight)
- [chainId](PoolsSubgraphRepository.md#chainid)
- [client](PoolsSubgraphRepository.md#client)
- [pools](PoolsSubgraphRepository.md#pools)
- [query](PoolsSubgraphRepository.md#query)
- [skip](PoolsSubgraphRepository.md#skip)

### Methods

- [all](PoolsSubgraphRepository.md#all)
- [block](PoolsSubgraphRepository.md#block)
- [fetch](PoolsSubgraphRepository.md#fetch)
- [fetchDefault](PoolsSubgraphRepository.md#fetchdefault)
- [find](PoolsSubgraphRepository.md#find)
- [findBy](PoolsSubgraphRepository.md#findby)
- [mapSubPoolToken](PoolsSubgraphRepository.md#mapsubpooltoken)
- [mapSubPools](PoolsSubgraphRepository.md#mapsubpools)
- [mapToken](PoolsSubgraphRepository.md#maptoken)
- [mapType](PoolsSubgraphRepository.md#maptype)
- [where](PoolsSubgraphRepository.md#where)

## Constructors

### constructor

• **new PoolsSubgraphRepository**(`options`)

Repository with optional lazy loaded blockHeight

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | `PoolsSubgraphRepositoryOptions` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraph.ts:71](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraph.ts#L71)

## Properties

### blockHeight

• `Private` **blockHeight**: `undefined` \| () => `Promise`<`undefined` \| `number`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraph.ts:61](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraph.ts#L61)

___

### chainId

• `Private` **chainId**: [`Network`](../enums/Network.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraph.ts:58](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraph.ts#L58)

___

### client

• `Private` **client**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `AllPools` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`Pool_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`Pool_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`AllPoolsQuery`\> |
| `Balancers` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`Balancer_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`Balancer_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`BalancersQuery`\> |
| `JoinExits` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`JoinExit_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`JoinExit_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`JoinExitsQuery`\> |
| `Pool` | (`variables`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `id`: `string`  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolQuery`\> |
| `PoolHistoricalLiquidities` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`PoolHistoricalLiquidity_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`PoolHistoricalLiquidity_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolHistoricalLiquiditiesQuery`\> |
| `PoolShare` | (`variables`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `id`: `string`  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolShareQuery`\> |
| `PoolShares` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`PoolShare_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`PoolShare_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolSharesQuery`\> |
| `PoolSnapshots` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`PoolSnapshot_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`PoolSnapshot_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolSnapshotsQuery`\> |
| `Pools` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`Pool_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`Pool_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolsQuery`\> |
| `TokenLatestPrice` | (`variables`: `Exact`<{ `id`: `string`  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`TokenLatestPriceQuery`\> |
| `TokenLatestPrices` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`LatestPrice_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`LatestPrice_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`TokenLatestPricesQuery`\> |
| `TokenPrices` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`TokenPrice_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`TokenPrice_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`TokenPricesQuery`\> |
| `User` | (`variables`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `id`: `string`  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`UserQuery`\> |
| `Users` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`User_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`User_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`UsersQuery`\> |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraph.ts:57](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraph.ts#L57)

___

### pools

• `Private` `Optional` **pools**: `Promise`<[`Pool`](../interfaces/Pool.md)[]\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraph.ts:59](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraph.ts#L59)

___

### query

• `Private` **query**: [`GraphQLQuery`](../interfaces/GraphQLQuery.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraph.ts:62](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraph.ts#L62)

___

### skip

• **skip**: `number` = `0`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraph.ts:60](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraph.ts#L60)

## Methods

### all

▸ **all**(): `Promise`<[`Pool`](../interfaces/Pool.md)[]\>

#### Returns

`Promise`<[`Pool`](../interfaces/Pool.md)[]\>

#### Implementation of

Searchable.all

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraph.ts:169](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraph.ts#L169)

___

### block

▸ **block**(): `Promise`<`undefined` \| { `number`: `undefined` \| `number`  }\>

#### Returns

`Promise`<`undefined` \| { `number`: `undefined` \| `number`  }\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraph.ts:176](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraph.ts#L176)

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

[balancer-sdk/balancer-js/src/modules/data/pool/subgraph.ts:117](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraph.ts#L117)

___

### fetchDefault

▸ `Private` **fetchDefault**(): `Promise`<[`Pool`](../interfaces/Pool.md)[]\>

We need a list of all the pools, for calculating APRs (nested pools), and for SOR (path finding).
All the pools are fetched on page load and cachced for speedy lookups.

#### Returns

`Promise`<[`Pool`](../interfaces/Pool.md)[]\>

Promise resolving to pools list

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraph.ts:104](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraph.ts#L104)

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

[balancer-sdk/balancer-js/src/modules/data/pool/subgraph.ts:138](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraph.ts#L138)

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

[balancer-sdk/balancer-js/src/modules/data/pool/subgraph.ts:142](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraph.ts#L142)

___

### mapSubPoolToken

▸ `Private` **mapSubPoolToken**(`token`): `Object`

#### Parameters

| Name | Type |
| :------ | :------ |
| `token` | `SubgraphSubPoolToken` |

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `balance` | `string` |
| `decimals` | `number` |
| `isExemptFromYieldProtocolFee` | `undefined` \| ``true`` |
| `priceRate` | `string` |
| `symbol` | `string` |
| `token` | `undefined` \| [`SubPoolMeta`](../interfaces/SubPoolMeta.md) |
| `weight` | `undefined` \| ``null`` \| `string` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraph.ts:266](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraph.ts#L266)

___

### mapSubPools

▸ `Private` **mapSubPools**(`metadata`): [`SubPoolMeta`](../interfaces/SubPoolMeta.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `metadata` | `SubgraphSubPoolMeta` |

#### Returns

[`SubPoolMeta`](../interfaces/SubPoolMeta.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraph.ts:242](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraph.ts#L242)

___

### mapToken

▸ `Private` **mapToken**(`subgraphToken`): [`PoolToken`](../interfaces/PoolToken.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `subgraphToken` | `SubgraphPoolTokenFragment` |

#### Returns

[`PoolToken`](../interfaces/PoolToken.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraph.ts:229](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraph.ts#L229)

___

### mapType

▸ `Private` **mapType**(`subgraphPool`): [`Pool`](../interfaces/Pool.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `subgraphPool` | `SubgraphPoolFragment` |

#### Returns

[`Pool`](../interfaces/Pool.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/subgraph.ts:188](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraph.ts#L188)

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

[balancer-sdk/balancer-js/src/modules/data/pool/subgraph.ts:180](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/subgraph.ts#L180)
