---
title: File-level node summaries (RFC)
type: doc-concept
provenance: doc
source: docs/node-summaries-rfc.md
updated: 2026-07-04
status: fresh
---
# File-level node summaries (RFC)

## Definition
A proposal (not yet implemented) to attach a compact, bounded summary (one sentence / ~200–300 chars) to file-level graph nodes, so an AI agent can decide whether to open a file without re-reading it. Summaries would be generated **deterministically first** from existing local signal — module docstrings, top comments, exported symbols, imports, relation counts, community/hub context — preserving graphify's offline default, with an opt-in LLM backend left as a follow-up. Two storage options are weighed: **Option A**, a `summary` attribute on file nodes inside `graph.json`; **Option B**, a sidecar `node-summaries.json` keyed by node ID.

## In graphify (grounded)
The RFC is a design doc, so it names surfaces rather than new symbols; it maps onto existing code as the *places summaries would appear*:
- Displayed in `graphify explain` — the node-lookup handler [`_tool_get_node`](../catalog/graphify/serve.md#_build_server._tool_get_node) in `serve.py`, and included in MCP node lookup.
- Optionally returned under a budget by `graphify query` — [`_tool_query_graph`](../catalog/graphify/serve.md#_build_server._tool_query_graph).
- Generated from the same node metadata (`label`, `source_file`, `file_type`) that [`to_json`](../catalog/graphify/export.md#to_json) already writes.
> [!inferred] No `summarize` / `--summarize-nodes` symbol exists in the current catalog — the RFC is a proposal, and the `graphify summarize` / `graphify . --summarize-nodes` flows it sketches are not yet in the code.

## Why it matters / when it applies
The RFC directly addresses the survey's central question — how a persistent artifact lets an agent navigate without re-reading source. It is graphify explicitly reasoning about the same token-saving, decide-before-you-open goal the [token benchmark](token-benchmark.md) measures, and about where synthesized prose should live relative to the raw graph.

## Connections
- Code concepts: [serve](../concepts/graphify-serve.md), [export](../concepts/graphify-export.md)
- Module catalogs: [serve](../catalog/graphify/serve.md), [export](../catalog/graphify/export.md)
- Related doc-concepts: [output-artifacts](output-artifacts.md), [graph-query-interface](graph-query-interface.md), [token-benchmark](token-benchmark.md)

## Source
Extracted from `docs/node-summaries-rfc.md` (kept in place).
