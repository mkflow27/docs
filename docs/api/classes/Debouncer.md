# Class: Debouncer<T, A\>

Aggregates attributes and exectutes a debounced call

**`Param`**

Function to debounce

**`Param`**

Debouncing waiting time [ms]

## Type parameters

| Name |
| :------ |
| `T` |
| `A` |

## Table of contents

### Constructors

- [constructor](Debouncer.md#constructor)

### Properties

- [fn](Debouncer.md#fn)
- [promisedCalls](Debouncer.md#promisedcalls)
- [promisedCount](Debouncer.md#promisedcount)
- [requestSet](Debouncer.md#requestset)
- [timeout](Debouncer.md#timeout)
- [wait](Debouncer.md#wait)

### Methods

- [debounceCancel](Debouncer.md#debouncecancel)
- [fetch](Debouncer.md#fetch)

## Constructors

### constructor

• **new Debouncer**<`T`, `A`\>(`fn`, `wait?`)

#### Type parameters

| Name |
| :------ |
| `T` |
| `A` |

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `fn` | (`attrs`: `A`[]) => `Promise`<`T`\> | `undefined` |
| `wait` | `number` | `200` |

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/debouncer.ts:38](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/debouncer.ts#L38)

## Properties

### fn

• `Private` **fn**: (`attrs`: `A`[]) => `Promise`<`T`\>

#### Type declaration

▸ (`attrs`): `Promise`<`T`\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `attrs` | `A`[] |

##### Returns

`Promise`<`T`\>

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/debouncer.ts:38](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/debouncer.ts#L38)

___

### promisedCalls

• **promisedCalls**: `Promised`<`T`\>[] = `[]`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/debouncer.ts:33](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/debouncer.ts#L33)

___

### promisedCount

• **promisedCount**: `number` = `0`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/debouncer.ts:34](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/debouncer.ts#L34)

___

### requestSet

• **requestSet**: `Set`<`A`\>

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/debouncer.ts:32](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/debouncer.ts#L32)

___

### timeout

• `Optional` **timeout**: `Timeout`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/debouncer.ts:35](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/debouncer.ts#L35)

___

### wait

• `Private` **wait**: `number` = `200`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/debouncer.ts:38](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/debouncer.ts#L38)

## Methods

### debounceCancel

▸ **debounceCancel**(): `void`

#### Returns

`void`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/debouncer.ts:36](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/debouncer.ts#L36)

___

### fetch

▸ **fetch**(`attr?`): `Promise`<`T`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `attr?` | `A` |

#### Returns

`Promise`<`T`\>

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/debouncer.ts:40](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/debouncer.ts#L40)
