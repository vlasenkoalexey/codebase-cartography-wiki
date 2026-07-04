---
title: 'Module: tests/unit/test_codegraph_query_tool_has.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_query_tool_has.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_query_tool_has`/TestCodeGraphQueryToolHas#
symbols:
  TestCodeGraphQueryToolHas.test_execute_has_filters_sources_by_related_symbols: test_execute_has_filters_sources_by_related_symbols().
  TestCodeGraphQueryToolHas.test_execute_has_reuses_relation_cache_for_later_include: test_execute_has_reuses_relation_cache_for_later_include().
  TestCodeGraphQueryToolHas.test_execute_has_reports_missing_direction: test_execute_has_reports_missing_direction().
  TestCodeGraphQueryToolHas.test_execute_reuses_relation_cache_within_single_chain: test_execute_reuses_relation_cache_within_single_chain().
  TestCodeGraphQueryToolHas.test_apply_step_rejects_unknown_step: test_apply_step_rejects_unknown_step().
  TestCodeGraphQueryToolHas._query_callees: _query_callees().
  TestCodeGraphQueryToolHas: ''
---
# Module: [`tests/unit/test_codegraph_query_tool_has.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_has.py)

## Classes
### `TestCodeGraphQueryToolHas`
- def: [`tests/unit/test_codegraph_query_tool_has.py:17`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_has.py#L17)
- signature: `class TestCodeGraphQueryToolHas:`
- members:
  - `test_apply_step_rejects_unknown_step(self)` — [`L171`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_has.py#L171)
  - `test_execute_has_filters_sources_by_related_symbols(self, tmp_path)` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_has.py#L19)
  - `test_execute_has_reports_missing_direction(self, tmp_path)` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_has.py#L124)
  - `test_execute_has_reuses_relation_cache_for_later_include(self, tmp_path)` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_has.py#L80)
  - `test_execute_reuses_relation_cache_within_single_chain(self, tmp_path)` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_has.py#L142)
- protocol/private: `_query_callees`[`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_has.py#L22)
- uses (calls/refs, reference-scoped): [`_apply_step`](../../tree_sitter_analyzer/mcp/tools/codegraph_query_tool.md#CodeGraphQueryTool._apply_step), [`execute`](../../tree_sitter_analyzer/mcp/tools/codegraph_query_tool.md#CodeGraphQueryTool.execute), [`_ChainStep`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.md#_ChainStep), [`CodeGraphQueryTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_query_tool.md#CodeGraphQueryTool), [`_QueryState`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_state.md#_QueryState)  (2 test-only)

