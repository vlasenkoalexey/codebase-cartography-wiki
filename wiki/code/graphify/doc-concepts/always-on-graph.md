---
title: Keeping the graph always-on
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Keeping the graph always-on

## Definition
graphify has two mechanisms for staying current and being used by default. **Git hooks** (`graphify hook install`) rebuild the graph after every commit and checkout — AST-only, no API cost — and set up a merge driver so `graph.json` is union-merged instead of left with conflict markers. **Always-on assistant instructions** (`graphify claude install`, etc.) write a config file and, on platforms that support it, a PreToolUse hook that fires before search/read tool calls and nudges the assistant toward `graphify query` instead of grepping or reading files one by one.

## In graphify (grounded)
- Git hooks are `hooks.py`: [`install`](../catalog/graphify/hooks.md#install) embeds the current interpreter path into the post-commit/post-checkout scripts (so they fire in GUI clients and CI), with [`uninstall`](../catalog/graphify/hooks.md#uninstall) and [`status`](../catalog/graphify/hooks.md#status).
- The rebuild the hook triggers is the incremental, cache-backed path — see [content-hash-cache](content-hash-cache.md) and the file watcher [`watch`](../catalog/graphify/watch.md#watch) / [`check_update`](../catalog/graphify/watch.md#check_update) in `watch.py` (the `--watch` flag).
- The assistant-instruction installers (`claude install`, `codex install`, …) are per-platform commands in `__main__.py`; they write `CLAUDE.md`/`AGENTS.md`/`.cursor/rules` sections and PreToolUse hooks that point at the query path.

## Why it matters / when it applies
Auto-rebuild is what keeps the "compile once" graph from going stale — the maintenance the survey identifies as the reason humans abandon wikis is pushed onto a hook that never forgets. The always-on instructions close the loop: they make the assistant actually prefer the persistent graph over re-deriving answers from raw files each query.

## Connections
- Code concepts: [hooks](../concepts/graphify-hooks.md), [watch](../concepts/graphify-watch.md)
- Module catalogs: [hooks](../catalog/graphify/hooks.md), [watch](../catalog/graphify/watch.md)
- Related doc-concepts: [content-hash-cache](content-hash-cache.md), [graph-query-interface](graph-query-interface.md), [work-memory](work-memory.md)

## Source
Extracted from `README.md` ("Make your assistant always use the graph", "Team setup") (kept in place).
