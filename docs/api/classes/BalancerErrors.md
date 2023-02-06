# Class: BalancerErrors

## Table of contents

### Constructors

- [constructor](BalancerErrors.md#constructor)

### Methods

- [encodeError](BalancerErrors.md#encodeerror)
- [isBalancerError](BalancerErrors.md#isbalancererror)
- [isErrorCode](BalancerErrors.md#iserrorcode)
- [parseErrorCode](BalancerErrors.md#parseerrorcode)
- [tryParseErrorCode](BalancerErrors.md#tryparseerrorcode)

## Constructors

### constructor

• `Private` **new BalancerErrors**()

Cannot be constructed.

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/errors.ts:148](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/errors.ts#L148)

## Methods

### encodeError

▸ `Static` **encodeError**(`error`): `string`

Encodes an error string into the corresponding error code

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `error` | `string` | a Balancer error message string |

#### Returns

`string`

a Balancer error code of the form `BAL#000`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/errors.ts:200](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/errors.ts#L200)

___

### isBalancerError

▸ `Static` **isBalancerError**(`error`): `boolean`

Tests whether a string is a known Balancer error message

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `error` | `string` | a string to be checked verified as a Balancer error message |

#### Returns

`boolean`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/errors.ts:192](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/errors.ts#L192)

___

### isErrorCode

▸ `Static` **isErrorCode**(`error`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `error` | `string` |

#### Returns

`boolean`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/errors.ts:152](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/errors.ts#L152)

___

### parseErrorCode

▸ `Static` **parseErrorCode**(`error`): `string`

Decodes a Balancer error code into the corresponding reason

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `error` | `string` | a Balancer error code of the form `BAL#000` |

#### Returns

`string`

The decoded error reason

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/errors.ts:164](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/errors.ts#L164)

___

### tryParseErrorCode

▸ `Static` **tryParseErrorCode**(`error`): `string`

Decodes a Balancer error code into the corresponding reason

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `error` | `string` | a Balancer error code of the form `BAL#000` |

#### Returns

`string`

The decoded error reason if passed a valid error code, otherwise returns passed input

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/errors.ts:180](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/errors.ts#L180)
