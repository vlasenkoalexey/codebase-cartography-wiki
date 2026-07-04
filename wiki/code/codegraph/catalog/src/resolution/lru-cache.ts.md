---
title: 'Module: src/resolution/lru-cache.ts'
type: catalog
provenance: extracted
module: src/resolution/lru-cache.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/`lru-cache.ts`/LRUCache#
symbols:
  LRUCache.set: set().
  LRUCache.store: store.
  LRUCache.get: get().
  LRUCache.-constructor: '`<constructor>`().'
  LRUCache.clear: clear().
  LRUCache: ''
  LRUCache.has: has().
  LRUCache.-get-size: '`<get>size`().'
  LRUCache.max: max.
---
# Module: [`src/resolution/lru-cache.ts`](../../../../../../raw/code/codegraph/src/resolution/lru-cache.ts)

## Classes
### `LRUCache`
- def: [`src/resolution/lru-cache.ts:14`](../../../../../../raw/code/codegraph/src/resolution/lru-cache.ts#L14)
- doc: Simple LRU cache backed by JavaScript's insertion-ordered Map.
- signature: `class LRUCache`
- members:
  - `<constructor>(max: number)` — [`L18`](../../../../../../raw/code/codegraph/src/resolution/lru-cache.ts#L18) — Simple LRU cache backed by JavaScript's insertion-ordered Map.
  - `<get>size` — [`L25`](../../../../../../raw/code/codegraph/src/resolution/lru-cache.ts#L25)
  - `clear(method)` — [`L59`](../../../../../../raw/code/codegraph/src/resolution/lru-cache.ts#L59)
  - `get(method)` — [`L29`](../../../../../../raw/code/codegraph/src/resolution/lru-cache.ts#L29)
  - `has(method)` — [`L42`](../../../../../../raw/code/codegraph/src/resolution/lru-cache.ts#L42)
  - `set(method)` — [`L46`](../../../../../../raw/code/codegraph/src/resolution/lru-cache.ts#L46)
  - `max` — [`L15`](../../../../../../raw/code/codegraph/src/resolution/lru-cache.ts#L15)
  - `store` — [`L16`](../../../../../../raw/code/codegraph/src/resolution/lru-cache.ts#L16)
- used by: [`createContext`](index.ts.md#ReferenceResolver.createContext), [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-index.ts), [`<constructor>`](index.ts.md#ReferenceResolver.-constructor), [`clearCaches`](index.ts.md#ReferenceResolver.clearCaches), [`readFileCached`](index.ts.md#ReferenceResolver.readFileCached), [`nameCache`](index.ts.md#ReferenceResolver.nameCache), [`importMappingCache`](index.ts.md#ReferenceResolver.importMappingCache), [`nodeCache`](index.ts.md#ReferenceResolver.nodeCache), [`reExportCache`](index.ts.md#ReferenceResolver.reExportCache), [`lowerNameCache`](index.ts.md#ReferenceResolver.lowerNameCache), [`methodMatchCache`](index.ts.md#ReferenceResolver.methodMatchCache), [`qualifiedNameCache`](index.ts.md#ReferenceResolver.qualifiedNameCache), [`fileCache`](index.ts.md#ReferenceResolver.fileCache), [`fileLinesCache`](index.ts.md#ReferenceResolver.fileLinesCache)

