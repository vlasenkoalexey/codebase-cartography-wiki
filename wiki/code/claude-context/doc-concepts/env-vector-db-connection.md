---
title: Vector DB connection (Milvus / Zilliz Cloud)
type: doc-concept
provenance: doc
source: docs/getting-started/environment-variables.md
updated: 2026-07-04
status: fresh
---
# Vector DB connection (Milvus / Zilliz Cloud)

## Definition
Vectors and BM25 sparse fields live in a Milvus / Zilliz Cloud collection. Two variables configure the
connection: `MILVUS_TOKEN` (authentication token — a Zilliz Personal API Key) and `MILVUS_ADDRESS`
(server endpoint). The address is **optional**: when only a token is given, Claude Context resolves the
public endpoint from the token via the Zilliz Cloud API. A third variable,
`MILVUS_COLLECTION_LIMIT_CHECK_TIMEOUT_MS`, tunes the pre-indexing collection-limit gRPC check.

## In claude-context (grounded)
[`createMcpConfig`](../catalog/packages/mcp/src/config.ts.md#createMcpConfig) reads the two connection
variables into [`ContextMcpConfig.milvusToken`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.milvusToken)
and [`ContextMcpConfig.milvusAddress`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.milvusAddress)
(the field's comment notes it "can be auto-resolved from token"). The auto-resolution is the Zilliz
Cloud path: [`ClusterManager.getAddressFromToken`](../catalog/packages/core/src/vectordb/zilliz-utils.ts.md#ClusterManager.getAddressFromToken)
is a static utility that calls the Zilliz Cloud REST API to look up the cluster's
`connectAddress` from the token, and the same [`ClusterManager`](../catalog/packages/core/src/vectordb/zilliz-utils.ts.md#ClusterManager)
can even [`createFreeCluster`](../catalog/packages/core/src/vectordb/zilliz-utils.ts.md#ClusterManager.createFreeCluster)
(driven by a [`ZillizConfig`](../catalog/packages/core/src/vectordb/zilliz-utils.ts.md#ZillizConfig))
when no cluster exists yet. This is why the doc marks `MILVUS_ADDRESS` "Auto-resolved from token" and
`MILVUS_TOKEN` "Recommended".

`MILVUS_COLLECTION_LIMIT_CHECK_TIMEOUT_MS` (default `15000`) is **not** a `ContextMcpConfig` field; it
is read directly from `process.env` inside the gRPC
[`checkCollectionLimit`](../catalog/packages/core/src/vectordb/milvus-vectordb.ts.md#MilvusVectorDatabase.checkCollectionLimit)
pre-check that runs before indexing begins. If the check exceeds the timeout, Claude Context logs the
timeout and proceeds without the limit pre-check rather than failing — raising the value gives slow or
loaded clusters more room. (The REST implementation does not implement this check.)

`logConfigurationSummary` prints the effective address, or `[Auto-resolve from token]` when only a
token is set, or `[Not configured]` when neither is present.

## Why it matters / when it applies
For Zilliz Cloud users the token alone is enough — the endpoint is discovered — which is why the Quick
Setup snippet ships both `MILVUS_ADDRESS` and `MILVUS_TOKEN` but a token-only config is valid. For a
self-hosted Milvus you must set `MILVUS_ADDRESS` explicitly (e.g. `localhost:19530`). The timeout knob
matters only on the pre-index limit check and is safe to leave at its default unless you see
`checkCollectionLimit timed out` warnings.

## Connections
- Code concepts: [Zilliz Cloud endpoint/provisioning](../concepts/packages-core-src-vectordb-zilliz-utils.ts.md) · [Milvus gRPC impl](../concepts/packages-core-src-vectordb-milvus-vectordb.ts.md) · [VectorDatabase contract](../concepts/packages-core-src-vectordb-types.ts.md) · [MCP env-var config resolution](../concepts/packages-mcp-src-config.ts.md)
- Module catalogs: [config.ts](../catalog/packages/mcp/src/config.ts.md) · [zilliz-utils.ts](../catalog/packages/core/src/vectordb/zilliz-utils.ts.md) · [milvus-vectordb.ts](../catalog/packages/core/src/vectordb/milvus-vectordb.ts.md)
- Related doc-concepts: [Global config & env-var resolution](env-global-config.md) · [Embedding provider & model selection](env-embedding-provider.md) · [Search & indexing tuning knobs](env-tuning-knobs.md)

## Source
Extracted from `docs/getting-started/environment-variables.md` (kept in place).
