---
title: 'Module: packages/core/src/context.abort.test.ts'
type: catalog
provenance: extracted
module: packages/core/src/context.abort.test.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-core 0.1.15 src/`context.abort.test.ts`/
symbols:
  CountingSplitter.split: CountingSplitter#split().
  TestEmbedding: TestEmbedding#
  createVectorDatabase: createVectorDatabase.
  CountingSplitter.calls: CountingSplitter#calls.
  CountingSplitter.-constructor: CountingSplitter#`<constructor>`().
  TestEmbedding.embed: TestEmbedding#embed().
  TestEmbedding.embedBatch: TestEmbedding#embedBatch().
  CountingSplitter: CountingSplitter#
  TestEmbedding.maxTokens: TestEmbedding#maxTokens.
  TestEmbedding.detectDimension: TestEmbedding#detectDimension().
  TestEmbedding.getDimension: TestEmbedding#getDimension().
  TestEmbedding.getProvider: TestEmbedding#getProvider().
  CountingSplitter.setChunkSize: CountingSplitter#setChunkSize().
  CountingSplitter.setChunkOverlap: CountingSplitter#setChunkOverlap().
---
# Module: [`packages/core/src/context.abort.test.ts`](../../../../../../../raw/code/claude-context/packages/core/src/context.abort.test.ts)

## Classes
### `CountingSplitter`  ·  implements/extends Splitter
- def: [`packages/core/src/context.abort.test.ts:33`](../../../../../../../raw/code/claude-context/packages/core/src/context.abort.test.ts#L33) — documented in [packages-core-src-splitter-index.ts](../../../../concepts/packages-core-src-splitter-index.ts.md)
- signature: `class CountingSplitter`
- members:
  - `<constructor>(onCall?: ((callIndex: number) => void) | undefined)` — [`L36`](../../../../../../../raw/code/claude-context/packages/core/src/context.abort.test.ts#L36)
  - `setChunkOverlap(method)` — [`L53`](../../../../../../../raw/code/claude-context/packages/core/src/context.abort.test.ts#L53) — Set chunk overlap size
  - `setChunkSize(method)` — [`L52`](../../../../../../../raw/code/claude-context/packages/core/src/context.abort.test.ts#L52) — Set chunk size
  - `split(method)` — [`L38`](../../../../../../../raw/code/claude-context/packages/core/src/context.abort.test.ts#L38) — Split code into code chunks — documented in [packages-core-src-splitter-index.ts](../../../../concepts/packages-core-src-splitter-index.ts.md)
  - `calls` — [`L34`](../../../../../../../raw/code/claude-context/packages/core/src/context.abort.test.ts#L34)
- uses (calls/refs, reference-scoped): [`Splitter`](splitter/index.ts.md#Splitter), [`metadata`](splitter/index.ts.md#CodeChunk.metadata), [`CodeChunk`](splitter/index.ts.md#CodeChunk), [`content`](splitter/index.ts.md#CodeChunk.content), [`filePath`](splitter/index.ts.md#CodeChunk.metadata.typeLiteral52.filePath), [`startLine`](splitter/index.ts.md#CodeChunk.metadata.typeLiteral52.startLine), [`endLine`](splitter/index.ts.md#CodeChunk.metadata.typeLiteral52.endLine), [`language`](splitter/index.ts.md#CodeChunk.metadata.typeLiteral52.language)
- used by: [`context.abort.test.ts`](context.abort.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.abort.test.ts), [`Splitter`](splitter/index.ts.md#Splitter), [`split`](splitter/index.ts.md#Splitter.split), [`setChunkOverlap`](splitter/index.ts.md#Splitter.setChunkOverlap), [`setChunkSize`](splitter/index.ts.md#Splitter.setChunkSize)

### `TestEmbedding`  ·  implements/extends Embedding
- def: [`packages/core/src/context.abort.test.ts:9`](../../../../../../../raw/code/claude-context/packages/core/src/context.abort.test.ts#L9) — documented in [packages-core-src-embedding-base-embedding.ts](../../../../concepts/packages-core-src-embedding-base-embedding.ts.md)
- signature: `class TestEmbedding`
- members:
  - `detectDimension(method)` — [`L12`](../../../../../../../raw/code/claude-context/packages/core/src/context.abort.test.ts#L12) — Detect embedding dimension
  - `embed(method)` — [`L16`](../../../../../../../raw/code/claude-context/packages/core/src/context.abort.test.ts#L16) — Generate text embedding vector
  - `embedBatch(method)` — [`L20`](../../../../../../../raw/code/claude-context/packages/core/src/context.abort.test.ts#L20) — Generate text embedding vectors in batch
  - `getDimension(method)` — [`L24`](../../../../../../../raw/code/claude-context/packages/core/src/context.abort.test.ts#L24) — Get embedding vector dimension
  - `getProvider(method)` — [`L28`](../../../../../../../raw/code/claude-context/packages/core/src/context.abort.test.ts#L28) — Get service provider name
  - `maxTokens` — [`L10`](../../../../../../../raw/code/claude-context/packages/core/src/context.abort.test.ts#L10) — documented in [packages-core-src-embedding-ollama-embedding.ts](../../../../concepts/packages-core-src-embedding-ollama-embedding.ts.md)
- uses (calls/refs, reference-scoped): [`Embedding`](embedding/base-embedding.ts.md#Embedding), [`EmbeddingVector`](embedding/base-embedding.ts.md#EmbeddingVector)
- used by: [`context.abort.test.ts`](context.abort.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.abort.test.ts), [`Embedding`](embedding/base-embedding.ts.md#Embedding), [`embed`](embedding/base-embedding.ts.md#Embedding.embed), [`embedBatch`](embedding/base-embedding.ts.md#Embedding.embedBatch), [`getProvider`](embedding/base-embedding.ts.md#Embedding.getProvider), [`detectDimension`](embedding/base-embedding.ts.md#Embedding.detectDimension), [`maxTokens`](embedding/base-embedding.ts.md#Embedding.maxTokens), [`getDimension`](embedding/base-embedding.ts.md#Embedding.getDimension)

## Module values
- `createVectorDatabase` — [`L56`](../../../../../../../raw/code/claude-context/packages/core/src/context.abort.test.ts#L56) — documented in [packages-core-src-vectordb-types.ts](../../../../concepts/packages-core-src-vectordb-types.ts.md)

