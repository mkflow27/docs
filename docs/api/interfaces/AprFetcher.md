# Interface: AprFetcher

## Callable

### AprFetcher

▸ **AprFetcher**(`network?`): `Promise`<{ `[address: string]`: `number`;  }\>

Common interface for fetching APR from external sources

#### Parameters

| Name | Type |
| :------ | :------ |
| `network?` | [`Network`](../enums/Network.md) |

#### Returns

`Promise`<{ `[address: string]`: `number`;  }\>

#### Defined in

[balancer-sdk/balancer-js/src/modules/data/token-yields/repository.ts:24](https://github.com/balancer-labs/balancer-sdk/blob/c094037b/balancer-js/src/modules/data/token-yields/repository.ts#L24)
