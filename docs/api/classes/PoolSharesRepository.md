# Class: PoolSharesRepository

## Hierarchy

- `BalancerSubgraphRepository`<[`PoolShare`](../interfaces/PoolShare.md), [`PoolShareAttributes`](../enums/PoolShareAttributes.md)\>

  ↳ **`PoolSharesRepository`**

## Table of contents

### Constructors

- [constructor](PoolSharesRepository.md#constructor)

### Properties

- [blockHeight](PoolSharesRepository.md#blockheight)
- [chainId](PoolSharesRepository.md#chainid)
- [client](PoolSharesRepository.md#client)

### Methods

- [find](PoolSharesRepository.md#find)
- [findAllBy](PoolSharesRepository.md#findallby)
- [findBy](PoolSharesRepository.md#findby)
- [findByPool](PoolSharesRepository.md#findbypool)
- [findByUser](PoolSharesRepository.md#findbyuser)
- [get](PoolSharesRepository.md#get)
- [mapType](PoolSharesRepository.md#maptype)
- [query](PoolSharesRepository.md#query)

## Constructors

### constructor

• **new PoolSharesRepository**(`url`, `chainId`, `blockHeight?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |
| `chainId` | [`Network`](../enums/Network.md) |
| `blockHeight?` | () => `Promise`<`undefined` \| `number`\> |

#### Inherited from

BalancerSubgraphRepository<
  PoolShare,
  PoolShareAttributes
\>.constructor

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/balancer-subgraph-repository.ts:11](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/balancer-subgraph-repository.ts#L11)

## Properties

### blockHeight

• `Protected` `Optional` **blockHeight**: () => `Promise`<`undefined` \| `number`\>

#### Type declaration

▸ (): `Promise`<`undefined` \| `number`\>

##### Returns

`Promise`<`undefined` \| `number`\>

#### Inherited from

BalancerSubgraphRepository.blockHeight

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/balancer-subgraph-repository.ts:14](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/balancer-subgraph-repository.ts#L14)

___

### chainId

• `Protected` **chainId**: [`Network`](../enums/Network.md)

#### Inherited from

BalancerSubgraphRepository.chainId

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/balancer-subgraph-repository.ts:13](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/balancer-subgraph-repository.ts#L13)

___

### client

• `Protected` **client**: `Object`

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

#### Inherited from

BalancerSubgraphRepository.client

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/balancer-subgraph-repository.ts:9](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/balancer-subgraph-repository.ts#L9)

## Methods

### find

▸ **find**(`id`): `Promise`<`undefined` \| [`PoolShare`](../interfaces/PoolShare.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |

#### Returns

`Promise`<`undefined` \| [`PoolShare`](../interfaces/PoolShare.md)\>

#### Inherited from

BalancerSubgraphRepository.find

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts:16](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts#L16)

___

### findAllBy

▸ **findAllBy**(`attribute`, `value`, `first?`, `skip?`): `Promise`<[`PoolShare`](../interfaces/PoolShare.md)[]\>

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `attribute` | [`PoolShareAttributes`](../enums/PoolShareAttributes.md) | `undefined` |
| `value` | `string` | `undefined` |
| `first` | `number` | `1000` |
| `skip` | `number` | `0` |

#### Returns

`Promise`<[`PoolShare`](../interfaces/PoolShare.md)[]\>

#### Inherited from

BalancerSubgraphRepository.findAllBy

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts:24](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts#L24)

___

### findBy

▸ **findBy**(`attribute`, `value`): `Promise`<`undefined` \| [`PoolShare`](../interfaces/PoolShare.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `attribute` | [`PoolShareAttributes`](../enums/PoolShareAttributes.md) |
| `value` | `string` |

#### Returns

`Promise`<`undefined` \| [`PoolShare`](../interfaces/PoolShare.md)\>

#### Inherited from

BalancerSubgraphRepository.findBy

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts:20](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts#L20)

___

### findByPool

▸ **findByPool**(`poolId`, `first?`, `skip?`): `Promise`<[`PoolShare`](../interfaces/PoolShare.md)[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `poolId` | `string` |
| `first?` | `number` |
| `skip?` | `number` |

#### Returns

`Promise`<[`PoolShare`](../interfaces/PoolShare.md)[]\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool-shares/repository.ts:46](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool-shares/repository.ts#L46)

___

### findByUser

▸ **findByUser**(`userAddress`, `first?`, `skip?`): `Promise`<[`PoolShare`](../interfaces/PoolShare.md)[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `userAddress` | `string` |
| `first?` | `number` |
| `skip?` | `number` |

#### Returns

`Promise`<[`PoolShare`](../interfaces/PoolShare.md)[]\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool-shares/repository.ts:33](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool-shares/repository.ts#L33)

___

### get

▸ **get**(`args`): `Promise`<`undefined` \| [`PoolShare`](../interfaces/PoolShare.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | `any` |

#### Returns

`Promise`<`undefined` \| [`PoolShare`](../interfaces/PoolShare.md)\>

#### Inherited from

BalancerSubgraphRepository.get

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts:11](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/repository/abstract-subgraph-repository.ts#L11)

___

### mapType

▸ **mapType**(`subgraphPoolShare`): [`PoolShare`](../interfaces/PoolShare.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `subgraphPoolShare` | `SubgraphPoolShareFragment` |

#### Returns

[`PoolShare`](../interfaces/PoolShare.md)

#### Overrides

BalancerSubgraphRepository.mapType

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool-shares/repository.ts:24](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool-shares/repository.ts#L24)

___

### query

▸ **query**(`args`): `Promise`<[`PoolShare`](../interfaces/PoolShare.md)[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | `any` |

#### Returns

`Promise`<[`PoolShare`](../interfaces/PoolShare.md)[]\>

#### Overrides

BalancerSubgraphRepository.query

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool-shares/repository.ts:14](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool-shares/repository.ts#L14)
