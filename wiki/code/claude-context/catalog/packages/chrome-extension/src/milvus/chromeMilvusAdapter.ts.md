---
title: 'Module: packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts'
type: catalog
provenance: extracted
module: packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-chrome-extension 0.1.4 src/milvus/`chromeMilvusAdapter.ts`/
symbols:
  ChromeMilvusAdapter.searchSimilar: ChromeMilvusAdapter#searchSimilar().
  ChromeMilvusAdapter.insertChunks: ChromeMilvusAdapter#insertChunks().
  ChromeMilvusAdapter.initialize: ChromeMilvusAdapter#initialize().
  ChromeMilvusAdapter.testConnection: ChromeMilvusAdapter#testConnection().
  ChromeMilvusAdapter.milvusDb: ChromeMilvusAdapter#milvusDb.
  ChromeMilvusAdapter.getCollectionStats: ChromeMilvusAdapter#getCollectionStats().
  ChromeMilvusAdapter.createCollection: ChromeMilvusAdapter#createCollection().
  ChromeMilvusAdapter.collectionName: ChromeMilvusAdapter#collectionName.
  ChromeMilvusAdapter.collectionExists: ChromeMilvusAdapter#collectionExists().
  ChromeMilvusAdapter.clearCollection: ChromeMilvusAdapter#clearCollection().
  CodeChunk: CodeChunk#
  ChromeMilvusAdapter.-constructor: ChromeMilvusAdapter#`<constructor>`().
  CodeChunk.content: CodeChunk#content.
  CodeChunk.id: CodeChunk#id.
  CodeChunk.relativePath: CodeChunk#relativePath.
  CodeChunk.startLine: CodeChunk#startLine.
  CodeChunk.endLine: CodeChunk#endLine.
  CodeChunk.fileExtension: CodeChunk#fileExtension.
  CodeChunk.metadata: CodeChunk#metadata.
  ChromeMilvusAdapter: ChromeMilvusAdapter#
  CodeChunk.vector: CodeChunk#vector.
  SearchResult: SearchResult#
  SearchResult.id: SearchResult#id.
  SearchResult.content: SearchResult#content.
  SearchResult.relativePath: SearchResult#relativePath.
  SearchResult.startLine: SearchResult#startLine.
  SearchResult.endLine: SearchResult#endLine.
  SearchResult.fileExtension: SearchResult#fileExtension.
  SearchResult.metadata: SearchResult#metadata.
  SearchResult.score: SearchResult#score.
---
# Module: [`packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts)

## Classes
### `ChromeMilvusAdapter`
- def: [`packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts:36`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L36)
- doc: Chrome Extension adapter for Milvus RESTful Vector Database
- signature: `class ChromeMilvusAdapter`
- members:
  - `<constructor>(collectionName?: string)` — [`L40`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L40) — Chrome Extension adapter for Milvus RESTful Vector Database
  - `clearCollection(method)` — [`L180`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L180) — Clear all data in the collection
  - `collectionExists(method)` — [`L86`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L86) — Check if collection exists — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `createCollection(method)` — [`L69`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L69) — Create collection for the repository — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `getCollectionStats(method)` — [`L197`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L197) — Get collection statistics
  - `initialize(method)` — [`L47`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L47) — Initialize connection to Milvus — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `insertChunks(method)` — [`L102`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L102) — Insert code chunks into Milvus — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `searchSimilar(method)` — [`L135`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L135) — Search for similar code chunks — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `testConnection(method)` — [`L216`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L216) — Test connection to Milvus — documented in [packages-chrome-extension-src-config-milvusConfig.ts](../../../../../concepts/packages-chrome-extension-src-config-milvusConfig.ts.md)
  - `collectionName` — [`L38`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L38) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
  - `milvusDb` — [`L37`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L37) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
- uses (calls/refs, reference-scoped): [`getMilvusConfig`](../config/milvusConfig.ts.md#MilvusConfigManager.getMilvusConfig), [`insert`](../stubs/milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.insert), [`search`](../stubs/milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.search), [`createCollection`](../stubs/milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.createCollection), [`<constructor>`](../stubs/milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.-constructor), [`document`](../stubs/milvus-vectordb-stub.ts.md#VectorSearchResult.document), [`hasCollection`](../stubs/milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.hasCollection), [`dropCollection`](../stubs/milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.dropCollection), [`getCollectionStats`](../stubs/milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.getCollectionStats), [`CodeChunk`](chromeMilvusAdapter.ts.md#CodeChunk), [`MilvusConfigManager`](../config/milvusConfig.ts.md#MilvusConfigManager), [`validateMilvusConfig`](../config/milvusConfig.ts.md#MilvusConfigManager.validateMilvusConfig), [`address`](../config/milvusConfig.ts.md#MilvusConfig.address), [`database`](../config/milvusConfig.ts.md#MilvusConfig.database), [`token`](../config/milvusConfig.ts.md#MilvusConfig.token), [`username`](../config/milvusConfig.ts.md#MilvusConfig.username), [`content`](chromeMilvusAdapter.ts.md#CodeChunk.content), [`password`](../config/milvusConfig.ts.md#MilvusConfig.password), [`score`](../stubs/milvus-vectordb-stub.ts.md#VectorSearchResult.score), [`SearchOptions`](../stubs/milvus-vectordb-stub.ts.md#SearchOptions), [`threshold`](../stubs/milvus-vectordb-stub.ts.md#SearchOptions.threshold), [`MilvusRestfulVectorDatabase`](../stubs/milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase), [`content`](../stubs/milvus-vectordb-stub.ts.md#VectorDocument.content), [`endLine`](chromeMilvusAdapter.ts.md#CodeChunk.endLine), [`endLine`](../stubs/milvus-vectordb-stub.ts.md#VectorDocument.endLine), [`fileExtension`](chromeMilvusAdapter.ts.md#CodeChunk.fileExtension), [`fileExtension`](../stubs/milvus-vectordb-stub.ts.md#VectorDocument.fileExtension), [`id`](chromeMilvusAdapter.ts.md#CodeChunk.id), [`id`](../stubs/milvus-vectordb-stub.ts.md#VectorDocument.id), [`metadata`](chromeMilvusAdapter.ts.md#CodeChunk.metadata), [`metadata`](../stubs/milvus-vectordb-stub.ts.md#VectorDocument.metadata), [`relativePath`](chromeMilvusAdapter.ts.md#CodeChunk.relativePath), [`relativePath`](../stubs/milvus-vectordb-stub.ts.md#VectorDocument.relativePath), [`startLine`](chromeMilvusAdapter.ts.md#CodeChunk.startLine), [`startLine`](../stubs/milvus-vectordb-stub.ts.md#VectorDocument.startLine), [`topK`](../stubs/milvus-vectordb-stub.ts.md#SearchOptions.topK), [`SearchResult`](chromeMilvusAdapter.ts.md#SearchResult), [`entityCount`](../stubs/milvus-vectordb-stub.ts.md#MilvusRestfulVectorDatabase.getCollectionStats.Promise.typeLiteral108.entityCount), [`vector`](chromeMilvusAdapter.ts.md#CodeChunk.vector)
- used by: [`background.ts`](../background.ts.md#scip-typescript-npm-zilliz-claude-context-chrome-extension-0.1.4-src-background.ts), [`searchSimilar`](../background.ts.md#MilvusVectorDB.searchSimilar), [`initialize`](../background.ts.md#MilvusVectorDB.initialize), [`<constructor>`](../background.ts.md#MilvusVectorDB.-constructor), [`adapter`](../background.ts.md#MilvusVectorDB.adapter), [`clear`](../background.ts.md#MilvusVectorDB.clear), [`addChunks`](../background.ts.md#MilvusVectorDB.addChunks), [`getStats`](../background.ts.md#MilvusVectorDB.getStats), [`handleTestMilvusConnection`](../background.ts.md#handleTestMilvusConnection)

### `CodeChunk`
- def: [`packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts:9`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L9) — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
- signature: `interface CodeChunk`
- members:
  - `content` — [`L11`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L11) — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `endLine` — [`L14`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L14)
  - `fileExtension` — [`L15`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L15)
  - `id` — [`L10`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L10)
  - `metadata` — [`L16`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L16) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
  - `relativePath` — [`L12`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L12)
  - `startLine` — [`L13`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L13)
  - `vector` — [`L17`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L17) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
- used by: [`background.ts`](../background.ts.md#scip-typescript-npm-zilliz-claude-context-chrome-extension-0.1.4-src-background.ts), [`totalChunks`](../background.ts.md#processFileList.Promise.typeLiteral278.totalChunks), [`insertChunks`](chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.insertChunks), [`searchSimilar`](../background.ts.md#MilvusVectorDB.searchSimilar), [`processChunkBatch`](../background.ts.md#processChunkBatch), [`processChunkBuffer`](../background.ts.md#processChunkBuffer), [`addChunks`](../background.ts.md#MilvusVectorDB.addChunks), [`chunk`](../background.ts.md#processChunkBuffer.chunkBuffer-Array.typeLiteral336.chunk)

### `SearchResult`
- def: [`packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts:20`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L20) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
- signature: `interface SearchResult`
- members:
  - `content` — [`L22`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L22)
  - `endLine` — [`L25`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L25)
  - `fileExtension` — [`L26`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L26)
  - `id` — [`L21`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L21)
  - `metadata` — [`L27`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L27)
  - `relativePath` — [`L23`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L23)
  - `score` — [`L28`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L28)
  - `startLine` — [`L24`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/milvus/chromeMilvusAdapter.ts#L24)
- used by: [`searchSimilar`](chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.searchSimilar), [`searchSimilar`](../background.ts.md#MilvusVectorDB.searchSimilar)

