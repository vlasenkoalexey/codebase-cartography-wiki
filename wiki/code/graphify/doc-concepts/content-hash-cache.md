---
title: The SHA256 content cache
type: doc-concept
provenance: doc
source: docs/how-it-works.md
updated: 2026-07-04
status: fresh
---
# The SHA256 content cache

## Definition
Every extracted file is fingerprinted by content hash. On a re-run, unchanged files are skipped entirely — only new or modified files go back through extraction. The cache lives in `graphify-out/cache/`. This is what makes `--update` incremental and keeps the post-commit hook cheap (AST-only, no API cost) on a repo that barely changed.

## In graphify (grounded)
- Fingerprinting and the cached/uncached split are `cache.py`: [`file_hash`](../catalog/graphify/cache.md#file_hash) computes the SHA256, and [`check_semantic_cache`](../catalog/graphify/cache.md#check_semantic_cache) partitions files into cached vs uncached before Pass 3.
- Results are persisted and reloaded via [`save_semantic_cache`](../catalog/graphify/cache.md#save_semantic_cache) / [`save_cached`](../catalog/graphify/cache.md#save_cached) and [`load_cached`](../catalog/graphify/cache.md#load_cached); [`cache_dir`](../catalog/graphify/cache.md#cache_dir) resolves the `graphify-out/cache/` location.
- Stale entries are swept by [`prune_semantic_cache`](../catalog/graphify/cache.md#prune_semantic_cache) / [`_cleanup_stale_ast_entries`](../catalog/graphify/cache.md#_cleanup_stale_ast_entries); the whole cache clears with [`clear_cache`](../catalog/graphify/cache.md#clear_cache).
- The `detect.py` incremental scan [`detect_incremental`](../catalog/graphify/detect.md#detect_incremental) uses the stat/hash index to decide what actually changed.

## Why it matters / when it applies
Content-hash caching is what turns a one-time expensive build into a cheap, continuously-current graph — the same "compile once, keep current, rebuild only the delta" property the survey cares about. It is what lets `graphify hook install` rebuild after every commit without re-spending tokens.

## Connections
- Code concepts: [cache](../concepts/graphify-cache.md), [detect](../concepts/graphify-detect.md), [watch](../concepts/graphify-watch.md)
- Module catalogs: [cache](../catalog/graphify/cache.md), [detect](../catalog/graphify/detect.md)
- Related doc-concepts: [three-pass-extraction](three-pass-extraction.md), [always-on-graph](always-on-graph.md), [parallel-extraction](parallel-extraction.md)

## Source
Extracted from `docs/how-it-works.md` ("SHA256 cache"); the `cache.py` responsibility is corroborated by `ARCHITECTURE.md` (kept in place).
