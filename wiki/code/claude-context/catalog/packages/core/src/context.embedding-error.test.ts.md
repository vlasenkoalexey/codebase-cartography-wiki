---
title: 'Module: packages/core/src/context.embedding-error.test.ts'
type: catalog
provenance: extracted
module: packages/core/src/context.embedding-error.test.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-core 0.1.15 src/`context.embedding-error.test.ts`/
symbols:
  OneChunkSplitter.split: OneChunkSplitter#split().
  FailingEmbedding.-constructor: FailingEmbedding#`<constructor>`().
  OneChunkSplitter: OneChunkSplitter#
  createVectorDatabase: createVectorDatabase.
  FailingEmbedding: FailingEmbedding#
  FailingEmbedding.embed: FailingEmbedding#embed().
  FailingEmbedding.embedBatch: FailingEmbedding#embedBatch().
  EmbeddingMode: EmbeddingMode#
  FailingEmbedding.maxTokens: FailingEmbedding#maxTokens.
  FailingEmbedding.detectDimension: FailingEmbedding#detectDimension().
  FailingEmbedding.getDimension: FailingEmbedding#getDimension().
  FailingEmbedding.getProvider: FailingEmbedding#getProvider().
  OneChunkSplitter.setChunkSize: OneChunkSplitter#setChunkSize().
  OneChunkSplitter.setChunkOverlap: OneChunkSplitter#setChunkOverlap().
---
# Module: [`packages/core/src/context.embedding-error.test.ts`](../../../../../../../raw/code/claude-context/packages/core/src/context.embedding-error.test.ts)

## Classes
### `EmbeddingMode`
- def: [`packages/core/src/context.embedding-error.test.ts:9`](../../../../../../../raw/code/claude-context/packages/core/src/context.embedding-error.test.ts#L9)
- signature: `type EmbeddingMode`
- used by: [`<constructor>`](context.embedding-error.test.ts.md#FailingEmbedding.-constructor)

### `FailingEmbedding`  ·  implements/extends Embedding
- def: [`packages/core/src/context.embedding-error.test.ts:11`](../../../../../../../raw/code/claude-context/packages/core/src/context.embedding-error.test.ts#L11) — documented in [packages-vscode-extension-src-config-configManager.ts](../../../../concepts/packages-vscode-extension-src-config-configManager.ts.md)
- signature: `class FailingEmbedding`
- members:
  - `<constructor>(mode: EmbeddingMode)` — [`L14`](../../../../../../../raw/code/claude-context/packages/core/src/context.embedding-error.test.ts#L14)
  - `detectDimension(method)` — [`L18`](../../../../../../../raw/code/claude-context/packages/core/src/context.embedding-error.test.ts#L18) — Detect embedding dimension
  - `embed(method)` — [`L22`](../../../../../../../raw/code/claude-context/packages/core/src/context.embedding-error.test.ts#L22) — Generate text embedding vector
  - `embedBatch(method)` — [`L26`](../../../../../../../raw/code/claude-context/packages/core/src/context.embedding-error.test.ts#L26) — Generate text embedding vectors in batch
  - `getDimension(method)` — [`L41`](../../../../../../../raw/code/claude-context/packages/core/src/context.embedding-error.test.ts#L41) — Get embedding vector dimension
  - `getProvider(method)` — [`L45`](../../../../../../../raw/code/claude-context/packages/core/src/context.embedding-error.test.ts#L45) — Get service provider name
  - `maxTokens` — [`L12`](../../../../../../../raw/code/claude-context/packages/core/src/context.embedding-error.test.ts#L12) — documented in [packages-core-src-embedding-voyageai-embedding.ts](../../../../concepts/packages-core-src-embedding-voyageai-embedding.ts.md)
- uses (calls/refs, reference-scoped): [`Embedding`](embedding/base-embedding.ts.md#Embedding), [`EmbeddingVector`](embedding/base-embedding.ts.md#EmbeddingVector), [`EmbeddingMode`](context.embedding-error.test.ts.md#EmbeddingMode)
- used by: [`Embedding`](embedding/base-embedding.ts.md#Embedding), [`context.embedding-error.test.ts`](context.embedding-error.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.embedding-error.test.ts), [`embed`](embedding/base-embedding.ts.md#Embedding.embed), [`embedBatch`](embedding/base-embedding.ts.md#Embedding.embedBatch), [`getProvider`](embedding/base-embedding.ts.md#Embedding.getProvider), [`detectDimension`](embedding/base-embedding.ts.md#Embedding.detectDimension), [`maxTokens`](embedding/base-embedding.ts.md#Embedding.maxTokens), [`getDimension`](embedding/base-embedding.ts.md#Embedding.getDimension)

### `OneChunkSplitter`  ·  implements/extends Splitter
- def: [`packages/core/src/context.embedding-error.test.ts:50`](../../../../../../../raw/code/claude-context/packages/core/src/context.embedding-error.test.ts#L50) — documented in [packages-core-src-splitter-index.ts](../../../../concepts/packages-core-src-splitter-index.ts.md)
- signature: `class OneChunkSplitter`
- members:
  - `setChunkOverlap(method)` — [`L64`](../../../../../../../raw/code/claude-context/packages/core/src/context.embedding-error.test.ts#L64) — Set chunk overlap size
  - `setChunkSize(method)` — [`L63`](../../../../../../../raw/code/claude-context/packages/core/src/context.embedding-error.test.ts#L63) — Set chunk size
  - `split(method)` — [`L51`](../../../../../../../raw/code/claude-context/packages/core/src/context.embedding-error.test.ts#L51) — Split code into code chunks
- uses (calls/refs, reference-scoped): [`Splitter`](splitter/index.ts.md#Splitter), [`metadata`](splitter/index.ts.md#CodeChunk.metadata), [`CodeChunk`](splitter/index.ts.md#CodeChunk), [`content`](splitter/index.ts.md#CodeChunk.content), [`filePath`](splitter/index.ts.md#CodeChunk.metadata.typeLiteral52.filePath), [`startLine`](splitter/index.ts.md#CodeChunk.metadata.typeLiteral52.startLine), [`endLine`](splitter/index.ts.md#CodeChunk.metadata.typeLiteral52.endLine), [`language`](splitter/index.ts.md#CodeChunk.metadata.typeLiteral52.language)
- used by: [`context.embedding-error.test.ts`](context.embedding-error.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.embedding-error.test.ts), [`Splitter`](splitter/index.ts.md#Splitter), [`split`](splitter/index.ts.md#Splitter.split), [`setChunkOverlap`](splitter/index.ts.md#Splitter.setChunkOverlap), [`setChunkSize`](splitter/index.ts.md#Splitter.setChunkSize)

## Module values
- `createVectorDatabase` — [`L67`](../../../../../../../raw/code/claude-context/packages/core/src/context.embedding-error.test.ts#L67)

