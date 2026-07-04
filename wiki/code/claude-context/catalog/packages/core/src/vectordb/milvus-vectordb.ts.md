---
title: 'Module: packages/core/src/vectordb/milvus-vectordb.ts'
type: catalog
provenance: extracted
module: packages/core/src/vectordb/milvus-vectordb.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-core 0.1.15 src/vectordb/`milvus-vectordb.ts`/Milvus
symbols:
  MilvusVectorDatabase.client: VectorDatabase#client.
  MilvusVectorDatabase.insert: VectorDatabase#insert().
  MilvusVectorDatabase.insertHybrid: VectorDatabase#insertHybrid().
  MilvusVectorDatabase.hybridSearch: VectorDatabase#hybridSearch().
  MilvusVectorDatabase.initializeClient: VectorDatabase#initializeClient().
  MilvusVectorDatabase.ensureInitialized: VectorDatabase#ensureInitialized().
  MilvusVectorDatabase.search: VectorDatabase#search().
  MilvusVectorDatabase.resolveAddress: VectorDatabase#resolveAddress().
  MilvusVectorDatabase.-constructor: VectorDatabase#`<constructor>`().
  MilvusVectorDatabase.createCollection: VectorDatabase#createCollection().
  MilvusVectorDatabase.createHybridCollection: VectorDatabase#createHybridCollection().
  MilvusVectorDatabase.ensureLoaded: VectorDatabase#ensureLoaded().
  MilvusVectorDatabase.delete: VectorDatabase#delete().
  MilvusVectorDatabase.query: VectorDatabase#query().
  MilvusVectorDatabase.getCollectionRowCount: VectorDatabase#getCollectionRowCount().
  MilvusConfig: Config#
  MilvusConfig.address: Config#address.
  MilvusVectorDatabase.initialize: VectorDatabase#initialize().
  MilvusVectorDatabase.config: VectorDatabase#config.
  MilvusVectorDatabase.waitForIndexReady: VectorDatabase#waitForIndexReady().
  MilvusVectorDatabase.dropCollection: VectorDatabase#dropCollection().
  MilvusVectorDatabase.hasCollection: VectorDatabase#hasCollection().
  MilvusVectorDatabase.listCollections: VectorDatabase#listCollections().
  MilvusVectorDatabase.getCollectionDescription: VectorDatabase#getCollectionDescription().
  MilvusVectorDatabase.loadCollectionWithRetry: VectorDatabase#loadCollectionWithRetry().
  MilvusVectorDatabase: VectorDatabase#
  MilvusConfig.token: Config#token.
  MilvusVectorDatabase.checkCollectionLimit: VectorDatabase#checkCollectionLimit().
  MilvusVectorDatabase.initializationPromise: VectorDatabase#initializationPromise.
  MilvusConfig.username: Config#username.
  MilvusConfig.password: Config#password.
  MilvusConfig.ssl: Config#ssl.
---
# Module: [`packages/core/src/vectordb/milvus-vectordb.ts`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts)

## Classes
### `MilvusConfig`
- def: [`packages/core/src/vectordb/milvus-vectordb.ts:13`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L13)
- signature: `interface MilvusConfig`
- members:
  - `address` — [`L14`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L14)
  - `password` — [`L17`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L17)
  - `ssl` — [`L18`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L18)
  - `token` — [`L15`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L15)
  - `username` — [`L16`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L16)
- used by: [`reloadContextConfiguration`](../../../vscode-extension/src/extension.ts.md#reloadContextConfiguration), [`index.ts`](index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-index.ts), [`createContextWithConfig`](../../../vscode-extension/src/extension.ts.md#createContextWithConfig), [`configManager.ts`](../../../vscode-extension/src/config/configManager.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-config-configManager.ts), [`initializeClient`](milvus-vectordb.ts.md#MilvusVectorDatabase.initializeClient), [`resolveAddress`](milvus-vectordb.ts.md#MilvusVectorDatabase.resolveAddress), [`getMilvusFullConfig`](../../../vscode-extension/src/config/configManager.ts.md#ConfigManager.getMilvusFullConfig), [`<constructor>`](milvus-vectordb.ts.md#MilvusVectorDatabase.-constructor), [`config`](milvus-vectordb.ts.md#MilvusVectorDatabase.config)

### `MilvusVectorDatabase`  ·  implements/extends VectorDatabase
- def: [`packages/core/src/vectordb/milvus-vectordb.ts:23`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L23) — documented in [packages-core-src-vectordb-types.ts](../../../../../concepts/packages-core-src-vectordb-types.ts.md)
- signature: `class MilvusVectorDatabase`
- members:
  - `<constructor>(config: MilvusConfig)` — [`L28`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L28)
  - `checkCollectionLimit(method)` — [`L758`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L758) — Wrapper method to handle collection creation with limit detection for gRPC client — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  - `createCollection(method)` — [`L215`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L215) — Create collection — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  - `createHybridCollection(method)` — [`L476`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L476) — Create collection with hybrid search support — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  - `delete(method)` — [`L421`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L421) — Delete documents — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  - `dropCollection(method)` — [`L306`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L306) — Drop collection — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  - `ensureInitialized(method)` — [`L74`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L74) — Ensure initialization is complete before method execution — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  - `ensureLoaded(method)` — [`L84`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L84) — Ensure collection is loaded before search/query operations — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  - `getCollectionDescription(method)` — [`L740`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L740) — Get collection description — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  - `getCollectionRowCount(method)` — [`L859`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L859) — Get the number of entities (rows) in a collection. — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  - `hasCollection(method)` — [`L318`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L318) — Check if collection exists — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  - `hybridSearch(method)` — [`L627`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L627) — Hybrid search with multiple vector fields — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  - `initialize(method)` — [`L35`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L35)
  - `initializeClient(method)` — [`L40`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L40) — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  - `insert(method)` — [`L345`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L345) — Insert vector documents — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  - `insertHybrid(method)` — [`L602`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L602) — Insert hybrid vector documents — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)
  - `listCollections(method)` — [`L332`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L332) — List all collections — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  - `loadCollectionWithRetry(method)` — [`L175`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L175) — Load collection with retry logic and exponential backoff — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  - `query(method)` — [`L435`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L435) — Query documents with filter conditions — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  - `resolveAddress(method)` — [`L56`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L56) — Resolve address from config or token — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `search(method)` — [`L371`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L371) — Search similar vectors — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  - `waitForIndexReady(method)` — [`L111`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L111) — Wait for an index to be ready before proceeding — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  - `client` — [`L25`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L25) — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
  - `config` — [`L24`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L24)
  - `initializationPromise` — [`L26`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/milvus-vectordb.ts#L26) — documented in [packages-core-src-vectordb-milvus-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md)
- uses (calls/refs, reference-scoped): [`getAddressFromToken`](zilliz-utils.ts.md#ClusterManager.getAddressFromToken), [`VectorDatabase`](types.ts.md#VectorDatabase), [`VectorDocument`](types.ts.md#VectorDocument), [`data`](types.ts.md#HybridSearchRequest.data), [`limit`](types.ts.md#HybridSearchRequest.limit), [`VectorSearchResult`](types.ts.md#VectorSearchResult), [`HybridSearchRequest`](types.ts.md#HybridSearchRequest), [`HybridSearchResult`](types.ts.md#HybridSearchResult), [`anns_field`](types.ts.md#HybridSearchRequest.anns_field), [`HybridSearchOptions`](types.ts.md#HybridSearchOptions), [`filterExpr`](types.ts.md#HybridSearchOptions.filterExpr), [`MilvusConfig`](milvus-vectordb.ts.md#MilvusConfig), [`SearchOptions`](types.ts.md#SearchOptions), [`address`](milvus-vectordb.ts.md#MilvusConfig.address), [`content`](types.ts.md#VectorDocument.content), [`endLine`](types.ts.md#VectorDocument.endLine), [`filterExpr`](types.ts.md#SearchOptions.filterExpr), [`metadata`](types.ts.md#VectorDocument.metadata), [`param`](types.ts.md#HybridSearchRequest.param), [`relativePath`](types.ts.md#VectorDocument.relativePath), [`startLine`](types.ts.md#VectorDocument.startLine), [`ClusterManager`](zilliz-utils.ts.md#ClusterManager), [`fileExtension`](types.ts.md#VectorDocument.fileExtension), [`id`](types.ts.md#VectorDocument.id), [`vector`](types.ts.md#VectorDocument.vector), [`token`](milvus-vectordb.ts.md#MilvusConfig.token), [`limit`](types.ts.md#HybridSearchOptions.limit), [`topK`](types.ts.md#SearchOptions.topK), [`password`](milvus-vectordb.ts.md#MilvusConfig.password), [`ssl`](milvus-vectordb.ts.md#MilvusConfig.ssl), [`username`](milvus-vectordb.ts.md#MilvusConfig.username)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-index.ts), [`VectorDatabase`](types.ts.md#VectorDatabase), [`hybridSearch`](types.ts.md#VectorDatabase.hybridSearch), [`search`](types.ts.md#VectorDatabase.search), [`hasCollection`](types.ts.md#VectorDatabase.hasCollection), [`insert`](types.ts.md#VectorDatabase.insert), [`insertHybrid`](types.ts.md#VectorDatabase.insertHybrid), [`dropCollection`](types.ts.md#VectorDatabase.dropCollection), [`query`](types.ts.md#VectorDatabase.query), [`createCollection`](types.ts.md#VectorDatabase.createCollection), [`createHybridCollection`](types.ts.md#VectorDatabase.createHybridCollection), [`delete`](types.ts.md#VectorDatabase.delete), [`checkCollectionLimit`](types.ts.md#VectorDatabase.checkCollectionLimit), [`getCollectionDescription`](types.ts.md#VectorDatabase.getCollectionDescription), [`getCollectionRowCount`](types.ts.md#VectorDatabase.getCollectionRowCount), [`listCollections`](types.ts.md#VectorDatabase.listCollections)

