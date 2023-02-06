# Class: BlockNumberRepository

## Implements

- [`Findable`](../interfaces/Findable.md)<`number`\>

## Table of contents

### Constructors

- [constructor](BlockNumberRepository.md#constructor)

### Properties

- [blocks](BlockNumberRepository.md#blocks)
- [endpoint](BlockNumberRepository.md#endpoint)

### Methods

- [find](BlockNumberRepository.md#find)
- [findBy](BlockNumberRepository.md#findby)

## Constructors

### constructor

• **new BlockNumberRepository**(`endpoint`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `endpoint` | `string` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/block-number/index.ts:40](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/block-number/index.ts#L40)

## Properties

### blocks

• **blocks**: `Object` = `{}`

#### Index signature

▪ [ts: `string`]: `Promise`<`number`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/block-number/index.ts:38](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/block-number/index.ts#L38)

___

### endpoint

• `Private` **endpoint**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/block-number/index.ts:40](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/block-number/index.ts#L40)

## Methods

### find

▸ **find**(`from`): `Promise`<`undefined` \| `number`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `from` | `string` |

#### Returns

`Promise`<`undefined` \| `number`\>

#### Implementation of

Findable.find

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/block-number/index.ts:42](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/block-number/index.ts#L42)

___

### findBy

▸ **findBy**(`attribute?`, `value?`): `Promise`<`undefined` \| `number`\>

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `attribute` | `string` | `''` |
| `value` | `string` | `''` |

#### Returns

`Promise`<`undefined` \| `number`\>

#### Implementation of

Findable.findBy

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/block-number/index.ts:56](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/block-number/index.ts#L56)
