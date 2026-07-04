---
title: 'Module: tests/unit/test_codegraph_query_tool_core.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_query_tool_core.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_query_tool_core`/TestCodeGraphQueryTool#
symbols:
  TestCodeGraphQueryTool.test_execute_explore_callers_related_and_take: test_execute_explore_callers_related_and_take().
  TestCodeGraphQueryTool.test_get_cache_requires_project_root_and_reuses_instance: test_get_cache_requires_project_root_and_reuses_instance().
  TestCodeGraphQueryTool.test_execute_runs_chain_in_one_tool: test_execute_runs_chain_in_one_tool().
  TestCodeGraphQueryTool.test_execute_search_limit_caps_symbols: test_execute_search_limit_caps_symbols().
  TestCodeGraphQueryTool.test_execute_semantic_search_uses_vector_backend: test_execute_semantic_search_uses_vector_backend().
  TestCodeGraphQueryTool.test_execute_uml_step_renders_current_relationships_as_mermaid: test_execute_uml_step_renders_current_relationships_as_mermaid().
  TestCodeGraphQueryTool.test_execute_explore_falls_back_to_concept_search_for_plain_language: test_execute_explore_falls_back_to_concept_search_for_plain_language().
  TestCodeGraphQueryTool.test_execute_include_source_can_trigger_concept_fallback: test_execute_include_source_can_trigger_concept_fallback().
  TestCodeGraphQueryTool.test_definition: test_definition().
  TestCodeGraphQueryTool.test_schema_requires_query: test_schema_requires_query().
  TestCodeGraphQueryTool.test_validate_requires_query: test_validate_requires_query().
  TestCodeGraphQueryTool.test_execute_returns_error_envelope_for_bad_chain: test_execute_returns_error_envelope_for_bad_chain().
  TestCodeGraphQueryTool.test_execute_collects_step_warnings_for_invalid_search_arg: test_execute_collects_step_warnings_for_invalid_search_arg().
  TestCodeGraphQueryTool._query_callers: _query_callers().
  TestCodeGraphQueryTool._query_callees: _query_callees().
  TestCodeGraphQueryTool: ''
---
# Module: [`tests/unit/test_codegraph_query_tool_core.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_core.py)

## Classes
### `TestCodeGraphQueryTool`
- def: [`tests/unit/test_codegraph_query_tool_core.py:17`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_core.py#L17)
- signature: `class TestCodeGraphQueryTool:`
- members:
  - `test_definition(self)` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_core.py#L18)
  - `test_execute_collects_step_warnings_for_invalid_search_arg(self, tmp_path)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_core.py#L110)
  - `test_execute_explore_callers_related_and_take(self, tmp_path)` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_core.py#L126)
  - `test_execute_explore_falls_back_to_concept_search_for_plain_language(self, tmp_path)` — [`L273`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_core.py#L273)
  - `test_execute_include_source_can_trigger_concept_fallback(self, tmp_path)` — [`L340`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_core.py#L340)
  - `test_execute_returns_error_envelope_for_bad_chain(self)` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_core.py#L96)
  - `test_execute_runs_chain_in_one_tool(self, tmp_path)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_core.py#L51)
  - `test_execute_search_limit_caps_symbols(self, tmp_path)` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_core.py#L195)
  - `test_execute_semantic_search_uses_vector_backend(self, tmp_path)` — [`L218`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_core.py#L218)
  - `test_execute_uml_step_renders_current_relationships_as_mermaid(self, tmp_path)` — [`L240`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_core.py#L240)
  - `test_get_cache_requires_project_root_and_reuses_instance(self, tmp_path)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_core.py#L34)
  - `test_schema_requires_query(self)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_core.py#L24)
  - `test_validate_requires_query(self)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_core.py#L30)
- protocol/private: `_query_callees`[`L146`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_core.py#L146), `_query_callers`[`L133`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool_core.py#L133)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/codegraph_query_tool.md#CodeGraphQueryTool.execute), [`set_project_path`](../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.set_project_path), [`CodeGraphQueryTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_query_tool.md#CodeGraphQueryTool), [`get_cache`](../../tree_sitter_analyzer/mcp/tools/codegraph_query_tool.md#CodeGraphQueryTool.get_cache), [`cache_initialized`](../../tree_sitter_analyzer/mcp/tools/codegraph_query_tool.md#CodeGraphQueryTool.cache_initialized), [`get_tool_definition`](../../tree_sitter_analyzer/mcp/tools/codegraph_query_tool.md#CodeGraphQueryTool.get_tool_definition), [`get_tool_schema`](../../tree_sitter_analyzer/mcp/tools/codegraph_query_tool.md#CodeGraphQueryTool.get_tool_schema), [`validate_arguments`](../../tree_sitter_analyzer/mcp/tools/codegraph_query_tool.md#CodeGraphQueryTool.validate_arguments)  (2 test-only)

