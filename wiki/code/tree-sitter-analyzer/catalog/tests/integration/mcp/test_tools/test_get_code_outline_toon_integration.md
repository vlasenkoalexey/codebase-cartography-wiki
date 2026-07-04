---
title: 'Module: tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_tools.test_get_code_outline_toon_integration`/
symbols:
  _payload_text: _payload_text().
  TestGetCodeOutlineToonIntegrationPython.test_python_file_toon_output_structure: TestGetCodeOutlineToonIntegrationPython#test_python_file_toon_output_structure().
  TestGetCodeOutlineToonIntegrationPython.test_python_file_toon_detects_classes_and_methods: TestGetCodeOutlineToonIntegrationPython#test_python_file_toon_detects_classes_and_methods().
  TestGetCodeOutlineToonIntegrationPython.test_python_file_json_format_parseable: TestGetCodeOutlineToonIntegrationPython#test_python_file_json_format_parseable().
  TestGetCodeOutlineToonIntegrationJava.test_java_file_toon_output_structure: TestGetCodeOutlineToonIntegrationJava#test_java_file_toon_output_structure().
  TestGetCodeOutlineToonIntegrationJava.test_java_file_toon_detects_class: TestGetCodeOutlineToonIntegrationJava#test_java_file_toon_detects_class().
  TestGetCodeOutlineToonIntegrationJava.test_java_file_default_format_is_toon: TestGetCodeOutlineToonIntegrationJava#test_java_file_default_format_is_toon().
  TestGetCodeOutlineToonVsJsonComparison.test_toon_is_shorter_than_json: TestGetCodeOutlineToonVsJsonComparison#test_toon_is_shorter_than_json().
  TestGetCodeOutlineToonVsJsonComparison.test_both_formats_contain_same_class_names: TestGetCodeOutlineToonVsJsonComparison#test_both_formats_contain_same_class_names().
  TestGetCodeOutlineToonVsJsonComparison.test_result_type_is_text_content_block: TestGetCodeOutlineToonVsJsonComparison#test_result_type_is_text_content_block().
  JAVA_CODE: JAVA_CODE.
  PYTHON_CODE: PYTHON_CODE.
  TestGetCodeOutlineToonIntegrationPython: TestGetCodeOutlineToonIntegrationPython#
  TestGetCodeOutlineToonIntegrationJava: TestGetCodeOutlineToonIntegrationJava#
  TestGetCodeOutlineToonVsJsonComparison: TestGetCodeOutlineToonVsJsonComparison#
---
# Module: [`tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py)

## Classes
### `TestGetCodeOutlineToonIntegrationJava`
- def: [`tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py:192`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py#L192)
- doc: Java 文件 TOON 格式集成测试
- signature: `class TestGetCodeOutlineToonIntegrationJava:`
- members:
  - `test_java_file_default_format_is_toon(self)` — [`L239`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py#L239) — 指定 output_format=toon 应返回 TOON 格式
  - `test_java_file_toon_detects_class(self)` — [`L219`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py#L219) — Java 文件 TOON 输出应检测到 DataService 类
  - `test_java_file_toon_output_structure(self)` — [`L197`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py#L197) — Java 文件 TOON 格式输出应包含预期结构字段
- uses (calls/refs, reference-scoped): [`GetCodeOutlineTool`](../../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool.execute)  (2 test-only)

### `TestGetCodeOutlineToonIntegrationPython`
- def: [`tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py:105`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py#L105)
- doc: Python 文件 TOON 格式集成测试
- signature: `class TestGetCodeOutlineToonIntegrationPython:`
- members:
  - `test_python_file_json_format_parseable(self)` — [`L164`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py#L164) — Python 文件 JSON 格式应可解析
  - `test_python_file_toon_detects_classes_and_methods(self)` — [`L142`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py#L142) — Python 文件 TOON 输出应检测到类和方法
  - `test_python_file_toon_output_structure(self)` — [`L110`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py#L110) — Python 文件 TOON 格式输出应包含预期结构字段
- uses (calls/refs, reference-scoped): [`GetCodeOutlineTool`](../../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool.execute)  (2 test-only)

### `TestGetCodeOutlineToonVsJsonComparison`
- def: [`tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py:266`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py#L266)
- doc: TOON 与 JSON 格式对比测试
- signature: `class TestGetCodeOutlineToonVsJsonComparison:`
- members:
  - `test_both_formats_contain_same_class_names(self)` — [`L299`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py#L299) — TOON 和 JSON 应包含相同的类名信息
  - `test_result_type_is_text_content_block(self)` — [`L330`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py#L330) — 两种格式的返回值都应是 MCP text content block
  - `test_toon_is_shorter_than_json(self)` — [`L271`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py#L271) — TOON 输出长度应小于等效 JSON 输出
- uses (calls/refs, reference-scoped): [`GetCodeOutlineTool`](../../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool.execute)  (3 test-only)

## Functions
- `_payload_text(result: dict)` — [`L18`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py#L18) — Normalize v1.13.0+ direct-dict and legacy MCP-wrapped outputs.

## Module values
- `JAVA_CODE` — [`L65`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py#L65)
- `PYTHON_CODE` — [`L34`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_toon_integration.py#L34)

