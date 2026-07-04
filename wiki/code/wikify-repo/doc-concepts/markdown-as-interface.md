---
title: Markdown as the interface — grep-native retrieval, no DB, no embeddings
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Markdown as the interface — grep-native retrieval, no DB, no embeddings

## Definition
The storage-format decision: the consumer is an **AI agent**, and agents already read
markdown and retrieve with `grep`/`ripgrep` natively — no query language, no graph
runtime, no vector index, no MCP server. **The output *is* the interface.** Drop
`wiki/` into a repo and any agent (Claude Code, Codex, Antigravity) answers from it
with zero adapter. This is the retrieval axis of the README's comparison table:
wikify-repo is "`grep` + `index.md`, no embeddings, no DB" where the graph tools need
a runtime to query.

## In wikify-repo (grounded)
The wiki is pure markdown, written by the deterministic assemble/coverage stages —
nothing else is shipped. [`write_top_index`](../catalog/wikify/assemble.md#write_top_index)
and [`write_repo_index`](../catalog/wikify/assemble.md#write_repo_index) produce the
`index.md` catalog an agent reads first; at this scale, "index + `grep`" replaces
embedding-based RAG. The rare short-hop navigation a graph DB is good at is instead
**materialized into the pages**: [`render_catalog`](../catalog/wikify/coverage.md#render_catalog)
(emitted by [`emit_catalogs`](../catalog/wikify/coverage.md#emit_catalogs)) writes,
per module, each symbol's `uses` / `used by` as relative markdown links — a grep-able
adjacency list. [`class_connections`](../catalog/wikify/coverage.md#class_connections)
rolls member-granular edges up to true class→class links. The
[`CoverageReport`](../catalog/wikify/coverage.md#CoverageReport) makes "whole repo
represented" a measured property in `index.md`.

The honest tradeoff (design decision 4): a graph DB wins at arbitrary *transitive*
queries ("every transitive caller of X"). wikify's answer is to **materialize** the
common ones (per-symbol uses-by, per-module catalogs) so frequent questions are
already answered as text, and the rare deep query drops to the pinned source.
Transitive traversal is an *ingestion-time* need (synthesis walks the graph once and
writes the conclusion down); at query time there is nothing for an index to
accelerate.

## Why it matters / when it applies
Ownership and zero-dependency retrieval: the result is plain markdown you own in your
own git repo — offline, git-diffable — that any agent reads with **nothing but
`grep`**. For *agent retrieval of internals knowledge*, materialized markdown beats a
live graph you have to query. Notably, to *consume* a wiki you don't even need the
`wikify` tool — just the committed markdown and a few lines in `CLAUDE.md`/`AGENTS.md`.

## Connections
- Code concepts: [Coverage](../concepts/wikify-coverage.md) — the materialized catalogs + adjacency lists.
- Module catalogs: [assemble](../catalog/wikify/assemble.md), [coverage](../catalog/wikify/coverage.md).
- Related doc-concepts: [concept-driven-synthesis-and-coverage](concept-driven-synthesis-and-coverage.md), [tool-positioning-comparison](tool-positioning-comparison.md), [python-llm-split](python-llm-split.md).

## Source
Extracted from `README.md` ("Why use a wiki as the storage format"; "Answer from a
wiki — no install needed"), with design decision 4 from `docs/design.md` ("Pure
markdown product"). Kept in place.
