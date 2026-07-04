---
title: Hybrid search (BM25 + dense vector)
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Hybrid search (BM25 + dense vector)

## Definition
Claude Context does not rely on dense-vector similarity alone. Its `index_codebase` and `search_code`
tools both run **hybrid search: BM25 (sparse, lexical) + dense vector (semantic)**. BM25 catches exact
lexical matches (identifiers, keywords), the dense embedding catches semantic paraphrase, and the two
rankings are fused. The README lists this as the first implementation detail — "advanced hybrid search
(BM25 + dense vector)" — and both MCP tools advertise it in their descriptions.

## In claude-context (grounded)
The [`VectorDatabase`](../catalog/packages/core/src/vectordb/types.ts.md#VectorDatabase) contract
exposes [`hybridSearch`](../catalog/packages/core/src/vectordb/types.ts.md#VectorDatabase.hybridSearch)
alongside plain `search`, taking a list of
[`HybridSearchRequest`](../catalog/packages/core/src/vectordb/types.ts.md#HybridSearchRequest)
(each carrying its own `anns_field`, `data`, `param`, `limit`) plus
[`HybridSearchOptions`](../catalog/packages/core/src/vectordb/types.ts.md#HybridSearchOptions) with a
[`RerankStrategy`](../catalog/packages/core/src/vectordb/types.ts.md#RerankStrategy) for fusion. The
Milvus implementation supplies the sparse+dense collection and the fused query:
[`MilvusVectorDatabase.createHybridCollection`](../catalog/packages/core/src/vectordb/milvus-vectordb.ts.md#MilvusVectorDatabase.createHybridCollection),
[`insertHybrid`](../catalog/packages/core/src/vectordb/milvus-vectordb.ts.md#MilvusVectorDatabase.insertHybrid),
and [`hybridSearch`](../catalog/packages/core/src/vectordb/milvus-vectordb.ts.md#MilvusVectorDatabase.hybridSearch).
Whether a given index runs in hybrid mode is decided by
[`Context.getIsHybrid`](../catalog/packages/core/src/context.ts.md#Context.getIsHybrid).

## Why it matters / when it applies
Pure semantic search misses when the query hinges on an exact token (a rare symbol name, an error
string); pure lexical search misses paraphrase. Fusing BM25 with dense vectors gives robust retrieval
across both cases — which is why it is the default for indexing and searching in this system rather
than an opt-in.

## Connections
- Code concepts: [VectorDatabase contract](../concepts/packages-core-src-vectordb-types.ts.md),
  [Milvus gRPC impl](../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md),
  [Milvus REST impl](../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md),
  [Context orchestrator](../concepts/packages-core-src-context.ts.md).
- Module catalogs: [vectordb/types.ts](../catalog/packages/core/src/vectordb/types.ts.md),
  [vectordb/milvus-vectordb.ts](../catalog/packages/core/src/vectordb/milvus-vectordb.ts.md).
- Related doc-concepts: [Semantic code search](semantic-code-search.md), [Embedding & vector
  backends](embedding-and-vector-backends.md), [MCP integration](mcp-integration.md).

## Source
Extracted from `README.md` (kept in place).
