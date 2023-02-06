# Class: FeeDistributorRepository

## Implements

- [`BaseFeeDistributor`](../interfaces/BaseFeeDistributor.md)

## Table of contents

### Constructors

- [constructor](FeeDistributorRepository.md#constructor)

### Properties

- [balAddress](FeeDistributorRepository.md#baladdress)
- [bbAUsdAddress](FeeDistributorRepository.md#bbausdaddress)
- [data](FeeDistributorRepository.md#data)
- [feeDistributorAddress](FeeDistributorRepository.md#feedistributoraddress)
- [multicall](FeeDistributorRepository.md#multicall)
- [veBalAddress](FeeDistributorRepository.md#vebaladdress)

### Methods

- [fetch](FeeDistributorRepository.md#fetch)
- [getPreviousWeek](FeeDistributorRepository.md#getpreviousweek)
- [multicallData](FeeDistributorRepository.md#multicalldata)

## Constructors

### constructor

• **new FeeDistributorRepository**(`multicallAddress`, `feeDistributorAddress`, `balAddress`, `veBalAddress`, `bbAUsdAddress`, `provider`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `multicallAddress` | `string` |
| `feeDistributorAddress` | `string` |
| `balAddress` | `string` |
| `veBalAddress` | `string` |
| `bbAUsdAddress` | `string` |
| `provider` | `Provider` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/fee-distributor/repository.ts:36](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/fee-distributor/repository.ts#L36)

## Properties

### balAddress

• `Private` **balAddress**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/fee-distributor/repository.ts:39](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/fee-distributor/repository.ts#L39)

___

### bbAUsdAddress

• `Private` **bbAUsdAddress**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/fee-distributor/repository.ts:41](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/fee-distributor/repository.ts#L41)

___

### data

• `Optional` **data**: [`FeeDistributorData`](../interfaces/FeeDistributorData.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/fee-distributor/repository.ts:34](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/fee-distributor/repository.ts#L34)

___

### feeDistributorAddress

• `Private` **feeDistributorAddress**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/fee-distributor/repository.ts:38](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/fee-distributor/repository.ts#L38)

___

### multicall

• **multicall**: `Contract`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/fee-distributor/repository.ts:33](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/fee-distributor/repository.ts#L33)

___

### veBalAddress

• `Private` **veBalAddress**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/fee-distributor/repository.ts:40](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/fee-distributor/repository.ts#L40)

## Methods

### fetch

▸ **fetch**(`timestamp`): `Promise`<[`FeeDistributorData`](../interfaces/FeeDistributorData.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `timestamp` | `number` |

#### Returns

`Promise`<[`FeeDistributorData`](../interfaces/FeeDistributorData.md)\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/fee-distributor/repository.ts:47](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/fee-distributor/repository.ts#L47)

___

### getPreviousWeek

▸ **getPreviousWeek**(`fromTimestamp`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `fromTimestamp` | `number` |

#### Returns

`number`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/fee-distributor/repository.ts:88](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/fee-distributor/repository.ts#L88)

___

### multicallData

▸ **multicallData**(`timestamp`): `Promise`<[`FeeDistributorData`](../interfaces/FeeDistributorData.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `timestamp` | `number` |

#### Returns

`Promise`<[`FeeDistributorData`](../interfaces/FeeDistributorData.md)\>

#### Implementation of

BaseFeeDistributor.multicallData

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/fee-distributor/repository.ts:80](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/fee-distributor/repository.ts#L80)
