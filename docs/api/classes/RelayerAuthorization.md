# Class: RelayerAuthorization

## Table of contents

### Constructors

- [constructor](RelayerAuthorization.md#constructor)

### Methods

- [encodeCalldataAuthorization](RelayerAuthorization.md#encodecalldataauthorization)
- [signAuthorizationFor](RelayerAuthorization.md#signauthorizationfor)
- [signBatchSwapAuthorization](RelayerAuthorization.md#signbatchswapauthorization)
- [signExitAuthorization](RelayerAuthorization.md#signexitauthorization)
- [signJoinAuthorization](RelayerAuthorization.md#signjoinauthorization)
- [signSetRelayerApprovalAuthorization](RelayerAuthorization.md#signsetrelayerapprovalauthorization)
- [signSwapAuthorization](RelayerAuthorization.md#signswapauthorization)

## Constructors

### constructor

• `Private` **new RelayerAuthorization**()

Cannot be constructed.

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/signatures.ts:28](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/signatures.ts#L28)

## Methods

### encodeCalldataAuthorization

▸ `Static` **encodeCalldataAuthorization**(`calldata`, `deadline`, `signature`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `calldata` | `string` |
| `deadline` | `BigNumberish` |
| `signature` | `string` |

#### Returns

`string`

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/signatures.ts:32](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/signatures.ts#L32)

___

### signAuthorizationFor

▸ `Static` **signAuthorizationFor**(`type`, `validator`, `user`, `allowedSender`, `allowedCalldata`, `deadline?`, `nonce?`): `Promise`<`string`\>

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `type` | [`RelayerAction`](../enums/RelayerAction.md) | `undefined` |
| `validator` | `Contract` | `undefined` |
| `user` | `Signer` & `TypedDataSigner` | `undefined` |
| `allowedSender` | [`Account`](../modules.md#account) | `undefined` |
| `allowedCalldata` | `string` | `undefined` |
| `deadline` | `BigNumberish` | `MAX_DEADLINE` |
| `nonce?` | `BigNumberish` | `undefined` |

#### Returns

`Promise`<`string`\>

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/signatures.ts:135](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/signatures.ts#L135)

___

### signBatchSwapAuthorization

▸ `Static` **signBatchSwapAuthorization**(`validator`, `user`, `allowedSender`, `allowedCalldata`, `deadline?`, `nonce?`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `validator` | `Contract` |
| `user` | `Signer` & `TypedDataSigner` |
| `allowedSender` | [`Account`](../modules.md#account) |
| `allowedCalldata` | `string` |
| `deadline?` | `BigNumberish` |
| `nonce?` | `BigNumberish` |

#### Returns

`Promise`<`string`\>

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/signatures.ts:99](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/signatures.ts#L99)

___

### signExitAuthorization

▸ `Static` **signExitAuthorization**(`validator`, `user`, `allowedSender`, `allowedCalldata`, `deadline?`, `nonce?`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `validator` | `Contract` |
| `user` | `Signer` & `TypedDataSigner` |
| `allowedSender` | [`Account`](../modules.md#account) |
| `allowedCalldata` | `string` |
| `deadline?` | `BigNumberish` |
| `nonce?` | `BigNumberish` |

#### Returns

`Promise`<`string`\>

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/signatures.ts:63](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/signatures.ts#L63)

___

### signJoinAuthorization

▸ `Static` **signJoinAuthorization**(`validator`, `user`, `allowedSender`, `allowedCalldata`, `deadline?`, `nonce?`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `validator` | `Contract` |
| `user` | `Signer` & `TypedDataSigner` |
| `allowedSender` | [`Account`](../modules.md#account) |
| `allowedCalldata` | `string` |
| `deadline?` | `BigNumberish` |
| `nonce?` | `BigNumberish` |

#### Returns

`Promise`<`string`\>

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/signatures.ts:45](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/signatures.ts#L45)

___

### signSetRelayerApprovalAuthorization

▸ `Static` **signSetRelayerApprovalAuthorization**(`validator`, `user`, `allowedSender`, `allowedCalldata`, `deadline?`, `nonce?`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `validator` | `Contract` |
| `user` | `Signer` & `TypedDataSigner` |
| `allowedSender` | [`Account`](../modules.md#account) |
| `allowedCalldata` | `string` |
| `deadline?` | `BigNumberish` |
| `nonce?` | `BigNumberish` |

#### Returns

`Promise`<`string`\>

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/signatures.ts:117](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/signatures.ts#L117)

___

### signSwapAuthorization

▸ `Static` **signSwapAuthorization**(`validator`, `user`, `allowedSender`, `allowedCalldata`, `deadline?`, `nonce?`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `validator` | `Contract` |
| `user` | `Signer` & `TypedDataSigner` |
| `allowedSender` | [`Account`](../modules.md#account) |
| `allowedCalldata` | `string` |
| `deadline?` | `BigNumberish` |
| `nonce?` | `BigNumberish` |

#### Returns

`Promise`<`string`\>

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/signatures.ts:81](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/signatures.ts#L81)
