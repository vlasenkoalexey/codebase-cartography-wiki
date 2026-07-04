---
title: 'Vector database: Zilliz Cloud vs local Milvus'
type: doc-concept
provenance: doc
source: raw/code/claude-context/docs/getting-started/prerequisites.md
updated: 2026-07-04
status: fresh
---

# Vector database: Zilliz Cloud vs local Milvus

## Definition
The **vector database** is where the embedded code chunks live and where semantic search actually
happens: it stores each chunk's vector and metadata and, at query time, returns the nearest vectors to
the query embedding. The prerequisites doc requires one because the embedding provider only *produces*
vectors — the vector DB is what *persists and searches* them. The doc offers two ways to get the same
engine (Milvus): **Zilliz Cloud** (a fully managed Milvus service) or **local Milvus** (self-hosted via
Docker). The choice is deployment-only; the code path is the same engine either way.

## In claude-context (grounded)
Both options are served by the single Milvus implementation of the
[`VectorDatabase`](../catalog/packages/core/src/vectordb/types.ts.md#VectorDatabase) contract,
[`MilvusVectorDatabase`](../catalog/packages/core/src/vectordb/milvus-vectordb.ts.md#MilvusVectorDatabase).
That contract is what the doc's "vector database" requirement ultimately satisfies — it declares the
operations the pipeline needs: [`createCollection`](../catalog/packages/core/src/vectordb/types.ts.md#VectorDatabase.createCollection),
[`insert`](../catalog/packages/core/src/vectordb/types.ts.md#VectorDatabase.insert),
[`search`](../catalog/packages/core/src/vectordb/types.ts.md#VectorDatabase.search), and the dense+BM25
[`hybridSearch`](../catalog/packages/core/src/vectordb/types.ts.md#VectorDatabase.hybridSearch).

The Zilliz-vs-local difference reduces to how the client gets a connection **address** and **token**:

- **Local Milvus (Advanced).** You supply a full endpoint directly through
  [`milvusAddress`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.milvusAddress) — the
  Milvus client's [`MilvusConfig.address`](../catalog/packages/core/src/vectordb/milvus-vectordb.ts.md#MilvusConfig.address)
  is set and used as-is. The doc's "more complex configuration" is exactly this: you run and address the
  Docker cluster yourself.
- **Zilliz Cloud (Recommended).** You supply only an API key
  ([`milvusToken`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.milvusToken)); the concrete
  cluster endpoint is *derived* from it. The
  [zilliz-utils](../concepts/packages-core-src-vectordb-zilliz-utils.ts.md) module's
  [`ClusterManager.getAddressFromToken`](../catalog/packages/core/src/vectordb/zilliz-utils.ts.md#ClusterManager.getAddressFromToken)
  calls the Zilliz Cloud API to resolve the token into a `connectAddress`, and
  [`createFreeCluster`](../catalog/packages/core/src/vectordb/zilliz-utils.ts.md#ClusterManager.createFreeCluster)
  can even provision a free cluster on the fly. This is why the doc calls it "fully managed … without
  the need to install and manage it": the token is enough, the address is discovered for you. The
  Milvus client's [`resolveAddress`](../catalog/packages/core/src/vectordb/milvus-vectordb.ts.md#MilvusVectorDatabase.resolveAddress)
  is where an address-less config is filled in from the token.

## Why it matters / when it applies
Choosing between the two is a deployment/ops decision, not a functional one — search quality, hybrid
retrieval, and the collection schema are identical because both run Milvus. Pick **Zilliz Cloud** to
skip infrastructure (only a token needed; endpoint auto-resolved/provisioned), or **local Milvus** to
keep all vectors on your own hardware at the cost of running and addressing the cluster yourself. Either
way the vector DB must exist before indexing, since every embedded chunk is inserted into a collection
and every search is a query against it.

## Connections
**Code concepts:** [VectorDatabase contract](../concepts/packages-core-src-vectordb-types.ts.md) ·
[Milvus gRPC impl](../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md) ·
[Milvus REST impl](../concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md) ·
[Zilliz Cloud endpoint/provisioning](../concepts/packages-core-src-vectordb-zilliz-utils.ts.md) ·
[MCP env-var config](../concepts/packages-mcp-src-config.ts.md)

**Module catalogs:** [`vectordb/types.ts`](../catalog/packages/core/src/vectordb/types.ts.md) ·
[`milvus-vectordb.ts`](../catalog/packages/core/src/vectordb/milvus-vectordb.ts.md) ·
[`zilliz-utils.ts`](../catalog/packages/core/src/vectordb/zilliz-utils.ts.md) ·
[`mcp/config.ts`](../catalog/packages/mcp/src/config.ts.md)

**Related doc-concepts:** [Embedding provider (why an API key is required)](prereq-embedding-provider.md)

## Source
[`docs/getting-started/prerequisites.md`](../../../../raw/code/claude-context/docs/getting-started/prerequisites.md)
— "Required Services → Vector Database (Zilliz Cloud / Local Milvus)".
