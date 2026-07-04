---
title: 'Module: tests/unit/mcp/test_search_content_execute.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_search_content_execute.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_search_content_execute`/
symbols:
  TestExecute.test_execute_with_cache_disabled: TestExecute#test_execute_with_cache_disabled().
  tool: tool().
  sample_project_structure: sample_project_structure().
  TestExecute: TestExecute#
  TestExecute.test_execute_rg_not_found: TestExecute#test_execute_rg_not_found().
  TestExecute.test_execute_total_only_mode: TestExecute#test_execute_total_only_mode().
  TestExecute.test_execute_count_only_matches_mode: TestExecute#test_execute_count_only_matches_mode().
  TestExecute.test_execute_summary_only_mode: TestExecute#test_execute_summary_only_mode().
  TestExecute.test_execute_group_by_file_mode: TestExecute#test_execute_group_by_file_mode().
  TestExecute.test_execute_with_file_output: TestExecute#test_execute_with_file_output().
  TestExecute.test_execute_with_suppress_output: TestExecute#test_execute_with_suppress_output().
  TestExecute.test_execute_with_toon_format: TestExecute#test_execute_with_toon_format().
  TestExecute.test_execute_rg_failure: TestExecute#test_execute_rg_failure().
  TestExecute.test_execute_with_cache_hit: TestExecute#test_execute_with_cache_hit().
  TestExecute.test_execute_with_parallel_processing: TestExecute#test_execute_with_parallel_processing().
  TestExecute.test_execute_with_files_parameter: TestExecute#test_execute_with_files_parameter().
  TestExecute.test_execute_with_optimize_paths: TestExecute#test_execute_with_optimize_paths().
  TestExecute.test_execute_file_save_error: TestExecute#test_execute_file_save_error().
  TestExecute.test_execute_with_timeout: TestExecute#test_execute_with_timeout().
  TestExecute.test_execute_with_max_count: TestExecute#test_execute_with_max_count().
---
# Module: [`tests/unit/mcp/test_search_content_execute.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py)

## Classes
### `TestExecute`
- def: [`tests/unit/mcp/test_search_content_execute.py:30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L30)
- doc: Tests for execute method.
- signature: `class TestExecute:`
- members:
  - `test_execute_count_only_matches_mode(self, tool, sample_project_structure)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L70)
  - `test_execute_file_save_error(self, tool, sample_project_structure)` — [`L419`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L419)
  - `test_execute_group_by_file_mode(self, tool, sample_project_structure)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L132)
  - `test_execute_rg_failure(self, tool, sample_project_structure)` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L266)
  - `test_execute_rg_not_found(self, tool)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L34)
  - `test_execute_summary_only_mode(self, tool, sample_project_structure)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L101)
  - `test_execute_total_only_mode(self, tool, sample_project_structure)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L45)
  - `test_execute_with_cache_disabled(self, tool, sample_project_structure)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L307)
  - `test_execute_with_cache_hit(self, tool, sample_project_structure)` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L288)
  - `test_execute_with_file_output(self, tool, sample_project_structure)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L167)
  - `test_execute_with_files_parameter(self, tool, sample_project_structure)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L366)
  - `test_execute_with_max_count(self, tool, sample_project_structure)` — [`L473`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L473)
  - `test_execute_with_optimize_paths(self, tool, sample_project_structure)` — [`L386`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L386)
  - `test_execute_with_parallel_processing(self, tool, sample_project_structure)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L329)
  - `test_execute_with_suppress_output(self, tool, sample_project_structure)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L199)
  - `test_execute_with_timeout(self, tool, sample_project_structure)` — [`L452`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L452)
  - `test_execute_with_toon_format(self, tool, sample_project_structure)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L234)
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.execute), [`cache`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.cache)

## Functions
- `sample_project_structure(tmp_path: Path)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L20)
- `tool()` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_execute.py#L15)

