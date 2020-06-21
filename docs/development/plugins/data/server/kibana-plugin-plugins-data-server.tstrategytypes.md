<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [kibana-plugin-plugins-data-server](./kibana-plugin-plugins-data-server.md) &gt; [TStrategyTypes](./kibana-plugin-plugins-data-server.tstrategytypes.md)

## TStrategyTypes type

Contains all known strategy type identifiers that will be used to map to request and response shapes. Plugins that wish to add their own custom search strategies should extend this type via:

const MY\_STRATEGY = 'MY\_STRATEGY';

declare module 'src/plugins/search/server' { export interface IRequestTypesMap { \[MY\_STRATEGY\]: IMySearchRequest; }

export interface IResponseTypesMap { \[MY\_STRATEGY\]: IMySearchResponse } }

<b>Signature:</b>

```typescript
export declare type TStrategyTypes = typeof ES_SEARCH_STRATEGY | string;
```