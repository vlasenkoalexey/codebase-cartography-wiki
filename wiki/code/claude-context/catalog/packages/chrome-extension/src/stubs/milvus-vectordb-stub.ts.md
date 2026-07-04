---
title: 'Module: packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts'
type: catalog
provenance: extracted
module: packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-chrome-extension 0.1.4 src/stubs/`milvus-vectordb-stub.ts`/
symbols:
  MilvusRestfulVectorDatabase.insert: MilvusRestfulVectorDatabase#insert().
  MilvusRestfulVectorDatabase.makeRequest: MilvusRestfulVectorDatabase#makeRequest().
  MilvusRestfulVectorDatabase.search: MilvusRestfulVectorDatabase#search().
  MilvusRestfulVectorDatabase.config: MilvusRestfulVectorDatabase#config.
  MilvusRestfulVectorDatabase.createCollection: MilvusRestfulVectorDatabase#createCollection().
  MilvusRestfulVectorDatabase.-constructor: MilvusRestfulVectorDatabase#`<constructor>`().
  VectorSearchResult.document: VectorSearchResult#document.
  MilvusRestfulVectorDatabase.hasCollection: MilvusRestfulVectorDatabase#hasCollection().
  MilvusRestfulConfig.database: MilvusRestfulConfig#database.
  MilvusRestfulVectorDatabase.createIndex: MilvusRestfulVectorDatabase#createIndex().
  MilvusRestfulVectorDatabase.loadCollection: MilvusRestfulVectorDatabase#loadCollection().
  MilvusRestfulVectorDatabase.dropCollection: MilvusRestfulVectorDatabase#dropCollection().
  MilvusRestfulVectorDatabase.getCollectionStats: MilvusRestfulVectorDatabase#getCollectionStats().
  MilvusRestfulVectorDatabase.delete: MilvusRestfulVectorDatabase#delete().
  VectorSearchResult.score: VectorSearchResult#score.
  createCollectionWithLimitCheck: createCollectionWithLimitCheck().
  VectorDocument: VectorDocument#
  SearchOptions: SearchOptions#
  SearchOptions.threshold: SearchOptions#threshold.
  VectorSearchResult: VectorSearchResult#
  VectorDocument.id: VectorDocument#id.
  VectorDocument.content: VectorDocument#content.
  VectorDocument.relativePath: VectorDocument#relativePath.
  VectorDocument.startLine: VectorDocument#startLine.
  VectorDocument.endLine: VectorDocument#endLine.
  VectorDocument.fileExtension: VectorDocument#fileExtension.
  VectorDocument.metadata: VectorDocument#metadata.
  SearchOptions.topK: SearchOptions#topK.
  MilvusRestfulConfig: MilvusRestfulConfig#
  MilvusRestfulConfig.address: MilvusRestfulConfig#address.
  MilvusRestfulConfig.token: MilvusRestfulConfig#token.
  MilvusRestfulConfig.username: MilvusRestfulConfig#username.
  MilvusRestfulConfig.password: MilvusRestfulConfig#password.
  MilvusRestfulVectorDatabase: MilvusRestfulVectorDatabase#
  MilvusRestfulVectorDatabase.baseUrl: MilvusRestfulVectorDatabase#baseUrl.
  VectorDocument.vector: VectorDocument#vector.
  MilvusRestfulVectorDatabase.getCollectionStats.Promise.typeLiteral108.entityCount: MilvusRestfulVectorDatabase#getCollectionStats().Promise:typeLiteral108:entityCount.
  COLLECTION_LIMIT_MESSAGE: COLLECTION_LIMIT_MESSAGE.
  SearchOptions.filter: SearchOptions#filter.
---
# Module: [`packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts)

## Classes
### `MilvusRestfulConfig`
- def: [`packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts:27`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L27) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
- signature: `interface MilvusRestfulConfig`
- members:
  - `address` — [`L28`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L28) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
  - `database` — [`L32`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L32) — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `password` — [`L31`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L31) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
  - `token` — [`L29`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L29) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
  - `username` — [`L30`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L30) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
- used by: [`insert`](milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.insert), [`makeRequest`](milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.makeRequest), [`search`](milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.search), [`config`](milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.config), [`createCollection`](milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.createCollection), [`<constructor>`](milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.-constructor), [`hasCollection`](milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.hasCollection), [`createIndex`](milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.createIndex), [`dropCollection`](milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.dropCollection), [`getCollectionStats`](milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.getCollectionStats), [`loadCollection`](milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.loadCollection), [`delete`](milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.delete)

### `MilvusRestfulVectorDatabase`
- def: [`packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts:39`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L39) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
- doc: Simplified Milvus Vector Database implementation for Chrome Extension
- signature: `class MilvusRestfulVectorDatabase`
- members:
  - `<constructor>(config: MilvusRestfulConfig)` — [`L43`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L43) — Simplified Milvus Vector Database implementation for Chrome Extension — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `createCollection(method)` — [`L114`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L114) — documented in [packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts](../../../../../concepts/packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts.md)
  - `createIndex(method)` — [`L192`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L192) — documented in [packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts](../../../../../concepts/packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts.md)
  - `delete(method)` — [`L341`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L341)
  - `dropCollection(method)` — [`L218`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L218)
  - `getCollectionStats(method)` — [`L360`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L360)
  - `hasCollection(method)` — [`L230`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L230) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
  - `insert(method)` — [`L244`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L244) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
  - `loadCollection(method)` — [`L211`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L211) — documented in [packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts](../../../../../concepts/packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts.md)
  - `makeRequest(method)` — [`L59`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L59) — Make HTTP request to Milvus REST API — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `search(method)` — [`L271`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L271) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
  - `baseUrl` — [`L41`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L41) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
  - `config` — [`L40`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L40) — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `entityCount` — [`L360`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L360)
- uses (calls/refs, reference-scoped): [`database`](milvus-vectordb-stub.ts.md#MilvusRestfulConfig.database), [`score`](milvus-vectordb-stub.ts.md#VectorSearchResult.score), [`createCollectionWithLimitCheck`](milvus-vectordb-stub.ts.md#createCollectionWithLimitCheck), [`SearchOptions`](milvus-vectordb-stub.ts.md#SearchOptions), [`VectorDocument`](milvus-vectordb-stub.ts.md#VectorDocument), [`VectorSearchResult`](milvus-vectordb-stub.ts.md#VectorSearchResult), [`threshold`](milvus-vectordb-stub.ts.md#SearchOptions.threshold), [`MilvusRestfulConfig`](milvus-vectordb-stub.ts.md#MilvusRestfulConfig), [`address`](milvus-vectordb-stub.ts.md#MilvusRestfulConfig.address), [`content`](milvus-vectordb-stub.ts.md#VectorDocument.content), [`endLine`](milvus-vectordb-stub.ts.md#VectorDocument.endLine), [`fileExtension`](milvus-vectordb-stub.ts.md#VectorDocument.fileExtension), [`id`](milvus-vectordb-stub.ts.md#VectorDocument.id), [`metadata`](milvus-vectordb-stub.ts.md#VectorDocument.metadata), [`password`](milvus-vectordb-stub.ts.md#MilvusRestfulConfig.password), [`relativePath`](milvus-vectordb-stub.ts.md#VectorDocument.relativePath), [`startLine`](milvus-vectordb-stub.ts.md#VectorDocument.startLine), [`token`](milvus-vectordb-stub.ts.md#MilvusRestfulConfig.token), [`topK`](milvus-vectordb-stub.ts.md#SearchOptions.topK), [`username`](milvus-vectordb-stub.ts.md#MilvusRestfulConfig.username), [`vector`](milvus-vectordb-stub.ts.md#VectorDocument.vector)
- used by: [`searchSimilar`](../milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.searchSimilar), [`insertChunks`](../milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.insertChunks), [`initialize`](../milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.initialize), [`testConnection`](../milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.testConnection), [`chromeMilvusAdapter.ts`](../milvus/chromeMilvusAdapter.ts.md#scip-typescript-npm-zilliz-claude-context-chrome-extension-0.1.4-src-milvus-chromeMilvusAdapter.ts), [`milvusDb`](../milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.milvusDb), [`getCollectionStats`](../milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.getCollectionStats), [`createCollection`](../milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.createCollection), [`clearCollection`](../milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.clearCollection), [`collectionExists`](../milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.collectionExists)

### `SearchOptions`
- def: [`packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts:16`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L16) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
- signature: `interface SearchOptions`
- members:
  - `filter` — [`L18`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L18)
  - `threshold` — [`L19`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L19) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
  - `topK` — [`L17`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L17) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
- used by: [`searchSimilar`](../milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.searchSimilar), [`chromeMilvusAdapter.ts`](../milvus/chromeMilvusAdapter.ts.md#scip-typescript-npm-zilliz-claude-context-chrome-extension-0.1.4-src-milvus-chromeMilvusAdapter.ts), [`search`](milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.search)

### `VectorDocument`
- def: [`packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts:5`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L5) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
- signature: `interface VectorDocument`
- members:
  - `content` — [`L8`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L8) — documented in [packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts](../../../../../concepts/packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts.md)
  - `endLine` — [`L11`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L11) — documented in [packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts](../../../../../concepts/packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts.md)
  - `fileExtension` — [`L12`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L12) — documented in [packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts](../../../../../concepts/packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts.md)
  - `id` — [`L6`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L6) — documented in [packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts](../../../../../concepts/packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts.md)
  - `metadata` — [`L13`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L13) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
  - `relativePath` — [`L9`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L9) — documented in [packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts](../../../../../concepts/packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts.md)
  - `startLine` — [`L10`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L10) — documented in [packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts](../../../../../concepts/packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts.md)
  - `vector` — [`L7`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L7) — documented in [packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts](../../../../../concepts/packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts.md)
- used by: [`searchSimilar`](../milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.searchSimilar), [`insert`](milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.insert), [`chromeMilvusAdapter.ts`](../milvus/chromeMilvusAdapter.ts.md#scip-typescript-npm-zilliz-claude-context-chrome-extension-0.1.4-src-milvus-chromeMilvusAdapter.ts), [`document`](milvus-vectordb-stub.ts.md#VectorSearchResult.document)

### `VectorSearchResult`
- def: [`packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts:22`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L22) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
- signature: `interface VectorSearchResult`
- members:
  - `document` — [`L23`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L23) — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `score` — [`L24`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L24) — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
- uses (calls/refs, reference-scoped): [`VectorDocument`](milvus-vectordb-stub.ts.md#VectorDocument)
- used by: [`searchSimilar`](../milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.searchSimilar), [`chromeMilvusAdapter.ts`](../milvus/chromeMilvusAdapter.ts.md#scip-typescript-npm-zilliz-claude-context-chrome-extension-0.1.4-src-milvus-chromeMilvusAdapter.ts), [`search`](milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.search)

## Functions
- `createCollectionWithLimitCheck(makeRequestFn: (endpoint: string, method: "GET" | "POST", data?: any) => Promise<any>, collectionSchema: any)` — [`L388`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L388) — Wrapper function to handle collection creation with limit detection

## Module values
- `COLLECTION_LIMIT_MESSAGE` — [`L382`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/stubs/milvus-vectordb-stub.ts#L382) — Special error type for collection limit exceeded

