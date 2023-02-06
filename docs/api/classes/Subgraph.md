# Class: Subgraph

## Table of contents

### Constructors

- [constructor](Subgraph.md#constructor)

### Properties

- [client](Subgraph.md#client)
- [url](Subgraph.md#url)

### Methods

- [initClient](Subgraph.md#initclient)

## Constructors

### constructor

• **new Subgraph**(`config`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `config` | [`BalancerSdkConfig`](../interfaces/BalancerSdkConfig.md) |

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/subgraph.module.ts:11](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/subgraph.module.ts#L11)

## Properties

### client

• `Readonly` **client**: `Object`

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

[balancer-sdk/balancer-js/src/modules/subgraph/subgraph.module.ts:9](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/subgraph.module.ts#L9)

___

### url

• `Readonly` **url**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/subgraph/subgraph.module.ts:8](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/subgraph.module.ts#L8)

## Methods

### initClient

▸ `Private` **initClient**(): `Object`

#### Returns

`Object`

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

[balancer-sdk/balancer-js/src/modules/subgraph/subgraph.module.ts:16](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/subgraph/subgraph.module.ts#L16)
