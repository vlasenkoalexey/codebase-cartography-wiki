---
title: Index-then-search workflow
type: doc-concept
provenance: doc
source: raw/code/claude-context/docs/getting-started/quick-start.md
updated: 2026-07-04
status: fresh
---
# Index-then-search workflow

## Definition
Once the server is wired in, the Quick Start reduces usage to three natural-language prompts:
**"Index this codebase"**, then **"Check the indexing status"**, then a semantic query like
**"Find functions that handle user authentication."** This is the core interaction loop: you must
**build the index once** before search returns anything, and because indexing is asynchronous you
**poll status** in between. Search is semantic (embedding similarity), not grep — the third prompt is
phrased as intent, not a literal string.

## In claude-context (grounded)
Each prompt is the assistant invoking one MCP tool that the server registered in
[`setupTools`](../catalog/packages/mcp/src/index.ts.md#ContextMcpServer.setupTools); every tool is a
method on [`ToolHandlers`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers):

- **"Index this codebase"** →
  [`handleIndexCodebase`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.handleIndexCodebase).
  Rather than block the assistant while a large repo is chunked and embedded, it kicks off
  [`startBackgroundIndexing`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.startBackgroundIndexing)
  and returns immediately — which is exactly why the doc tells you to check status as a separate
  step. The actual work runs through the core pipeline
  [`Context.indexCodebase`](../catalog/packages/core/src/context.ts.md#Context.indexCodebase)
  (walk files → AST-chunk → embed → upsert to the vector DB).
- **"Check the indexing status"** →
  [`handleGetIndexingStatus`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.handleGetIndexingStatus).
  It reports progress from the persisted snapshot — the
  [`indexingPercentage`](../catalog/packages/mcp/src/config.ts.md#CodebaseInfoIndexing.indexingPercentage)
  of an in-flight
  [`CodebaseInfoIndexing`](../catalog/packages/mcp/src/config.ts.md#CodebaseInfoIndexing) entry, or a
  terminal [`CodebaseInfoIndexed`](../catalog/packages/mcp/src/config.ts.md#CodebaseInfoIndexed) /
  [`CodebaseInfoIndexFailed`](../catalog/packages/mcp/src/config.ts.md#CodebaseInfoIndexFailed) state.
  The status the user sees is this snapshot state machine surfaced back through the tool.
- **"Find functions that handle user authentication"** →
  [`handleSearchCode`](../catalog/packages/mcp/src/handlers.ts.md#ToolHandlers.handleSearchCode),
  which delegates to
  [`Context.semanticSearch`](../catalog/packages/core/src/context.ts.md#Context.semanticSearch): the
  query string is embedded with the *same* provider used at index time and matched against the vector
  DB. This is why the prompt is written as intent — retrieval is by embedding similarity over the
  indexed chunks, so it only returns meaningful hits *after* indexing has completed.

## Why it matters / when it applies
The ordering is a hard dependency, not a suggestion: search reads a collection that indexing writes,
so an un-indexed (or still-indexing) codebase yields nothing useful — hence the explicit
index → status → search sequence in the Quick Start. Understanding that the three prompts are three
distinct MCP tool calls (and that indexing is deliberately backgrounded with a pollable status)
explains the whole first-run experience and where to look when a search "finds nothing": check the
snapshot status before assuming the search is broken.

## Connections
**Code concepts:** [MCP tools (index/search/clear/status)](../concepts/packages-mcp-src-handlers.ts.md) ·
[Context orchestrator (index/search pipeline)](../concepts/packages-core-src-context.ts.md) ·
[Indexed-codebase snapshot persistence](../concepts/packages-mcp-src-snapshot.ts.md) ·
[AST-aware chunking](../concepts/packages-core-src-splitter-ast-splitter.ts.md) ·
[MCP background sync loop](../concepts/packages-mcp-src-sync.ts.md)

**Module catalogs:** [`packages/mcp/src/handlers.ts`](../catalog/packages/mcp/src/handlers.ts.md) ·
[`packages/core/src/context.ts`](../catalog/packages/core/src/context.ts.md) ·
[`packages/mcp/src/config.ts`](../catalog/packages/mcp/src/config.ts.md)

**Related doc-concepts:** [MCP server setup model (stdio + env-var config)](quickstart-mcp-server-setup.md)

## Source
[`docs/getting-started/quick-start.md`](../../../../raw/code/claude-context/docs/getting-started/quick-start.md)
— "Step 3: Start Using Claude Context".
