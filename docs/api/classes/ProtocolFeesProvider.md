# Class: ProtocolFeesProvider

## Table of contents

### Constructors

- [constructor](ProtocolFeesProvider.md#constructor)

### Properties

- [multicall](ProtocolFeesProvider.md#multicall)
- [protocolFeePercentagesProviderAddress](ProtocolFeesProvider.md#protocolfeepercentagesprovideraddress)
- [protocolFees](ProtocolFeesProvider.md#protocolfees)

### Methods

- [fetch](ProtocolFeesProvider.md#fetch)
- [getFees](ProtocolFeesProvider.md#getfees)

## Constructors

### constructor

• **new ProtocolFeesProvider**(`multicallAddress`, `protocolFeePercentagesProviderAddress`, `provider`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `multicallAddress` | `string` |
| `protocolFeePercentagesProviderAddress` | `string` |
| `provider` | `Provider` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/protocol-fees/provider.ts:25](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/protocol-fees/provider.ts#L25)

## Properties

### multicall

• **multicall**: `Contract`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/protocol-fees/provider.ts:22](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/protocol-fees/provider.ts#L22)

___

### protocolFeePercentagesProviderAddress

• `Private` **protocolFeePercentagesProviderAddress**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/protocol-fees/provider.ts:27](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/protocol-fees/provider.ts#L27)

___

### protocolFees

• `Optional` **protocolFees**: [`ProtocolFees`](../interfaces/ProtocolFees.md)

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/protocol-fees/provider.ts:23](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/protocol-fees/provider.ts#L23)

## Methods

### fetch

▸ `Private` **fetch**(): `Promise`<[`ProtocolFees`](../interfaces/ProtocolFees.md)\>

#### Returns

`Promise`<[`ProtocolFees`](../interfaces/ProtocolFees.md)\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/protocol-fees/provider.ts:33](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/protocol-fees/provider.ts#L33)

___

### getFees

▸ **getFees**(): `Promise`<[`ProtocolFees`](../interfaces/ProtocolFees.md)\>

#### Returns

`Promise`<[`ProtocolFees`](../interfaces/ProtocolFees.md)\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/protocol-fees/provider.ts:60](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/protocol-fees/provider.ts#L60)
