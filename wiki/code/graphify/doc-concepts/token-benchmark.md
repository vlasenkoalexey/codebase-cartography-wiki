---
title: The token-reduction benchmark
type: doc-concept
provenance: doc
source: docs/how-it-works.md
updated: 2026-07-04
status: fresh
---
# The token-reduction benchmark

## Definition
graphify's value proposition is measured, not asserted. The first run extracts and builds the graph (this costs tokens); every subsequent query reads the compact graph instead of raw files, and that is where savings compound. On a mixed corpus (Karpathy repos + 5 papers + 4 images, 52 files) it reports **71.5x fewer tokens per query** vs reading raw files. Reduction scales with corpus size — 6 files is ~1x (the graph's value there is structural clarity, not compression); at 52 files the savings compound.

## In graphify (grounded)
- The benchmark is `benchmark.py`: [`run_benchmark`](../catalog/graphify/benchmark.md#run_benchmark) compares whole-corpus token cost against per-query subgraph cost ([`_query_subgraph_tokens`](../catalog/graphify/benchmark.md#_query_subgraph_tokens)), and [`print_benchmark`](../catalog/graphify/benchmark.md#print_benchmark) renders the table.
- The "compact graph per query" side of the comparison is the same subgraph engine the [query interface](graph-query-interface.md) uses.
- Each `worked/` folder in the repo ships the raw inputs and actual output so the numbers are reproducible.

## Why it matters / when it applies
This benchmark is the crux of graphify's comparability to other code-comprehension tools: it quantifies the RAG-vs-persistent-graph trade the survey studies — pay once to compile the graph, then answer many questions cheaply — and it honestly notes the regime (small corpora) where the graph buys clarity rather than compression.

## Connections
- Code concepts: [serve](../concepts/graphify-serve.md)
- Module catalogs: [benchmark](../catalog/graphify/benchmark.md), [serve](../catalog/graphify/serve.md)
- Related doc-concepts: [graph-query-interface](graph-query-interface.md), [output-artifacts](output-artifacts.md)

## Source
Extracted from `docs/how-it-works.md` ("Token benchmark") (kept in place).
