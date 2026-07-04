---
title: 'Module: tests/integration/formatters/test_real_integration.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/test_real_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters.test_real_integration`/
symbols:
  TestRealIntegration.run_validation: TestRealIntegration#run_validation().
  run_integration_tests: run_integration_tests().
  TestRealIntegration.test_schema_validation_with_real_output: TestRealIntegration#test_schema_validation_with_real_output().
  TestRealIntegration.test_table_format_tool_integration: TestRealIntegration#test_table_format_tool_integration().
  TestRealIntegration.test_format_consistency_across_types: TestRealIntegration#test_format_consistency_across_types().
  TestRealIntegration.test_quick_validation_with_real_analyzer: TestRealIntegration#test_quick_validation_with_real_analyzer().
  TestRealIntegration.real_analyzer_function: TestRealIntegration#real_analyzer_function().
  TestRealIntegration: TestRealIntegration#
  TestRealIntegration.temp_python_file: TestRealIntegration#temp_python_file().
---
# Module: [`tests/integration/formatters/test_real_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_real_integration.py)

## Classes
### `TestRealIntegration`
- def: [`tests/integration/formatters/test_real_integration.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_real_integration.py#L20)
- doc: Test with real tree-sitter-analyzer functionality
- signature: `class TestRealIntegration:`
- members:
  - `real_analyzer_function(source_code: str, format_type: str = "full")` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_real_integration.py#L227)
  - `run_validation()` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_real_integration.py#L162)
  - `temp_python_file(self)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_real_integration.py#L24) — Create temporary Python file for testing
  - `test_format_consistency_across_types(self, temp_python_file)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_real_integration.py#L119) — Test format consistency across different output types
  - `test_quick_validation_with_real_analyzer(self, temp_python_file)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_real_integration.py#L222) — Test quick validation function with real analyzer
  - `test_schema_validation_with_real_output(self, temp_python_file)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_real_integration.py#L153) — Test schema validation with real analyzer output
  - `test_table_format_tool_integration(self, temp_python_file)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_real_integration.py#L65) — Test TableFormatTool with format testing framework
- uses (calls/refs, reference-scoped): [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute)  (7 test-only)
- used by: (1 test-only callers)

## Functions
- `run_integration_tests()` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_real_integration.py#L266)

