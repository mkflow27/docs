# Class: GaugeControllerMulticallRepository

## Table of contents

### Constructors

- [constructor](GaugeControllerMulticallRepository.md#constructor)

### Properties

- [gaugeControllerAddress](GaugeControllerMulticallRepository.md#gaugecontrolleraddress)
- [multicall](GaugeControllerMulticallRepository.md#multicall)

### Methods

- [getRelativeWeights](GaugeControllerMulticallRepository.md#getrelativeweights)

## Constructors

### constructor

• **new GaugeControllerMulticallRepository**(`multicallAddress`, `gaugeControllerAddress`, `provider`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `multicallAddress` | `string` |
| `gaugeControllerAddress` | `string` |
| `provider` | `Provider` |

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/gauge-controller/multicall.ts:15](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/gauge-controller/multicall.ts#L15)

## Properties

### gaugeControllerAddress

• `Private` **gaugeControllerAddress**: `string`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/gauge-controller/multicall.ts:17](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/gauge-controller/multicall.ts#L17)

___

### multicall

• **multicall**: `Contract`

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/gauge-controller/multicall.ts:13](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/gauge-controller/multicall.ts#L13)

## Methods

### getRelativeWeights

▸ **getRelativeWeights**(`gaugeAddresses`, `timestamp?`): `Promise`<{ `[gaugeAddress: string]`: `number`;  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `gaugeAddresses` | `string`[] |
| `timestamp?` | `number` |

#### Returns

`Promise`<{ `[gaugeAddress: string]`: `number`;  }\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/gauge-controller/multicall.ts:23](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/gauge-controller/multicall.ts#L23)
