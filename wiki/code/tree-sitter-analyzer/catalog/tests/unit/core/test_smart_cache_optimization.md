---
title: 'Module: tests/unit/core/test_smart_cache_optimization.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_smart_cache_optimization.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_smart_cache_optimization`/
symbols:
  TestSmartCacheOptimization.test_cache_key_derivation: TestSmartCacheOptimization#test_cache_key_derivation().
  TestSmartCacheOptimization.test_cache_can_derive_file_list: TestSmartCacheOptimization#test_cache_can_derive_file_list().
  TestSmartCacheOptimization.test_cache_derive_file_list_result: TestSmartCacheOptimization#test_cache_derive_file_list_result().
  TestSmartCacheOptimization.test_get_compatible_result_direct_hit: TestSmartCacheOptimization#test_get_compatible_result_direct_hit().
  TestSmartCacheOptimization.test_get_compatible_result_derivation: TestSmartCacheOptimization#test_get_compatible_result_derivation().
  TestSmartCacheOptimization.test_search_content_smart_caching_integration: TestSmartCacheOptimization#test_search_content_smart_caching_integration().
  TestSmartCacheOptimization.test_determine_requested_format: TestSmartCacheOptimization#test_determine_requested_format().
  TestSmartCacheOptimization.test_total_only_to_count_only_cross_caching: TestSmartCacheOptimization#test_total_only_to_count_only_cross_caching().
  TestSmartCacheOptimization.test_create_count_only_cache_key: TestSmartCacheOptimization#test_create_count_only_cache_key().
  clear_cache_between_tests: clear_cache_between_tests().
  TestSmartCacheOptimization.test_extract_file_list_from_count_data: TestSmartCacheOptimization#test_extract_file_list_from_count_data().
  TestSmartCacheOptimization.test_create_file_summary_from_count_data: TestSmartCacheOptimization#test_create_file_summary_from_count_data().
  mock_external_commands: mock_external_commands().
  TestSmartCacheOptimization: TestSmartCacheOptimization#
---
# Module: [`tests/unit/core/test_smart_cache_optimization.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_smart_cache_optimization.py)

## Classes
### `TestSmartCacheOptimization`
- def: [`tests/unit/core/test_smart_cache_optimization.py:35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_smart_cache_optimization.py#L35)
- doc: Test cases for smart cross-format cache optimization.
- signature: `class TestSmartCacheOptimization:`
- members:
  - `test_cache_can_derive_file_list(self)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_smart_cache_optimization.py#L75) — Test detection of derivable count results.
  - `test_cache_derive_file_list_result(self)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_smart_cache_optimization.py#L97) — Test file list result derivation.
  - `test_cache_key_derivation(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_smart_cache_optimization.py#L64) — Test cache key derivation for cross-format optimization.
  - `test_create_count_only_cache_key(self)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_smart_cache_optimization.py#L280) — Test creation of count_only cache key from total_only arguments.
  - `test_create_file_summary_from_count_data(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_smart_cache_optimization.py#L48) — Test file summary creation from count data.
  - `test_determine_requested_format(self)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_smart_cache_optimization.py#L199) — Test format determination from arguments.
  - `test_extract_file_list_from_count_data(self)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_smart_cache_optimization.py#L38) — Test file list extraction from count data.
  - `test_get_compatible_result_derivation(self)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_smart_cache_optimization.py#L134) — Test cross-format result derivation.
  - `test_get_compatible_result_direct_hit(self)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_smart_cache_optimization.py#L121) — Test that direct cache hits work normally.
  - `test_search_content_smart_caching_integration(self, mock_validate_roots, mock_run_command)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_smart_cache_optimization.py#L158) — Test smart caching integration in SearchContentTool.
  - `test_total_only_to_count_only_cross_caching(self, mock_validate_roots, mock_run_command)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_smart_cache_optimization.py#L221) — Test that total_only results can serve future count_only_matches queries.
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.execute), [`SearchCache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`get_compatible_result`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get_compatible_result), [`_derive_file_list_result`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._derive_file_list_result), [`create_file_summary_from_count_data`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.md#create_file_summary_from_count_data), [`extract_file_list_from_count_data`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_result_utils.md#extract_file_list_from_count_data), [`_create_count_only_cache_key`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool._create_count_only_cache_key), [`_can_derive_file_list`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._can_derive_file_list), [`_derive_count_key_from_cache_key`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._derive_count_key_from_cache_key), [`_determine_requested_format`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool._determine_requested_format)

## Functions
- `clear_cache_between_tests()` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_smart_cache_optimization.py#L28) — Clear cache before each test to avoid interference
- `mock_external_commands(monkeypatch)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_smart_cache_optimization.py#L19) — Auto-mock external command availability checks for all tests in this module.

