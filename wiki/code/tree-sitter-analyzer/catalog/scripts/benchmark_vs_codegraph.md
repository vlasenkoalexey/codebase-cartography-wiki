---
title: 'Module: scripts/benchmark_vs_codegraph.py'
type: catalog
provenance: extracted
module: scripts/benchmark_vs_codegraph.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.benchmark_vs_codegraph`/
symbols:
  generate_report: generate_report().
  benchmark_search_symbol: benchmark_search_symbol().
  ComparisonRow: ComparisonRow#
  run_synthetic_benchmark: run_synthetic_benchmark().
  PROJECT_ROOT: PROJECT_ROOT.
  ComparisonRow.delta: ComparisonRow#delta.
  run_capability_comparison: run_capability_comparison().
  BenchmarkResult.tool_calls: BenchmarkResult#tool_calls.
  ComparisonRow.metric: ComparisonRow#metric.
  BenchmarkResult: BenchmarkResult#
  ComparisonRow.codegraph: ComparisonRow#codegraph.
  ComparisonRow.our_value: ComparisonRow#our_value.
  BenchmarkResult.query: BenchmarkResult#query.
  BenchmarkResult.total_time_s: BenchmarkResult#total_time_s.
  BenchmarkResult.found_symbols: BenchmarkResult#found_symbols.
  BenchmarkResult.expected_symbols: BenchmarkResult#expected_symbols.
  BENCHMARK_QUERIES: BENCHMARK_QUERIES.
  BenchmarkResult.tokens_approx: BenchmarkResult#tokens_approx.
  BenchmarkResult.notes: BenchmarkResult#notes.
---
# Module: [`scripts/benchmark_vs_codegraph.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py)

## Classes
### `BenchmarkResult`
- def: [`scripts/benchmark_vs_codegraph.py:23`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py#L23)
- signature: `class BenchmarkResult:`
- members:
  - `expected_symbols` — [`L29`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py#L29)
  - `found_symbols` — [`L28`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py#L28)
  - `notes` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py#L30)
  - `query` — [`L24`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py#L24)
  - `tokens_approx` — [`L27`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py#L27)
  - `tool_calls` — [`L25`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py#L25)
  - `total_time_s` — [`L26`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py#L26)
- used by: [`benchmark_search_symbol`](benchmark_vs_codegraph.md#benchmark_search_symbol)

### `ComparisonRow`
- def: [`scripts/benchmark_vs_codegraph.py:34`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py#L34)
- signature: `class ComparisonRow:`
- members:
  - `codegraph` — [`L36`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py#L36)
  - `delta` — [`L38`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py#L38)
  - `metric` — [`L35`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py#L35)
  - `our_value` — [`L37`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py#L37)
- used by: [`generate_report`](benchmark_vs_codegraph.md#generate_report), [`run_capability_comparison`](benchmark_vs_codegraph.md#run_capability_comparison)

## Functions
- `benchmark_search_symbol(query_text: str, expected: list[str])` — [`L111`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py#L111) — Simulate what an agent would do with our tools to answer a question.
- `generate_report()` — [`L237`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py#L237)
- `run_capability_comparison()` — [`L186`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py#L186) — Compare feature parity between CodeGraph and tree-sitter-analyzer.
- `run_synthetic_benchmark()` — [`L144`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py#L144) — Run benchmark without MCP overhead, just measure raw analysis speed.

## Module values
- `BENCHMARK_QUERIES` — [`L41`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py#L41)
- `PROJECT_ROOT` — [`L19`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_vs_codegraph.py#L19)

