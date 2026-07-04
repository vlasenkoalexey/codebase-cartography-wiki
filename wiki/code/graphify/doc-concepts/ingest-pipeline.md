---
title: The ingest pipeline
type: doc-concept
provenance: doc
source: ARCHITECTURE.md
updated: 2026-07-04
status: fresh
---
# The ingest pipeline

## Definition
graphify turns any input into a knowledge graph through a fixed, linear pipeline of stages, each a single pure function in its own module: `detect() → extract() → build_graph() → cluster() → analyze() → report() → export()`. Stages communicate only through plain Python dicts and NetworkX graphs — "no shared state, no side effects outside `graphify-out/`" — so the whole comprehension flow is a readable composition of one-responsibility modules.

## In graphify (grounded)
Each documented stage maps to a real entry point:
- **detect** — [`detect`](../catalog/graphify/detect.md#detect) filters a directory to the file list worth indexing (`collect_files` in the doc's table).
- **extract** — [`extract`](../catalog/graphify/extract.md#extract) turns one file into a `{nodes, edges}` dict.
- **build** — [`build`](../catalog/graphify/build.md#build) / [`build_from_json`](../catalog/graphify/build.md#build_from_json) merge extraction dicts into one `nx.Graph`.
- **cluster** — [`cluster`](../catalog/graphify/cluster.md#cluster) attaches a `community` to every node.
- **analyze** — [`god_nodes`](../catalog/graphify/analyze.md#god_nodes), [`surprising_connections`](../catalog/graphify/analyze.md#surprising_connections), [`suggest_questions`](../catalog/graphify/analyze.md#suggest_questions) produce the analysis dict.
- **report** — [`generate`](../catalog/graphify/report.md#generate) renders `GRAPH_REPORT.md`.
- **export** — [`to_json`](../catalog/graphify/export.md#to_json) / [`to_html`](../catalog/graphify/export.md#to_html) write the `graphify-out/` artifacts.

The stages are wired together by the CLI in `graphify/__main__.py`.

## Why it matters / when it applies
This staged, side-effect-free shape is what makes graphify comparable to other code-comprehension tools: ingestion is deterministic and inspectable, each stage can be re-run in isolation (e.g. `--cluster-only` re-runs only `cluster` → `analyze` → `report`), and the only durable output is markdown/JSON under `graphify-out/`.

## Connections
- Code concepts: [detect](../concepts/graphify-detect.md), [extract](../concepts/graphify-extract.md), [build](../concepts/graphify-build.md), [cluster](../concepts/graphify-cluster.md), [analyze](../concepts/graphify-analyze.md), [export](../concepts/graphify-export.md), [__main__](../concepts/graphify-__main__.md)
- Module catalogs: [detect](../catalog/graphify/detect.md), [extract](../catalog/graphify/extract.md), [build](../catalog/graphify/build.md), [cluster](../catalog/graphify/cluster.md), [analyze](../catalog/graphify/analyze.md), [report](../catalog/graphify/report.md), [export](../catalog/graphify/export.md)
- Related doc-concepts: [three-pass-extraction](three-pass-extraction.md), [extraction-schema](extraction-schema.md), [community-detection](community-detection.md), [god-nodes-report](god-nodes-report.md), [output-artifacts](output-artifacts.md)

## Source
Extracted from `ARCHITECTURE.md` (kept in place).
