# Class: BalancerError

Balancer Error

## Hierarchy

- `Error`

  ↳ **`BalancerError`**

## Table of contents

### Constructors

- [constructor](BalancerError.md#constructor)

### Properties

- [code](BalancerError.md#code)
- [message](BalancerError.md#message)
- [name](BalancerError.md#name)
- [stack](BalancerError.md#stack)
- [prepareStackTrace](BalancerError.md#preparestacktrace)
- [stackTraceLimit](BalancerError.md#stacktracelimit)

### Methods

- [captureStackTrace](BalancerError.md#capturestacktrace)
- [getMessage](BalancerError.md#getmessage)

## Constructors

### constructor

• **new BalancerError**(`code`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `code` | [`BalancerErrorCode`](../enums/BalancerErrorCode.md) |

#### Overrides

Error.constructor

#### Defined in

[balancer-sdk/balancer-js/src/balancerErrors.ts:34](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/balancerErrors.ts#L34)

## Properties

### code

• **code**: [`BalancerErrorCode`](../enums/BalancerErrorCode.md)

#### Defined in

[balancer-sdk/balancer-js/src/balancerErrors.ts:34](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/balancerErrors.ts#L34)

___

### message

• **message**: `string`

#### Inherited from

Error.message

#### Defined in

docs/node_modules/typescript/lib/lib.es5.d.ts:1054

___

### name

• **name**: `string`

#### Inherited from

Error.name

#### Defined in

docs/node_modules/typescript/lib/lib.es5.d.ts:1053

___

### stack

• `Optional` **stack**: `string`

#### Inherited from

Error.stack

#### Defined in

docs/node_modules/typescript/lib/lib.es5.d.ts:1055

___

### prepareStackTrace

▪ `Static` `Optional` **prepareStackTrace**: (`err`: `Error`, `stackTraces`: `CallSite`[]) => `any`

#### Type declaration

▸ (`err`, `stackTraces`): `any`

Optional override for formatting stack traces

**`See`**

https://v8.dev/docs/stack-trace-api#customizing-stack-traces

##### Parameters

| Name | Type |
| :------ | :------ |
| `err` | `Error` |
| `stackTraces` | `CallSite`[] |

##### Returns

`any`

#### Inherited from

Error.prepareStackTrace

#### Defined in

balancer-sdk/balancer-js/node_modules/@types/node/globals.d.ts:11

___

### stackTraceLimit

▪ `Static` **stackTraceLimit**: `number`

#### Inherited from

Error.stackTraceLimit

#### Defined in

balancer-sdk/balancer-js/node_modules/@types/node/globals.d.ts:13

## Methods

### captureStackTrace

▸ `Static` **captureStackTrace**(`targetObject`, `constructorOpt?`): `void`

Create .stack property on a target object

#### Parameters

| Name | Type |
| :------ | :------ |
| `targetObject` | `object` |
| `constructorOpt?` | `Function` |

#### Returns

`void`

#### Inherited from

Error.captureStackTrace

#### Defined in

balancer-sdk/balancer-js/node_modules/@types/node/globals.d.ts:4

___

### getMessage

▸ `Static` **getMessage**(`code`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `code` | [`BalancerErrorCode`](../enums/BalancerErrorCode.md) |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/balancerErrors.ts:39](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/balancerErrors.ts#L39)
