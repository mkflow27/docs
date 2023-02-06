# Class: FeeCollectorRepository

## Implements

- [`Findable`](../interfaces/Findable.md)<`number`\>

## Table of contents

### Constructors

- [constructor](FeeCollectorRepository.md#constructor)

### Properties

- [provider](FeeCollectorRepository.md#provider)
- [swapFeePercentage](FeeCollectorRepository.md#swapfeepercentage)
- [vault](FeeCollectorRepository.md#vault)

### Methods

- [fetch](FeeCollectorRepository.md#fetch)
- [find](FeeCollectorRepository.md#find)
- [findBy](FeeCollectorRepository.md#findby)

## Constructors

### constructor

• **new FeeCollectorRepository**(`vaultAddress`, `provider`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `vaultAddress` | `string` |
| `provider` | `Provider` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/fee-collector/repository.ts:22](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/fee-collector/repository.ts#L22)

## Properties

### provider

• `Private` **provider**: `Provider`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/fee-collector/repository.ts:22](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/fee-collector/repository.ts#L22)

___

### swapFeePercentage

• `Optional` **swapFeePercentage**: `number`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/fee-collector/repository.ts:20](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/fee-collector/repository.ts#L20)

___

### vault

• **vault**: `Contract`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/fee-collector/repository.ts:19](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/fee-collector/repository.ts#L19)

## Methods

### fetch

▸ **fetch**(): `Promise`<`number`\>

#### Returns

`Promise`<`number`\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/fee-collector/repository.ts:26](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/fee-collector/repository.ts#L26)

___

### find

▸ **find**(): `Promise`<`number`\>

#### Returns

`Promise`<`number`\>

#### Implementation of

Findable.find

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/fee-collector/repository.ts:39](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/fee-collector/repository.ts#L39)

___

### findBy

▸ **findBy**(): `Promise`<`number`\>

#### Returns

`Promise`<`number`\>

#### Implementation of

Findable.findBy

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/fee-collector/repository.ts:48](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/fee-collector/repository.ts#L48)
