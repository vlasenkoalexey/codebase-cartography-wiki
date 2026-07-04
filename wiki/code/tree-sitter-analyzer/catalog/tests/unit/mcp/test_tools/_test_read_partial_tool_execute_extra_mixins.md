---
title: 'Module: tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_tools._test_read_partial_tool_execute_extra_mixins`/ReadPartialToolExecuteExtra
symbols:
  ReadPartialToolExecuteExtraMixin.test_execute_success_with_output_file_text: Mixin#test_execute_success_with_output_file_text().
  ReadPartialToolExecuteExtraMixin.test_execute_success_with_output_file_json: Mixin#test_execute_success_with_output_file_json().
  ReadPartialToolExecuteExtraMixin.test_execute_success_with_output_file_raw: Mixin#test_execute_success_with_output_file_raw().
  ReadPartialToolExecuteExtraMixin.test_execute_output_file_toon_format: Mixin#test_execute_output_file_toon_format().
  ReadPartialToolExecuteExtraMixin.test_execute_output_file_save_error: Mixin#test_execute_output_file_save_error().
  ReadPartialToolExecuteExtraMixin.test_execute_suppress_output_with_output_file: Mixin#test_execute_suppress_output_with_output_file().
  ReadPartialToolExecuteExtraMixin.test_execute_resolve_path_value_error: Mixin#test_execute_resolve_path_value_error().
  ReadPartialToolExecuteExtraMixin.test_execute_content_none: Mixin#test_execute_content_none().
  ReadPartialToolExecuteExtraContinuedMixin.test_execute_output_format_json: ContinuedMixin#test_execute_output_format_json().
  ReadPartialToolExecuteExtraContinuedMixin.test_execute_general_exception: ContinuedMixin#test_execute_general_exception().
  ReadPartialToolExecuteExtraMixin: Mixin#
  ReadPartialToolExecuteExtraContinuedMixin: ContinuedMixin#
  ReadPartialToolExecuteExtraContinuedMixin.test_agent_summary_for_small_exact_range: ContinuedMixin#test_agent_summary_for_small_exact_range().
  ReadPartialToolExecuteExtraContinuedMixin.test_agent_summary_for_large_range: ContinuedMixin#test_agent_summary_for_large_range().
---
# Module: [`tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py)

## Classes
### `ReadPartialToolExecuteExtraContinuedMixin`
- def: [`tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py:234`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py#L234)
- doc: Additional read_partial execute and agent summary tests.
- signature: `class ReadPartialToolExecuteExtraContinuedMixin:`
- members:
  - `test_agent_summary_for_large_range(self)` — [`L253`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py#L253)
  - `test_agent_summary_for_small_exact_range(self)` — [`L237`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py#L237)
  - `test_execute_general_exception(self)` — [`L294`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py#L294)
  - `test_execute_output_format_json(self)` — [`L270`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py#L270)
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.execute), [`build_agent_summary`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_helpers.md#build_agent_summary)  (1 test-only)
- used by: (1 test-only callers)

### `ReadPartialToolExecuteExtraMixin`
- def: [`tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py:16`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py#L16)
- doc: Additional tests for uncovered execute() paths.
- signature: `class ReadPartialToolExecuteExtraMixin:`
- members:
  - `test_execute_content_none(self)` — [`L30`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py#L30)
  - `test_execute_output_file_save_error(self)` — [`L168`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py#L168)
  - `test_execute_output_file_toon_format(self)` — [`L137`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py#L137)
  - `test_execute_resolve_path_value_error(self)` — [`L20`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py#L20)
  - `test_execute_success_with_output_file_json(self)` — [`L74`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py#L74)
  - `test_execute_success_with_output_file_raw(self)` — [`L106`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py#L106)
  - `test_execute_success_with_output_file_text(self)` — [`L42`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py#L42)
  - `test_execute_suppress_output_with_output_file(self)` — [`L201`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_execute_extra_mixins.py#L201)
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.execute), [`file_output_manager`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.file_output_manager)  (1 test-only)
- used by: (1 test-only callers)

