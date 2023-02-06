# @balancer-labs/sdk

## Table of contents

### Namespaces

- [balEmissions](modules/balEmissions.md)

### Enumerations

- [BalancerErrorCode](enums/BalancerErrorCode.md)
- [ComposableStablePoolExitKind](enums/ComposableStablePoolExitKind.md)
- [ComposableStablePoolJoinKind](enums/ComposableStablePoolJoinKind.md)
- [GaugeShareAttributes](enums/GaugeShareAttributes.md)
- [Network](enums/Network.md)
- [PoolBalanceOpKind](enums/PoolBalanceOpKind.md)
- [PoolFilter](enums/PoolFilter.md)
- [PoolGaugesAttributes](enums/PoolGaugesAttributes.md)
- [PoolJoinExitAttributes](enums/PoolJoinExitAttributes.md)
- [PoolShareAttributes](enums/PoolShareAttributes.md)
- [PoolSpecialization](enums/PoolSpecialization.md)
- [PoolType](enums/PoolType.md)
- [RelayerAction](enums/RelayerAction.md)
- [StablePhantomPoolJoinKind](enums/StablePhantomPoolJoinKind.md)
- [StablePoolExitKind](enums/StablePoolExitKind.md)
- [StablePoolJoinKind](enums/StablePoolJoinKind.md)
- [SwapType](enums/SwapType.md)
- [SwapTypes](enums/SwapTypes.md)
- [UserBalanceOpKind](enums/UserBalanceOpKind.md)
- [WeightedPoolExitKind](enums/WeightedPoolExitKind.md)
- [WeightedPoolJoinKind](enums/WeightedPoolJoinKind.md)

### Classes

- [AaveHelpers](classes/AaveHelpers.md)
- [AaveRates](classes/AaveRates.md)
- [AssetHelpers](classes/AssetHelpers.md)
- [BalancerAPIArgsFormatter](classes/BalancerAPIArgsFormatter.md)
- [BalancerError](classes/BalancerError.md)
- [BalancerErrors](classes/BalancerErrors.md)
- [BalancerMinterAuthorization](classes/BalancerMinterAuthorization.md)
- [BalancerSDK](classes/BalancerSDK.md)
- [BlockNumberRepository](classes/BlockNumberRepository.md)
- [CoingeckoHistoricalPriceRepository](classes/CoingeckoHistoricalPriceRepository.md)
- [CoingeckoPriceRepository](classes/CoingeckoPriceRepository.md)
- [ComposableStablePoolEncoder](classes/ComposableStablePoolEncoder.md)
- [Data](classes/Data.md)
- [Debouncer](classes/Debouncer.md)
- [FeeCollectorRepository](classes/FeeCollectorRepository.md)
- [FeeDistributorRepository](classes/FeeDistributorRepository.md)
- [GaugeControllerMulticallRepository](classes/GaugeControllerMulticallRepository.md)
- [GaugeSharesRepository](classes/GaugeSharesRepository.md)
- [GraphQLArgsBuilder](classes/GraphQLArgsBuilder.md)
- [HistoricalPriceProvider](classes/HistoricalPriceProvider.md)
- [Liquidity](classes/Liquidity.md)
- [LiquidityGaugeSubgraphRPCProvider](classes/LiquidityGaugeSubgraphRPCProvider.md)
- [LiquidityGaugesMulticallRepository](classes/LiquidityGaugesMulticallRepository.md)
- [LiquidityGaugesSubgraphRepository](classes/LiquidityGaugesSubgraphRepository.md)
- [ManagedPoolEncoder](classes/ManagedPoolEncoder.md)
- [PoolGaugesRepository](classes/PoolGaugesRepository.md)
- [PoolJoinExitRepository](classes/PoolJoinExitRepository.md)
- [PoolSharesRepository](classes/PoolSharesRepository.md)
- [Pools](classes/Pools.md)
- [PoolsBalancerAPIRepository](classes/PoolsBalancerAPIRepository.md)
- [PoolsFallbackRepository](classes/PoolsFallbackRepository.md)
- [PoolsStaticRepository](classes/PoolsStaticRepository.md)
- [PoolsSubgraphOnChainRepository](classes/PoolsSubgraphOnChainRepository.md)
- [PoolsSubgraphRepository](classes/PoolsSubgraphRepository.md)
- [ProtocolFeesProvider](classes/ProtocolFeesProvider.md)
- [Relayer](classes/Relayer.md)
- [RelayerAuthorization](classes/RelayerAuthorization.md)
- [RouteProposer](classes/RouteProposer.md)
- [SOR](classes/SOR.md)
- [Sor](classes/Sor-1.md)
- [StablePoolEncoder](classes/StablePoolEncoder.md)
- [StaticTokenPriceProvider](classes/StaticTokenPriceProvider.md)
- [StaticTokenProvider](classes/StaticTokenProvider.md)
- [Subgraph](classes/Subgraph.md)
- [SubgraphArgsFormatter](classes/SubgraphArgsFormatter.md)
- [SubgraphPriceRepository](classes/SubgraphPriceRepository.md)
- [Swaps](classes/Swaps.md)
- [TokenPriceProvider](classes/TokenPriceProvider.md)
- [TokenYieldsRepository](classes/TokenYieldsRepository.md)
- [WeightedPoolEncoder](classes/WeightedPoolEncoder.md)

### Interfaces

- [AprBreakdown](interfaces/AprBreakdown.md)
- [AprFetcher](interfaces/AprFetcher.md)
- [BalancerDataRepositories](interfaces/BalancerDataRepositories.md)
- [BalancerNetworkConfig](interfaces/BalancerNetworkConfig.md)
- [BalancerSDKRoot](interfaces/BalancerSDKRoot.md)
- [BalancerSdkConfig](interfaces/BalancerSdkConfig.md)
- [BalancerSdkSorConfig](interfaces/BalancerSdkSorConfig.md)
- [BalancerTenderlyConfig](interfaces/BalancerTenderlyConfig.md)
- [BaseFeeDistributor](interfaces/BaseFeeDistributor.md)
- [BuildTransactionParameters](interfaces/BuildTransactionParameters.md)
- [ContractAddresses](interfaces/ContractAddresses.md)
- [EncodeBatchSwapInput](interfaces/EncodeBatchSwapInput.md)
- [EncodeExitPoolInput](interfaces/EncodeExitPoolInput.md)
- [EncodeJoinPoolInput](interfaces/EncodeJoinPoolInput.md)
- [EncodeUnwrapAaveStaticTokenInput](interfaces/EncodeUnwrapAaveStaticTokenInput.md)
- [EncodeWrapAaveDynamicTokenInput](interfaces/EncodeWrapAaveDynamicTokenInput.md)
- [ExitAndBatchSwapInput](interfaces/ExitAndBatchSwapInput.md)
- [FeeDistributorData](interfaces/FeeDistributorData.md)
- [FetchPoolsInput](interfaces/FetchPoolsInput.md)
- [FindRouteParameters](interfaces/FindRouteParameters.md)
- [Findable](interfaces/Findable.md)
- [GaugeShare](interfaces/GaugeShare.md)
- [GraphQLArgs](interfaces/GraphQLArgs.md)
- [GraphQLArgsFormatter](interfaces/GraphQLArgsFormatter.md)
- [GraphQLQuery](interfaces/GraphQLQuery.md)
- [IAaveRates](interfaces/IAaveRates.md)
- [LiquidityGauge](interfaces/LiquidityGauge.md)
- [NewPath](interfaces/NewPath.md)
- [OnchainPoolData](interfaces/OnchainPoolData.md)
- [OnchainTokenData](interfaces/OnchainTokenData.md)
- [Pool](interfaces/Pool.md)
- [PoolBPTValue](interfaces/PoolBPTValue.md)
- [PoolDataService](interfaces/PoolDataService.md)
- [PoolDictionary](interfaces/PoolDictionary.md)
- [PoolGauges](interfaces/PoolGauges.md)
- [PoolJoinExit](interfaces/PoolJoinExit.md)
- [PoolRepository](interfaces/PoolRepository.md)
- [PoolShare](interfaces/PoolShare.md)
- [PoolToken](interfaces/PoolToken.md)
- [PoolWithMethods](interfaces/PoolWithMethods.md)
- [PoolsFallbackRepositoryOptions](interfaces/PoolsFallbackRepositoryOptions.md)
- [PoolsRepositoryFetchOptions](interfaces/PoolsRepositoryFetchOptions.md)
- [PriceRateProvider](interfaces/PriceRateProvider.md)
- [ProtocolFees](interfaces/ProtocolFees.md)
- [QuerySimpleFlashSwapParameters](interfaces/QuerySimpleFlashSwapParameters.md)
- [QuerySimpleFlashSwapResponse](interfaces/QuerySimpleFlashSwapResponse.md)
- [QueryWithSorInput](interfaces/QueryWithSorInput.md)
- [QueryWithSorOutput](interfaces/QueryWithSorOutput.md)
- [RewardData](interfaces/RewardData.md)
- [Searchable](interfaces/Searchable.md)
- [SimpleFlashSwapParameters](interfaces/SimpleFlashSwapParameters.md)
- [SubPool](interfaces/SubPool.md)
- [SubPoolMeta](interfaces/SubPoolMeta.md)
- [SubgraphPoolBase](interfaces/SubgraphPoolBase.md)
- [SwapAttributes](interfaces/SwapAttributes.md)
- [SwapInfo](interfaces/SwapInfo.md)
- [SwapInput](interfaces/SwapInput.md)
- [SwapOptions](interfaces/SwapOptions.md)
- [SwapTransactionRequest](interfaces/SwapTransactionRequest.md)
- [SwapV2](interfaces/SwapV2.md)
- [Token](interfaces/Token.md)
- [TokenProvider](interfaces/TokenProvider.md)
- [TransactionData](interfaces/TransactionData.md)

### Type Aliases

- [Account](modules.md#account)
- [Address](modules.md#address)
- [BatchSwap](modules.md#batchswap)
- [BatchSwapStep](modules.md#batchswapstep)
- [Currency](modules.md#currency)
- [ExitPoolData](modules.md#exitpooldata)
- [ExitPoolRequest](modules.md#exitpoolrequest)
- [FundManagement](modules.md#fundmanagement)
- [GraphQLFilter](modules.md#graphqlfilter)
- [GraphQLFilterOperator](modules.md#graphqlfilteroperator)
- [HistoricalPrices](modules.md#historicalprices)
- [JoinPoolData](modules.md#joinpooldata)
- [JoinPoolRequest](modules.md#joinpoolrequest)
- [NamedPools](modules.md#namedpools)
- [OutputReference](modules.md#outputreference)
- [PoolAttribute](modules.md#poolattribute)
- [PoolBalanceOp](modules.md#poolbalanceop)
- [PoolReference](modules.md#poolreference)
- [Price](modules.md#price)
- [SingleSwap](modules.md#singleswap)
- [Swap](modules.md#swap)
- [TokenAttribute](modules.md#tokenattribute)
- [TokenPrices](modules.md#tokenprices)
- [UserBalanceOp](modules.md#userbalanceop)

### Variables

- [APR\_THRESHOLD](modules.md#apr-threshold)
- [SHALLOW\_COMPOSABLE\_STABLE\_BUFFER](modules.md#shallow-composable-stable-buffer)

### Functions

- [POOLS](modules.md#pools)
- [accountToAddress](modules.md#accounttoaddress)
- [addressMapIn](modules.md#addressmapin)
- [bn](modules.md#bn)
- [buildRelayerCalls](modules.md#buildrelayercalls)
- [canUseJoinExit](modules.md#canusejoinexit)
- [formatFixed](modules.md#formatfixed)
- [formatFromBigInt18](modules.md#formatfrombigint18)
- [formatSequence](modules.md#formatsequence)
- [getLimitsForSlippage](modules.md#getlimitsforslippage)
- [getPoolAddress](modules.md#getpooladdress)
- [getPoolNonce](modules.md#getpoolnonce)
- [getPoolSpecialization](modules.md#getpoolspecialization)
- [getTokenAddressesForSwap](modules.md#gettokenaddressesforswap)
- [insert](modules.md#insert)
- [isNormalizedWeights](modules.md#isnormalizedweights)
- [isSameAddress](modules.md#issameaddress)
- [parseFixed](modules.md#parsefixed)
- [parsePoolInfo](modules.md#parsepoolinfo)
- [parseToBigInt18](modules.md#parsetobigint18)
- [parseToPoolsDict](modules.md#parsetopoolsdict)
- [phantomStableBPTForTokensZeroPriceImpact](modules.md#phantomstablebptfortokenszeropriceimpact)
- [queryBatchSwapTokensIn](modules.md#querybatchswaptokensin)
- [queryBatchSwapTokensOut](modules.md#querybatchswaptokensout)
- [signPermit](modules.md#signpermit)
- [someJoinExit](modules.md#somejoinexit)
- [splitPoolId](modules.md#splitpoolid)
- [stableBPTForTokensZeroPriceImpact](modules.md#stablebptfortokenszeropriceimpact)
- [toNormalizedWeights](modules.md#tonormalizedweights)
- [tokenAddressForPricing](modules.md#tokenaddressforpricing)
- [tokensToTokenPrices](modules.md#tokenstotokenprices)
- [unwrapToken](modules.md#unwraptoken)
- [weightedBPTForTokensZeroPriceImpact](modules.md#weightedbptfortokenszeropriceimpact)

## Type Aliases

### Account

Ƭ **Account**: `string` \| `Signer` \| `Contract`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/signatures.ts:7](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/signatures.ts#L7)

___

### Address

Ƭ **Address**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:31](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L31)

___

### BatchSwap

Ƭ **BatchSwap**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `assets` | `string`[] |
| `deadline` | `BigNumberish` |
| `funds` | [`FundManagement`](modules.md#fundmanagement) |
| `kind` | [`SwapType`](enums/SwapType.md) |
| `limits` | `BigNumberish`[] |
| `outputReferences?` | { `index`: `BigNumberish` ; `key`: `BigNumberish`  }[] |
| `swaps` | [`BatchSwapStep`](modules.md#batchswapstep)[] |
| `value?` | `BigNumberish` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/types.ts:43](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/types.ts#L43)

___

### BatchSwapStep

Ƭ **BatchSwapStep**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `amount` | `string` |
| `assetInIndex` | `number` |
| `assetOutIndex` | `number` |
| `poolId` | `string` |
| `userData` | `string` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/types.ts:35](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/types.ts#L35)

___

### Currency

Ƭ **Currency**: ``"eth"`` \| ``"usd"``

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:194](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L194)

___

### ExitPoolData

Ƭ **ExitPoolData**: [`ExitPoolRequest`](modules.md#exitpoolrequest) & [`EncodeExitPoolInput`](interfaces/EncodeExitPoolInput.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/types.ts:76](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/types.ts#L76)

___

### ExitPoolRequest

Ƭ **ExitPoolRequest**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `assets` | `string`[] |
| `minAmountsOut` | `string`[] |
| `toInternalBalance` | `boolean` |
| `userData` | `string` |

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:147](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L147)

___

### FundManagement

Ƭ **FundManagement**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `fromInternalBalance` | `boolean` |
| `recipient` | `string` |
| `sender` | `string` |
| `toInternalBalance` | `boolean` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/types.ts:10](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/types.ts#L10)

___

### GraphQLFilter

Ƭ **GraphQLFilter**: { [operator in GraphQLFilterOperator]?: any }

#### Defined in

[balancer-sdk/balancer-js/src/lib/graphql/types.ts:9](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/graphql/types.ts#L9)

___

### GraphQLFilterOperator

Ƭ **GraphQLFilterOperator**: ``"gt"`` \| ``"lt"`` \| ``"eq"`` \| ``"in"`` \| ``"not_in"`` \| ``"contains"``

#### Defined in

[balancer-sdk/balancer-js/src/lib/graphql/types.ts:1](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/graphql/types.ts#L1)

___

### HistoricalPrices

Ƭ **HistoricalPrices**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `market_caps` | [[`number`, `number`]] |
| `prices` | [[`number`, `number`]] |
| `total_volumes` | [[`number`, `number`]] |

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:198](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L198)

___

### JoinPoolData

Ƭ **JoinPoolData**: [`JoinPoolRequest`](modules.md#joinpoolrequest) & [`EncodeJoinPoolInput`](interfaces/EncodeJoinPoolInput.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/types.ts:77](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/types.ts#L77)

___

### JoinPoolRequest

Ƭ **JoinPoolRequest**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `assets` | `string`[] |
| `fromInternalBalance` | `boolean` |
| `maxAmountsIn` | `BigNumberish`[] |
| `userData` | `string` |

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:138](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L138)

___

### NamedPools

Ƭ **NamedPools**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `bbAaveUSD` | { `v1`: `string` ; `v2`: `string`  } |
| `bbAaveUSD.v1` | `string` |
| `bbAaveUSD.v2` | `string` |
| `mai4` | { `mai4`: `string` ; `maiBbaUsd`: `string`  } |
| `mai4.mai4` | `string` |
| `mai4.maiBbaUsd` | `string` |
| `stMatic` | { `v1`: `string` ; `v2`: `string`  } |
| `stMatic.v1` | `string` |
| `stMatic.v2` | `string` |
| `staBAL` | `string` |
| `veBAL` | `string` |
| `xMatic` | { `v1`: `string` ; `v2`: `string`  } |
| `xMatic.v1` | `string` |
| `xMatic.v2` | `string` |

#### Defined in

[balancer-sdk/balancer-js/src/lib/constants/pools.ts:30](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/constants/pools.ts#L30)

___

### OutputReference

Ƭ **OutputReference**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `index` | `number` |
| `key` | `BigNumber` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/relayer/types.ts:11](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/relayer/types.ts#L11)

___

### PoolAttribute

Ƭ **PoolAttribute**: ``"id"`` \| ``"address"``

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/pool/types.ts:1](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/pool/types.ts#L1)

___

### PoolBalanceOp

Ƭ **PoolBalanceOp**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `amount` | `BigNumberish` |
| `kind` | [`PoolBalanceOpKind`](enums/PoolBalanceOpKind.md) |
| `poolId` | `string` |
| `token` | `string` |

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:177](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L177)

___

### PoolReference

Ƭ **PoolReference**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `id` | `string` |

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:125](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L125)

___

### Price

Ƭ **Price**: { [currency in Currency]?: string }

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:196](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L196)

___

### SingleSwap

Ƭ **SingleSwap**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `amount` | `BigNumberish` |
| `assetIn` | `string` |
| `assetOut` | `string` |
| `kind` | [`SwapType`](enums/SwapType.md) |
| `poolId` | `string` |
| `userData` | `string` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/types.ts:17](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/types.ts#L17)

___

### Swap

Ƭ **Swap**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `deadline` | `BigNumberish` |
| `funds` | [`FundManagement`](modules.md#fundmanagement) |
| `limit` | `BigNumberish` |
| `outputReference?` | `BigNumberish` |
| `request` | [`SingleSwap`](modules.md#singleswap) |
| `value?` | `BigNumberish` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/types.ts:26](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/types.ts#L26)

___

### TokenAttribute

Ƭ **TokenAttribute**: ``"address"`` \| ``"symbol"``

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token/types.ts:3](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token/types.ts#L3)

___

### TokenPrices

Ƭ **TokenPrices**: `Object`

#### Index signature

▪ [address: `string`]: [`Price`](modules.md#price)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:197](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L197)

___

### UserBalanceOp

Ƭ **UserBalanceOp**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `amount` | `BigNumberish` |
| `asset` | `string` |
| `kind` | [`UserBalanceOpKind`](enums/UserBalanceOpKind.md) |
| `recipient` | `string` |
| `sender` | `string` |

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:163](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L163)

## Variables

### APR\_THRESHOLD

• `Const` **APR\_THRESHOLD**: ``10000``

#### Defined in

[balancer-sdk/balancer-js/src/lib/constants/pools.ts:5](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/constants/pools.ts#L5)

___

### SHALLOW\_COMPOSABLE\_STABLE\_BUFFER

• `Const` **SHALLOW\_COMPOSABLE\_STABLE\_BUFFER**: ``1000000``

For proportional exits from ComposableStable pools the ExactBPTInForTokensOut
exit type was removed. Therefore we have to use BPTInForExactTokensOut which
makes proportional exits using a user's total BPT balance impossible. In
order to 'fix' this we need to subtract a little bit from the bptIn value
when calculating the ExactTokensOut. The variable below is that "little bit".

#### Defined in

[balancer-sdk/balancer-js/src/lib/constants/pools.ts:14](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/constants/pools.ts#L14)

## Functions

### POOLS

▸ **POOLS**(`networkId`): `Pools`

#### Parameters

| Name | Type |
| :------ | :------ |
| `networkId` | [`Network`](enums/Network.md) |

#### Returns

`Pools`

#### Defined in

[balancer-sdk/balancer-js/src/lib/constants/pools.ts:688](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/constants/pools.ts#L688)

___

### accountToAddress

▸ **accountToAddress**(`account`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `account` | [`Account`](modules.md#account) |

#### Returns

`Promise`<`string`\>

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/signatures.ts:9](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/signatures.ts#L9)

___

### addressMapIn

▸ **addressMapIn**(`address`, `chainId`): `string`

Maps testnet tokens, eg: on Göreli to a mainnet one.
Used to get the pricing information on networks not supported by a price feed.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `address` | `string` | Address on a testnet network |
| `chainId` | [`Network`](enums/Network.md) | - |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/tokens.ts:33](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/tokens.ts#L33)

___

### bn

▸ **bn**(`value`): `BigNumber`

Like parseEther but for numbers. Converts floating point to BigNumber using 18 decimals

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`BigNumber`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/math.ts:35](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/math.ts#L35)

___

### buildRelayerCalls

▸ **buildRelayerCalls**(`swapInfo`, `pools`, `user`, `relayerAddress`, `wrappedNativeAsset`, `slippage`, `authorisation`): `Object`

Given swapInfo from the SOR construct the Relayer multicall to execture swaps/joins/exits.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `swapInfo` | [`SwapInfo`](interfaces/SwapInfo.md) | Returned from SOR |
| `pools` | [`SubgraphPoolBase`](interfaces/SubgraphPoolBase.md)[] | Pool info from SOR |
| `user` | `string` | Address of user |
| `relayerAddress` | `string` | Address of Relayer (>=V4) |
| `wrappedNativeAsset` | `string` | Address of Native asset |
| `slippage` | `string` | [bps], eg: 1 === 0.01%, 100 === 1% |
| `authorisation` | `undefined` \| `string` | Encoded authorisation call. |

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `data` | `string` |
| `rawCalls` | `string`[] |
| `to` | `string` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/joinAndExit.ts:971](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/joinAndExit.ts#L971)

___

### canUseJoinExit

▸ **canUseJoinExit**(`swapType`, `tokenIn`, `tokenOut`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapType` | [`SwapTypes`](enums/SwapTypes.md) |
| `tokenIn` | `string` |
| `tokenOut` | `string` |

#### Returns

`boolean`

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/joinAndExit.ts:129](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/joinAndExit.ts#L129)

___

### formatFixed

▸ **formatFixed**(`value`, `decimals`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `BigNumber` |
| `decimals` | `BigNumberish` |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/math.ts:19](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/math.ts#L19)

___

### formatFromBigInt18

▸ **formatFromBigInt18**(`value`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `bigint` |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/math.ts:28](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/math.ts#L28)

___

### formatSequence

▸ **formatSequence**(`swapKind`, `sequence`, `tokenAddresses`): [`SwapV2`](interfaces/SwapV2.md)[]

Formats a sequence of swaps to the format expected by the Balance Vault.

**`Dev`**

Intermediate swaps' amounts are replaced with the sentinel value of zero
     and exact output sequences are reversed.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `swapKind` | [`SwapTypes`](enums/SwapTypes.md) | a SwapTypes enum for whether the swap has an exact input or exact output |
| `sequence` | `Swap`[] | a sequence of swaps which form a path from the input token to the output token |
| `tokenAddresses` | `string`[] | an array of all the token address which are involved in the batchSwap |

#### Returns

[`SwapV2`](interfaces/SwapV2.md)[]

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:355

___

### getLimitsForSlippage

▸ **getLimitsForSlippage**(`tokensIn`, `tokensOut`, `swapType`, `deltas`, `assets`, `slippage`): `BigNumberish`[]

Helper to create limits using a defined slippage amount.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tokensIn` | `string`[] | Array of token in addresses. |
| `tokensOut` | `string`[] | Array of token out addresses. |
| `swapType` | [`SwapType`](enums/SwapType.md) | Type of swap - SwapExactIn or SwapExactOut |
| `deltas` | `BigNumberish`[] | An array with the net Vault asset balance deltas. Positive amounts represent tokens (or ETH) sent to the Vault, and negative amounts represent tokens (or ETH) sent by the Vault. Each delta corresponds to the asset at the same index in the `assets` array. |
| `assets` | `string`[] | array contains the addresses of all assets involved in the swaps. |
| `slippage` | `BigNumberish` | Slippage to be applied. i.e. 5%=50000000000000000. |

#### Returns

`BigNumberish`[]

Returns an array (same length as assets) with limits applied for each asset.

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/helpers.ts:17](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/helpers.ts#L17)

___

### getPoolAddress

▸ **getPoolAddress**(`poolId`): `string`

Extracts a pool's address from its poolId

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `poolId` | `string` | a bytes32 string of the pool's ID |

#### Returns

`string`

the pool's address

#### Defined in

[balancer-sdk/balancer-js/src/pool-utils/poolId.ts:29](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-utils/poolId.ts#L29)

___

### getPoolNonce

▸ **getPoolNonce**(`poolId`): `BigNumber`

Extracts a pool's nonce from its poolId

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `poolId` | `string` | a bytes32 string of the pool's ID |

#### Returns

`BigNumber`

the pool's nonce

#### Defined in

[balancer-sdk/balancer-js/src/pool-utils/poolId.ts:54](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-utils/poolId.ts#L54)

___

### getPoolSpecialization

▸ **getPoolSpecialization**(`poolId`): [`PoolSpecialization`](enums/PoolSpecialization.md)

Extracts a pool's specialization from its poolId

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `poolId` | `string` | a bytes32 string of the pool's ID |

#### Returns

[`PoolSpecialization`](enums/PoolSpecialization.md)

the pool's specialization

#### Defined in

[balancer-sdk/balancer-js/src/pool-utils/poolId.ts:39](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-utils/poolId.ts#L39)

___

### getTokenAddressesForSwap

▸ **getTokenAddressesForSwap**(`swaps`): `string`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `swaps` | `Swap`[] |

#### Returns

`string`[]

an array of deduplicated token addresses used in the provided swaps

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:345

___

### insert

▸ **insert**<`T`\>(`arr`, `index`, `newItem`): `T`[]

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `arr` | `T`[] |
| `index` | `number` |
| `newItem` | `T` |

#### Returns

`T`[]

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/index.ts:16](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/index.ts#L16)

___

### isNormalizedWeights

▸ **isNormalizedWeights**(`weights`): `boolean`

Check whether a set of weights are normalized

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `weights` | `BigNumberish`[] | an array of potentially unnormalized weights |

#### Returns

`boolean`

a boolean of whether the weights are normalized

#### Defined in

[balancer-sdk/balancer-js/src/pool-weighted/normalizedWeights.ts:42](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-weighted/normalizedWeights.ts#L42)

___

### isSameAddress

▸ **isSameAddress**(`address1`, `address2`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `address1` | `string` |
| `address2` | `string` |

#### Returns

`boolean`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/index.ts:13](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/index.ts#L13)

___

### parseFixed

▸ **parseFixed**(`value`, `decimals?`): `BigNumber`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |
| `decimals?` | `BigNumberish` |

#### Returns

`BigNumber`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/math.ts:8](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/math.ts#L8)

___

### parsePoolInfo

▸ **parsePoolInfo**(`pool`, `wrappedNativeAsset?`): `Object`

Parse pool info into EVM amounts. Sorts by token order if wrappedNativeAsset param passed.

#### Parameters

| Name | Type |
| :------ | :------ |
| `pool` | [`Pool`](interfaces/Pool.md) |
| `wrappedNativeAsset?` | `string` |

#### Returns

`Object`

parsed pool info

| Name | Type |
| :------ | :------ |
| `bptIndex` | `number` |
| `parsedAmp` | `undefined` \| `string` |
| `parsedBalances` | `string`[] |
| `parsedBalancesWithoutBpt` | `string`[] |
| `parsedDecimals` | (`undefined` \| `string`)[] |
| `parsedPriceRates` | (`undefined` \| `string`)[] |
| `parsedSwapFee` | `string` |
| `parsedTokens` | `string`[] |
| `parsedTokensWithoutBpt` | `string`[] |
| `parsedTotalShares` | `string` |
| `parsedWeights` | (`undefined` \| `string`)[] |
| `scalingFactors` | `bigint`[] |
| `scalingFactorsWithoutBpt` | `bigint`[] |
| `upScaledBalances` | `string`[] |

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/poolHelper.ts:15](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/poolHelper.ts#L15)

___

### parseToBigInt18

▸ **parseToBigInt18**(`value`): `bigint`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`bigint`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/math.ts:24](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/math.ts#L24)

___

### parseToPoolsDict

▸ **parseToPoolsDict**(`pools`, `timestamp`): [`PoolDictionary`](interfaces/PoolDictionary.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `pools` | [`SubgraphPoolBase`](interfaces/SubgraphPoolBase.md)[] |
| `timestamp` | `number` |

#### Returns

[`PoolDictionary`](interfaces/PoolDictionary.md)

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:357

___

### phantomStableBPTForTokensZeroPriceImpact

▸ **phantomStableBPTForTokensZeroPriceImpact**(`allBalances`, `decimals`, `amounts`, `virtualBptSupply`, `amp`, `fee`, `rates`): `BigNumber$1`

#### Parameters

| Name | Type |
| :------ | :------ |
| `allBalances` | `BigNumberish`[] |
| `decimals` | `number`[] |
| `amounts` | `BigNumberish`[] |
| `virtualBptSupply` | `BigNumberish` |
| `amp` | `BigNumberish` |
| `fee` | `BigNumberish` |
| `rates` | `BigNumberish`[] |

#### Returns

`BigNumber$1`

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:326

___

### queryBatchSwapTokensIn

▸ **queryBatchSwapTokensIn**(`sor`, `vaultContract`, `tokensIn`, `amountsIn`, `tokenOut`): `Promise`<{ `amountTokenOut`: `string` ; `assets`: `string`[] ; `swaps`: [`SwapV2`](interfaces/SwapV2.md)[]  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `sor` | [`SOR`](classes/SOR.md) |
| `vaultContract` | `Contract` |
| `tokensIn` | `string`[] |
| `amountsIn` | `BigNumberish`[] |
| `tokenOut` | `string` |

#### Returns

`Promise`<{ `amountTokenOut`: `string` ; `assets`: `string`[] ; `swaps`: [`SwapV2`](interfaces/SwapV2.md)[]  }\>

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:331

___

### queryBatchSwapTokensOut

▸ **queryBatchSwapTokensOut**(`sor`, `vaultContract`, `tokenIn`, `amountsIn`, `tokensOut`): `Promise`<{ `amountTokensOut`: `string`[] ; `assets`: `string`[] ; `swaps`: [`SwapV2`](interfaces/SwapV2.md)[]  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `sor` | [`SOR`](classes/SOR.md) |
| `vaultContract` | `Contract` |
| `tokenIn` | `string` |
| `amountsIn` | `BigNumberish`[] |
| `tokensOut` | `string`[] |

#### Returns

`Promise`<{ `amountTokensOut`: `string`[] ; `assets`: `string`[] ; `swaps`: [`SwapV2`](interfaces/SwapV2.md)[]  }\>

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:336

___

### signPermit

▸ **signPermit**(`token`, `owner`, `spender`, `amount`, `deadline?`, `nonce?`): `Promise`<{ `deadline`: `BigNumber` ; `nonce`: `BigNumber` ; `r`: `string` ; `s`: `string` ; `v`: `number`  }\>

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `token` | `Contract` | `undefined` |
| `owner` | `Signer` & `TypedDataSigner` | `undefined` |
| `spender` | [`Account`](modules.md#account) | `undefined` |
| `amount` | `BigNumberish` | `undefined` |
| `deadline` | `BigNumberish` | `MAX_DEADLINE` |
| `nonce?` | `BigNumberish` | `undefined` |

#### Returns

`Promise`<{ `deadline`: `BigNumber` ; `nonce`: `BigNumber` ; `r`: `string` ; `s`: `string` ; `v`: `number`  }\>

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/permit.ts:8](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/permit.ts#L8)

___

### someJoinExit

▸ **someJoinExit**(`pools`, `swaps`, `assets`): `boolean`

Find if any of the swaps are join/exits. If yes these swaps should be routed via Relayer.

#### Parameters

| Name | Type |
| :------ | :------ |
| `pools` | [`SubgraphPoolBase`](interfaces/SubgraphPoolBase.md)[] |
| `swaps` | [`SwapV2`](interfaces/SwapV2.md)[] |
| `assets` | `string`[] |

#### Returns

`boolean`

#### Defined in

[balancer-sdk/balancer-js/src/modules/swaps/joinAndExit.ts:208](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/swaps/joinAndExit.ts#L208)

___

### splitPoolId

▸ **splitPoolId**(`poolId`): `Object`

Splits a poolId into its components, i.e. pool address, pool specialization and its nonce

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `poolId` | `string` | a bytes32 string of the pool's ID |

#### Returns

`Object`

an object with the decomposed poolId

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `nonce` | `BigNumber` |
| `specialization` | [`PoolSpecialization`](enums/PoolSpecialization.md) |

#### Defined in

[balancer-sdk/balancer-js/src/pool-utils/poolId.ts:10](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-utils/poolId.ts#L10)

___

### stableBPTForTokensZeroPriceImpact

▸ **stableBPTForTokensZeroPriceImpact**(`allBalances`, `decimals`, `amounts`, `bptTotalSupply`, `amp`): `BigNumber$1`

#### Parameters

| Name | Type |
| :------ | :------ |
| `allBalances` | `BigNumberish`[] |
| `decimals` | `number`[] |
| `amounts` | `BigNumberish`[] |
| `bptTotalSupply` | `BigNumberish` |
| `amp` | `BigNumberish` |

#### Returns

`BigNumber$1`

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:323

___

### toNormalizedWeights

▸ **toNormalizedWeights**(`weights`): `BigNumber`[]

Normalize an array of token weights to ensure they sum to `1e18`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `weights` | `BigNumber`[] | an array of token weights to be normalized |

#### Returns

`BigNumber`[]

an equivalent set of normalized weights

#### Defined in

[balancer-sdk/balancer-js/src/pool-weighted/normalizedWeights.ts:13](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/pool-weighted/normalizedWeights.ts#L13)

___

### tokenAddressForPricing

▸ **tokenAddressForPricing**(`address`, `chainId`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `chainId` | [`Network`](enums/Network.md) |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/tokens.ts:16](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/tokens.ts#L16)

___

### tokensToTokenPrices

▸ **tokensToTokenPrices**(`tokens`): [`TokenPrices`](modules.md#tokenprices)

#### Parameters

| Name | Type |
| :------ | :------ |
| `tokens` | [`Token`](interfaces/Token.md)[] |

#### Returns

[`TokenPrices`](modules.md#tokenprices)

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/tokens.ts:5](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/tokens.ts#L5)

___

### unwrapToken

▸ **unwrapToken**(`wrappedAddress`, `chainId`): `string`

Finds an underlying token address for a wrapped one

#### Parameters

| Name | Type |
| :------ | :------ |
| `wrappedAddress` | `string` |
| `chainId` | [`Network`](enums/Network.md) |

#### Returns

`string`

underlying token address

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/tokens.ts:45](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/tokens.ts#L45)

___

### weightedBPTForTokensZeroPriceImpact

▸ **weightedBPTForTokensZeroPriceImpact**(`balances`, `decimals`, `normalizedWeights`, `amounts`, `bptTotalSupply`): `BigNumber$1`

#### Parameters

| Name | Type |
| :------ | :------ |
| `balances` | `BigNumberish`[] |
| `decimals` | `number`[] |
| `normalizedWeights` | `BigNumberish`[] |
| `amounts` | `BigNumberish`[] |
| `bptTotalSupply` | `BigNumberish` |

#### Returns

`BigNumber$1`

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:321
