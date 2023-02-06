# Class: Sor

## Hierarchy

- [`SOR`](SOR.md)

  ↳ **`Sor`**

## Table of contents

### Constructors

- [constructor](Sor-1.md#constructor)

### Properties

- [provider](Sor-1.md#provider)
- [routeProposer](Sor-1.md#routeproposer)
- [swapCostCalculator](Sor-1.md#swapcostcalculator)

### Methods

- [fetchPools](Sor-1.md#fetchpools)
- [getCostOfSwapInToken](Sor-1.md#getcostofswapintoken)
- [getPools](Sor-1.md#getpools)
- [getSwaps](Sor-1.md#getswaps)
- [getPoolDataService](Sor-1.md#getpooldataservice)
- [getSorConfig](Sor-1.md#getsorconfig)
- [getSorNetworkConfig](Sor-1.md#getsornetworkconfig)
- [getTokenPriceService](Sor-1.md#gettokenpriceservice)

## Constructors

### constructor

• **new Sor**(`sdkConfig`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `sdkConfig` | [`BalancerSdkConfig`](../interfaces/BalancerSdkConfig.md) |

#### Overrides

[SOR](SOR.md).[constructor](SOR.md#constructor)

#### Defined in

[balancer-sdk/balancer-js/src/modules/sor/sor.module.ts:18](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sor/sor.module.ts#L18)

## Properties

### provider

• **provider**: `Provider`

#### Inherited from

[SOR](SOR.md).[provider](SOR.md#provider)

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:272

___

### routeProposer

• `Readonly` **routeProposer**: [`RouteProposer`](RouteProposer.md)

#### Inherited from

[SOR](SOR.md).[routeProposer](SOR.md#routeproposer)

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:275

___

### swapCostCalculator

• `Readonly` **swapCostCalculator**: `SwapCostCalculator`

#### Inherited from

[SOR](SOR.md).[swapCostCalculator](SOR.md#swapcostcalculator)

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:276

## Methods

### fetchPools

▸ **fetchPools**(): `Promise`<`boolean`\>

fetchPools Retrieves pools information and saves to internal pools cache.

#### Returns

`Promise`<`boolean`\>

True if pools fetched successfully, False if not.

#### Inherited from

[SOR](SOR.md).[fetchPools](SOR.md#fetchpools)

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:291

___

### getCostOfSwapInToken

▸ **getCostOfSwapInToken**(`outputToken`, `outputTokenDecimals`, `gasPrice`, `swapGas?`): `Promise`<`BigNumber`\>

getCostOfSwapInToken Calculates and saves price of a swap in outputToken denomination. Used to determine if extra swaps are cost effective.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `outputToken` | `string` | Address of outputToken. |
| `outputTokenDecimals` | `number` | Decimals of outputToken. |
| `gasPrice` | `BigNumber` | Gas price used to calculate cost. |
| `swapGas?` | `BigNumber` | Gas cost of a swap. Default=85000. |

#### Returns

`Promise`<`BigNumber`\>

Price of a swap in outputToken denomination.

#### Inherited from

[SOR](SOR.md).[getCostOfSwapInToken](SOR.md#getcostofswapintoken)

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:313

___

### getPools

▸ **getPools**(`useBpts?`): [`SubgraphPoolBase`](../interfaces/SubgraphPoolBase.md)[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `useBpts?` | `boolean` |

#### Returns

[`SubgraphPoolBase`](../interfaces/SubgraphPoolBase.md)[]

#### Inherited from

[SOR](SOR.md).[getPools](SOR.md#getpools)

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:286

___

### getSwaps

▸ **getSwaps**(`tokenIn`, `tokenOut`, `swapType`, `swapAmount`, `swapOptions?`, `useBpts?`): `Promise`<[`SwapInfo`](../interfaces/SwapInfo.md)\>

/**
 * getSwaps Retrieve information for best swap tokenIn>tokenOut.
 *

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tokenIn` | `string` | Address of tokenIn. * |
| `tokenOut` | `string` | Address of tokenOut. * |
| `swapType` | [`SwapTypes`](../enums/SwapTypes.md) | SwapExactIn where the amount of tokens in (sent to the Pool) is known or SwapExactOut where the amount of tokens out (received from the Pool) is known. * |
| `swapAmount` | `BigNumberish` | Either amountIn or amountOut depending on the `swapType` value. * |
| `swapOptions?` | `Partial`<[`SwapOptions`](../interfaces/SwapOptions.md)\> | * |
| `useBpts?` | `boolean` | Set to true to consider join/exit weighted pool paths (these will need formatted and submitted via Relayer) * |

#### Returns

`Promise`<[`SwapInfo`](../interfaces/SwapInfo.md)\>

Swap information including return amount and swaps structure to be submitted to Vault.

#### Inherited from

[SOR](SOR.md).[getSwaps](SOR.md#getswaps)

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:304

___

### getPoolDataService

▸ `Static` `Private` **getPoolDataService**(`network`, `sorConfig`, `provider`, `subgraphClient`): [`PoolDataService`](../interfaces/PoolDataService.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `network` | [`BalancerNetworkConfig`](../interfaces/BalancerNetworkConfig.md) |
| `sorConfig` | [`BalancerSdkSorConfig`](../interfaces/BalancerSdkSorConfig.md) |
| `provider` | `Provider` |
| `subgraphClient` | `Object` |
| `subgraphClient.AllPools` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`Pool_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`Pool_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`AllPoolsQuery`\> |
| `subgraphClient.Balancers` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`Balancer_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`Balancer_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`BalancersQuery`\> |
| `subgraphClient.JoinExits` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`JoinExit_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`JoinExit_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`JoinExitsQuery`\> |
| `subgraphClient.Pool` | (`variables`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `id`: `string`  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolQuery`\> |
| `subgraphClient.PoolHistoricalLiquidities` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`PoolHistoricalLiquidity_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`PoolHistoricalLiquidity_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolHistoricalLiquiditiesQuery`\> |
| `subgraphClient.PoolShare` | (`variables`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `id`: `string`  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolShareQuery`\> |
| `subgraphClient.PoolShares` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`PoolShare_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`PoolShare_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolSharesQuery`\> |
| `subgraphClient.PoolSnapshots` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`PoolSnapshot_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`PoolSnapshot_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolSnapshotsQuery`\> |
| `subgraphClient.Pools` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`Pool_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`Pool_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolsQuery`\> |
| `subgraphClient.TokenLatestPrice` | (`variables`: `Exact`<{ `id`: `string`  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`TokenLatestPriceQuery`\> |
| `subgraphClient.TokenLatestPrices` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`LatestPrice_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`LatestPrice_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`TokenLatestPricesQuery`\> |
| `subgraphClient.TokenPrices` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`TokenPrice_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`TokenPrice_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`TokenPricesQuery`\> |
| `subgraphClient.User` | (`variables`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `id`: `string`  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`UserQuery`\> |
| `subgraphClient.Users` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`User_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`User_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`UsersQuery`\> |

#### Returns

[`PoolDataService`](../interfaces/PoolDataService.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/sor/sor.module.ts:66](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sor/sor.module.ts#L66)

___

### getSorConfig

▸ `Static` `Private` **getSorConfig**(`config`): [`BalancerSdkSorConfig`](../interfaces/BalancerSdkSorConfig.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `config` | [`BalancerSdkConfig`](../interfaces/BalancerSdkConfig.md) |

#### Returns

[`BalancerSdkSorConfig`](../interfaces/BalancerSdkSorConfig.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/sor/sor.module.ts:44](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sor/sor.module.ts#L44)

___

### getSorNetworkConfig

▸ `Static` `Private` **getSorNetworkConfig**(`network`): `SorConfig`

#### Parameters

| Name | Type |
| :------ | :------ |
| `network` | [`BalancerNetworkConfig`](../interfaces/BalancerNetworkConfig.md) |

#### Returns

`SorConfig`

#### Defined in

[balancer-sdk/balancer-js/src/modules/sor/sor.module.ts:53](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sor/sor.module.ts#L53)

___

### getTokenPriceService

▸ `Static` `Private` **getTokenPriceService**(`network`, `sorConfig`, `subgraphClient`): `TokenPriceService`

#### Parameters

| Name | Type |
| :------ | :------ |
| `network` | [`BalancerNetworkConfig`](../interfaces/BalancerNetworkConfig.md) |
| `sorConfig` | [`BalancerSdkSorConfig`](../interfaces/BalancerSdkSorConfig.md) |
| `subgraphClient` | `Object` |
| `subgraphClient.AllPools` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`Pool_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`Pool_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`AllPoolsQuery`\> |
| `subgraphClient.Balancers` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`Balancer_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`Balancer_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`BalancersQuery`\> |
| `subgraphClient.JoinExits` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`JoinExit_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`JoinExit_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`JoinExitsQuery`\> |
| `subgraphClient.Pool` | (`variables`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `id`: `string`  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolQuery`\> |
| `subgraphClient.PoolHistoricalLiquidities` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`PoolHistoricalLiquidity_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`PoolHistoricalLiquidity_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolHistoricalLiquiditiesQuery`\> |
| `subgraphClient.PoolShare` | (`variables`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `id`: `string`  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolShareQuery`\> |
| `subgraphClient.PoolShares` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`PoolShare_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`PoolShare_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolSharesQuery`\> |
| `subgraphClient.PoolSnapshots` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`PoolSnapshot_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`PoolSnapshot_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolSnapshotsQuery`\> |
| `subgraphClient.Pools` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`Pool_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`Pool_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`PoolsQuery`\> |
| `subgraphClient.TokenLatestPrice` | (`variables`: `Exact`<{ `id`: `string`  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`TokenLatestPriceQuery`\> |
| `subgraphClient.TokenLatestPrices` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`LatestPrice_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`LatestPrice_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`TokenLatestPricesQuery`\> |
| `subgraphClient.TokenPrices` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`TokenPrice_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`TokenPrice_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`TokenPricesQuery`\> |
| `subgraphClient.User` | (`variables`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `id`: `string`  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`UserQuery`\> |
| `subgraphClient.Users` | (`variables?`: `Exact`<{ `block?`: `InputMaybe`<`Block_Height`\> ; `first?`: `InputMaybe`<`number`\> ; `orderBy?`: `InputMaybe`<`User_OrderBy`\> ; `orderDirection?`: `InputMaybe`<`OrderDirection`\> ; `skip?`: `InputMaybe`<`number`\> ; `where?`: `InputMaybe`<`User_Filter`\>  }\>, `requestHeaders?`: `HeadersInit`) => `Promise`<`UsersQuery`\> |

#### Returns

`TokenPriceService`

#### Defined in

[balancer-sdk/balancer-js/src/modules/sor/sor.module.ts:82](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/sor/sor.module.ts#L82)
