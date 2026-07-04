---
title: Embedding provider (why an API key is required)
type: doc-concept
provenance: doc
source: raw/code/claude-context/docs/getting-started/prerequisites.md
updated: 2026-07-04
status: fresh
---

# Embedding provider (why an API key is required)

## Definition
Claude Context makes a codebase *semantically* searchable by converting each code chunk into a
high-dimensional vector and storing it for nearest-neighbour retrieval. An **embedding provider** is
the external (or local) service that performs that text→vector conversion. The prerequisites doc
requires you to pick exactly one provider and supply its credential (an API key, or a local Ollama
install) because nothing in the index/search pipeline can run without a way to produce vectors — the
key is the entry ticket to the embedding half of the pipeline, not incidental setup.

## In claude-context (grounded)
Every provider the doc lists is a concrete subclass of the abstract
[`Embedding`](../catalog/packages/core/src/embedding/base-embedding.ts.md#Embedding) base contract,
which fixes the two methods the pipeline calls —
[`embed`](../catalog/packages/core/src/embedding/base-embedding.ts.md#Embedding.embed) (one text) and
[`embedBatch`](../catalog/packages/core/src/embedding/base-embedding.ts.md#Embedding.embedBatch) (many)
— plus [`getProvider`](../catalog/packages/core/src/embedding/base-embedding.ts.md#Embedding.getProvider)
and [`getDimension`](../catalog/packages/core/src/embedding/base-embedding.ts.md#Embedding.getDimension).
The doc's four options map one-to-one onto the shipped subclasses:

- **OpenAI** (`text-embedding-3-small/large`) → `OpenAIEmbedding`
- **VoyageAI** (`voyage-code-3`) → `VoyageAIEmbedding`
- **Gemini** (`gemini-embedding-001`) → `GeminiEmbedding`
- **Ollama** (local, `nomic-embed-text`) → `OllamaEmbedding`

Because they share the `Embedding` contract, the rest of the system is provider-agnostic: the
orchestrator holds one `Embedding` and calls `embed`/`embedBatch` without caring which cloud is
behind it (see the [Context orchestrator](../concepts/packages-core-src-context.ts.md) concept).

Which provider is used, and which credential is read, is resolved from environment variables at MCP
startup. The config surface exposes
[`embeddingProvider`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.embeddingProvider) and
one key field per option —
[`openaiApiKey`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.openaiApiKey),
[`voyageaiApiKey`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.voyageaiApiKey),
[`geminiApiKey`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.geminiApiKey) — assembled by
[`createMcpConfig`](../catalog/packages/mcp/src/config.ts.md#createMcpConfig). Ollama takes no key but
needs [`ollamaDimension`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.ollamaDimension)
because a local model can't be probed the same way a hosted one is.

> [!inferred]
> The doc marks OpenAI "Recommended" and VoyageAI's `voyage-code-3` "optimized for code"; those are
> product recommendations, not properties enforced by the code — the base contract treats all four
> providers identically.

## Why it matters / when it applies
This is a hard prerequisite: the indexing pipeline embeds every chunk before storage and embeds the
query before search, so with no provider credential there is no vector to store or match against. The
choice is also a lock-in point for the vector database — an index built with one provider's model
(and its dimension) can't be searched with another provider's vectors, since the collection is created
for a fixed dimension. The Ollama option exists so the whole pipeline can run fully local, with no data
leaving the machine.

## Connections
**Code concepts:** [Embedding base contract](../concepts/packages-core-src-embedding-base-embedding.ts.md) ·
[OpenAI](../concepts/packages-core-src-embedding-openai-embedding.ts.md) ·
[Gemini](../concepts/packages-core-src-embedding-gemini-embedding.ts.md) ·
[Ollama](../concepts/packages-core-src-embedding-ollama-embedding.ts.md) ·
[VoyageAI](../concepts/packages-core-src-embedding-voyageai-embedding.ts.md) ·
[Context orchestrator](../concepts/packages-core-src-context.ts.md) ·
[MCP env-var config](../concepts/packages-mcp-src-config.ts.md)

**Module catalogs:** [`base-embedding.ts`](../catalog/packages/core/src/embedding/base-embedding.ts.md) ·
[`mcp/config.ts`](../catalog/packages/mcp/src/config.ts.md)

**Related doc-concepts:** [Vector database: Zilliz Cloud vs local Milvus](prereq-vector-database.md)

## Source
[`docs/getting-started/prerequisites.md`](../../../../raw/code/claude-context/docs/getting-started/prerequisites.md)
— "Required Services → Embedding Provider (Choose One)".
