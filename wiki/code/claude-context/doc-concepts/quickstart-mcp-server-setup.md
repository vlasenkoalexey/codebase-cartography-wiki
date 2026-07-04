---
title: MCP server setup model (stdio + env-var config)
type: doc-concept
provenance: doc
source: raw/code/claude-context/docs/getting-started/quick-start.md
updated: 2026-07-04
status: fresh
---
# MCP server setup model (stdio + env-var config)

## Definition
Claude Context ships to an AI assistant as an **MCP (Model Context Protocol) server**, not a library
the host imports. Every integration in the Quick Start — Claude Code, Codex CLI, Gemini CLI, Cursor,
Windsurf, Claude Desktop, and the rest — reduces to the same three-part recipe: a **command**
(`npx @zilliz/claude-context-mcp@latest`), a **transport** (stdio; the host spawns the process and
talks to it over stdin/stdout), and a **bag of environment variables** carrying credentials and
provider choice. The dozens of client blocks in the doc are the *same server* wired into different
config files — the mental model is "one stdio server, configured entirely through env vars."

## In claude-context (grounded)
When the host launches `npx @zilliz/claude-context-mcp@latest`, the package's entrypoint
[`main()`](../catalog/packages/mcp/src/index.ts.md#main) runs. It reads the process environment,
resolves it into one typed config object via
[`createMcpConfig()`](../catalog/packages/mcp/src/config.ts.md#createMcpConfig), constructs a
[`ContextMcpServer`](../catalog/packages/mcp/src/index.ts.md#ContextMcpServer), registers the MCP
tools with [`setupTools`](../catalog/packages/mcp/src/index.ts.md#ContextMcpServer.setupTools), and
begins serving with [`start`](../catalog/packages/mcp/src/index.ts.md#ContextMcpServer.start) over the
stdio transport. So the "single command" in the Quick Start is literally the process the host spawns;
there is no daemon and no port.

Every `env` key in the client snippets maps to a field on
[`ContextMcpConfig`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig):

- **Credentials / endpoints** — `OPENAI_API_KEY` →
  [`openaiApiKey`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.openaiApiKey),
  `MILVUS_ADDRESS` →
  [`milvusAddress`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.milvusAddress),
  `MILVUS_TOKEN` →
  [`milvusToken`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.milvusToken). The default
  setup points `MILVUS_ADDRESS`/`MILVUS_TOKEN` at a **Zilliz Cloud** endpoint — the managed vector DB
  is the persistence layer for the index.
- **Provider selection** — `EMBEDDING_PROVIDER` →
  [`embeddingProvider`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.embeddingProvider)
  chooses between OpenAI, VoyageAI, Gemini, and Ollama (the four alternative Cursor blocks in the
  doc). `EMBEDDING_MODEL` →
  [`embeddingModel`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.embeddingModel) picks
  the model; when omitted, the config falls back through
  [`getEmbeddingModelForProvider`](../catalog/packages/mcp/src/config.ts.md#getEmbeddingModelForProvider)
  /
  [`getDefaultModelForProvider`](../catalog/packages/mcp/src/config.ts.md#getDefaultModelForProvider),
  which is why the OpenAI block needs no `EMBEDDING_MODEL` but the VoyageAI block pins
  `voyage-code-3`.
- **Provider-specific keys** — `VOYAGEAI_API_KEY` →
  [`voyageaiApiKey`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.voyageaiApiKey),
  `GEMINI_API_KEY` →
  [`geminiApiKey`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.geminiApiKey),
  `OLLAMA_HOST` →
  [`ollamaHost`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.ollamaHost) (with
  `EMBEDDING_MODEL=nomic-embed-text` and no cloud key, since Ollama runs locally).

The doc's closing tip — prefer [global environment variables](environment-variables.md) over
per-client `env` blocks — works precisely because resolution is centralized in `createMcpConfig()`:
the server reads `process.env` regardless of which config file put the values there.

## Why it matters / when it applies
This is the seam that makes Claude Context "an AI assistant plugin." Because the whole surface is one
stdio command plus env vars, adding a new host (the "Other MCP Clients" block just runs the bare
`npx` command) requires no code — only telling that host how to spawn the process and pass
environment. It also localizes every decision that changes behavior (which embedding provider, which
vector DB, which model) into `ContextMcpConfig`, so the same server binary serves OpenAI-on-Zilliz,
Voyage-on-Zilliz, or Ollama-on-local without rebuilds.

## Connections
**Code concepts:** [MCP server configuration resolution](../concepts/packages-mcp-src-config.ts.md) ·
[MCP tools (index/search/clear/status)](../concepts/packages-mcp-src-handlers.ts.md) ·
[Embedding base contract](../concepts/packages-core-src-embedding-base-embedding.ts.md) ·
[OpenAI](../concepts/packages-core-src-embedding-openai-embedding.ts.md) /
[VoyageAI](../concepts/packages-core-src-embedding-voyageai-embedding.ts.md) /
[Gemini](../concepts/packages-core-src-embedding-gemini-embedding.ts.md) /
[Ollama](../concepts/packages-core-src-embedding-ollama-embedding.ts.md) providers ·
[VectorDatabase contract](../concepts/packages-core-src-vectordb-types.ts.md) ·
[Zilliz Cloud provisioning](../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)

**Module catalogs:** [`packages/mcp/src/config.ts`](../catalog/packages/mcp/src/config.ts.md) ·
[`packages/mcp/src/index.ts`](../catalog/packages/mcp/src/index.ts.md)

**Related doc-concepts:** [Index-then-search workflow](quickstart-index-then-search-workflow.md)

## Source
[`docs/getting-started/quick-start.md`](../../../../raw/code/claude-context/docs/getting-started/quick-start.md)
— "1-Minute Setup for Claude Code" and "Alternative Quick Setups".
