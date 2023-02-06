# Interface: BaseFeeDistributor

## Implemented by

- [`FeeDistributorRepository`](../classes/FeeDistributorRepository.md)

## Table of contents

### Properties

- [multicallData](BaseFeeDistributor.md#multicalldata)

## Properties

### multicallData

• **multicallData**: (`ts`: `number`) => `Promise`<[`FeeDistributorData`](FeeDistributorData.md)\>

#### Type declaration

▸ (`ts`): `Promise`<[`FeeDistributorData`](FeeDistributorData.md)\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `ts` | `number` |

##### Returns

`Promise`<[`FeeDistributorData`](FeeDistributorData.md)\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/fee-distributor/repository.ts:17](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/fee-distributor/repository.ts#L17)
