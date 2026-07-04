---
title: Architecture & packages
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Architecture & packages

## Definition
Claude Context is a monorepo built around three consumer-facing packages that all sit on top of one
core indexing engine. The README names them: **`@zilliz/claude-context-core`** (the indexing engine
with embedding + vector-database integration), the **VSCode Extension** (Semantic Code Search in the
IDE), and **`@zilliz/claude-context-mcp`** (the MCP server for AI-agent integration). A Chrome
extension also exists (marked "robust Chrome extension" on the roadmap). The core engine's pipeline is:
walk files → AST-chunk → embed → store in a vector DB → hybrid-search.

## In claude-context (grounded)
The engine is the [`Context`](../catalog/packages/core/src/context.ts.md#Context) class, wired from an
embedding provider, a vector database, and a code splitter — the exact three constructor inputs shown
in the README's core-package example. Its two public verbs are
[`indexCodebase`](../catalog/packages/core/src/context.ts.md#Context.indexCodebase) and
[`semanticSearch`](../catalog/packages/core/src/context.ts.md#Context.semanticSearch).

The README calls out four implementation details, each grounded in a subsystem:
- **Intelligent code chunking (AST):** [`AstCodeSplitter`](../catalog/packages/core/src/splitter/ast-splitter.ts.md#AstCodeSplitter),
  which splits on [`SPLITTABLE_NODE_TYPES`](../catalog/packages/core/src/splitter/ast-splitter.ts.md#SPLITTABLE_NODE_TYPES)
  and falls back via [`langchainFallback`](../catalog/packages/core/src/splitter/ast-splitter.ts.md#AstCodeSplitter.langchainFallback)
  when a language is unsupported. Both obey the [`Splitter`](../catalog/packages/core/src/splitter/index.ts.md#Splitter)
  contract and emit [`CodeChunk`](../catalog/packages/core/src/splitter/index.ts.md#CodeChunk)s; the
  choice is a [`SplitterType`](../catalog/packages/core/src/splitter/index.ts.md#SplitterType)
  (`AST` or `LANGCHAIN`).
- **Incremental indexing (Merkle trees):** [`MerkleDAG`](../catalog/packages/core/src/sync/merkle.ts.md#MerkleDAG)
  with [`compare`](../catalog/packages/core/src/sync/merkle.ts.md#MerkleDAG.compare) detects the
  added/removed/modified set, driven by
  [`FileSynchronizer.checkForChanges`](../catalog/packages/core/src/sync/synchronizer.ts.md#FileSynchronizer.checkForChanges)
  so only changed files are re-embedded.
- **Hybrid code search** — see [Hybrid search](hybrid-search.md).
- **Scalable / customizable** — the vector-DB and embedding backends below.

## Why it matters / when it applies
Separating a reusable core from three thin front-ends (MCP, VSCode, Chrome) is what lets the same
indexing engine serve an AI agent, an IDE, and a browser without duplicating the pipeline. AST
chunking keeps each embedded unit a coherent syntactic span (a function/class) rather than an
arbitrary character window; Merkle-based incremental sync keeps re-indexing cheap on large,
frequently-edited repos.

## Connections
- Code concepts: [Context orchestrator](../concepts/packages-core-src-context.ts.md),
  [AST splitter](../concepts/packages-core-src-splitter-ast-splitter.ts.md),
  [Splitter contract](../concepts/packages-core-src-splitter-index.ts.md),
  [Merkle-DAG change detection](../concepts/packages-core-src-sync-merkle.ts.md),
  [FileSynchronizer](../concepts/packages-core-src-sync-synchronizer.ts.md).
- Module catalogs: [context.ts](../catalog/packages/core/src/context.ts.md),
  [splitter/ast-splitter.ts](../catalog/packages/core/src/splitter/ast-splitter.ts.md),
  [sync/merkle.ts](../catalog/packages/core/src/sync/merkle.ts.md).
- Related doc-concepts: [Semantic code search](semantic-code-search.md),
  [Embedding & vector backends](embedding-and-vector-backends.md),
  [Hybrid search](hybrid-search.md), [MCP integration](mcp-integration.md).

## Source
Extracted from `README.md` (kept in place).
