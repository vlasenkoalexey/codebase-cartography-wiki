---
title: 'Module: benchmarks/codegraph_compare/adapters/__init__.py'
type: catalog
provenance: extracted
module: benchmarks/codegraph_compare/adapters/__init__.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `benchmarks.codegraph_compare.adapters`/
symbols:
  RunConfig: RunConfig#
  IndexStats: IndexStats#
  BenchmarkAdapter: BenchmarkAdapter#
  get_adapter: get_adapter().
  BenchmarkAdapter.prepare_index: BenchmarkAdapter#prepare_index().
  BenchmarkAdapter.build_run_config: BenchmarkAdapter#build_run_config().
  ToolMetrics: ToolMetrics#
  BenchmarkAdapter.parse_tool_metrics: BenchmarkAdapter#parse_tool_metrics().
  IndexStats.build_seconds: IndexStats#build_seconds.
  IndexStats.file_count: IndexStats#file_count.
  RunConfig.system_prompt: RunConfig#system_prompt.
  RunConfig.extra_context: RunConfig#extra_context.
  IndexStats.index_size_bytes: IndexStats#index_size_bytes.
  RunConfig.arm_id: RunConfig#arm_id.
  RunConfig.repo_path: RunConfig#repo_path.
  BenchmarkAdapter.arm_id: BenchmarkAdapter#arm_id.
  ToolMetrics.tool_calls: ToolMetrics#tool_calls.
  ToolMetrics.file_reads: ToolMetrics#file_reads.
  ToolMetrics.search_calls: ToolMetrics#search_calls.
  ToolMetrics.index_queries: ToolMetrics#index_queries.
  RunConfig.allowed_tools: RunConfig#allowed_tools.
  RunConfig.forbidden_tools: RunConfig#forbidden_tools.
---
# Module: [`benchmarks/codegraph_compare/adapters/__init__.py`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py)

## Classes
### `BenchmarkAdapter`  ·  implements/extends ABC
- def: [`benchmarks/codegraph_compare/adapters/__init__.py:59`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L59)
- doc: Base class for all benchmark arms.
- signature: `class BenchmarkAdapter(ABC):`
- members:
  - `build_run_config(self, repo_path: Path, question_prompt: str)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L75) — Return the RunConfig for a single question run against *repo_path*.
  - `parse_tool_metrics(self, transcript_text: str)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L80) — Parse raw transcript text and return aggregated tool-usage counts.
  - `prepare_index(self, repo_path: Path, cold: bool)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L65) — Build (cold=True) or verify (cold=False, warm) the index.
  - `arm_id` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L62)
- uses (calls/refs, reference-scoped): (15 test-only callers)
- used by: (11 test-only callers)

### `IndexStats`
- def: [`benchmarks/codegraph_compare/adapters/__init__.py:23`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L23)
- doc: Statistics collected during index preparation.
- signature: `class IndexStats:`
- members:
  - `build_seconds` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L26)
  - `file_count` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L28)
  - `index_size_bytes` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L27)
- used by: (10 test-only callers)

### `RunConfig`
- def: [`benchmarks/codegraph_compare/adapters/__init__.py:42`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L42)
- doc: Full configuration for one benchmark question run.
- signature: `class RunConfig:`
- members:
  - `allowed_tools` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L48)
  - `arm_id` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L45)
  - `extra_context` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L51)
  - `forbidden_tools` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L49)
  - `repo_path` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L46)
  - `system_prompt` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L47)
- used by: (10 test-only callers)

### `ToolMetrics`
- def: [`benchmarks/codegraph_compare/adapters/__init__.py:32`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L32)
- doc: Tool-usage counts parsed from a single transcript run.
- signature: `class ToolMetrics:`
- members:
  - `file_reads` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L36)
  - `index_queries` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L38)
  - `search_calls` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L37)
  - `tool_calls` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L35)
- used by: (5 test-only callers)

## Functions
- `get_adapter(arm_id: str)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/__init__.py#L90) — Return the right adapter instance for *arm_id*.

