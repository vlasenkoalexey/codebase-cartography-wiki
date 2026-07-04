---
title: 'Module: tree_sitter_analyzer/mcp/tools/search_content_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/search_content_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.search_content_helpers`/
symbols:
  run_search: run_search().
  handle_output_and_cache: handle_output_and_cache().
  _handle_file_output: _handle_file_output().
  save_enriched_output: save_enriched_output().
  logger: logger.
  _cache_result: _cache_result().
  build_next_steps: build_next_steps().
  TOOL_SCHEMA.TOOL_SCHEMA: TOOL_SCHEMA.TOOL_SCHEMA.
  should_use_parallel: should_use_parallel().
  _prepare_search_roots: _prepare_search_roots().
  _run_parallel_search: _run_parallel_search().
  _run_single_search: _run_single_search().
  _make_minimal: _make_minimal().
---
# Module: [`tree_sitter_analyzer/mcp/tools/search_content_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_helpers.py)

## Functions
- `_cache_result(cache: Any, cache_key: str | None, result: dict[str, Any])` — [`L389`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_helpers.py#L389) — Cache the result if cache and key are available.
- `_handle_file_output(result: dict[str, Any], output_file: str, suppress_output: bool, output_format: str, file_output_manager: Any, cache: Any, cache_key: str | None)` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_helpers.py#L345) — Save results to file and optionally suppress output.
- `_make_minimal(result: dict[str, Any])` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_helpers.py#L397) — Create a minimal response for suppress_output mode.
- `_prepare_search_roots(path_resolver: Any, arguments: dict[str, Any], rg_args: dict[str, Any], roots: list[str] | None, files: list[str] | None)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_helpers.py#L242) — Convert explicit files into parent search roots and include globs.
- `_run_parallel_search(search_roots: list[str], count_only_matches: bool, timeout_ms: int | None, max_count: int | None, rg_args: dict[str, Any], fd_rg_utils: Any)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_helpers.py#L268) — Execute rg against root chunks and merge results.
- `_run_single_search(search_roots: list[str] | None, count_only_matches: bool, timeout_ms: int | None, rg_args: dict[str, Any], fd_rg_utils: Any)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_helpers.py#L292) — Execute rg once and return raw process output.
- `build_next_steps(matches: list[dict[str, Any]])` — [`L458`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_helpers.py#L458) — Build next_steps suggestions for AI agents.
- `handle_output_and_cache(result: dict[str, Any], arguments: dict[str, Any], file_output_manager: Any, cache: Any, cache_key: str | None, output_format: str)` — [`L309`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_helpers.py#L309) — Handle output_file, suppress_output, and caching.
- `run_search(path_resolver: Any, arguments: dict[str, Any], rg_args: dict[str, Any], roots: list[str] | None, files: list[str] | None, max_count: int | None, fd_rg_utils: Any)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_helpers.py#L193) — Execute ripgrep in file, single-root, or parallel-root mode.
- `save_enriched_output(result: dict[str, Any], matches: list[dict[str, Any]], arguments: dict[str, Any], output_format: str, file_output_manager: Any, fd_rg_utils: Any)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_helpers.py#L416) — Save enriched search results to file, mutating result with status.
- `should_use_parallel(arguments: dict[str, Any], search_roots: list[str] | None)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_helpers.py#L231) — Return whether the search should fan out across root chunks.

## Module values
- `TOOL_SCHEMA` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_helpers.py#L20)
- `logger` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_helpers.py#L18)

