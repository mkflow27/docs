# Class: SOR

## Hierarchy

- **`SOR`**

  ↳ [`Sor`](Sor-1.md)

## Table of contents

### Constructors

- [constructor](SOR.md#constructor)

### Properties

- [config](SOR.md#config)
- [defaultSwapOptions](SOR.md#defaultswapoptions)
- [getBestPaths](SOR.md#getbestpaths)
- [poolCacher](SOR.md#poolcacher)
- [processSwaps](SOR.md#processswaps)
- [provider](SOR.md#provider)
- [routeProposer](SOR.md#routeproposer)
- [swapCostCalculator](SOR.md#swapcostcalculator)
- [useBpt](SOR.md#usebpt)

### Methods

- [fetchPools](SOR.md#fetchpools)
- [getCostOfSwapInToken](SOR.md#getcostofswapintoken)
- [getPools](SOR.md#getpools)
- [getSwaps](SOR.md#getswaps)

## Constructors

### constructor

• **new SOR**(`provider`, `config`, `poolDataService`, `tokenPriceService`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `provider` | `Provider` | Provider. |
| `config` | `SorConfig` | Chain specific configuration for the SOR. |
| `poolDataService` | [`PoolDataService`](../interfaces/PoolDataService.md) | Generic service that fetches pool data from an external data source. |
| `tokenPriceService` | `TokenPriceService` | Generic service that fetches token prices from an external price feed. Used in calculating swap cost. |

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:285

## Properties

### config

• `Private` `Readonly` **config**: `any`

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:273

___

### defaultSwapOptions

• `Private` `Readonly` **defaultSwapOptions**: `any`

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:278

___

### getBestPaths

• `Private` **getBestPaths**: `any`

Find optimal routes for trade from given candidate paths

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:318

___

### poolCacher

• `Private` `Readonly` **poolCacher**: `any`

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:274

___

### processSwaps

• `Private` **processSwaps**: `any`

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:314

___

### provider

• **provider**: `Provider`

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:272

___

### routeProposer

• `Readonly` **routeProposer**: [`RouteProposer`](RouteProposer.md)

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:275

___

### swapCostCalculator

• `Readonly` **swapCostCalculator**: `SwapCostCalculator`

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:276

___

### useBpt

• `Private` **useBpt**: `any`

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:277

## Methods

### fetchPools

▸ **fetchPools**(): `Promise`<`boolean`\>

fetchPools Retrieves pools information and saves to internal pools cache.

#### Returns

`Promise`<`boolean`\>

True if pools fetched successfully, False if not.

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

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:304
