---
title: God nodes and the graph report
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# God nodes and the graph report

## Definition
`GRAPH_REPORT.md` is graphify's human-readable synthesis of the graph. Its highlights are **god nodes** (the most-connected concepts, "everything flows through these"), **surprising connections** (links between things in different files/modules, ranked by how unexpected they are), **the "why"** (inline `# NOTE:`/`# WHY:`/`# HACK:` comments, docstrings, and design rationale extracted as separate nodes linked to the code they explain), **suggested questions** (4–5 the graph is uniquely positioned to answer), and **confidence tags** on every inferred relationship.

## In graphify (grounded)
- The analysis behind the report is `analyze.py`: [`god_nodes`](../catalog/graphify/analyze.md#god_nodes) ranks the hubs, [`surprising_connections`](../catalog/graphify/analyze.md#surprising_connections) (scored by [`_surprise_score`](../catalog/graphify/analyze.md#_surprise_score) / [`_cross_community_surprises`](../catalog/graphify/analyze.md#_cross_community_surprises)) finds the unexpected links, and [`suggest_questions`](../catalog/graphify/analyze.md#suggest_questions) drafts the questions.
- The "why" nodes come from rationale extraction — e.g. [`_extract_python_rationale`](../catalog/graphify/extract.md#_extract_python_rationale) in `extract.py` pulls `# NOTE:`/`# WHY:`/`# HACK:` comments as `rationale`-typed nodes.
- The markdown itself is rendered by [`generate`](../catalog/graphify/report.md#generate), which also surfaces AMBIGUOUS edges for review.

## Why it matters / when it applies
The report is the "read this first" surface for a codebase you don't know: god nodes tell you where to start, surprising connections point at hidden coupling, and the rationale nodes preserve the design "why" that source and docstrings usually lose. `--exclude-hubs` lets you suppress utility super-hubs so they don't dominate the god-node ranking.

## Connections
- Code concepts: [analyze](../concepts/graphify-analyze.md), [extract](../concepts/graphify-extract.md)
- Module catalogs: [analyze](../catalog/graphify/analyze.md), [report](../catalog/graphify/report.md)
- Related doc-concepts: [community-detection](community-detection.md), [confidence-labels](confidence-labels.md), [output-artifacts](output-artifacts.md), [graph-query-interface](graph-query-interface.md)

## Source
Extracted from `README.md` ("What's in the report") (kept in place).
