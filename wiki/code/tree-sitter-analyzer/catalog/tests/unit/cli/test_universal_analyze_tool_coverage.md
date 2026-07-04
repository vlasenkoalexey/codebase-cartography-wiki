---
title: 'Module: tests/unit/cli/test_universal_analyze_tool_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_universal_analyze_tool_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_universal_analyze_tool_coverage`/TestUniversalAnalyzeTool
symbols:
  TestUniversalAnalyzeToolAnalysisTypes.tool: AnalysisTypes#tool().
  TestUniversalAnalyzeToolValidation.tool: Validation#tool().
  TestUniversalAnalyzeToolConfiguration.tool: Configuration#tool().
  TestUniversalAnalyzeToolErrorHandling.tool: ErrorHandling#tool().
  TestUniversalAnalyzeToolErrorHandling.test_execute_invalid_analysis_type: ErrorHandling#test_execute_invalid_analysis_type().
  TestUniversalAnalyzeToolErrorHandling.test_execute_unsupported_language: ErrorHandling#test_execute_unsupported_language().
  TestUniversalAnalyzeToolErrorHandling.test_execute_unknown_file_extension: ErrorHandling#test_execute_unknown_file_extension().
  TestUniversalAnalyzeToolAnalysisTypes: AnalysisTypes#
  TestUniversalAnalyzeToolAnalysisTypes.temp_dir: AnalysisTypes#temp_dir().
  TestUniversalAnalyzeToolAnalysisTypes.sample_python_file: AnalysisTypes#sample_python_file().
  TestUniversalAnalyzeToolAnalysisTypes.sample_java_file: AnalysisTypes#sample_java_file().
  TestUniversalAnalyzeToolAnalysisTypes.test_execute_basic_analysis: AnalysisTypes#test_execute_basic_analysis().
  TestUniversalAnalyzeToolAnalysisTypes.test_execute_detailed_analysis: AnalysisTypes#test_execute_detailed_analysis().
  TestUniversalAnalyzeToolAnalysisTypes.test_execute_structure_analysis: AnalysisTypes#test_execute_structure_analysis().
  TestUniversalAnalyzeToolAnalysisTypes.test_execute_metrics_analysis: AnalysisTypes#test_execute_metrics_analysis().
  TestUniversalAnalyzeToolAnalysisTypes.test_execute_with_include_ast: AnalysisTypes#test_execute_with_include_ast().
  TestUniversalAnalyzeToolAnalysisTypes.test_execute_with_include_queries: AnalysisTypes#test_execute_with_include_queries().
  TestUniversalAnalyzeToolAnalysisTypes.test_execute_java_file_basic: AnalysisTypes#test_execute_java_file_basic().
  TestUniversalAnalyzeToolAnalysisTypes.test_execute_java_file_detailed: AnalysisTypes#test_execute_java_file_detailed().
  TestUniversalAnalyzeToolAnalysisTypes.test_execute_java_file_structure: AnalysisTypes#test_execute_java_file_structure().
  TestUniversalAnalyzeToolAnalysisTypes.test_execute_java_file_metrics: AnalysisTypes#test_execute_java_file_metrics().
  TestUniversalAnalyzeToolAnalysisTypes.test_execute_java_with_include_ast: AnalysisTypes#test_execute_java_with_include_ast().
  TestUniversalAnalyzeToolAnalysisTypes.test_execute_java_with_include_queries: AnalysisTypes#test_execute_java_with_include_queries().
  TestUniversalAnalyzeToolValidation: Validation#
  TestUniversalAnalyzeToolValidation.temp_dir: Validation#temp_dir().
  TestUniversalAnalyzeToolValidation.test_validate_arguments_valid: Validation#test_validate_arguments_valid().
  TestUniversalAnalyzeToolValidation.test_validate_arguments_missing_file_path: Validation#test_validate_arguments_missing_file_path().
  TestUniversalAnalyzeToolValidation.test_validate_arguments_invalid_file_path_type: Validation#test_validate_arguments_invalid_file_path_type().
  TestUniversalAnalyzeToolValidation.test_validate_arguments_empty_file_path: Validation#test_validate_arguments_empty_file_path().
  TestUniversalAnalyzeToolValidation.test_validate_arguments_invalid_language_type: Validation#test_validate_arguments_invalid_language_type().
  TestUniversalAnalyzeToolValidation.test_validate_arguments_invalid_analysis_type_type: Validation#test_validate_arguments_invalid_analysis_type_type().
  TestUniversalAnalyzeToolValidation.test_validate_arguments_invalid_analysis_type_value: Validation#test_validate_arguments_invalid_analysis_type_value().
  TestUniversalAnalyzeToolValidation.test_validate_arguments_invalid_include_ast_type: Validation#test_validate_arguments_invalid_include_ast_type().
  TestUniversalAnalyzeToolValidation.test_validate_arguments_invalid_include_queries_type: Validation#test_validate_arguments_invalid_include_queries_type().
  TestUniversalAnalyzeToolConfiguration: Configuration#
  TestUniversalAnalyzeToolConfiguration.temp_dir: Configuration#temp_dir().
  TestUniversalAnalyzeToolConfiguration.test_get_tool_definition: Configuration#test_get_tool_definition().
  TestUniversalAnalyzeToolConfiguration.test_set_project_path: Configuration#test_set_project_path().
  TestUniversalAnalyzeToolErrorHandling: ErrorHandling#
  TestUniversalAnalyzeToolErrorHandling.temp_dir: ErrorHandling#temp_dir().
  TestUniversalAnalyzeToolErrorHandling.test_execute_with_explicit_language: ErrorHandling#test_execute_with_explicit_language().
---
# Module: [`tests/unit/cli/test_universal_analyze_tool_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py)

## Classes
### `TestUniversalAnalyzeToolAnalysisTypes`
- def: [`tests/unit/cli/test_universal_analyze_tool_coverage.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L18)
- doc: Test different analysis types in UniversalAnalyzeTool.
- signature: `class TestUniversalAnalyzeToolAnalysisTypes:`
- members:
  - `sample_java_file(self, temp_dir)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L61) — Create a sample Java file for testing.
  - `sample_python_file(self, temp_dir)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L33) — Create a sample Python file for testing.
  - `temp_dir(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L22) — Create a temporary directory for testing.
  - `test_execute_basic_analysis(self, tool, sample_python_file)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L88) — Test basic analysis type.
  - `test_execute_detailed_analysis(self, tool, sample_python_file)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L99) — Test detailed analysis type.
  - `test_execute_java_file_basic(self, tool, sample_java_file)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L149) — Test Java file analysis with basic type.
  - `test_execute_java_file_detailed(self, tool, sample_java_file)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L159) — Test Java file analysis with detailed type.
  - `test_execute_java_file_metrics(self, tool, sample_java_file)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L177) — Test Java file analysis with metrics type.
  - `test_execute_java_file_structure(self, tool, sample_java_file)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L168) — Test Java file analysis with structure type.
  - `test_execute_java_with_include_ast(self, tool, sample_java_file)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L186) — Test Java file analysis with include_ast option.
  - `test_execute_java_with_include_queries(self, tool, sample_java_file)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L195) — Test Java file analysis with include_queries option.
  - `test_execute_metrics_analysis(self, tool, sample_python_file)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L119) — Test metrics analysis type.
  - `test_execute_structure_analysis(self, tool, sample_python_file)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L109) — Test structure analysis type.
  - `test_execute_with_include_ast(self, tool, sample_python_file)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L129) — Test analysis with include_ast option.
  - `test_execute_with_include_queries(self, tool, sample_python_file)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L139) — Test analysis with include_queries option.
  - `tool(self, temp_dir)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L28) — Create a UniversalAnalyzeTool instance for testing.
- uses (calls/refs, reference-scoped): [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool)

### `TestUniversalAnalyzeToolConfiguration`
- def: [`tests/unit/cli/test_universal_analyze_tool_coverage.py:273`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L273)
- doc: Test configuration methods in UniversalAnalyzeTool.
- signature: `class TestUniversalAnalyzeToolConfiguration:`
- members:
  - `temp_dir(self)` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L277) — Create a temporary directory for testing.
  - `test_get_tool_definition(self, tool)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L287) — Test get_tool_definition returns valid schema.
  - `test_set_project_path(self, tool, temp_dir)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L303) — Test set_project_path updates the project path.
  - `tool(self, temp_dir)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L283) — Create a UniversalAnalyzeTool instance for testing.
- uses (calls/refs, reference-scoped): [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool)

### `TestUniversalAnalyzeToolErrorHandling`
- def: [`tests/unit/cli/test_universal_analyze_tool_coverage.py:316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L316)
- doc: Test error handling in UniversalAnalyzeTool.
- signature: `class TestUniversalAnalyzeToolErrorHandling:`
- members:
  - `temp_dir(self)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L320) — Create a temporary directory for testing.
  - `test_execute_invalid_analysis_type(self, tool, temp_dir)` — [`L331`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L331) — Test execute with invalid analysis_type.
  - `test_execute_unknown_file_extension(self, tool, temp_dir)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L357) — Test execute with unknown file extension.
  - `test_execute_unsupported_language(self, tool, temp_dir)` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L344) — Test execute with unsupported language.
  - `test_execute_with_explicit_language(self, tool, temp_dir)` — [`L370`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L370) — Test execute with explicitly specified language.
  - `tool(self, temp_dir)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L326) — Create a UniversalAnalyzeTool instance for testing.
- uses (calls/refs, reference-scoped): [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`AnalysisError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#AnalysisError)

### `TestUniversalAnalyzeToolValidation`
- def: [`tests/unit/cli/test_universal_analyze_tool_coverage.py:205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L205)
- doc: Test argument validation in UniversalAnalyzeTool.
- signature: `class TestUniversalAnalyzeToolValidation:`
- members:
  - `temp_dir(self)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L209) — Create a temporary directory for testing.
  - `test_validate_arguments_empty_file_path(self, tool)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L236) — Test validate_arguments with empty file_path.
  - `test_validate_arguments_invalid_analysis_type_type(self, tool)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L248) — Test validate_arguments with invalid analysis_type type.
  - `test_validate_arguments_invalid_analysis_type_value(self, tool)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L254) — Test validate_arguments with invalid analysis_type value.
  - `test_validate_arguments_invalid_file_path_type(self, tool)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L230) — Test validate_arguments with invalid file_path type.
  - `test_validate_arguments_invalid_include_ast_type(self, tool)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L260) — Test validate_arguments with invalid include_ast type.
  - `test_validate_arguments_invalid_include_queries_type(self, tool)` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L266) — Test validate_arguments with invalid include_queries type.
  - `test_validate_arguments_invalid_language_type(self, tool)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L242) — Test validate_arguments with invalid language type.
  - `test_validate_arguments_missing_file_path(self, tool)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L224) — Test validate_arguments with missing file_path.
  - `test_validate_arguments_valid(self, tool)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L219) — Test validate_arguments with valid arguments.
  - `tool(self, temp_dir)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_coverage.py#L215) — Create a UniversalAnalyzeTool instance for testing.
- uses (calls/refs, reference-scoped): [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool)

