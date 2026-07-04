---
title: 'Module: tests/unit/search/test_search_content_parallel.py'
type: catalog
provenance: extracted
module: tests/unit/search/test_search_content_parallel.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.search.test_search_content_parallel`/TestSearchContentParallel#
symbols:
  TestSearchContentParallel.tool: tool().
  TestSearchContentParallel.test_split_roots_for_parallel_processing: test_split_roots_for_parallel_processing().
  TestSearchContentParallel.test_parallel_rg_searches_execution: test_parallel_rg_searches_execution().
  TestSearchContentParallel.test_merge_json_results: test_merge_json_results().
  TestSearchContentParallel.test_merge_count_results: test_merge_count_results().
  TestSearchContentParallel: ''
  TestSearchContentParallel.test_parallel_processing_enabled_by_default: test_parallel_processing_enabled_by_default().
  TestSearchContentParallel.test_parallel_processing_disabled_option: test_parallel_processing_disabled_option().
  TestSearchContentParallel.test_single_root_uses_single_command: test_single_root_uses_single_command().
  TestSearchContentParallel.test_parallel_processing_with_count_only: test_parallel_processing_with_count_only().
  TestSearchContentParallel.test_parallel_processing_error_handling: test_parallel_processing_error_handling().
  TestSearchContentParallel.test_validate_enable_parallel_argument: test_validate_enable_parallel_argument().
---
# Module: [`tests/unit/search/test_search_content_parallel.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/search/test_search_content_parallel.py)

## Classes
### `TestSearchContentParallel`
- def: [`tests/unit/search/test_search_content_parallel.py:14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/search/test_search_content_parallel.py#L14)
- doc: Test parallel processing functionality in search_content tool.
- signature: `class TestSearchContentParallel:`
- members:
  - `test_merge_count_results(self)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/search/test_search_content_parallel.py#L184) — Test merging of count results from parallel searches.
  - `test_merge_json_results(self)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/search/test_search_content_parallel.py#L168) — Test merging of JSON results from parallel searches.
  - `test_parallel_processing_disabled_option(self, tool)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/search/test_search_content_parallel.py#L52) — Test that parallel processing can be disabled via option.
  - `test_parallel_processing_enabled_by_default(self, tool)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/search/test_search_content_parallel.py#L23) — Test that parallel processing is enabled by default for multiple roots.
  - `test_parallel_processing_error_handling(self, tool)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/search/test_search_content_parallel.py#L234) — Test error handling in parallel processing.
  - `test_parallel_processing_with_count_only(self, tool)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/search/test_search_content_parallel.py#L201) — Test parallel processing works with count-only mode.
  - `test_parallel_rg_searches_execution(self)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/search/test_search_content_parallel.py#L144) — Test parallel ripgrep search execution.
  - `test_single_root_uses_single_command(self, tool)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/search/test_search_content_parallel.py#L88) — Test that single root directory uses single command execution.
  - `test_split_roots_for_parallel_processing(self)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/search/test_search_content_parallel.py#L122) — Test root splitting logic for parallel processing.
  - `test_validate_enable_parallel_argument(self, tool)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/search/test_search_content_parallel.py#L262) — Test validation of enable_parallel argument.
  - `tool(self)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/search/test_search_content_parallel.py#L18) — Create a SearchContentTool instance for testing.
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`merge_rg_results`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#merge_rg_results), [`run_parallel_rg_searches`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#run_parallel_rg_searches), [`split_roots_for_parallel_processing`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#split_roots_for_parallel_processing)

