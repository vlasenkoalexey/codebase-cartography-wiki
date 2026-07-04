---
title: 'Module: understand-anything-plugin/packages/core/src/search.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/search.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/`search.ts`/
symbols:
  SearchEngine.search: SearchEngine#search().
  SearchEngine.-constructor: SearchEngine#`<constructor>`().
  SearchResult.nodeId: SearchResult#nodeId.
  SearchEngine.updateNodes: SearchEngine#updateNodes().
  SearchOptions.types: SearchOptions#types.
  SearchEngine.fuse: SearchEngine#fuse.
  FUSE_OPTIONS: FUSE_OPTIONS.
  SearchEngine.nodes: SearchEngine#nodes.
  SearchResult: SearchResult#
  SearchResult.score: SearchResult#score.
  SearchOptions: SearchOptions#
  SearchEngine: SearchEngine#
  SearchOptions.limit: SearchOptions#limit.
---
# Module: [`understand-anything-plugin/packages/core/src/search.ts`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/search.ts)

## Classes
### `SearchEngine`
- def: [`understand-anything-plugin/packages/core/src/search.ts:27`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/search.ts#L27)
- signature: `class SearchEngine`
- members:
  - `<constructor>(nodes: GraphNode[])` — [`L31`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/search.ts#L31)
  - `search(method)` — [`L36`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/search.ts#L36)
  - `updateNodes(method)` — [`L61`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/search.ts#L61)
  - `fuse` — [`L28`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/search.ts#L28)
  - `nodes` — [`L29`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/search.ts#L29)
- uses (calls/refs, reference-scoped): [`GraphNode`](types.ts.md#GraphNode), [`types`](search.ts.md#SearchOptions.types), [`FUSE_OPTIONS`](search.ts.md#FUSE_OPTIONS), [`SearchResult`](search.ts.md#SearchResult), [`SearchOptions`](search.ts.md#SearchOptions), [`limit`](search.ts.md#SearchOptions.limit)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`search.test.ts`](__tests__/search.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-search.test.ts)

### `SearchOptions`
- def: [`understand-anything-plugin/packages/core/src/search.ts:9`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/search.ts#L9)
- signature: `interface SearchOptions`
- members:
  - `limit` — [`L11`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/search.ts#L11)
  - `types` — [`L10`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/search.ts#L10)
- uses (calls/refs, reference-scoped): [`type`](types.ts.md#GraphNode.type), [`GraphNode`](types.ts.md#GraphNode)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`search`](search.ts.md#SearchEngine.search)

### `SearchResult`
- def: [`understand-anything-plugin/packages/core/src/search.ts:4`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/search.ts#L4)
- signature: `interface SearchResult`
- members:
  - `nodeId` — [`L5`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/search.ts#L5)
  - `score` — [`L6`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/search.ts#L6)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`search.test.ts`](__tests__/search.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-search.test.ts), [`embedding-search.test.ts`](__tests__/embedding-search.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-embedding-search.test.ts), [`search`](embedding-search.ts.md#SemanticSearchEngine.search), [`search`](search.ts.md#SearchEngine.search), [`embedding-search.ts`](embedding-search.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-embedding-search.ts)

## Module values
- `FUSE_OPTIONS` — [`L14`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/search.ts#L14)

