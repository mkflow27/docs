# Interface: PoolWithMethods

Pool use-cases / controller layer

## Hierarchy

- [`Pool`](Pool.md)

- `ParamsBuilder`

  ↳ **`PoolWithMethods`**

## Table of contents

### Properties

- [address](PoolWithMethods.md#address)
- [amp](PoolWithMethods.md#amp)
- [apr](PoolWithMethods.md#apr)
- [boost](PoolWithMethods.md#boost)
- [buildExitExactBPTIn](PoolWithMethods.md#buildexitexactbptin)
- [buildExitExactTokensOut](PoolWithMethods.md#buildexitexacttokensout)
- [buildJoin](PoolWithMethods.md#buildjoin)
- [calcPriceImpact](PoolWithMethods.md#calcpriceimpact)
- [calcSpotPrice](PoolWithMethods.md#calcspotprice)
- [chainId](PoolWithMethods.md#chainid)
- [createTime](PoolWithMethods.md#createtime)
- [factory](PoolWithMethods.md#factory)
- [feesSnapshot](PoolWithMethods.md#feessnapshot)
- [id](PoolWithMethods.md#id)
- [isNew](PoolWithMethods.md#isnew)
- [liquidity](PoolWithMethods.md#liquidity)
- [lowerTarget](PoolWithMethods.md#lowertarget)
- [mainIndex](PoolWithMethods.md#mainindex)
- [mainTokens](PoolWithMethods.md#maintokens)
- [name](PoolWithMethods.md#name)
- [onchain](PoolWithMethods.md#onchain)
- [owner](PoolWithMethods.md#owner)
- [poolType](PoolWithMethods.md#pooltype)
- [poolTypeVersion](PoolWithMethods.md#pooltypeversion)
- [priceRateProviders](PoolWithMethods.md#pricerateproviders)
- [protocolSwapFeeCache](PoolWithMethods.md#protocolswapfeecache)
- [protocolYieldFeeCache](PoolWithMethods.md#protocolyieldfeecache)
- [swapEnabled](PoolWithMethods.md#swapenabled)
- [swapFee](PoolWithMethods.md#swapfee)
- [symbol](PoolWithMethods.md#symbol)
- [tokenAddresses](PoolWithMethods.md#tokenaddresses)
- [tokens](PoolWithMethods.md#tokens)
- [tokensList](PoolWithMethods.md#tokenslist)
- [totalLiquidity](PoolWithMethods.md#totalliquidity)
- [totalShares](PoolWithMethods.md#totalshares)
- [totalSwapFee](PoolWithMethods.md#totalswapfee)
- [totalSwapVolume](PoolWithMethods.md#totalswapvolume)
- [totalWeight](PoolWithMethods.md#totalweight)
- [unwrappedTokens](PoolWithMethods.md#unwrappedtokens)
- [upperTarget](PoolWithMethods.md#uppertarget)
- [volumeSnapshot](PoolWithMethods.md#volumesnapshot)
- [wrappedIndex](PoolWithMethods.md#wrappedindex)
- [wrappedTokens](PoolWithMethods.md#wrappedtokens)

### Methods

- [buildQueryExitExactOut](PoolWithMethods.md#buildqueryexitexactout)
- [buildQueryExitProportionally](PoolWithMethods.md#buildqueryexitproportionally)
- [buildQueryExitToSingleToken](PoolWithMethods.md#buildqueryexittosingletoken)
- [buildQueryJoinExactIn](PoolWithMethods.md#buildqueryjoinexactin)
- [buildQueryJoinExactOut](PoolWithMethods.md#buildqueryjoinexactout)

## Properties

### address

• **address**: `string`

#### Inherited from

[Pool](Pool.md).[address](Pool.md#address)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:273](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L273)

___

### amp

• `Optional` **amp**: `string`

#### Inherited from

[Pool](Pool.md).[amp](Pool.md#amp)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:300](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L300)

___

### apr

• `Optional` **apr**: [`AprBreakdown`](AprBreakdown.md)

#### Inherited from

[Pool](Pool.md).[apr](Pool.md#apr)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:303](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L303)

___

### boost

• `Optional` **boost**: `string`

#### Inherited from

[Pool](Pool.md).[boost](Pool.md#boost)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:297](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L297)

___

### buildExitExactBPTIn

• **buildExitExactBPTIn**: (`exiter`: `string`, `bptIn`: `string`, `slippage`: `string`, `shouldUnwrapNativeAsset?`: `boolean`, `singleTokenMaxOut?`: `string`) => `ExitExactBPTInAttributes`

#### Type declaration

▸ (`exiter`, `bptIn`, `slippage`, `shouldUnwrapNativeAsset?`, `singleTokenMaxOut?`): `ExitExactBPTInAttributes`

##### Parameters

| Name | Type |
| :------ | :------ |
| `exiter` | `string` |
| `bptIn` | `string` |
| `slippage` | `string` |
| `shouldUnwrapNativeAsset?` | `boolean` |
| `singleTokenMaxOut?` | `string` |

##### Returns

`ExitExactBPTInAttributes`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:333](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L333)

___

### buildExitExactTokensOut

• **buildExitExactTokensOut**: (`exiter`: `string`, `tokensOut`: `string`[], `amountsOut`: `string`[], `slippage`: `string`) => `ExitExactTokensOutAttributes`

#### Type declaration

▸ (`exiter`, `tokensOut`, `amountsOut`, `slippage`): `ExitExactTokensOutAttributes`

##### Parameters

| Name | Type |
| :------ | :------ |
| `exiter` | `string` |
| `tokensOut` | `string`[] |
| `amountsOut` | `string`[] |
| `slippage` | `string` |

##### Returns

`ExitExactTokensOutAttributes`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:340](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L340)

___

### buildJoin

• **buildJoin**: (`joiner`: `string`, `tokensIn`: `string`[], `amountsIn`: `string`[], `slippage`: `string`) => `JoinPoolAttributes`

#### Type declaration

▸ (`joiner`, `tokensIn`, `amountsIn`, `slippage`): `JoinPoolAttributes`

##### Parameters

| Name | Type |
| :------ | :------ |
| `joiner` | `string` |
| `tokensIn` | `string`[] |
| `amountsIn` | `string`[] |
| `slippage` | `string` |

##### Returns

`JoinPoolAttributes`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:322](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L322)

___

### calcPriceImpact

• **calcPriceImpact**: (`amountsIn`: `string`[], `minBPTOut`: `string`, `isJoin`: `boolean`) => `Promise`<`string`\>

#### Type declaration

▸ (`amountsIn`, `minBPTOut`, `isJoin`): `Promise`<`string`\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `amountsIn` | `string`[] |
| `minBPTOut` | `string` |
| `isJoin` | `boolean` |

##### Returns

`Promise`<`string`\>

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:328](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L328)

___

### calcSpotPrice

• **calcSpotPrice**: (`tokenIn`: `string`, `tokenOut`: `string`) => `string`

#### Type declaration

▸ (`tokenIn`, `tokenOut`): `string`

##### Parameters

| Name | Type |
| :------ | :------ |
| `tokenIn` | `string` |
| `tokenOut` | `string` |

##### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:346](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L346)

___

### chainId

• **chainId**: `number`

#### Inherited from

[Pool](Pool.md).[chainId](Pool.md#chainid)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:274](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L274)

___

### createTime

• `Optional` **createTime**: `number`

#### Inherited from

[Pool](Pool.md).[createTime](Pool.md#createtime)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:290](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L290)

___

### factory

• `Optional` **factory**: `string`

#### Inherited from

[Pool](Pool.md).[factory](Pool.md#factory)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:281](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L281)

___

### feesSnapshot

• `Optional` **feesSnapshot**: `string`

#### Inherited from

[Pool](Pool.md).[feesSnapshot](Pool.md#feessnapshot)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:296](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L296)

___

### id

• **id**: `string`

#### Inherited from

[Pool](Pool.md).[id](Pool.md#id)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:271](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L271)

___

### isNew

• `Optional` **isNew**: `boolean`

#### Inherited from

[Pool](Pool.md).[isNew](Pool.md#isnew)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:294](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L294)

___

### liquidity

• `Optional` **liquidity**: `string`

#### Inherited from

[Pool](Pool.md).[liquidity](Pool.md#liquidity)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:304](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L304)

___

### lowerTarget

• **lowerTarget**: `string`

#### Inherited from

[Pool](Pool.md).[lowerTarget](Pool.md#lowertarget)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:306](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L306)

___

### mainIndex

• `Optional` **mainIndex**: `number`

#### Inherited from

[Pool](Pool.md).[mainIndex](Pool.md#mainindex)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:302](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L302)

___

### mainTokens

• `Optional` **mainTokens**: `string`[]

#### Inherited from

[Pool](Pool.md).[mainTokens](Pool.md#maintokens)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:291](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L291)

___

### name

• **name**: `string`

#### Inherited from

[Pool](Pool.md).[name](Pool.md#name)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:272](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L272)

___

### onchain

• `Optional` **onchain**: [`OnchainPoolData`](OnchainPoolData.md)

#### Inherited from

[Pool](Pool.md).[onchain](Pool.md#onchain)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:289](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L289)

___

### owner

• `Optional` **owner**: `string`

#### Inherited from

[Pool](Pool.md).[owner](Pool.md#owner)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:280](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L280)

___

### poolType

• **poolType**: [`PoolType`](../enums/PoolType.md)

#### Inherited from

[Pool](Pool.md).[poolType](Pool.md#pooltype)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:275](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L275)

___

### poolTypeVersion

• **poolTypeVersion**: `number`

#### Inherited from

[Pool](Pool.md).[poolTypeVersion](Pool.md#pooltypeversion)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:276](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L276)

___

### priceRateProviders

• `Optional` **priceRateProviders**: [`PriceRateProvider`](PriceRateProvider.md)[]

#### Inherited from

[Pool](Pool.md).[priceRateProviders](Pool.md#pricerateproviders)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:308](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L308)

___

### protocolSwapFeeCache

• **protocolSwapFeeCache**: `string`

#### Inherited from

[Pool](Pool.md).[protocolSwapFeeCache](Pool.md#protocolswapfeecache)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:279](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L279)

___

### protocolYieldFeeCache

• **protocolYieldFeeCache**: `string`

#### Inherited from

[Pool](Pool.md).[protocolYieldFeeCache](Pool.md#protocolyieldfeecache)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:278](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L278)

___

### swapEnabled

• **swapEnabled**: `boolean`

#### Inherited from

[Pool](Pool.md).[swapEnabled](Pool.md#swapenabled)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:299](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L299)

___

### swapFee

• **swapFee**: `string`

#### Inherited from

[Pool](Pool.md).[swapFee](Pool.md#swapfee)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:277](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L277)

___

### symbol

• `Optional` **symbol**: `string`

#### Inherited from

[Pool](Pool.md).[symbol](Pool.md#symbol)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:298](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L298)

___

### tokenAddresses

• `Optional` **tokenAddresses**: `string`[]

#### Inherited from

[Pool](Pool.md).[tokenAddresses](Pool.md#tokenaddresses)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:284](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L284)

___

### tokens

• **tokens**: [`PoolToken`](PoolToken.md)[]

#### Inherited from

[Pool](Pool.md).[tokens](Pool.md#tokens)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:282](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L282)

___

### tokensList

• **tokensList**: `string`[]

#### Inherited from

[Pool](Pool.md).[tokensList](Pool.md#tokenslist)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:283](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L283)

___

### totalLiquidity

• **totalLiquidity**: `string`

#### Inherited from

[Pool](Pool.md).[totalLiquidity](Pool.md#totalliquidity)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:285](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L285)

___

### totalShares

• **totalShares**: `string`

#### Inherited from

[Pool](Pool.md).[totalShares](Pool.md#totalshares)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:286](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L286)

___

### totalSwapFee

• `Optional` **totalSwapFee**: `string`

#### Inherited from

[Pool](Pool.md).[totalSwapFee](Pool.md#totalswapfee)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:287](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L287)

___

### totalSwapVolume

• `Optional` **totalSwapVolume**: `string`

#### Inherited from

[Pool](Pool.md).[totalSwapVolume](Pool.md#totalswapvolume)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:288](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L288)

___

### totalWeight

• **totalWeight**: `string`

#### Inherited from

[Pool](Pool.md).[totalWeight](Pool.md#totalweight)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:305](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L305)

___

### unwrappedTokens

• `Optional` **unwrappedTokens**: `string`[]

#### Inherited from

[Pool](Pool.md).[unwrappedTokens](Pool.md#unwrappedtokens)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:293](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L293)

___

### upperTarget

• **upperTarget**: `string`

#### Inherited from

[Pool](Pool.md).[upperTarget](Pool.md#uppertarget)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:307](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L307)

___

### volumeSnapshot

• `Optional` **volumeSnapshot**: `string`

#### Inherited from

[Pool](Pool.md).[volumeSnapshot](Pool.md#volumesnapshot)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:295](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L295)

___

### wrappedIndex

• `Optional` **wrappedIndex**: `number`

#### Inherited from

[Pool](Pool.md).[wrappedIndex](Pool.md#wrappedindex)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:301](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L301)

___

### wrappedTokens

• `Optional` **wrappedTokens**: `string`[]

#### Inherited from

[Pool](Pool.md).[wrappedTokens](Pool.md#wrappedtokens)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:292](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L292)

## Methods

### buildQueryExitExactOut

▸ **buildQueryExitExactOut**(`params`): `queryExitParams`

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | `ExitExactOutParams` |

#### Returns

`queryExitParams`

#### Inherited from

Queries.ParamsBuilder.buildQueryExitExactOut

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/queries/types.ts:31](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/queries/types.ts#L31)

___

### buildQueryExitProportionally

▸ **buildQueryExitProportionally**(`params`): `queryExitParams`

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | `ExitProportionallyParams` |

#### Returns

`queryExitParams`

#### Inherited from

Queries.ParamsBuilder.buildQueryExitProportionally

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/queries/types.ts:28](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/queries/types.ts#L28)

___

### buildQueryExitToSingleToken

▸ **buildQueryExitToSingleToken**(`params`): `queryExitParams`

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | `ExitToSingleTokenParams` |

#### Returns

`queryExitParams`

#### Inherited from

Queries.ParamsBuilder.buildQueryExitToSingleToken

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/queries/types.ts:27](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/queries/types.ts#L27)

___

### buildQueryJoinExactIn

▸ **buildQueryJoinExactIn**(`params`): `queryJoinParams`

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | `JoinExactInParams` |

#### Returns

`queryJoinParams`

#### Inherited from

Queries.ParamsBuilder.buildQueryJoinExactIn

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/queries/types.ts:25](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/queries/types.ts#L25)

___

### buildQueryJoinExactOut

▸ **buildQueryJoinExactOut**(`params`): `queryJoinParams`

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | `JoinExactOutParams` |

#### Returns

`queryJoinParams`

#### Inherited from

Queries.ParamsBuilder.buildQueryJoinExactOut

#### Defined in

[balancer-sdk/balancer-js/src/modules/pools/queries/types.ts:26](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/pools/queries/types.ts#L26)
