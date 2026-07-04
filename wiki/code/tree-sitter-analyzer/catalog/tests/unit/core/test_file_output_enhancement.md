---
title: 'Module: tests/unit/core/test_file_output_enhancement.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_file_output_enhancement.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_file_output_enhancement`/TestFileOutputEnhancement#
symbols:
  TestFileOutputEnhancement.test_query_code_with_file_output: test_query_code_with_file_output().
  TestFileOutputEnhancement.test_query_code_with_suppress_output: test_query_code_with_suppress_output().
  TestFileOutputEnhancement.test_query_code_summary_format_with_file_output: test_query_code_summary_format_with_file_output().
  TestFileOutputEnhancement.test_file_output_error_handling: test_file_output_error_handling().
  TestFileOutputEnhancement.test_automatic_extension_detection: test_automatic_extension_detection().
  TestFileOutputEnhancement.test_extract_code_section_with_file_output: test_extract_code_section_with_file_output().
  TestFileOutputEnhancement.test_extract_code_section_with_suppress_output: test_extract_code_section_with_suppress_output().
  TestFileOutputEnhancement.test_extract_code_section_argument_validation: test_extract_code_section_argument_validation().
  TestFileOutputEnhancement.test_query_code_argument_validation: test_query_code_argument_validation().
  TestFileOutputEnhancement: ''
  TestFileOutputEnhancement.temp_dir: temp_dir().
  TestFileOutputEnhancement.sample_python_file: sample_python_file().
  TestFileOutputEnhancement.sample_javascript_file: sample_javascript_file().
---
# Module: [`tests/unit/core/test_file_output_enhancement.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_enhancement.py)

## Classes
### `TestFileOutputEnhancement`
- def: [`tests/unit/core/test_file_output_enhancement.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_enhancement.py#L20)
- doc: Test file output enhancement for MCP tools
- signature: `class TestFileOutputEnhancement:`
- members:
  - `sample_javascript_file(self, temp_dir)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_enhancement.py#L58) — Create a sample JavaScript file for testing
  - `sample_python_file(self, temp_dir)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_enhancement.py#L30) — Create a sample Python file for testing
  - `temp_dir(self)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_enhancement.py#L24) — Create temporary directory for test files
  - `test_automatic_extension_detection(self, sample_python_file, temp_dir)` — [`L406`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_enhancement.py#L406) — Test automatic file extension detection
  - `test_extract_code_section_argument_validation(self, temp_dir)` — [`L328`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_enhancement.py#L328) — Test argument validation for extract_code_section tool
  - `test_extract_code_section_with_file_output(self, sample_python_file, temp_dir)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_enhancement.py#L84) — Test extract_code_section tool with file output functionality
  - `test_extract_code_section_with_suppress_output(self, sample_python_file, temp_dir)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_enhancement.py#L123) — Test extract_code_section tool with output suppression
  - `test_file_output_error_handling(self, sample_python_file, temp_dir)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_enhancement.py#L377) — Test error handling when file output fails
  - `test_query_code_argument_validation(self, temp_dir)` — [`L352`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_enhancement.py#L352) — Test argument validation for query_code tool
  - `test_query_code_summary_format_with_file_output(self, sample_python_file, temp_dir)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_enhancement.py#L261) — Test query_code tool with summary format and file output
  - `test_query_code_with_file_output(self, sample_javascript_file, temp_dir)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_enhancement.py#L155) — Test query_code tool with file output functionality
  - `test_query_code_with_suppress_output(self, sample_python_file, temp_dir)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_enhancement.py#L212) — Test query_code tool with output suppression
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.execute), [`execute`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool.execute), [`validate_arguments`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.validate_arguments), [`file_output_manager`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.file_output_manager), [`query_service`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool.query_service), [`validate_arguments`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool.validate_arguments)

