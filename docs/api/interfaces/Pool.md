# Interface: Pool

## Hierarchy

- **`Pool`**

  ↳ [`PoolWithMethods`](PoolWithMethods.md)

## Table of contents

### Properties

- [address](Pool.md#address)
- [amp](Pool.md#amp)
- [apr](Pool.md#apr)
- [boost](Pool.md#boost)
- [chainId](Pool.md#chainid)
- [createTime](Pool.md#createtime)
- [factory](Pool.md#factory)
- [feesSnapshot](Pool.md#feessnapshot)
- [id](Pool.md#id)
- [isNew](Pool.md#isnew)
- [liquidity](Pool.md#liquidity)
- [lowerTarget](Pool.md#lowertarget)
- [mainIndex](Pool.md#mainindex)
- [mainTokens](Pool.md#maintokens)
- [name](Pool.md#name)
- [onchain](Pool.md#onchain)
- [owner](Pool.md#owner)
- [poolType](Pool.md#pooltype)
- [poolTypeVersion](Pool.md#pooltypeversion)
- [priceRateProviders](Pool.md#pricerateproviders)
- [protocolSwapFeeCache](Pool.md#protocolswapfeecache)
- [protocolYieldFeeCache](Pool.md#protocolyieldfeecache)
- [swapEnabled](Pool.md#swapenabled)
- [swapFee](Pool.md#swapfee)
- [symbol](Pool.md#symbol)
- [tokenAddresses](Pool.md#tokenaddresses)
- [tokens](Pool.md#tokens)
- [tokensList](Pool.md#tokenslist)
- [totalLiquidity](Pool.md#totalliquidity)
- [totalShares](Pool.md#totalshares)
- [totalSwapFee](Pool.md#totalswapfee)
- [totalSwapVolume](Pool.md#totalswapvolume)
- [totalWeight](Pool.md#totalweight)
- [unwrappedTokens](Pool.md#unwrappedtokens)
- [upperTarget](Pool.md#uppertarget)
- [volumeSnapshot](Pool.md#volumesnapshot)
- [wrappedIndex](Pool.md#wrappedindex)
- [wrappedTokens](Pool.md#wrappedtokens)

## Properties

### address

• **address**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:273](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L273)

___

### amp

• `Optional` **amp**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:300](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L300)

___

### apr

• `Optional` **apr**: [`AprBreakdown`](AprBreakdown.md)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:303](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L303)

___

### boost

• `Optional` **boost**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:297](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L297)

___

### chainId

• **chainId**: `number`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:274](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L274)

___

### createTime

• `Optional` **createTime**: `number`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:290](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L290)

___

### factory

• `Optional` **factory**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:281](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L281)

___

### feesSnapshot

• `Optional` **feesSnapshot**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:296](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L296)

___

### id

• **id**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:271](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L271)

___

### isNew

• `Optional` **isNew**: `boolean`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:294](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L294)

___

### liquidity

• `Optional` **liquidity**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:304](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L304)

___

### lowerTarget

• **lowerTarget**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:306](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L306)

___

### mainIndex

• `Optional` **mainIndex**: `number`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:302](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L302)

___

### mainTokens

• `Optional` **mainTokens**: `string`[]

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:291](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L291)

___

### name

• **name**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:272](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L272)

___

### onchain

• `Optional` **onchain**: [`OnchainPoolData`](OnchainPoolData.md)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:289](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L289)

___

### owner

• `Optional` **owner**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:280](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L280)

___

### poolType

• **poolType**: [`PoolType`](../enums/PoolType.md)

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:275](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L275)

___

### poolTypeVersion

• **poolTypeVersion**: `number`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:276](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L276)

___

### priceRateProviders

• `Optional` **priceRateProviders**: [`PriceRateProvider`](PriceRateProvider.md)[]

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:308](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L308)

___

### protocolSwapFeeCache

• **protocolSwapFeeCache**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:279](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L279)

___

### protocolYieldFeeCache

• **protocolYieldFeeCache**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:278](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L278)

___

### swapEnabled

• **swapEnabled**: `boolean`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:299](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L299)

___

### swapFee

• **swapFee**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:277](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L277)

___

### symbol

• `Optional` **symbol**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:298](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L298)

___

### tokenAddresses

• `Optional` **tokenAddresses**: `string`[]

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:284](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L284)

___

### tokens

• **tokens**: [`PoolToken`](PoolToken.md)[]

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:282](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L282)

___

### tokensList

• **tokensList**: `string`[]

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:283](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L283)

___

### totalLiquidity

• **totalLiquidity**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:285](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L285)

___

### totalShares

• **totalShares**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:286](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L286)

___

### totalSwapFee

• `Optional` **totalSwapFee**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:287](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L287)

___

### totalSwapVolume

• `Optional` **totalSwapVolume**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:288](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L288)

___

### totalWeight

• **totalWeight**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:305](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L305)

___

### unwrappedTokens

• `Optional` **unwrappedTokens**: `string`[]

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:293](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L293)

___

### upperTarget

• **upperTarget**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:307](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L307)

___

### volumeSnapshot

• `Optional` **volumeSnapshot**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:295](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L295)

___

### wrappedIndex

• `Optional` **wrappedIndex**: `number`

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:301](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L301)

___

### wrappedTokens

• `Optional` **wrappedTokens**: `string`[]

#### Defined in

[balancer-sdk/balancer-js/src/types.ts:292](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/types.ts#L292)
