---
title: Semantic code search
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Semantic code search

## Definition
Claude Context is an MCP plugin that gives AI coding agents (Claude Code and others) semantic
search over an *entire* codebase. Instead of the agent doing multi-round file discovery — or the
caller stuffing whole directories into the model's context on every request — the codebase is
embedded once into a vector database, and each query retrieves only the handful of relevant chunks.
The README's two headline claims: "your entire codebase as context" (find relevant code across
millions of lines with no multi-round discovery) and "cost-effective for large codebases" (only the
related code enters the context window, so token cost stays bounded).

## In claude-context (grounded)
The search entry point is [`Context.semanticSearch`](../catalog/packages/core/src/context.ts.md#Context.semanticSearch)
on the core [`Context`](../catalog/packages/core/src/context.ts.md#Context) orchestrator — the README's
`context.semanticSearch('./your-project', 'vector database operations', 5)` example maps directly to
it. Indexing is the mirror path, [`Context.indexCodebase`](../catalog/packages/core/src/context.ts.md#Context.indexCodebase),
which walks the code files, chunks them, embeds each chunk, and inserts the vectors. A search returns
[`VectorSearchResult`](../catalog/packages/core/src/vectordb/types.ts.md#VectorSearchResult) records
carrying `relativePath`, `startLine`/`endLine`, `score`, and `content` — exactly the fields the
README prints per hit. Overlapping hits are collapsed by
[`Context.deduplicateResults`](../catalog/packages/core/src/context.ts.md#Context.deduplicateResults).

The README quantifies the payoff: the controlled evaluation reports ~40% token reduction at
equivalent retrieval quality versus loading directories directly.

## Why it matters / when it applies
This is the whole value proposition: for a large codebase, exhaustive grep/read is slow and
expensive, and blindly loading directories burns tokens. Semantic retrieval turns a natural-language
question ("find functions that handle user authentication") into the ten relevant chunks, keeping the
agent's context small and its answers grounded. It applies whenever the codebase is too big to fit —
or too expensive to repeatedly load — into the model's window.

## Connections
- Code concepts: [Context orchestrator](../concepts/packages-core-src-context.ts.md) — the index/search
  pipeline; [VectorDatabase contract](../concepts/packages-core-src-vectordb-types.ts.md) — the result
  shape.
- Module catalogs: [context.ts](../catalog/packages/core/src/context.ts.md),
  [vectordb/types.ts](../catalog/packages/core/src/vectordb/types.ts.md).
- Related doc-concepts: [Hybrid search](hybrid-search.md), [Architecture &
  packages](architecture-packages.md), [MCP integration](mcp-integration.md).

## Source
Extracted from `README.md` (kept in place).
