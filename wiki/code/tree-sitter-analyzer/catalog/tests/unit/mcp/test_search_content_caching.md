---
title: 'Module: tests/unit/mcp/test_search_content_caching.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_search_content_caching.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_search_content_caching`/
symbols:
  TestCreateCountOnlyCacheKeyNoCache.test_returns_none_when_no_cache: TestCreateCountOnlyCacheKeyNoCache#test_returns_none_when_no_cache().
  tool: tool().
  sample_project_structure: sample_project_structure().
  TestCacheHitBranches: TestCacheHitBranches#
  TestCacheHitBranches.test_cache_hit_total_only_returns_int: TestCacheHitBranches#test_cache_hit_total_only_returns_int().
  TestCacheHitBranches.test_cache_hit_total_only_dict_with_total_matches: TestCacheHitBranches#test_cache_hit_total_only_dict_with_total_matches().
  TestCacheHitBranches.test_cache_hit_total_only_dict_with_count: TestCacheHitBranches#test_cache_hit_total_only_dict_with_count().
  TestCacheHitBranches.test_cache_hit_total_only_dict_no_match_key: TestCacheHitBranches#test_cache_hit_total_only_dict_no_match_key().
  TestCacheHitBranches.test_cache_hit_non_total_only_dict: TestCacheHitBranches#test_cache_hit_non_total_only_dict().
  TestCacheHitBranches.test_cache_hit_non_total_only_int: TestCacheHitBranches#test_cache_hit_non_total_only_int().
  TestCacheHitBranches.test_cache_hit_non_total_only_other_type: TestCacheHitBranches#test_cache_hit_non_total_only_other_type().
  TestSummaryOutputPaths: TestSummaryOutputPaths#
  TestSummaryOutputPaths.test_summary_with_output_file: TestSummaryOutputPaths#test_summary_with_output_file().
  TestSummaryOutputPaths.test_summary_with_output_file_error: TestSummaryOutputPaths#test_summary_with_output_file_error().
  TestSummaryOutputPaths.test_summary_toon_format: TestSummaryOutputPaths#test_summary_toon_format().
  TestSuppressOutputEndPath: TestSuppressOutputEndPath#
  TestSuppressOutputEndPath.test_suppress_output_no_file_returns_copy_without_results: TestSuppressOutputEndPath#test_suppress_output_no_file_returns_copy_without_results().
  TestCreateCountOnlyCacheKeyNoCache: TestCreateCountOnlyCacheKeyNoCache#
---
# Module: [`tests/unit/mcp/test_search_content_caching.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_caching.py)

## Classes
### `TestCacheHitBranches`
- def: [`tests/unit/mcp/test_search_content_caching.py:37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_caching.py#L37)
- doc: Tests for execute() cache-hit branches (lines 382-416).
- signature: `class TestCacheHitBranches:`
- members:
  - `test_cache_hit_non_total_only_dict(self, tool)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_caching.py#L77)
  - `test_cache_hit_non_total_only_int(self, tool)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_caching.py#L87)
  - `test_cache_hit_non_total_only_other_type(self, tool)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_caching.py#L98)
  - `test_cache_hit_total_only_dict_no_match_key(self, tool)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_caching.py#L68)
  - `test_cache_hit_total_only_dict_with_count(self, tool)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_caching.py#L59)
  - `test_cache_hit_total_only_dict_with_total_matches(self, tool)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_caching.py#L50)
  - `test_cache_hit_total_only_returns_int(self, tool)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_caching.py#L41)

### `TestCreateCountOnlyCacheKeyNoCache`
- def: [`tests/unit/mcp/test_search_content_caching.py:236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_caching.py#L236)
- doc: Tests for _create_count_only_cache_key when cache is None (line 317).
- signature: `class TestCreateCountOnlyCacheKeyNoCache:`
- members:
  - `test_returns_none_when_no_cache(self)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_caching.py#L239)
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`_create_count_only_cache_key`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool._create_count_only_cache_key)

### `TestSummaryOutputPaths`
- def: [`tests/unit/mcp/test_search_content_caching.py:108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_caching.py#L108)
- doc: Tests for summary mode file output (lines 789-844).
- signature: `class TestSummaryOutputPaths:`
- members:
  - `test_summary_toon_format(self, tool, sample_project_structure)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_caching.py#L175)
  - `test_summary_with_output_file(self, tool, sample_project_structure)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_caching.py#L112)
  - `test_summary_with_output_file_error(self, tool, sample_project_structure)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_caching.py#L142)

### `TestSuppressOutputEndPath`
- def: [`tests/unit/mcp/test_search_content_caching.py:202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_caching.py#L202)
- doc: Tests for final suppress_output path without output_file (lines 914-919).
- signature: `class TestSuppressOutputEndPath:`
- members:
  - `test_suppress_output_no_file_returns_copy_without_results(self, tool, sample_project_structure)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_caching.py#L206)

## Functions
- `sample_project_structure(tmp_path: Path)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_caching.py#L21)
- `tool()` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_caching.py#L16)

