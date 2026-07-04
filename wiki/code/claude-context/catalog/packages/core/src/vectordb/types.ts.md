---
title: 'Module: packages/core/src/vectordb/types.ts'
type: catalog
provenance: extracted
module: packages/core/src/vectordb/types.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-core 0.1.15 src/vectordb/`types.ts`/
symbols:
  VectorDatabase: VectorDatabase#
  VectorDocument: VectorDocument#
  VectorDatabase.hybridSearch: VectorDatabase#hybridSearch().
  HybridSearchRequest.data: HybridSearchRequest#data.
  VectorDatabase.search: VectorDatabase#search().
  HybridSearchRequest.limit: HybridSearchRequest#limit.
  VectorSearchResult: VectorSearchResult#
  VectorDatabase.hasCollection: VectorDatabase#hasCollection().
  VectorDatabase.insert: VectorDatabase#insert().
  VectorDatabase.insertHybrid: VectorDatabase#insertHybrid().
  HybridSearchRequest: HybridSearchRequest#
  HybridSearchRequest.anns_field: HybridSearchRequest#anns_field.
  HybridSearchResult: HybridSearchResult#
  VectorSearchResult.document: VectorSearchResult#document.
  HybridSearchResult.document: HybridSearchResult#document.
  HybridSearchOptions: HybridSearchOptions#
  HybridSearchOptions.filterExpr: HybridSearchOptions#filterExpr.
  VectorDatabase.dropCollection: VectorDatabase#dropCollection().
  VectorDatabase.query: VectorDatabase#query().
  VectorDocument.content: VectorDocument#content.
  VectorDocument.relativePath: VectorDocument#relativePath.
  VectorDocument.startLine: VectorDocument#startLine.
  VectorDocument.endLine: VectorDocument#endLine.
  VectorDocument.metadata: VectorDocument#metadata.
  SearchOptions: SearchOptions#
  SearchOptions.filterExpr: SearchOptions#filterExpr.
  HybridSearchRequest.param: HybridSearchRequest#param.
  VectorDatabase.createCollection: VectorDatabase#createCollection().
  VectorDatabase.createHybridCollection: VectorDatabase#createHybridCollection().
  VectorDatabase.delete: VectorDatabase#delete().
  VectorDatabase.listCollections: VectorDatabase#listCollections().
  VectorDatabase.getCollectionDescription: VectorDatabase#getCollectionDescription().
  VectorDatabase.checkCollectionLimit: VectorDatabase#checkCollectionLimit().
  VectorDatabase.getCollectionRowCount: VectorDatabase#getCollectionRowCount().
  VectorDocument.id: VectorDocument#id.
  VectorDocument.vector: VectorDocument#vector.
  VectorDocument.fileExtension: VectorDocument#fileExtension.
  COLLECTION_LIMIT_MESSAGE: COLLECTION_LIMIT_MESSAGE.
  HybridSearchOptions.rerank: HybridSearchOptions#rerank.
  SearchOptions.topK: SearchOptions#topK.
  HybridSearchOptions.limit: HybridSearchOptions#limit.
  RerankStrategy: RerankStrategy#
  VectorSearchResult.score: VectorSearchResult#score.
  HybridSearchResult.score: HybridSearchResult#score.
  SearchOptions.filter: SearchOptions#filter.
  SearchOptions.threshold: SearchOptions#threshold.
  RerankStrategy.strategy: RerankStrategy#strategy.
  RerankStrategy.params: RerankStrategy#params.
---
# Module: [`packages/core/src/vectordb/types.ts`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts)

## Classes
### `HybridSearchOptions`
- def: [`packages/core/src/vectordb/types.ts:28`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L28) — documented in [packages-core-src-vectordb-milvus-restful-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md)
- signature: `interface HybridSearchOptions`
- members:
  - `filterExpr` — [`L31`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L31) — documented in [packages-core-src-vectordb-milvus-restful-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md)
  - `limit` — [`L30`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L30) — documented in [packages-core-src-vectordb-milvus-restful-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md)
  - `rerank` — [`L29`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L29)
- uses (calls/refs, reference-scoped): [`RerankStrategy`](types.ts.md#RerankStrategy)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-index.ts), [`context.ts`](../context.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.ts), [`hybridSearch`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.hybridSearch), [`hybridSearch`](milvus-vectordb.ts.md#MilvusVectorDatabase.hybridSearch), [`milvus-restful-vectordb.ts`](milvus-restful-vectordb.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-milvus-restful-vectordb.ts), [`milvus-vectordb.ts`](milvus-vectordb.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-milvus-vectordb.ts), [`hybridSearch`](types.ts.md#VectorDatabase.hybridSearch)

### `HybridSearchRequest`
- def: [`packages/core/src/vectordb/types.ts:21`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L21) — documented in [packages-core-src-vectordb-milvus-restful-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md)
- signature: `interface HybridSearchRequest`
- members:
  - `anns_field` — [`L23`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L23) — documented in [packages-core-src-vectordb-milvus-restful-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md)
  - `data` — [`L22`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L22) — documented in [packages-core-src-vectordb-milvus-restful-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md)
  - `limit` — [`L25`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L25) — documented in [packages-core-src-vectordb-milvus-restful-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md)
  - `param` — [`L24`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L24) — documented in [packages-core-src-vectordb-milvus-restful-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md)
- used by: [`semanticSearch`](../context.ts.md#Context.semanticSearch), [`index.ts`](index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-index.ts), [`context.ts`](../context.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.ts), [`hybridSearch`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.hybridSearch), [`hybridSearch`](milvus-vectordb.ts.md#MilvusVectorDatabase.hybridSearch), [`milvus-restful-vectordb.ts`](milvus-restful-vectordb.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-milvus-restful-vectordb.ts), [`milvus-vectordb.ts`](milvus-vectordb.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-milvus-vectordb.ts), [`hybridSearch`](types.ts.md#VectorDatabase.hybridSearch)

### `HybridSearchResult`
- def: [`packages/core/src/vectordb/types.ts:44`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L44) — documented in [packages-core-src-vectordb-milvus-restful-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md)
- signature: `interface HybridSearchResult`
- members:
  - `document` — [`L45`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L45) — documented in [packages-core-src-vectordb-types.ts](../../../../../concepts/packages-core-src-vectordb-types.ts.md)
  - `score` — [`L46`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L46)
- uses (calls/refs, reference-scoped): [`VectorDocument`](types.ts.md#VectorDocument)
- used by: [`semanticSearch`](../context.ts.md#Context.semanticSearch), [`index.ts`](index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-index.ts), [`context.ts`](../context.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.ts), [`hybridSearch`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.hybridSearch), [`hybridSearch`](milvus-vectordb.ts.md#MilvusVectorDatabase.hybridSearch), [`milvus-restful-vectordb.ts`](milvus-restful-vectordb.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-milvus-restful-vectordb.ts), [`milvus-vectordb.ts`](milvus-vectordb.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-milvus-vectordb.ts), [`hybridSearch`](types.ts.md#VectorDatabase.hybridSearch)

### `RerankStrategy`
- def: [`packages/core/src/vectordb/types.ts:34`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L34)
- signature: `interface RerankStrategy`
- members:
  - `params` — [`L36`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L36)
  - `strategy` — [`L35`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L35)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-index.ts), [`rerank`](types.ts.md#HybridSearchOptions.rerank)

### `SearchOptions`
- def: [`packages/core/src/vectordb/types.ts:13`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L13)
- signature: `interface SearchOptions`
- members:
  - `filter` — [`L15`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L15)
  - `filterExpr` — [`L17`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L17)
  - `threshold` — [`L16`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L16)
  - `topK` — [`L14`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L14)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-index.ts), [`milvus-restful-vectordb.ts`](milvus-restful-vectordb.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-milvus-restful-vectordb.ts), [`milvus-vectordb.ts`](milvus-vectordb.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-milvus-vectordb.ts), [`search`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.search), [`search`](milvus-vectordb.ts.md#MilvusVectorDatabase.search), [`search`](types.ts.md#VectorDatabase.search)

### `VectorDatabase`
- def: [`packages/core/src/vectordb/types.ts:49`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L49) — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)
- signature: `interface VectorDatabase`
- members:
  - `checkCollectionLimit(method)` — [`L140`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L140) — Check collection limit
  - `createCollection(method)` — [`L56`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L56) — Create collection
  - `createHybridCollection(method)` — [`L64`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L64) — Create collection with hybrid search support
  - `delete(method)` — [`L118`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L118) — Delete documents
  - `dropCollection(method)` — [`L70`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L70) — Drop collection
  - `getCollectionDescription(method)` — [`L134`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L134) — Get collection description
  - `getCollectionRowCount(method)` — [`L147`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L147) — Get the number of entities (rows) in a collection.
  - `hasCollection(method)` — [`L76`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L76) — Check if collection exists
  - `hybridSearch(method)` — [`L111`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L111) — Hybrid search with multiple vector fields — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)
  - `insert(method)` — [`L88`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L88) — Insert vector documents — documented in [packages-core-src-vectordb-milvus-restful-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md)
  - `insertHybrid(method)` — [`L95`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L95) — Insert hybrid vector documents — documented in [packages-core-src-vectordb-milvus-restful-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md)
  - `listCollections(method)` — [`L81`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L81) — List all collections
  - `query(method)` — [`L127`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L127) — Query documents with filter conditions
  - `search(method)` — [`L103`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L103) — Search similar vectors
- uses (calls/refs, reference-scoped): [`hybridSearch`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.hybridSearch), [`insert`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.insert), [`insertHybrid`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.insertHybrid), [`hybridSearch`](milvus-vectordb.ts.md#MilvusVectorDatabase.hybridSearch), [`insert`](milvus-vectordb.ts.md#MilvusVectorDatabase.insert), [`insertHybrid`](milvus-vectordb.ts.md#MilvusVectorDatabase.insertHybrid), [`search`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.search), [`createCollection`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.createCollection), [`createHybridCollection`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.createHybridCollection), [`search`](milvus-vectordb.ts.md#MilvusVectorDatabase.search), [`delete`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.delete), [`getCollectionRowCount`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.getCollectionRowCount), [`query`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.query), [`VectorDocument`](types.ts.md#VectorDocument), [`dropCollection`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.dropCollection), [`getCollectionDescription`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.getCollectionDescription), [`hasCollection`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.hasCollection), [`listCollections`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.listCollections), [`createCollection`](milvus-vectordb.ts.md#MilvusVectorDatabase.createCollection), [`createHybridCollection`](milvus-vectordb.ts.md#MilvusVectorDatabase.createHybridCollection), [`VectorSearchResult`](types.ts.md#VectorSearchResult), [`HybridSearchRequest`](types.ts.md#HybridSearchRequest), [`HybridSearchResult`](types.ts.md#HybridSearchResult), [`delete`](milvus-vectordb.ts.md#MilvusVectorDatabase.delete), [`getCollectionRowCount`](milvus-vectordb.ts.md#MilvusVectorDatabase.getCollectionRowCount), [`query`](milvus-vectordb.ts.md#MilvusVectorDatabase.query), [`HybridSearchOptions`](types.ts.md#HybridSearchOptions), [`SearchOptions`](types.ts.md#SearchOptions), [`dropCollection`](milvus-vectordb.ts.md#MilvusVectorDatabase.dropCollection), [`getCollectionDescription`](milvus-vectordb.ts.md#MilvusVectorDatabase.getCollectionDescription), [`hasCollection`](milvus-vectordb.ts.md#MilvusVectorDatabase.hasCollection), [`listCollections`](milvus-vectordb.ts.md#MilvusVectorDatabase.listCollections), [`MilvusRestfulVectorDatabase`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase), [`MilvusVectorDatabase`](milvus-vectordb.ts.md#MilvusVectorDatabase), [`checkCollectionLimit`](milvus-vectordb.ts.md#MilvusVectorDatabase.checkCollectionLimit), [`checkCollectionLimit`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.checkCollectionLimit)
- used by: [`semanticSearch`](../context.ts.md#Context.semanticSearch), [`index.ts`](index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-index.ts), [`context.splitter.test.ts`](../context.splitter.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.splitter.test.ts), [`context.ignore-patterns.test.ts`](../context.ignore-patterns.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.ignore-patterns.test.ts), [`context.ts`](../context.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.ts), [`processChunkBatch`](../context.ts.md#Context.processChunkBatch), [`context.abort.test.ts`](../context.abort.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.abort.test.ts), [`context.embedding-error.test.ts`](../context.embedding-error.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.embedding-error.test.ts), [`milvus-restful-vectordb.ts`](milvus-restful-vectordb.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-milvus-restful-vectordb.ts), [`prepareCollection`](../context.ts.md#Context.prepareCollection), [`milvus-vectordb.ts`](milvus-vectordb.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-milvus-vectordb.ts), [`vectorDatabase`](../context.ts.md#Context.vectorDatabase), [`clearIndex`](../context.ts.md#Context.clearIndex), [`createVectorDatabase`](../context.ignore-patterns.test.ts.md#createVectorDatabase), [`hasIndex`](../context.ts.md#Context.hasIndex), [`deleteFileChunks`](../context.ts.md#Context.deleteFileChunks), [`createVectorDatabase`](../context.abort.test.ts.md#createVectorDatabase), [`updateVectorDatabase`](../context.ts.md#Context.updateVectorDatabase), [`createVectorDatabase`](../context.embedding-error.test.ts.md#createVectorDatabase), [`createVectorDatabase`](../context.splitter.test.ts.md#createVectorDatabase), [`getVectorDatabase`](../context.ts.md#Context.getVectorDatabase), [`MilvusRestfulVectorDatabase`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase), [`vectorDatabase`](../context.ts.md#ContextConfig.vectorDatabase), [`MilvusVectorDatabase`](milvus-vectordb.ts.md#MilvusVectorDatabase)

### `VectorDocument`
- def: [`packages/core/src/vectordb/types.ts:2`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L2) — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)
- signature: `interface VectorDocument`
- members:
  - `content` — [`L5`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L5) — documented in [packages-core-src-vectordb-milvus-restful-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md)
  - `endLine` — [`L8`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L8) — documented in [packages-core-src-vectordb-milvus-restful-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md)
  - `fileExtension` — [`L9`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L9) — documented in [packages-core-src-vectordb-milvus-restful-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md)
  - `id` — [`L3`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L3) — documented in [packages-core-src-vectordb-milvus-restful-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md)
  - `metadata` — [`L10`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L10) — documented in [packages-core-src-vectordb-milvus-restful-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md)
  - `relativePath` — [`L6`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L6) — documented in [packages-core-src-vectordb-milvus-restful-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md)
  - `startLine` — [`L7`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L7) — documented in [packages-core-src-vectordb-milvus-restful-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md)
  - `vector` — [`L4`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L4) — documented in [packages-core-src-vectordb-milvus-restful-vectordb.ts](../../../../../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md)
- used by: [`semanticSearch`](../context.ts.md#Context.semanticSearch), [`index.ts`](index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-index.ts), [`context.ts`](../context.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.ts), [`processChunkBatch`](../context.ts.md#Context.processChunkBatch), [`insert`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.insert), [`insertHybrid`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.insertHybrid), [`insert`](milvus-vectordb.ts.md#MilvusVectorDatabase.insert), [`insertHybrid`](milvus-vectordb.ts.md#MilvusVectorDatabase.insertHybrid), [`milvus-restful-vectordb.ts`](milvus-restful-vectordb.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-milvus-restful-vectordb.ts), [`milvus-vectordb.ts`](milvus-vectordb.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-milvus-vectordb.ts), [`insert`](types.ts.md#VectorDatabase.insert), [`insertHybrid`](types.ts.md#VectorDatabase.insertHybrid), [`document`](types.ts.md#HybridSearchResult.document), [`document`](types.ts.md#VectorSearchResult.document)

### `VectorSearchResult`
- def: [`packages/core/src/vectordb/types.ts:39`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L39)
- signature: `interface VectorSearchResult`
- members:
  - `document` — [`L40`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L40) — documented in [packages-core-src-vectordb-types.ts](../../../../../concepts/packages-core-src-vectordb-types.ts.md)
  - `score` — [`L41`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L41)
- uses (calls/refs, reference-scoped): [`VectorDocument`](types.ts.md#VectorDocument)
- used by: [`semanticSearch`](../context.ts.md#Context.semanticSearch), [`index.ts`](index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-index.ts), [`context.ts`](../context.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.ts), [`milvus-restful-vectordb.ts`](milvus-restful-vectordb.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-milvus-restful-vectordb.ts), [`milvus-vectordb.ts`](milvus-vectordb.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-milvus-vectordb.ts), [`search`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.search), [`search`](milvus-vectordb.ts.md#MilvusVectorDatabase.search), [`search`](types.ts.md#VectorDatabase.search)

## Module values
- `COLLECTION_LIMIT_MESSAGE` — [`L154`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/types.ts#L154) — Special error message for collection limit exceeded

