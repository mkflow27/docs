# Interface: TokenProvider

## Table of contents

### Properties

- [find](TokenProvider.md#find)
- [findBy](TokenProvider.md#findby)

## Properties

### find

• **find**: (`address`: `string`) => `Promise`<`undefined` \| [`Token`](Token.md)\>

#### Type declaration

▸ (`address`): `Promise`<`undefined` \| [`Token`](Token.md)\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |

##### Returns

`Promise`<`undefined` \| [`Token`](Token.md)\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token/types.ts:6](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token/types.ts#L6)

___

### findBy

• **findBy**: (`attribute`: [`TokenAttribute`](../modules.md#tokenattribute), `value`: `string`) => `Promise`<`undefined` \| [`Token`](Token.md)\>

#### Type declaration

▸ (`attribute`, `value`): `Promise`<`undefined` \| [`Token`](Token.md)\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `attribute` | [`TokenAttribute`](../modules.md#tokenattribute) |
| `value` | `string` |

##### Returns

`Promise`<`undefined` \| [`Token`](Token.md)\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token/types.ts:7](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token/types.ts#L7)
