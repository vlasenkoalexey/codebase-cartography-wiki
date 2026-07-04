---
title: Search & indexing tuning knobs
type: doc-concept
provenance: doc
source: docs/getting-started/environment-variables.md
updated: 2026-07-04
status: fresh
---
# Search & indexing tuning knobs

## Definition
Three "advanced configuration" variables tune retrieval quality, indexing throughput, and collection
naming without changing the connection or provider: `HYBRID_MODE` (BM25 + dense hybrid search vs
dense-only, default `true`), `EMBEDDING_BATCH_SIZE` (chunks embedded per request, default `100`), and
`CODE_CHUNKS_COLLECTION_NAME_OVERRIDE` (a human-readable prefix for the Milvus collection name).

## In claude-context (grounded)
**`HYBRID_MODE`** is read in the core layer by
[`Context.getIsHybrid`](../catalog/packages/core/src/context.ts.md#Context.getIsHybrid), which returns
`true` unless the variable is explicitly the string `"false"`. This flag is load-bearing beyond search:
it selects the collection prefix (`hybrid_code_chunks` vs `code_chunks`) and whether indexing writes a
sparse BM25 field alongside the dense vector, so flipping it also implies a different collection.

**`EMBEDDING_BATCH_SIZE`** is parsed inside the indexing loop of
[`Context.indexCodebase`](../catalog/packages/core/src/context.ts.md#Context.indexCodebase) —
`Math.max(1, parseInt(env || '100'))` — and controls how many chunks are buffered before an embedding
call is flushed. It is a local of the indexing method rather than a distinct catalog symbol, so there is
no dedicated anchor for it; the mechanism lives on the Context concept page.

**`CODE_CHUNKS_COLLECTION_NAME_OVERRIDE`** is the one tuning knob that *is* a resolver field: it lands
in [`ContextMcpConfig.collectionNameOverride`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.collectionNameOverride)
via [`createMcpConfig`](../catalog/packages/mcp/src/config.ts.md#createMcpConfig). When set, the
collection becomes `code_chunks_<override>_<pathHash>` (or `hybrid_code_chunks_<override>_<pathHash>`)
after sanitization; the per-codebase `<pathHash>` is always appended so multiple codebases stay
distinct under one override, and unsetting it reverts to the plain hash-based name for that path.

## Why it matters / when it applies
`HYBRID_MODE` is the main retrieval-quality lever — hybrid combines lexical BM25 recall with dense
semantic recall and is on by default; drop to dense-only only to shrink storage or if the backend lacks
BM25. `EMBEDDING_BATCH_SIZE` trades indexing latency against provider rate limits: larger batches index
faster but can hit per-request token/size caps. The collection-name override is purely ergonomic —
readable collection names in the Milvus/Zilliz console — with the path hash preserving uniqueness.

## Connections
- Code concepts: [Context orchestrator (index/search pipeline)](../concepts/packages-core-src-context.ts.md) · [Milvus gRPC impl (dense + BM25 hybrid)](../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md) · [MCP env-var config resolution](../concepts/packages-mcp-src-config.ts.md)
- Module catalogs: [context.ts](../catalog/packages/core/src/context.ts.md) · [config.ts](../catalog/packages/mcp/src/config.ts.md)
- Related doc-concepts: [Global config & env-var resolution](env-global-config.md) · [Vector DB connection](env-vector-db-connection.md) · [Splitter selection & file filters](env-splitter.md)

## Source
Extracted from `docs/getting-started/environment-variables.md` (kept in place).
