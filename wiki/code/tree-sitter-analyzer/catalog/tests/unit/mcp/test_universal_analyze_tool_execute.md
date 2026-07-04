---
title: 'Module: tests/unit/mcp/test_universal_analyze_tool_execute.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_universal_analyze_tool_execute.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_universal_analyze_tool_execute`/
symbols:
  tool: tool().
  TestUniversalAnalyzeToolExecute.test_execute_missing_file_path: TestUniversalAnalyzeToolExecute#test_execute_missing_file_path().
  TestUniversalAnalyzeToolExecute.test_execute_file_not_found: TestUniversalAnalyzeToolExecute#test_execute_file_not_found().
  TestUniversalAnalyzeToolExecute.test_execute_language_not_detected: TestUniversalAnalyzeToolExecute#test_execute_language_not_detected().
  TestUniversalAnalyzeToolExecute.test_execute_language_not_supported: TestUniversalAnalyzeToolExecute#test_execute_language_not_supported().
  TestUniversalAnalyzeToolExecute.test_execute_invalid_analysis_type: TestUniversalAnalyzeToolExecute#test_execute_invalid_analysis_type().
  TestUniversalAnalyzeToolExecute: TestUniversalAnalyzeToolExecute#
  TestUniversalAnalyzeToolExecute.test_execute_success_basic_analysis: TestUniversalAnalyzeToolExecute#test_execute_success_basic_analysis().
  TestUniversalAnalyzeToolExecute.test_execute_success_detailed_analysis: TestUniversalAnalyzeToolExecute#test_execute_success_detailed_analysis().
  TestUniversalAnalyzeToolExecute.test_execute_success_structure_analysis: TestUniversalAnalyzeToolExecute#test_execute_success_structure_analysis().
  TestUniversalAnalyzeToolExecute.test_execute_success_metrics_analysis: TestUniversalAnalyzeToolExecute#test_execute_success_metrics_analysis().
  TestUniversalAnalyzeToolExecute.test_execute_with_include_ast: TestUniversalAnalyzeToolExecute#test_execute_with_include_ast().
  TestUniversalAnalyzeToolExecute.test_execute_with_include_queries: TestUniversalAnalyzeToolExecute#test_execute_with_include_queries().
  TestUniversalAnalyzeToolExecute.test_execute_with_json_output_format: TestUniversalAnalyzeToolExecute#test_execute_with_json_output_format().
  TestUniversalAnalyzeToolExecute.test_execute_analysis_failure: TestUniversalAnalyzeToolExecute#test_execute_analysis_failure().
---
# Module: [`tests/unit/mcp/test_universal_analyze_tool_execute.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_execute.py)

## Classes
### `TestUniversalAnalyzeToolExecute`
- def: [`tests/unit/mcp/test_universal_analyze_tool_execute.py:22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_execute.py#L22)
- doc: Tests for execute method.
- signature: `class TestUniversalAnalyzeToolExecute:`
- members:
  - `test_execute_analysis_failure(self, tool)` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_execute.py#L393) — Test execute handles analysis engine failure.
  - `test_execute_file_not_found(self, tool)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_execute.py#L33) — Test execute fails when file doesn't exist.
  - `test_execute_invalid_analysis_type(self, tool)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_execute.py#L86) — Test execute fails when analysis_type is invalid.
  - `test_execute_language_not_detected(self, tool)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_execute.py#L48) — Test execute fails when language cannot be detected.
  - `test_execute_language_not_supported(self, tool)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_execute.py#L65) — Test execute fails when language is not supported.
  - `test_execute_missing_file_path(self, tool)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_execute.py#L26) — Test execute fails when file_path is missing.
  - `test_execute_success_basic_analysis(self, tool)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_execute.py#L107) — Test successful basic analysis.
  - `test_execute_success_detailed_analysis(self, tool)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_execute.py#L147) — Test successful detailed analysis.
  - `test_execute_success_metrics_analysis(self, tool)` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_execute.py#L227) — Test successful metrics analysis.
  - `test_execute_success_structure_analysis(self, tool)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_execute.py#L187) — Test successful structure analysis.
  - `test_execute_with_include_ast(self, tool)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_execute.py#L267) — Test execute with include_ast=True.
  - `test_execute_with_include_queries(self, tool)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_execute.py#L307) — Test execute with include_queries=True.
  - `test_execute_with_json_output_format(self, tool)` — [`L353`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_execute.py#L353) — Test execute with output_format='json'.
- uses (calls/refs, reference-scoped): [`AnalysisError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#AnalysisError)

## Functions
- `tool()` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_execute.py#L17) — Create a UniversalAnalyzeTool instance for testing.

