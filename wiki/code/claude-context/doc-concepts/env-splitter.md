---
title: Splitter selection & file filters
type: doc-concept
provenance: doc
source: docs/getting-started/environment-variables.md
updated: 2026-07-04
status: fresh
---
# Splitter selection & file filters

## Definition
`SPLITTER_TYPE` chooses how source files are cut into chunks before embedding: `ast` (default —
tree-sitter, syntax-aware) or `langchain` (a generic recursive character splitter fallback). Two
companion variables control *which* files get chunked at all: `CUSTOM_EXTENSIONS` adds file extensions
to include (comma-separated, e.g. `.vue,.svelte,.astro`) and `CUSTOM_IGNORE_PATTERNS` adds ignore
globs (e.g. `temp/**,*.backup`).

## In claude-context (grounded)
The splitter kind is the string union
[`RequestSplitterType`](../catalog/packages/mcp/src/config.ts.md#RequestSplitterType) (`'ast' | 'langchain'`).
In the MCP server the choice is **per index request**, not a server-wide env field: a raw value is
normalized by [`resolveRequestSplitterType`](../catalog/packages/mcp/src/splitter.ts.md#resolveRequestSplitterType)
(guarded by [`isRequestSplitterType`](../catalog/packages/mcp/src/splitter.ts.md#isRequestSplitterType))
and turned into a concrete splitter by
[`createRequestSplitter`](../catalog/packages/mcp/src/splitter.ts.md#createRequestSplitter).

> [!inferred]
> The `SPLITTER_TYPE` environment variable itself is read in the standalone `examples/basic-usage`
> entrypoint (`envManager.get('SPLITTER_TYPE')`), not in the MCP server's
> [`createMcpConfig`](../catalog/packages/mcp/src/config.ts.md#createMcpConfig) — so it is not a
> `ContextMcpConfig` field. Regardless of entry point the default is `ast`: a fresh
> [`Context`](../concepts/packages-core-src-context.ts.md) constructs an `AstCodeSplitter` when no
> splitter is supplied, and [`Context.updateSplitter`](../catalog/packages/core/src/context.ts.md#Context.updateSplitter)
> swaps it later. [`Context.getSplitterInfo`](../catalog/packages/core/src/context.ts.md#Context.getSplitterInfo)
> reports the active splitter's type and supported languages.

The file filters are read in the core layer, again outside `ContextMcpConfig`:
[`Context.getCustomExtensionsFromEnv`](../catalog/packages/core/src/context.ts.md#Context.getCustomExtensionsFromEnv)
parses `CUSTOM_EXTENSIONS` and
[`Context.getCustomIgnorePatternsFromEnv`](../catalog/packages/core/src/context.ts.md#Context.getCustomIgnorePatternsFromEnv)
parses `CUSTOM_IGNORE_PATTERNS`, each splitting on commas and merging into the built-in
include/ignore sets used during a codebase walk.

## Why it matters / when it applies
`ast` gives semantically coherent chunks (whole functions/classes) for the ~9 languages the AST
splitter supports; `langchain` is the escape hatch for languages or files the AST path can't parse. The
two filter variables are how you extend indexing to framework file types (`.vue`, `.svelte`) or exclude
generated/vendor directories without editing code — they matter whenever a repo's important files are
being skipped or its noise is being indexed.

## Connections
- Code concepts: [AST-aware chunking](../concepts/packages-core-src-splitter-ast-splitter.ts.md) · [Splitter contract + LangChain fallback](../concepts/packages-core-src-splitter-index.ts.md) · [Context orchestrator](../concepts/packages-core-src-context.ts.md)
- Module catalogs: [splitter.ts (MCP)](../catalog/packages/mcp/src/splitter.ts.md) · [config.ts](../catalog/packages/mcp/src/config.ts.md) · [context.ts](../catalog/packages/core/src/context.ts.md)
- Related doc-concepts: [Global config & env-var resolution](env-global-config.md) · [Search & indexing tuning knobs](env-tuning-knobs.md)

## Source
Extracted from `docs/getting-started/environment-variables.md` (kept in place).
