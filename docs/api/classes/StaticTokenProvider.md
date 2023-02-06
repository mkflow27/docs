# Class: StaticTokenProvider

## Implements

- [`Findable`](../interfaces/Findable.md)<[`Token`](../interfaces/Token.md), [`TokenAttribute`](../modules.md#tokenattribute)\>

## Table of contents

### Constructors

- [constructor](StaticTokenProvider.md#constructor)

### Properties

- [tokens](StaticTokenProvider.md#tokens)

### Methods

- [find](StaticTokenProvider.md#find)
- [findBy](StaticTokenProvider.md#findby)

## Constructors

### constructor

• **new StaticTokenProvider**(`tokens`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `tokens` | [`Token`](../interfaces/Token.md)[] |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token/static.ts:5](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token/static.ts#L5)

## Properties

### tokens

• `Private` **tokens**: [`Token`](../interfaces/Token.md)[]

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token/static.ts:5](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token/static.ts#L5)

## Methods

### find

▸ **find**(`address`): `Promise`<`undefined` \| [`Token`](../interfaces/Token.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |

#### Returns

`Promise`<`undefined` \| [`Token`](../interfaces/Token.md)\>

#### Implementation of

Findable.find

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token/static.ts:7](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token/static.ts#L7)

___

### findBy

▸ **findBy**(`attribute`, `value`): `Promise`<`undefined` \| [`Token`](../interfaces/Token.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `attribute` | [`TokenAttribute`](../modules.md#tokenattribute) |
| `value` | `string` |

#### Returns

`Promise`<`undefined` \| [`Token`](../interfaces/Token.md)\>

#### Implementation of

Findable.findBy

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token/static.ts:13](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token/static.ts#L13)
