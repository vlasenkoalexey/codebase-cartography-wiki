---
title: Work memory and reflection
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Work memory and reflection

## Definition
graphify can remember how questions turned out and feed that back into future answers. `graphify save-result` records a Q&A outcome (`useful`, `dead_end`, or `corrected`) into `graphify-out/memory/`. `graphify reflect` then aggregates those outcomes into `reflections/LESSONS.md` and, with `--graph`, writes a work-memory overlay (`.graphify_learning.json`) that tags nodes preferred/tentative/contested with recency-weighted provenance — so `graphify explain`/`query` later show a "Lesson:" hint, flagged "code changed — re-verify" when the underlying source has moved on.

## In graphify (grounded)
- Recording an outcome is [`save_query_result`](../catalog/graphify/ingest.md#save_query_result) (outcomes enumerated in [`OUTCOMES`](../catalog/graphify/ingest.md#OUTCOMES)).
- Aggregation is `reflect.py`: [`reflect`](../catalog/graphify/reflect.md#reflect) reads the memory docs ([`load_memory_docs`](../catalog/graphify/reflect.md#load_memory_docs) / [`parse_memory_doc`](../catalog/graphify/reflect.md#parse_memory_doc)), rolls them up with [`aggregate_lessons`](../catalog/graphify/reflect.md#aggregate_lessons), and renders [`render_lessons_md`](../catalog/graphify/reflect.md#render_lessons_md). `--if-stale` short-circuits via [`lessons_fresh`](../catalog/graphify/reflect.md#lessons_fresh).
- The graph overlay is [`build_learning_overlay`](../catalog/graphify/reflect.md#build_learning_overlay) / [`write_learning_sidecar`](../catalog/graphify/reflect.md#write_learning_sidecar); the "code changed — re-verify" flag comes from a stored [`_code_fingerprint`](../catalog/graphify/reflect.md#_code_fingerprint) compared on load.

## Why it matters / when it applies
Reflection is graphify's answer to a compounding knowledge base: not just the structural graph, but a learned layer over it that accumulates which nodes proved useful and which were dead ends — and self-invalidates when the code moves. It is the tool's own instance of the survey's "explorations should compound like ingests" principle.

## Connections
- Code concepts: [reflect](../concepts/graphify-reflect.md)
- Module catalogs: [reflect](../catalog/graphify/reflect.md), [ingest](../catalog/graphify/ingest.md)
- Related doc-concepts: [graph-query-interface](graph-query-interface.md), [always-on-graph](always-on-graph.md)

## Source
Extracted from `README.md` ("Full command reference" — `save-result` / `reflect`) (kept in place).
