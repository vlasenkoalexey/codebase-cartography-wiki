---
title: 'Module: tests/unit/mcp/test_search_content_tool_cache.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_search_content_tool_cache.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_search_content_tool_cache`/
symbols:
  _TMPDIR: _TMPDIR.
  TestCreateCountOnlyCacheKeyNoCache.test_returns_none_when_no_cache: TestCreateCountOnlyCacheKeyNoCache#test_returns_none_when_no_cache().
  tool: tool().
  TestCacheHitBranches.test_cache_hit_total_only_returns_int: TestCacheHitBranches#test_cache_hit_total_only_returns_int().
  TestCacheHitBranches.test_cache_hit_total_only_dict_with_total_matches: TestCacheHitBranches#test_cache_hit_total_only_dict_with_total_matches().
  TestCacheHitBranches.test_cache_hit_total_only_dict_with_count: TestCacheHitBranches#test_cache_hit_total_only_dict_with_count().
  TestCacheHitBranches.test_cache_hit_total_only_dict_no_match_key: TestCacheHitBranches#test_cache_hit_total_only_dict_no_match_key().
  TestCacheHitBranches.test_cache_hit_non_total_only_dict: TestCacheHitBranches#test_cache_hit_non_total_only_dict().
  TestCacheHitBranches.test_cache_hit_non_total_only_int: TestCacheHitBranches#test_cache_hit_non_total_only_int().
  TestCacheHitBranches.test_cache_hit_non_total_only_other_type: TestCacheHitBranches#test_cache_hit_non_total_only_other_type().
  sample_project_structure: sample_project_structure().
  TestCacheHitBranches: TestCacheHitBranches#
  TestSummaryOutputPaths: TestSummaryOutputPaths#
  TestSummaryOutputPaths.test_summary_with_output_file: TestSummaryOutputPaths#test_summary_with_output_file().
  TestSummaryOutputPaths.test_summary_with_output_file_error: TestSummaryOutputPaths#test_summary_with_output_file_error().
  TestSummaryOutputPaths.test_summary_toon_format: TestSummaryOutputPaths#test_summary_toon_format().
  TestSuppressOutputEndPath: TestSuppressOutputEndPath#
  TestSuppressOutputEndPath.test_suppress_output_no_file_returns_copy_without_results: TestSuppressOutputEndPath#test_suppress_output_no_file_returns_copy_without_results().
  TestCreateCountOnlyCacheKeyNoCache: TestCreateCountOnlyCacheKeyNoCache#
---
# Module: [`tests/unit/mcp/test_search_content_tool_cache.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py)

## Classes
### `TestCacheHitBranches`
- def: [`tests/unit/mcp/test_search_content_tool_cache.py:48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py#L48)
- doc: Tests for execute() cache-hit branches (lines 382-416).
- signature: `class TestCacheHitBranches:`
- members:
  - `test_cache_hit_non_total_only_dict(self, tool)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py#L88)
  - `test_cache_hit_non_total_only_int(self, tool)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py#L98)
  - `test_cache_hit_non_total_only_other_type(self, tool)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py#L109)
  - `test_cache_hit_total_only_dict_no_match_key(self, tool)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py#L79)
  - `test_cache_hit_total_only_dict_with_count(self, tool)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py#L70)
  - `test_cache_hit_total_only_dict_with_total_matches(self, tool)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py#L61)
  - `test_cache_hit_total_only_returns_int(self, tool)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py#L52)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestCreateCountOnlyCacheKeyNoCache`
- def: [`tests/unit/mcp/test_search_content_tool_cache.py:247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py#L247)
- doc: Tests for _create_count_only_cache_key when cache is None (line 317).
- signature: `class TestCreateCountOnlyCacheKeyNoCache:`
- members:
  - `test_returns_none_when_no_cache(self)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py#L250)
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`_create_count_only_cache_key`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool._create_count_only_cache_key)

### `TestSummaryOutputPaths`
- def: [`tests/unit/mcp/test_search_content_tool_cache.py:119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py#L119)
- doc: Tests for summary mode file output (lines 789-844).
- signature: `class TestSummaryOutputPaths:`
- members:
  - `test_summary_toon_format(self, tool, sample_project_structure)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py#L186)
  - `test_summary_with_output_file(self, tool, sample_project_structure)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py#L123)
  - `test_summary_with_output_file_error(self, tool, sample_project_structure)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py#L153)

### `TestSuppressOutputEndPath`
- def: [`tests/unit/mcp/test_search_content_tool_cache.py:213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py#L213)
- doc: Tests for final suppress_output path without output_file (lines 914-919).
- signature: `class TestSuppressOutputEndPath:`
- members:
  - `test_suppress_output_no_file_returns_copy_without_results(self, tool, sample_project_structure)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py#L217)

## Functions
- `sample_project_structure(tmp_path: Path)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py#L33) — Create a sample project structure for testing.
- `tool()` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py#L27) — Create a fresh tool instance for each test.

## Module values
- `_TMPDIR` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_cache.py#L23)

