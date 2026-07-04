---
title: The graphify-out artifacts and graph format
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# The graphify-out artifacts and graph format

## Definition
A single `/graphify .` run produces three files under `graphify-out/`: **`graph.html`** (open in any browser — click nodes, filter, search), **`GRAPH_REPORT.md`** (the highlights), and **`graph.json`** (the full graph, queryable anytime without re-reading files). `graph.json` uses NetworkX's node-link format: each node has `id`, `label`, `file_type`, `source_file`; each edge has `source`, `target`, `relation`, `confidence`, optional `confidence_score`, and `source_file`. `graphify-out/` is meant to be committed so a whole team starts with the map.

## In graphify (grounded)
Artifacts are written by `export.py`:
- `graph.json` — [`to_json`](../catalog/graphify/export.md#to_json).
- `graph.html` — [`to_html`](../catalog/graphify/export.md#to_html) / [`generate_html`](../catalog/graphify/export.md#generate_html), capped at [`MAX_NODES_FOR_VIZ`](../catalog/graphify/export.md#MAX_NODES_FOR_VIZ) nodes (the README's ">5000 nodes / `--no-viz`" note).
- Optional exports: `--svg` [`to_svg`](../catalog/graphify/export.md#to_svg), `--graphml` [`to_graphml`](../catalog/graphify/export.md#to_graphml), `--obsidian` [`to_obsidian`](../catalog/graphify/export.md#to_obsidian), and Neo4j/FalkorDB via [`to_cypher`](../catalog/graphify/export.md#to_cypher) + [`push_to_neo4j`](../catalog/graphify/export.md#push_to_neo4j) / [`push_to_falkordb`](../catalog/graphify/export.md#push_to_falkordb).
- `GRAPH_REPORT.md` is produced by the report stage (see [god-nodes-report](god-nodes-report.md)).
- Where `graphify-out/` lives is resolved by [`GRAPHIFY_OUT`](../catalog/graphify/paths.md#GRAPHIFY_OUT) / [`out_path`](../catalog/graphify/paths.md#out_path) in `paths.py`; `manifest.json` keys are stored relative so committing is portable.

## Why it matters / when it applies
These three files are the persistent, compounding artifact that replaces re-reading raw files on every question — the compile-once, query-many core of graphify's value. Committing them means every teammate's assistant reads the graph immediately instead of rebuilding it.

## Connections
- Code concepts: [export](../concepts/graphify-export.md), [paths](../concepts/graphify-paths.md), [multigraph_compat](../concepts/graphify-multigraph_compat.md)
- Module catalogs: [export](../catalog/graphify/export.md), [paths](../catalog/graphify/paths.md), [report](../catalog/graphify/report.md)
- Related doc-concepts: [extraction-schema](extraction-schema.md), [god-nodes-report](god-nodes-report.md), [graph-query-interface](graph-query-interface.md), [node-summaries](node-summaries.md)

## Source
Extracted from `README.md` and `docs/how-it-works.md` ("The graph format") (kept in place).
