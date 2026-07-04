---
title: Embedding providers & vector databases
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Embedding providers & vector databases

## Definition
Claude Context is pluggable at both ends of the retrieval pipeline. The README's "Supported
Technologies" list names four **embedding providers** — OpenAI, VoyageAI, Ollama, Gemini — behind one
interface, and two **vector-database backends** — self-hosted Milvus or the fully-managed Zilliz
Cloud. You pick a provider by API key / model (e.g. `text-embedding-3-large` for OpenAI,
`voyage-code-3` for VoyageAI) and a vector store by address/token; the rest of the pipeline is
unchanged.

## In claude-context (grounded)
All providers implement one base contract,
[`Embedding`](../catalog/packages/core/src/embedding/base-embedding.ts.md#Embedding), with
[`embed`](../catalog/packages/core/src/embedding/base-embedding.ts.md#Embedding.embed) /
`embedBatch` / `detectDimension`. The four concrete classes are
[`OpenAIEmbedding`](../catalog/packages/core/src/embedding/openai-embedding.ts.md#OpenAIEmbedding),
[`VoyageAIEmbedding`](../catalog/packages/core/src/embedding/voyageai-embedding.ts.md#VoyageAIEmbedding),
[`GeminiEmbedding`](../catalog/packages/core/src/embedding/gemini-embedding.ts.md#GeminiEmbedding), and
[`OllamaEmbedding`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding)
(Ollama being the README's path to a fully-local deployment).

On the storage side, the [`VectorDatabase`](../catalog/packages/core/src/vectordb/types.ts.md#VectorDatabase)
interface has two Milvus implementations —
[`MilvusVectorDatabase`](../catalog/packages/core/src/vectordb/milvus-vectordb.ts.md#MilvusVectorDatabase)
(gRPC, used in the README's `new MilvusVectorDatabase({ address, token })` example) and a REST variant.
Zilliz Cloud is reached through the same Milvus address/token, with cluster provisioning handled by
[`ClusterManager`](../catalog/packages/core/src/vectordb/zilliz-utils.ts.md#ClusterManager) —
[`getAddressFromToken`](../catalog/packages/core/src/vectordb/zilliz-utils.ts.md#ClusterManager.getAddressFromToken)
resolves an endpoint from just a token and
[`createFreeCluster`](../catalog/packages/core/src/vectordb/zilliz-utils.ts.md#ClusterManager.createFreeCluster)
can provision one.

## Why it matters / when it applies
Embedding quality dominates retrieval quality, and different teams have different constraints — cost,
latency, on-prem/local (Ollama), or a code-specialized model (VoyageAI's `voyage-code-3`). Pinning
the pipeline to one provider or one database would be a hard ceiling; the shared `Embedding` and
`VectorDatabase` contracts make the choice a config swap. Zilliz Cloud is the README's answer to
"scalable, no matter how large your codebase" — a managed Milvus so you don't run the DB yourself.

## Connections
- Code concepts: [Embedding base contract](../concepts/packages-core-src-embedding-base-embedding.ts.md),
  [OpenAI](../concepts/packages-core-src-embedding-openai-embedding.ts.md) /
  [VoyageAI](../concepts/packages-core-src-embedding-voyageai-embedding.ts.md) /
  [Gemini](../concepts/packages-core-src-embedding-gemini-embedding.ts.md) /
  [Ollama](../concepts/packages-core-src-embedding-ollama-embedding.ts.md) providers,
  [VectorDatabase contract](../concepts/packages-core-src-vectordb-types.ts.md),
  [Milvus gRPC impl](../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md),
  [Zilliz Cloud utils](../concepts/packages-core-src-vectordb-zilliz-utils.ts.md).
- Module catalogs: [embedding/base-embedding.ts](../catalog/packages/core/src/embedding/base-embedding.ts.md),
  [vectordb/types.ts](../catalog/packages/core/src/vectordb/types.ts.md),
  [vectordb/zilliz-utils.ts](../catalog/packages/core/src/vectordb/zilliz-utils.ts.md).
- Related doc-concepts: [Hybrid search](hybrid-search.md), [Architecture &
  packages](architecture-packages.md), [MCP integration](mcp-integration.md).

## Source
Extracted from `README.md` (kept in place).
