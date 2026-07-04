---
title: 'Module: tests/unit/test_codegraph_query_tool_advanced.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_query_tool_advanced.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_query_tool_advanced`/TestCodeGraphQueryToolAdvanced#
symbols:
  TestCodeGraphQueryToolAdvanced.test_execute_batch_seed_include_sort_and_answer: test_execute_batch_seed_include_sort_and_answer().
  TestCodeGraphQueryToolAdvanced.test_execute_compact_answer_removes_duplicate_source_payload: test_execute_compact_answer_removes_duplicate_source_payload().
  TestCodeGraphQueryToolAdvanced.test_execute_filter_narrows_current_selection_and_rebuilds_source: test_execute_filter_narrows_current_selection_and_rebuilds_source().
  TestCodeGraphQueryToolAdvanced.test_execute_exclude_removes_matching_selection: test_execute_exclude_removes_matching_selection().
  TestCodeGraphQueryToolAdvanced.test_execute_filter_prunes_relationships_to_kept_entries: test_execute_filter_prunes_relationships_to_kept_entries().
  TestCodeGraphQueryToolAdvanced.test_execute_filter_keeps_relationships_for_kept_source: test_execute_filter_keeps_relationships_for_kept_source().
  TestCodeGraphQueryToolAdvanced.test_execute_filter_removes_relationships_without_kept_edges: test_execute_filter_removes_relationships_without_kept_edges().
  TestCodeGraphQueryToolAdvanced.test_execute_filter_applies_to_later_concept_fallback: test_execute_filter_applies_to_later_concept_fallback().
  TestCodeGraphQueryToolAdvanced.test_execute_symbol_filter_applies_to_later_concept_fallback: test_execute_symbol_filter_applies_to_later_concept_fallback().
  TestCodeGraphQueryToolAdvanced: ''
---
# Module: [`tests/unit/test_codegraph_query_tool_advanced.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_advanced.py)

## Classes
### `TestCodeGraphQueryToolAdvanced`
- def: [`tests/unit/test_codegraph_query_tool_advanced.py:17`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_advanced.py#L17)
- signature: `class TestCodeGraphQueryToolAdvanced:`
- members:
  - `test_execute_batch_seed_include_sort_and_answer(self, tmp_path)` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_advanced.py#L154)
  - `test_execute_compact_answer_removes_duplicate_source_payload(self, tmp_path)` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_advanced.py#L209)
  - `test_execute_exclude_removes_matching_selection(self, tmp_path)` — [`L288`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_advanced.py#L288)
  - `test_execute_filter_applies_to_later_concept_fallback(self, tmp_path)` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_advanced.py#L19)
  - `test_execute_filter_keeps_relationships_for_kept_source(self, tmp_path)` — [`L351`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_advanced.py#L351)
  - `test_execute_filter_narrows_current_selection_and_rebuilds_source(self, tmp_path)` — [`L251`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_advanced.py#L251)
  - `test_execute_filter_prunes_relationships_to_kept_entries(self, tmp_path)` — [`L308`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_advanced.py#L308)
  - `test_execute_filter_removes_relationships_without_kept_edges(self, tmp_path)` — [`L388`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_advanced.py#L388)
  - `test_execute_symbol_filter_applies_to_later_concept_fallback(self, tmp_path)` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_advanced.py#L89)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/codegraph_query_tool.md#CodeGraphQueryTool.execute), [`CodeGraphQueryTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_query_tool.md#CodeGraphQueryTool)  (2 test-only)

