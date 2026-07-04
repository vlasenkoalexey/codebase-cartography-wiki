---
title: 'Module: tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_tools.test_get_code_outline_tool_toon`/TestGetCodeOutlineTool
symbols:
  TestGetCodeOutlineToolToonExecution.test_execute_with_toon_format_returns_flat_envelope: ToonExecution#test_execute_with_toon_format_returns_flat_envelope().
  TestGetCodeOutlineToolToonExecution.test_execute_with_json_format_returns_structured_dict: ToonExecution#test_execute_with_json_format_returns_structured_dict().
  TestGetCodeOutlineToolToonExecution.test_execute_defaults_to_toon_when_format_not_specified: ToonExecution#test_execute_defaults_to_toon_when_format_not_specified().
  TestGetCodeOutlineToolToonStructure.test_toon_output_contains_expected_fields: ToonStructure#test_toon_output_contains_expected_fields().
  TestGetCodeOutlineToolToonStructure.test_toon_output_uses_compact_format: ToonStructure#test_toon_output_uses_compact_format().
  TestGetCodeOutlineToolToonFormat.test_tool_schema_includes_output_format_parameter: ToonFormat#test_tool_schema_includes_output_format_parameter().
  TestGetCodeOutlineToolToonFormat.test_default_output_format_is_toon: ToonFormat#test_default_output_format_is_toon().
  TestGetCodeOutlineToolToonFormat.test_validate_arguments_accepts_toon_format: ToonFormat#test_validate_arguments_accepts_toon_format().
  TestGetCodeOutlineToolToonFormat.test_validate_arguments_accepts_json_format: ToonFormat#test_validate_arguments_accepts_json_format().
  TestGetCodeOutlineToolToonFormat.test_validate_arguments_rejects_invalid_format: ToonFormat#test_validate_arguments_rejects_invalid_format().
  TestGetCodeOutlineToolToonFormat.test_validate_arguments_allows_missing_output_format: ToonFormat#test_validate_arguments_allows_missing_output_format().
  TestGetCodeOutlineToolDefinition.test_get_tool_definition_includes_output_format: Definition#test_get_tool_definition_includes_output_format().
  TestGetCodeOutlineToolToonFormat: ToonFormat#
  TestGetCodeOutlineToolToonExecution: ToonExecution#
  TestGetCodeOutlineToolToonStructure: ToonStructure#
  TestGetCodeOutlineToolDefinition: Definition#
---
# Module: [`tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py)

## Classes
### `TestGetCodeOutlineToolDefinition`
- def: [`tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py:318`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py#L318)
- doc: 测试工具定义包含 output_format 信息
- signature: `class TestGetCodeOutlineToolDefinition:`
- members:
  - `test_get_tool_definition_includes_output_format(self)` — [`L321`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py#L321) — get_tool_definition 应包含 output_format 参数说明
- uses (calls/refs, reference-scoped): [`GetCodeOutlineTool`](../../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool), [`get_tool_definition`](../../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool.get_tool_definition)

### `TestGetCodeOutlineToolToonExecution`
- def: [`tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py:85`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py#L85)
- doc: 测试 TOON 格式的执行逻辑
- signature: `class TestGetCodeOutlineToolToonExecution:`
- members:
  - `test_execute_defaults_to_toon_when_format_not_specified(self)` — [`L183`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py#L183) — execute 在未指定格式时应默认使用 TOON, 返回 ``format=toon`` envelope.
  - `test_execute_with_json_format_returns_structured_dict(self)` — [`L141`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py#L141) — execute 使用 json 格式时应返回结构化 dict（无 toon_content blob）.
  - `test_execute_with_toon_format_returns_flat_envelope(self)` — [`L89`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py#L89) — execute 使用 toon 格式时应返回扁平 envelope，包含 toon_content blob.
- uses (calls/refs, reference-scoped): [`GetCodeOutlineTool`](../../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool.execute), [`analysis_engine`](../../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool.analysis_engine)

### `TestGetCodeOutlineToolToonFormat`
- def: [`tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py:20`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py#L20)
- doc: 测试 TOON 格式支持的基本功能
- signature: `class TestGetCodeOutlineToolToonFormat:`
- members:
  - `test_default_output_format_is_toon(self)` — [`L33`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py#L33) — 默认输出格式应为 TOON
  - `test_tool_schema_includes_output_format_parameter(self)` — [`L23`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py#L23) — 工具 schema 应包含 output_format 参数
  - `test_validate_arguments_accepts_json_format(self)` — [`L51`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py#L51) — 验证参数应接受 json 格式
  - `test_validate_arguments_accepts_toon_format(self)` — [`L40`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py#L40) — 验证参数应接受 toon 格式
  - `test_validate_arguments_allows_missing_output_format(self)` — [`L73`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py#L73) — 验证参数应允许省略 output_format（使用默认值）
  - `test_validate_arguments_rejects_invalid_format(self)` — [`L62`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py#L62) — 验证参数应拒绝无效格式
- uses (calls/refs, reference-scoped): [`GetCodeOutlineTool`](../../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool.validate_arguments), [`get_tool_schema`](../../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool.get_tool_schema)

### `TestGetCodeOutlineToolToonStructure`
- def: [`tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py:223`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py#L223)
- doc: 测试 TOON 格式输出的结构正确性
- signature: `class TestGetCodeOutlineToolToonStructure:`
- members:
  - `test_toon_output_contains_expected_fields(self)` — [`L227`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py#L227) — TOON 输出应包含预期的字段
  - `test_toon_output_uses_compact_format(self)` — [`L273`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_get_code_outline_tool_toon.py#L273) — TOON 输出应使用紧凑格式（无引号、无括号）
- uses (calls/refs, reference-scoped): [`GetCodeOutlineTool`](../../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool.execute), [`analysis_engine`](../../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool.analysis_engine)

