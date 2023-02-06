# Class: RouteProposer

## Table of contents

### Constructors

- [constructor](RouteProposer.md#constructor)

### Properties

- [cache](RouteProposer.md#cache)
- [config](RouteProposer.md#config)

### Methods

- [getCandidatePaths](RouteProposer.md#getcandidatepaths)
- [getCandidatePathsFromDict](RouteProposer.md#getcandidatepathsfromdict)

## Constructors

### constructor

• **new RouteProposer**(`config`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `config` | `SorConfig` |

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:233

## Properties

### cache

• **cache**: `Record`<`string`, { `paths`: [`NewPath`](../interfaces/NewPath.md)[]  }\>

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:230

___

### config

• `Private` `Readonly` **config**: `any`

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:229

## Methods

### getCandidatePaths

▸ **getCandidatePaths**(`tokenIn`, `tokenOut`, `swapType`, `pools`, `swapOptions`): [`NewPath`](../interfaces/NewPath.md)[]

Given a list of pools and a desired input/output, returns a set of possible paths to route through

#### Parameters

| Name | Type |
| :------ | :------ |
| `tokenIn` | `string` |
| `tokenOut` | `string` |
| `swapType` | [`SwapTypes`](../enums/SwapTypes.md) |
| `pools` | [`SubgraphPoolBase`](../interfaces/SubgraphPoolBase.md)[] |
| `swapOptions` | [`SwapOptions`](../interfaces/SwapOptions.md) |

#### Returns

[`NewPath`](../interfaces/NewPath.md)[]

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:237

___

### getCandidatePathsFromDict

▸ **getCandidatePathsFromDict**(`tokenIn`, `tokenOut`, `swapType`, `poolsAllDict`, `maxPools`): [`NewPath`](../interfaces/NewPath.md)[]

Given a pool dictionary and a desired input/output, returns a set of possible paths to route through.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tokenIn` | `string` | Address of tokenIn |
| `tokenOut` | `string` | Address of tokenOut |
| `swapType` | [`SwapTypes`](../enums/SwapTypes.md) | SwapExactIn where the amount of tokens in (sent to the Pool) is known or SwapExactOut where the amount of tokens out (received from the Pool) is known. |
| `poolsAllDict` | [`PoolDictionary`](../interfaces/PoolDictionary.md) | Dictionary of pools. |
| `maxPools` | `number` | Maximum number of pools to hop through. |

#### Returns

[`NewPath`](../interfaces/NewPath.md)[]

Array of possible paths sorted by liquidity.

#### Defined in

balancer-sdk/balancer-js/node_modules/@balancer-labs/sor/dist/index.d.ts:247
