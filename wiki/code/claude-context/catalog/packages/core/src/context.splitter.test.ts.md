---
title: 'Module: packages/core/src/context.splitter.test.ts'
type: catalog
provenance: extracted
module: packages/core/src/context.splitter.test.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-core 0.1.15 src/`context.splitter.test.ts`/
symbols:
  RecordingSplitter.split: RecordingSplitter#split().
  RecordingSplitter.calls: RecordingSplitter#calls.
  TestEmbedding: TestEmbedding#
  createVectorDatabase: createVectorDatabase.
  RecordingSplitter.-constructor: RecordingSplitter#`<constructor>`().
  TestEmbedding.embed: TestEmbedding#embed().
  TestEmbedding.embedBatch: TestEmbedding#embedBatch().
  RecordingSplitter: RecordingSplitter#
  RecordingSplitter.calls.Array.typeLiteral3.code: RecordingSplitter#calls.Array:typeLiteral3:code.
  RecordingSplitter.calls.Array.typeLiteral3.language: RecordingSplitter#calls.Array:typeLiteral3:language.
  RecordingSplitter.calls.Array.typeLiteral3.filePath: RecordingSplitter#calls.Array:typeLiteral3:filePath.
  TestEmbedding.maxTokens: TestEmbedding#maxTokens.
  TestEmbedding.detectDimension: TestEmbedding#detectDimension().
  TestEmbedding.getDimension: TestEmbedding#getDimension().
  TestEmbedding.getProvider: TestEmbedding#getProvider().
  RecordingSplitter.setChunkSize: RecordingSplitter#setChunkSize().
  RecordingSplitter.setChunkOverlap: RecordingSplitter#setChunkOverlap().
---
# Module: [`packages/core/src/context.splitter.test.ts`](../../../../../../../raw/code/claude-context/packages/core/src/context.splitter.test.ts)

## Classes
### `RecordingSplitter`  ·  implements/extends Splitter
- def: [`packages/core/src/context.splitter.test.ts:34`](../../../../../../../raw/code/claude-context/packages/core/src/context.splitter.test.ts#L34) — documented in [packages-core-src-splitter-index.ts](../../../../concepts/packages-core-src-splitter-index.ts.md)
- signature: `class RecordingSplitter`
- members:
  - `<constructor>(label: string)` — [`L37`](../../../../../../../raw/code/claude-context/packages/core/src/context.splitter.test.ts#L37)
  - `setChunkOverlap(method)` — [`L54`](../../../../../../../raw/code/claude-context/packages/core/src/context.splitter.test.ts#L54) — Set chunk overlap size
  - `setChunkSize(method)` — [`L52`](../../../../../../../raw/code/claude-context/packages/core/src/context.splitter.test.ts#L52) — Set chunk size
  - `split(method)` — [`L39`](../../../../../../../raw/code/claude-context/packages/core/src/context.splitter.test.ts#L39) — Split code into code chunks
  - `calls` — [`L35`](../../../../../../../raw/code/claude-context/packages/core/src/context.splitter.test.ts#L35)
  - `code` — [`L35`](../../../../../../../raw/code/claude-context/packages/core/src/context.splitter.test.ts#L35)
  - `filePath` — [`L35`](../../../../../../../raw/code/claude-context/packages/core/src/context.splitter.test.ts#L35)
  - `language` — [`L35`](../../../../../../../raw/code/claude-context/packages/core/src/context.splitter.test.ts#L35)
- uses (calls/refs, reference-scoped): [`Splitter`](splitter/index.ts.md#Splitter), [`metadata`](splitter/index.ts.md#CodeChunk.metadata), [`CodeChunk`](splitter/index.ts.md#CodeChunk), [`content`](splitter/index.ts.md#CodeChunk.content), [`filePath`](splitter/index.ts.md#CodeChunk.metadata.typeLiteral52.filePath), [`startLine`](splitter/index.ts.md#CodeChunk.metadata.typeLiteral52.startLine), [`endLine`](splitter/index.ts.md#CodeChunk.metadata.typeLiteral52.endLine), [`language`](splitter/index.ts.md#CodeChunk.metadata.typeLiteral52.language)
- used by: [`context.splitter.test.ts`](context.splitter.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.splitter.test.ts), [`Splitter`](splitter/index.ts.md#Splitter), [`split`](splitter/index.ts.md#Splitter.split), [`setChunkOverlap`](splitter/index.ts.md#Splitter.setChunkOverlap), [`setChunkSize`](splitter/index.ts.md#Splitter.setChunkSize)

### `TestEmbedding`  ·  implements/extends Embedding
- def: [`packages/core/src/context.splitter.test.ts:10`](../../../../../../../raw/code/claude-context/packages/core/src/context.splitter.test.ts#L10) — documented in [packages-core-src-embedding-base-embedding.ts](../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
- signature: `class TestEmbedding`
- members:
  - `detectDimension(method)` — [`L13`](../../../../../../../raw/code/claude-context/packages/core/src/context.splitter.test.ts#L13) — Detect embedding dimension
  - `embed(method)` — [`L17`](../../../../../../../raw/code/claude-context/packages/core/src/context.splitter.test.ts#L17) — Generate text embedding vector
  - `embedBatch(method)` — [`L21`](../../../../../../../raw/code/claude-context/packages/core/src/context.splitter.test.ts#L21) — Generate text embedding vectors in batch
  - `getDimension(method)` — [`L25`](../../../../../../../raw/code/claude-context/packages/core/src/context.splitter.test.ts#L25) — Get embedding vector dimension
  - `getProvider(method)` — [`L29`](../../../../../../../raw/code/claude-context/packages/core/src/context.splitter.test.ts#L29) — Get service provider name
  - `maxTokens` — [`L11`](../../../../../../../raw/code/claude-context/packages/core/src/context.splitter.test.ts#L11) — documented in [packages-core-src-embedding-voyageai-embedding.ts](../../../../concepts/packages-core-src-embedding-voyageai-embedding.ts.md)
- uses (calls/refs, reference-scoped): [`Embedding`](embedding/base-embedding.ts.md#Embedding), [`EmbeddingVector`](embedding/base-embedding.ts.md#EmbeddingVector)
- used by: [`context.splitter.test.ts`](context.splitter.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.splitter.test.ts), [`Embedding`](embedding/base-embedding.ts.md#Embedding), [`embed`](embedding/base-embedding.ts.md#Embedding.embed), [`embedBatch`](embedding/base-embedding.ts.md#Embedding.embedBatch), [`getProvider`](embedding/base-embedding.ts.md#Embedding.getProvider), [`detectDimension`](embedding/base-embedding.ts.md#Embedding.detectDimension), [`maxTokens`](embedding/base-embedding.ts.md#Embedding.maxTokens), [`getDimension`](embedding/base-embedding.ts.md#Embedding.getDimension)

## Module values
- `createVectorDatabase` — [`L57`](../../../../../../../raw/code/claude-context/packages/core/src/context.splitter.test.ts#L57)

