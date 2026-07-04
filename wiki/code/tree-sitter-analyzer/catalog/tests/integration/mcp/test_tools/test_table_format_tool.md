---
title: 'Module: tests/integration/mcp/test_tools/test_table_format_tool.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_tools/test_table_format_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_tools.test_table_format_tool`/TestTableFormatTool#
symbols:
  TestTableFormatTool.tool: tool.
  TestTableFormatTool.test_execute_with_file_output: test_execute_with_file_output().
  TestTableFormatTool.test_execute_file_output_error: test_execute_file_output_error().
  TestTableFormatTool.test_file_path: test_file_path.
  TestTableFormatTool.test_execute_success: test_execute_success().
  TestTableFormatTool.test_execute_with_explicit_language: test_execute_with_explicit_language().
  TestTableFormatTool.test_execute_different_formats: test_execute_different_formats().
  TestTableFormatTool.test_execute_structure_analysis_failure: test_execute_structure_analysis_failure().
  TestTableFormatTool.test_execute_file_not_found: test_execute_file_not_found().
  TestTableFormatTool._create_mock_structure_data: _create_mock_structure_data().
  TestTableFormatTool.test_java_content: test_java_content.
  TestTableFormatTool.teardown_method: teardown_method().
  TestTableFormatTool.test_get_tool_schema: test_get_tool_schema().
  TestTableFormatTool.test_get_tool_definition: test_get_tool_definition().
  TestTableFormatTool.test_get_tool_definition_fallback: test_get_tool_definition_fallback().
  TestTableFormatTool.test_execute_missing_file_path: test_execute_missing_file_path().
  TestTableFormatTool.test_validate_arguments_success: test_validate_arguments_success().
  TestTableFormatTool.test_validate_arguments_missing_required: test_validate_arguments_missing_required().
  TestTableFormatTool.test_validate_arguments_invalid_file_path: test_validate_arguments_invalid_file_path().
  TestTableFormatTool.test_validate_arguments_invalid_format_type: test_validate_arguments_invalid_format_type().
  TestTableFormatTool.test_validate_arguments_invalid_language: test_validate_arguments_invalid_language().
  TestTableFormatTool.test_validate_arguments_invalid_output_file: test_validate_arguments_invalid_output_file().
  TestTableFormatTool.test_init: test_init().
  TestTableFormatTool.temp_dir: temp_dir.
  TestTableFormatTool: ''
  TestTableFormatTool.setup_method: setup_method().
---
# Module: [`tests/integration/mcp/test_tools/test_table_format_tool.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py)

## Classes
### `TestTableFormatTool`
- def: [`tests/integration/mcp/test_tools/test_table_format_tool.py:19`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L19)
- doc: Test cases for TableFormatTool class.
- signature: `class TestTableFormatTool:`
- members:
  - `_create_mock_structure_data(self)` — [`L567`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L567) — Create mock structure data matching the actual implementation format.
  - `setup_method(self)` — [`L22`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L22) — Set up test fixtures before each test method.
  - `teardown_method(self)` — [`L48`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L48) — Clean up test fixtures after each test method.
  - `test_execute_different_formats(self, mocker)` — [`L282`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L282) — Test execute with different output formats.
  - `test_execute_file_not_found(self, mocker)` — [`L178`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L178) — Test execute with non-existent file.
  - `test_execute_file_output_error(self, mocker)` — [`L426`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L426) — Test execute with file output error handling.
  - `test_execute_missing_file_path(self)` — [`L170`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L170) — Test execute with missing file_path argument.
  - `test_execute_structure_analysis_failure(self, mocker)` — [`L244`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L244) — Test execute when structure analysis fails.
  - `test_execute_success(self, mocker)` — [`L106`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L106) — Test successful execution of analyze_code_structure tool with CLI-compatible flow.
  - `test_execute_with_explicit_language(self, mocker)` — [`L194`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L194) — Test execute with explicitly specified language.
  - `test_execute_with_file_output(self, mocker)` — [`L350`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L350) — Test execute with file output functionality.
  - `test_get_tool_definition(self, mocker)` — [`L87`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L87) — Test get_tool_definition method.
  - `test_get_tool_definition_fallback(self, mocker)` — [`L96`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L96) — Test get_tool_definition fallback when MCP is not available.
  - `test_get_tool_schema(self)` — [`L61`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L61) — Test get_tool_schema method returns proper JSON schema.
  - `test_init(self)` — [`L56`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L56) — Test TableFormatTool initialization.
  - `test_validate_arguments_invalid_file_path(self)` — [`L524`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L524) — Test validation with invalid file_path.
  - `test_validate_arguments_invalid_format_type(self)` — [`L536`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L536) — Test validation with invalid format_type.
  - `test_validate_arguments_invalid_language(self)` — [`L548`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L548) — Test validation with invalid language.
  - `test_validate_arguments_invalid_output_file(self)` — [`L555`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L555) — Test validation with invalid output_file.
  - `test_validate_arguments_missing_required(self)` — [`L517`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L517) — Test validation with missing required arguments.
  - `test_validate_arguments_success(self)` — [`L505`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L505) — Test successful argument validation.
  - `temp_dir` — [`L27`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L27)
  - `test_file_path` — [`L28`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L28)
  - `test_java_content` — [`L31`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L31)
  - `tool` — [`L24`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_table_format_tool.py#L24)
- uses (calls/refs, reference-scoped): [`AnalyzeCodeStructureTool`](../../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute), [`path_resolver`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.path_resolver), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.validate_arguments), [`get_tool_definition`](../../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.get_tool_definition), [`file_output_manager`](../../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.file_output_manager), [`analysis_engine`](../../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.analysis_engine), [`get_tool_schema`](../../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.get_tool_schema)

