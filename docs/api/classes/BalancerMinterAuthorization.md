# Class: BalancerMinterAuthorization

## Table of contents

### Constructors

- [constructor](BalancerMinterAuthorization.md#constructor)

### Methods

- [signSetMinterApproval](BalancerMinterAuthorization.md#signsetminterapproval)

## Constructors

### constructor

• `Private` **new BalancerMinterAuthorization**()

Cannot be constructed.

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/signatures.ts:181](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/signatures.ts#L181)

## Methods

### signSetMinterApproval

▸ `Static` **signSetMinterApproval**(`minterContract`, `minter`, `approval`, `user`, `deadline?`, `nonce?`): `Promise`<{ `deadline`: `BigNumber` ; `r`: `string` ; `s`: `string` ; `v`: `number`  }\>

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `minterContract` | `Contract` | `undefined` |
| `minter` | [`Account`](../modules.md#account) | `undefined` |
| `approval` | `boolean` | `undefined` |
| `user` | `Signer` & `TypedDataSigner` | `undefined` |
| `deadline` | `BigNumberish` | `MAX_DEADLINE` |
| `nonce?` | `BigNumberish` | `undefined` |

#### Returns

`Promise`<{ `deadline`: `BigNumber` ; `r`: `string` ; `s`: `string` ; `v`: `number`  }\>

#### Defined in

[balancer-sdk/balancer-js/src/lib/utils/signatures.ts:185](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/utils/signatures.ts#L185)
