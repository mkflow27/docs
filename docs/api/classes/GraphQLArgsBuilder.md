# Class: GraphQLArgsBuilder

## Table of contents

### Constructors

- [constructor](GraphQLArgsBuilder.md#constructor)

### Properties

- [args](GraphQLArgsBuilder.md#args)

### Methods

- [format](GraphQLArgsBuilder.md#format)
- [merge](GraphQLArgsBuilder.md#merge)

## Constructors

### constructor

• **new GraphQLArgsBuilder**(`args`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | [`GraphQLArgs`](../interfaces/GraphQLArgs.md) |

#### Defined in

[balancer-sdk/balancer-js/src/lib/graphql/args-builder.ts:7](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/graphql/args-builder.ts#L7)

## Properties

### args

• `Readonly` **args**: [`GraphQLArgs`](../interfaces/GraphQLArgs.md)

#### Defined in

[balancer-sdk/balancer-js/src/lib/graphql/args-builder.ts:7](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/graphql/args-builder.ts#L7)

## Methods

### format

▸ **format**(`formatter`): `unknown`

#### Parameters

| Name | Type |
| :------ | :------ |
| `formatter` | [`GraphQLArgsFormatter`](../interfaces/GraphQLArgsFormatter.md) |

#### Returns

`unknown`

#### Defined in

[balancer-sdk/balancer-js/src/lib/graphql/args-builder.ts:23](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/graphql/args-builder.ts#L23)

___

### merge

▸ **merge**(`other`): [`GraphQLArgsBuilder`](GraphQLArgsBuilder.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `other` | [`GraphQLArgsBuilder`](GraphQLArgsBuilder.md) |

#### Returns

[`GraphQLArgsBuilder`](GraphQLArgsBuilder.md)

#### Defined in

[balancer-sdk/balancer-js/src/lib/graphql/args-builder.ts:9](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/lib/graphql/args-builder.ts#L9)
