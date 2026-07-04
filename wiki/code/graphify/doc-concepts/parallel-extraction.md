---
title: Parallel extraction
type: doc-concept
provenance: doc
source: docs/how-it-works.md
updated: 2026-07-04
status: fresh
---
# Parallel extraction

## Definition
graphify parallelizes both extraction passes. Code files are extracted with a `ProcessPoolExecutor` — genuine multiprocessing that bypasses Python's GIL (about 1.66x faster than sequential on 84 code files). Doc/paper/image batches are dispatched as parallel LLM subagents. This is what keeps a large corpus fast even though every file is parsed or read.

## In graphify (grounded)
- The code-side parallelism is `extract.py`: [`_extract_parallel`](../catalog/graphify/extract.md#_extract_parallel) runs the process pool, with [`_extract_sequential`](../catalog/graphify/extract.md#_extract_sequential) as the fallback and [`_extract_single_file`](../catalog/graphify/extract.md#_extract_single_file) as the per-file unit of work.
- Worker count is tunable via the `--max-workers` flag / `GRAPHIFY_MAX_WORKERS` env var.
- The doc/paper/image side (Pass 3) fans out subagents in the assistant; `--max-concurrency` caps how many LLM calls run at once (useful for local inference).

## Why it matters / when it applies
Parallel AST extraction is what makes graphify practical on real repos — the local, no-API code pass scales with cores, so building the initial graph over hundreds of files stays interactive. On memory- or rate-limited setups the `--max-workers` / `--max-concurrency` levers trade throughput for resource headroom.

## Connections
- Code concepts: [extract](../concepts/graphify-extract.md)
- Module catalogs: [extract](../catalog/graphify/extract.md)
- Related doc-concepts: [three-pass-extraction](three-pass-extraction.md), [content-hash-cache](content-hash-cache.md)

## Source
Extracted from `docs/how-it-works.md` ("Parallel extraction") (kept in place).
