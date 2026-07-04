---
title: Embedding provider & model selection
type: doc-concept
provenance: doc
source: docs/getting-started/environment-variables.md
updated: 2026-07-04
status: fresh
---
# Embedding provider & model selection

## Definition
Claude Context turns code chunks into vectors with a pluggable embedding backend. Which backend, and
which model, is chosen entirely by environment variables: `EMBEDDING_PROVIDER` picks one of
`OpenAI` (default), `VoyageAI`, `Gemini`, `Ollama` (the source also supports `OpenRouter`), and
`EMBEDDING_MODEL` is a **universal** model-name variable that works for every provider. Each provider
has its own credential variable (`OPENAI_API_KEY`, `VOYAGEAI_API_KEY`, `GEMINI_API_KEY`, …) and
optional custom-endpoint base URLs.

## In claude-context (grounded)
[`createMcpConfig`](../catalog/packages/mcp/src/config.ts.md#createMcpConfig) reads
`EMBEDDING_PROVIDER` into [`ContextMcpConfig.embeddingProvider`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.embeddingProvider),
defaulting to `OpenAI`. The model is **not** read directly — it is resolved by
[`getEmbeddingModelForProvider`](../catalog/packages/mcp/src/config.ts.md#getEmbeddingModelForProvider)
into [`ContextMcpConfig.embeddingModel`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.embeddingModel).
That helper encodes two rules: for **Ollama** it prefers `OLLAMA_MODEL`, then `EMBEDDING_MODEL`, then
the default; for every other provider it uses `EMBEDDING_MODEL` or the default. Defaults come from
[`getDefaultModelForProvider`](../catalog/packages/mcp/src/config.ts.md#getDefaultModelForProvider)
(`text-embedding-3-small` for OpenAI, `voyage-code-3` for VoyageAI, `gemini-embedding-001` for Gemini,
`nomic-embed-text` for Ollama, `openai/text-embedding-3-small` for OpenRouter).

Credentials and endpoints map one-to-one onto config fields:
[`openaiApiKey`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.openaiApiKey) /
[`openaiBaseUrl`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.openaiBaseUrl),
[`voyageaiApiKey`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.voyageaiApiKey),
[`geminiApiKey`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.geminiApiKey) /
[`geminiBaseUrl`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.geminiBaseUrl),
[`openrouterApiKey`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.openrouterApiKey), and
the Ollama trio [`ollamaHost`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.ollamaHost)
(`OLLAMA_HOST`, default `http://127.0.0.1:11434`),
[`ollamaModel`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.ollamaModel), and
[`ollamaDimension`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.ollamaDimension)
(from `EMBEDDING_DIMENSION`, validated as a positive integer via
[`getPositiveIntegerFromEnv`](../catalog/packages/mcp/src/config.ts.md#getPositiveIntegerFromEnv)).

The resolved config is handed to
[`createEmbeddingInstance`](../catalog/packages/mcp/src/embedding.ts.md#createEmbeddingInstance),
which constructs the concrete embedder. Each provider class exposes a static `getSupportedModels`
(e.g. [`OpenAIEmbedding.getSupportedModels`](../catalog/packages/core/src/embedding/openai-embedding.ts.md#OpenAIEmbedding.getSupportedModels))
that the doc points readers to for the authoritative model list; Ollama has no such list because
models are whatever you have pulled locally.

## Why it matters / when it applies
Provider/model selection is the first thing to get right: the wrong `EMBEDDING_PROVIDER` without its
matching API key fails at startup (the redacted summary shows "❌ Missing"), and switching providers or
models changes vector dimensionality, so it effectively means re-indexing into a fresh collection.
`EMBEDDING_MODEL` being universal means you rarely touch provider-specific model variables — the one
exception is Ollama's `OLLAMA_MODEL` back-compat alias.

## Connections
- Code concepts: [Embedding base contract](../concepts/packages-core-src-embedding-base-embedding.ts.md) · [OpenAI](../concepts/packages-core-src-embedding-openai-embedding.ts.md) · [Gemini](../concepts/packages-core-src-embedding-gemini-embedding.ts.md) · [Ollama](../concepts/packages-core-src-embedding-ollama-embedding.ts.md) · [VoyageAI](../concepts/packages-core-src-embedding-voyageai-embedding.ts.md) · [MCP env-var config resolution](../concepts/packages-mcp-src-config.ts.md)
- Module catalogs: [config.ts](../catalog/packages/mcp/src/config.ts.md) · [embedding.ts (MCP)](../catalog/packages/mcp/src/embedding.ts.md) · [openai-embedding.ts](../catalog/packages/core/src/embedding/openai-embedding.ts.md)
- Related doc-concepts: [Global config & env-var resolution](env-global-config.md) · [Vector DB connection](env-vector-db-connection.md)

## Source
Extracted from `docs/getting-started/environment-variables.md` (kept in place).
