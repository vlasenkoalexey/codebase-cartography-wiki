---
title: 'Module: tests/unit/mcp/test_analyze_code_structure_tool_execute.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_analyze_code_structure_tool_execute.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_analyze_code_structure_tool_execute`/
symbols:
  tool: tool().
  tool_with_project_root: tool_with_project_root().
  TestAnalyzeCodeStructureToolExecute.test_extract_metadata_from_result: TestAnalyzeCodeStructureToolExecute#test_extract_metadata_from_result().
  TestAnalyzeCodeStructureToolExecute: TestAnalyzeCodeStructureToolExecute#
  TestAnalyzeCodeStructureToolExecute.test_execute_file_not_found: TestAnalyzeCodeStructureToolExecute#test_execute_file_not_found().
  TestAnalyzeCodeStructureToolExecute.test_execute_success_full_format: TestAnalyzeCodeStructureToolExecute#test_execute_success_full_format().
  TestAnalyzeCodeStructureToolExecute.test_execute_success_compact_format: TestAnalyzeCodeStructureToolExecute#test_execute_success_compact_format().
  TestAnalyzeCodeStructureToolExecute.test_execute_success_csv_format: TestAnalyzeCodeStructureToolExecute#test_execute_success_csv_format().
  TestAnalyzeCodeStructureToolExecute.test_execute_with_language_specified: TestAnalyzeCodeStructureToolExecute#test_execute_with_language_specified().
  TestAnalyzeCodeStructureToolExecute.test_execute_with_file_output: TestAnalyzeCodeStructureToolExecute#test_execute_with_file_output().
  TestAnalyzeCodeStructureToolExecute.test_execute_with_suppress_output: TestAnalyzeCodeStructureToolExecute#test_execute_with_suppress_output().
  TestAnalyzeCodeStructureToolExecute.test_execute_with_output_format_json: TestAnalyzeCodeStructureToolExecute#test_execute_with_output_format_json().
  TestAnalyzeCodeStructureToolExecute.test_execute_with_output_format_toon: TestAnalyzeCodeStructureToolExecute#test_execute_with_output_format_toon().
  TestAnalyzeCodeStructureToolExecute.test_execute_analysis_failure: TestAnalyzeCodeStructureToolExecute#test_execute_analysis_failure().
  TestAnalyzeCodeStructureToolExecute.test_execute_unsupported_format_type: TestAnalyzeCodeStructureToolExecute#test_execute_unsupported_format_type().
  TestAnalyzeCodeStructureToolExecute.test_execute_file_save_error: TestAnalyzeCodeStructureToolExecute#test_execute_file_save_error().
---
# Module: [`tests/unit/mcp/test_analyze_code_structure_tool_execute.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_execute.py)

## Classes
### `TestAnalyzeCodeStructureToolExecute`
- def: [`tests/unit/mcp/test_analyze_code_structure_tool_execute.py:31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_execute.py#L31)
- doc: Tests for execute method.
- signature: `class TestAnalyzeCodeStructureToolExecute:`
- members:
  - `test_execute_analysis_failure(self, tool)` — [`L448`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_execute.py#L448) — Test execute handles analysis engine failure.
  - `test_execute_file_not_found(self, tool)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_execute.py#L35) — Test execute fails when file doesn't exist.
  - `test_execute_file_save_error(self, tool, tmp_path)` — [`L509`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_execute.py#L509) — Test execute handles file save error.
  - `test_execute_success_compact_format(self, tool, tmp_path)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_execute.py#L100) — Test successful execution with compact format.
  - `test_execute_success_csv_format(self, tool, tmp_path)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_execute.py#L152) — Test successful execution with CSV format.
  - `test_execute_success_full_format(self, tool, tmp_path)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_execute.py#L48) — Test successful execution with full format.
  - `test_execute_unsupported_format_type(self, tool, tmp_path)` — [`L467`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_execute.py#L467) — Test execute fails with unsupported format type.
  - `test_execute_with_file_output(self, tool, tmp_path)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_execute.py#L247) — Test execute with file output enabled.
  - `test_execute_with_language_specified(self, tool, tmp_path)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_execute.py#L202) — Test execute with language explicitly specified.
  - `test_execute_with_output_format_json(self, tool, tmp_path)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_execute.py#L356) — Test execute with output_format='json'.
  - `test_execute_with_output_format_toon(self, tool, tmp_path)` — [`L402`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_execute.py#L402) — Test execute with output_format='toon'.
  - `test_execute_with_suppress_output(self, tool, tmp_path)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_execute.py#L299) — Test execute with suppress_output enabled.
  - `test_extract_metadata_from_result(self, tool)` — [`L564`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_execute.py#L564) — Test metadata extraction from analysis result.
- uses (calls/refs, reference-scoped): [`_convert_analysis_result`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#_convert_analysis_result)

## Functions
- `tool()` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_execute.py#L20) — Create an AnalyzeCodeStructureTool instance for testing.
- `tool_with_project_root()` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_execute.py#L26) — Create an AnalyzeCodeStructureTool instance with a project root.

