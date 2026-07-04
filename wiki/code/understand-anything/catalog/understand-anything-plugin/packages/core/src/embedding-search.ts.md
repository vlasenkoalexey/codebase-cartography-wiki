---
title: 'Module: understand-anything-plugin/packages/core/src/embedding-search.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/embedding-search.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/`embedding-search.ts`/
symbols:
  SemanticSearchEngine.search: SemanticSearchEngine#search().
  SemanticSearchEngine.-constructor: SemanticSearchEngine#`<constructor>`().
  cosineSimilarity: cosineSimilarity().
  SemanticSearchEngine.hasEmbeddings: SemanticSearchEngine#hasEmbeddings().
  SemanticSearchEngine.nodes: SemanticSearchEngine#nodes.
  SemanticSearchEngine.updateNodes: SemanticSearchEngine#updateNodes().
  SemanticSearchEngine.embeddings: SemanticSearchEngine#embeddings.
  SemanticSearchEngine.addEmbedding: SemanticSearchEngine#addEmbedding().
  SemanticSearchOptions: SemanticSearchOptions#
  SemanticSearchEngine: SemanticSearchEngine#
  SemanticSearchOptions.limit: SemanticSearchOptions#limit.
  SemanticSearchOptions.threshold: SemanticSearchOptions#threshold.
  SemanticSearchOptions.types: SemanticSearchOptions#types.
---
# Module: [`understand-anything-plugin/packages/core/src/embedding-search.ts`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/embedding-search.ts)

## Classes
### `SemanticSearchEngine`
- def: [`understand-anything-plugin/packages/core/src/embedding-search.ts:37`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/embedding-search.ts#L37)
- doc: Semantic search engine using vector embeddings.
- signature: `class SemanticSearchEngine`
- members:
  - `<constructor>(nodes: GraphNode[], embeddings: Record<string, number[]>)` — [`L41`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/embedding-search.ts#L41) — Semantic search engine using vector embeddings.
  - `addEmbedding(method)` — [`L50`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/embedding-search.ts#L50)
  - `hasEmbeddings(method)` — [`L46`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/embedding-search.ts#L46)
  - `search(method)` — [`L54`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/embedding-search.ts#L54)
  - `updateNodes(method)` — [`L80`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/embedding-search.ts#L80)
  - `embeddings` — [`L39`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/embedding-search.ts#L39)
  - `nodes` — [`L38`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/embedding-search.ts#L38)
- uses (calls/refs, reference-scoped): [`id`](types.ts.md#GraphNode.id), [`type`](types.ts.md#GraphNode.type), [`GraphNode`](types.ts.md#GraphNode), [`cosineSimilarity`](embedding-search.ts.md#cosineSimilarity), [`SearchResult`](search.ts.md#SearchResult), [`SemanticSearchOptions`](embedding-search.ts.md#SemanticSearchOptions), [`limit`](embedding-search.ts.md#SemanticSearchOptions.limit), [`threshold`](embedding-search.ts.md#SemanticSearchOptions.threshold), [`types`](embedding-search.ts.md#SemanticSearchOptions.types)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`embedding-search.test.ts`](__tests__/embedding-search.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-embedding-search.test.ts)

### `SemanticSearchOptions`
- def: [`understand-anything-plugin/packages/core/src/embedding-search.ts:4`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/embedding-search.ts#L4)
- signature: `interface SemanticSearchOptions`
- members:
  - `limit` — [`L5`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/embedding-search.ts#L5)
  - `threshold` — [`L6`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/embedding-search.ts#L6)
  - `types` — [`L7`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/embedding-search.ts#L7)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`search`](embedding-search.ts.md#SemanticSearchEngine.search)

## Functions
- `cosineSimilarity(a: number[], b: number[])` — [`L14`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/embedding-search.ts#L14) — Compute cosine similarity between two vectors.

