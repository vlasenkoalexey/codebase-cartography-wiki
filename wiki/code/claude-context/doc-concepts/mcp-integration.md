---
title: MCP integration
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# MCP integration

## Definition
The Model Context Protocol (MCP) is the recommended and headline way to use Claude Context: the
`@zilliz/claude-context-mcp` package is a stdio MCP server that any MCP-compatible client — Claude
Code, Cursor, Gemini CLI, Codex, Windsurf, VS Code, Cline, and more — can register (typically as
`npx @zilliz/claude-context-mcp@latest` with a couple of env vars). Once registered, the agent can
index a codebase and search it in natural language ("Index this codebase", then "Find functions that
handle user authentication"). The README lists four tools the server exposes.

## In claude-context (grounded)
The server is [`ContextMcpServer`](../catalog/packages/mcp/src/index.ts.md#ContextMcpServer); its
[`setupTools`](../catalog/packages/mcp/src/index.ts.md#ContextMcpServer.setupTools) registers the tool
set and [`start`](../catalog/packages/mcp/src/index.ts.md#ContextMcpServer.start) runs it over stdio
from [`main`](../catalog/packages/mcp/src/index.ts.md#main). The four README tools map one-to-one to
handlers on [`ToolHandlers`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers):
- `index_codebase` → [`handleIndexCodebase`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.handleIndexCodebase)
- `search_code` → [`handleSearchCode`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.handleSearchCode)
- `clear_index` → [`handleClearIndex`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.handleClearIndex)
- `get_indexing_status` → [`handleGetIndexingStatus`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.handleGetIndexingStatus)

Configuration comes entirely from environment variables (`OPENAI_API_KEY`, `MILVUS_ADDRESS`,
`MILVUS_TOKEN`, …), resolved by [`createMcpConfig`](../catalog/packages/mcp/src/config.ts.md#createMcpConfig)
into a [`ContextMcpConfig`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig); the provider
choice is [`ContextMcpConfig.embeddingProvider`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig.embeddingProvider),
with [`getEmbeddingModelForProvider`](../catalog/packages/mcp/src/config.ts.md#getEmbeddingModelForProvider)
picking the default model. Indexing status (progress %, indexed/failed state) that
`get_indexing_status` reports is persisted across restarts by the
[`SnapshotManager`](../catalog/packages/mcp/src/snapshot.ts.md#SnapshotManager).

## Why it matters / when it applies
MCP is the seam that turns the core engine into a capability the agent can call mid-conversation —
no bespoke integration per client, just the standard protocol over stdio. It is the intended entry
point for the whole system: the README frames the core package and VSCode extension as "other ways to
use" it. Env-var config keeps secrets and backend choice out of code and lets each client pass its own.

## Connections
- Code concepts: [MCP tool handlers](../concepts/packages-mcp-src-handlers.ts.md),
  [MCP env-var config](../concepts/packages-mcp-src-config.ts.md),
  [MCP snapshot persistence](../concepts/packages-mcp-src-snapshot.ts.md),
  [MCP background sync](../concepts/packages-mcp-src-sync.ts.md),
  [Context orchestrator](../concepts/packages-core-src-context.ts.md).
- Module catalogs: [mcp/index.ts](../catalog/packages/mcp/src/index.ts.md),
  [mcp/handlers.ts](../catalog/packages/mcp/src/handlers.ts.md),
  [mcp/config.ts](../catalog/packages/mcp/src/config.ts.md).
- Related doc-concepts: [Semantic code search](semantic-code-search.md), [Hybrid
  search](hybrid-search.md), [Architecture & packages](architecture-packages.md),
  [Embedding & vector backends](embedding-and-vector-backends.md).

## Source
Extracted from `README.md` (kept in place).
