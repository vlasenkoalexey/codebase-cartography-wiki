---
title: 'Module: packages/chrome-extension/src/background.ts'
type: catalog
provenance: extracted
module: packages/chrome-extension/src/background.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-chrome-extension 0.1.4 src/`background.ts`/
symbols:
  handleIndexRepo: handleIndexRepo().
  processFileList.Promise.typeLiteral278.totalChunks: processFileList().Promise:typeLiteral278:totalChunks.
  MilvusVectorDB.searchSimilar: MilvusVectorDB#searchSimilar().
  handleSearchCode: handleSearchCode().
  MilvusVectorDB.initialize: MilvusVectorDB#initialize().
  processChunkBatch: processChunkBatch().
  handleCheckIndexStatus: handleCheckIndexStatus().
  handleClearIndex: handleClearIndex().
  processChunkBuffer: processChunkBuffer().
  MilvusVectorDB.adapter: MilvusVectorDB#adapter.
  MilvusVectorDB.-constructor: MilvusVectorDB#`<constructor>`().
  MilvusVectorDB.clear: MilvusVectorDB#clear().
  EmbeddingModel.embedBatch: EmbeddingModel#embedBatch().
  EmbeddingModel.getConfig: EmbeddingModel#getConfig().
  MilvusVectorDB.addChunks: MilvusVectorDB#addChunks().
  MilvusVectorDB.getStats: MilvusVectorDB#getStats().
  fetchRepoFiles: fetchRepoFiles().
  fetchFileContent: fetchFileContent().
  handleTestMilvusConnection: handleTestMilvusConnection().
  handleGetIndexedRepos: handleGetIndexedRepos().
  getGitHubToken: getGitHubToken().
  EmbeddingModel.getInstance: EmbeddingModel#getInstance().
  EmbeddingModel.embedSingle: EmbeddingModel#embedSingle().
  checkRepositoryAccess: checkRepositoryAccess().
  processFileList: processFileList().
  processChunkBuffer.chunkBuffer-Array.typeLiteral336.chunk: processChunkBuffer().(chunkBuffer)Array:typeLiteral336:chunk.
  EmbeddingModel.config: EmbeddingModel#config.
  MilvusVectorDB: MilvusVectorDB#
  MilvusVectorDB.repoCollectionName: MilvusVectorDB#repoCollectionName.
  EMBEDDING_DIM: EMBEDDING_DIM.
  EMBEDDING_BATCH_SIZE: EMBEDDING_BATCH_SIZE.
  EmbeddingModel: EmbeddingModel#
  handleRateLimit: handleRateLimit().
  processFileList.Promise.typeLiteral278.processedFiles: processFileList().Promise:typeLiteral278:processedFiles.
  EmbeddingModel.getConfig.Promise.typeLiteral19.apiKey: EmbeddingModel#getConfig().Promise:typeLiteral19:apiKey.
  EmbeddingModel.getConfig.Promise.typeLiteral19.model: EmbeddingModel#getConfig().Promise:typeLiteral19:model.
  splitCode: splitCode().
  validateGitHubToken: validateGitHubToken().
  MAX_TOKENS_PER_BATCH: MAX_TOKENS_PER_BATCH.
  MAX_CHUNKS_PER_BATCH: MAX_CHUNKS_PER_BATCH.
  cosSim: cosSim().
  processChunkBuffer.chunkBuffer-Array.typeLiteral336.repoId: processChunkBuffer().(chunkBuffer)Array:typeLiteral336:repoId.
---
# Module: [`packages/chrome-extension/src/background.ts`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts)

## Classes
### `EmbeddingModel`
- def: [`packages/chrome-extension/src/background.ts:32`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L32) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
- signature: `class EmbeddingModel`
- members:
  - `embedBatch(method)` — [`L46`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L46) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `embedSingle(method)` — [`L70`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L70) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `getConfig(method)` — [`L35`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L35) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `getInstance(method)` — [`L75`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L75)
  - `apiKey` — [`L35`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L35)
  - `config` — [`L33`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L33)
  - `model` — [`L35`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L35)
- uses (calls/refs, reference-scoped): [`MilvusConfigManager`](config/milvusConfig.ts.md#MilvusConfigManager), [`getOpenAIConfig`](config/milvusConfig.ts.md#MilvusConfigManager.getOpenAIConfig)
- used by: [`handleSearchCode`](background.ts.md#handleSearchCode), [`processChunkBatch`](background.ts.md#processChunkBatch)

### `MilvusVectorDB`
- def: [`packages/chrome-extension/src/background.ts:87`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L87)
- signature: `class MilvusVectorDB`
- members:
  - `<constructor>(repoId: string)` — [`L91`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L91) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `addChunks(method)` — [`L109`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L109) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `clear(method)` — [`L141`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L141)
  - `getStats(method)` — [`L152`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L152)
  - `initialize(method)` — [`L96`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L96) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `searchSimilar(method)` — [`L120`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L120) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `adapter` — [`L88`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L88) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `repoCollectionName` — [`L89`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L89) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
- uses (calls/refs, reference-scoped): [`searchSimilar`](milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.searchSimilar), [`insertChunks`](milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.insertChunks), [`initialize`](milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.initialize), [`getCollectionStats`](milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.getCollectionStats), [`createCollection`](milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.createCollection), [`clearCollection`](milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.clearCollection), [`collectionExists`](milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.collectionExists), [`CodeChunk`](milvus/chromeMilvusAdapter.ts.md#CodeChunk), [`<constructor>`](milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter.-constructor), [`ChromeMilvusAdapter`](milvus/chromeMilvusAdapter.ts.md#ChromeMilvusAdapter), [`EMBEDDING_DIM`](background.ts.md#EMBEDDING_DIM), [`content`](milvus/chromeMilvusAdapter.ts.md#SearchResult.content), [`endLine`](milvus/chromeMilvusAdapter.ts.md#SearchResult.endLine), [`fileExtension`](milvus/chromeMilvusAdapter.ts.md#SearchResult.fileExtension), [`id`](milvus/chromeMilvusAdapter.ts.md#SearchResult.id), [`metadata`](milvus/chromeMilvusAdapter.ts.md#SearchResult.metadata), [`relativePath`](milvus/chromeMilvusAdapter.ts.md#SearchResult.relativePath), [`score`](milvus/chromeMilvusAdapter.ts.md#SearchResult.score), [`startLine`](milvus/chromeMilvusAdapter.ts.md#SearchResult.startLine)
- used by: [`handleIndexRepo`](background.ts.md#handleIndexRepo), [`handleSearchCode`](background.ts.md#handleSearchCode), [`handleCheckIndexStatus`](background.ts.md#handleCheckIndexStatus), [`processChunkBatch`](background.ts.md#processChunkBatch), [`handleClearIndex`](background.ts.md#handleClearIndex), [`processChunkBuffer`](background.ts.md#processChunkBuffer), [`processFileList`](background.ts.md#processFileList)

## Functions
- `checkRepositoryAccess(owner: string, repo: string)` — [`L264`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L264) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
- `cosSim(a: number[], b: number[])` — [`L16`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L16)
- `fetchFileContent(owner: string, repo: string, path: string)` — [`L355`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L355) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
- `fetchRepoFiles(owner: string, repo: string)` — [`L313`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L313) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
- `getGitHubToken()` — [`L243`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L243) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
- `handleCheckIndexStatus(request: any, sendResponse: Function)` — [`L671`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L671) — documented in [packages-chrome-extension-src-storage-indexedRepoManager.ts](../../../../concepts/packages-chrome-extension-src-storage-indexedRepoManager.ts.md)
- `handleClearIndex(request: any, sendResponse: Function)` — [`L650`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L650) — documented in [packages-chrome-extension-src-storage-indexedRepoManager.ts](../../../../concepts/packages-chrome-extension-src-storage-indexedRepoManager.ts.md)
- `handleGetIndexedRepos(sendResponse: Function)` — [`L713`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L713)
- `handleIndexRepo(request: any, sendResponse: Function)` — [`L441`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L441) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
- `handleRateLimit(response: Response)` — [`L294`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L294)
- `handleSearchCode(request: any, sendResponse: Function)` — [`L623`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L623) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
- `handleTestMilvusConnection(sendResponse: Function)` — [`L403`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L403) — documented in [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](../../../../concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md)
- `processChunkBatch(chunks: CodeChunk[], vectorDB: MilvusVectorDB)` — [`L608`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L608) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
- `processChunkBuffer(chunkBuffer: { chunk: CodeChunk; repoId: string; }[], vectorDB: MilvusVectorDB)` — [`L592`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L592) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
- `processFileList(files: any[], owner: string, repo: string, repoId: string, vectorDB: MilvusVectorDB, chunkSize: number, chunkOverlap: number)` — [`L498`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L498) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
- `splitCode(content: string, language?: string, chunkSize?: number, chunkOverlap?: number)` — [`L164`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L164)
- `validateGitHubToken(token: string)` — [`L214`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L214)

## Module values
- `EMBEDDING_BATCH_SIZE` — [`L11`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L11) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)
- `EMBEDDING_DIM` — [`L10`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L10)
- `MAX_CHUNKS_PER_BATCH` — [`L13`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L13)
- `MAX_TOKENS_PER_BATCH` — [`L12`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L12)
- `chunk` — [`L593`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L593)
- `processedFiles` — [`L506`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L506)
- `repoId` — [`L593`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L593)
- `totalChunks` — [`L506`](../../../../../../../raw/code/claude-context/packages/chrome-extension/src/background.ts#L506) — documented in [packages-chrome-extension-src-background.ts](../../../../concepts/packages-chrome-extension-src-background.ts.md)

