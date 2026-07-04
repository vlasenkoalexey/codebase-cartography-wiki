---
title: 'Module: scripts/benchmark_real_projects.py'
type: catalog
provenance: extracted
module: scripts/benchmark_real_projects.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.benchmark_real_projects`/
symbols:
  main: main().
  run_analysis._analyze: run_analysis()._analyze().
  BENCH_DIR: BENCH_DIR.
  clone_project: clone_project().
  run_analysis: run_analysis().
  CODEGRAPH_BASELINES: CODEGRAPH_BASELINES.
  OUR_PROJECTS: OUR_PROJECTS.
  BenchmarkRun: BenchmarkRun#
  BenchmarkRun.project: BenchmarkRun#project.
  BenchmarkRun.query: BenchmarkRun#query.
  BenchmarkRun.language: BenchmarkRun#language.
  BenchmarkRun.index_files: BenchmarkRun#index_files.
  BenchmarkRun.tool_calls_needed: BenchmarkRun#tool_calls_needed.
  BenchmarkRun.analysis_time_s: BenchmarkRun#analysis_time_s.
  BenchmarkRun.file_reads_needed: BenchmarkRun#file_reads_needed.
  BenchmarkRun.found_symbols: BenchmarkRun#found_symbols.
  BenchmarkRun.expected_symbols: BenchmarkRun#expected_symbols.
  BenchmarkRun.recall: BenchmarkRun#recall.
  BenchmarkRun.comparable_cg: BenchmarkRun#comparable_cg.
  BenchmarkRun.cg_tool_calls: BenchmarkRun#cg_tool_calls.
  BenchmarkRun.cg_time_s: BenchmarkRun#cg_time_s.
  BenchmarkRun.cg_file_reads: BenchmarkRun#cg_file_reads.
  count_source_files: count_source_files().
  BenchmarkRun.index_time_s: BenchmarkRun#index_time_s.
  BenchmarkRun.index_symbols: BenchmarkRun#index_symbols.
  BenchmarkRun.tokens_approx: BenchmarkRun#tokens_approx.
---
# Module: [`scripts/benchmark_real_projects.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py)

## Classes
### `BenchmarkRun`
- def: [`scripts/benchmark_real_projects.py:124`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L124)
- signature: `class BenchmarkRun:`
- members:
  - `analysis_time_s` — [`L132`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L132)
  - `cg_file_reads` — [`L141`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L141)
  - `cg_time_s` — [`L140`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L140)
  - `cg_tool_calls` — [`L139`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L139)
  - `comparable_cg` — [`L138`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L138)
  - `expected_symbols` — [`L136`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L136)
  - `file_reads_needed` — [`L133`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L133)
  - `found_symbols` — [`L135`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L135)
  - `index_files` — [`L129`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L129)
  - `index_symbols` — [`L130`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L130)
  - `index_time_s` — [`L128`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L128)
  - `language` — [`L127`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L127)
  - `project` — [`L125`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L125)
  - `query` — [`L126`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L126)
  - `recall` — [`L137`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L137)
  - `tokens_approx` — [`L134`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L134)
  - `tool_calls_needed` — [`L131`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L131)
- used by: [`main`](benchmark_real_projects.md#main)

## Functions
- `_analyze()` — [`L179`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L179)
- `clone_project(name: str, url: str)` — [`L144`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L144)
- `count_source_files(project_dir: Path, language: str)` — [`L158`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L158)
- `main()` — [`L253`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L253)
- `run_analysis(project_dir: Path, language: str, query_symbols: list[str])` — [`L175`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L175) — Run our MCP tools and count what an agent would need.

## Module values
- `BENCH_DIR` — [`L37`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L37)
- `CODEGRAPH_BASELINES` — [`L40`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L40)
- `OUR_PROJECTS` — [`L59`](../../../../../raw/code/tree-sitter-analyzer/scripts/benchmark_real_projects.py#L59)

