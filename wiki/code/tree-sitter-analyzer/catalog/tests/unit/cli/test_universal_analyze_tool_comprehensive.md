---
title: 'Module: tests/unit/cli/test_universal_analyze_tool_comprehensive.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_universal_analyze_tool_comprehensive.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_universal_analyze_tool_comprehensive`/Test
symbols:
  TestUniversalAnalyzeToolInitialization.test_init_without_project_root: UniversalAnalyzeToolInitialization#test_init_without_project_root().
  TestUniversalAnalyzeToolInitialization.test_init_with_project_root: UniversalAnalyzeToolInitialization#test_init_with_project_root().
  TestUniversalAnalyzeToolInitialization.test_set_project_path: UniversalAnalyzeToolInitialization#test_set_project_path().
  TestExecution.test_execute_missing_file_path: Execution#test_execute_missing_file_path().
  TestExecution.test_execute_file_not_found: Execution#test_execute_file_not_found().
  TestExecution.test_execute_language_detection_failure: Execution#test_execute_language_detection_failure().
  TestExecution.test_execute_invalid_analysis_type: Execution#test_execute_invalid_analysis_type().
  TestExecution.test_execute_basic_analysis_python: Execution#test_execute_basic_analysis_python().
  TestExecution.test_execute_detailed_analysis: Execution#test_execute_detailed_analysis().
  TestExecution.test_execute_with_include_ast: Execution#test_execute_with_include_ast().
  TestExecution.test_execute_with_include_queries: Execution#test_execute_with_include_queries().
  TestExecution.test_execute_structure_analysis: Execution#test_execute_structure_analysis().
  TestExecution.test_execute_metrics_analysis: Execution#test_execute_metrics_analysis().
  TestAvailableQueries.test_get_available_queries_python: AvailableQueries#test_get_available_queries_python().
  TestAvailableQueries.test_get_available_queries_error_handling: AvailableQueries#test_get_available_queries_error_handling().
  TestEdgeCases.test_execute_with_special_characters_in_path: EdgeCases#test_execute_with_special_characters_in_path().
  TestEdgeCases.test_execute_with_empty_file: EdgeCases#test_execute_with_empty_file().
  TestEdgeCases.test_execute_with_analysis_failure: EdgeCases#test_execute_with_analysis_failure().
  TestToolDefinition.test_get_tool_definition_structure: ToolDefinition#test_get_tool_definition_structure().
  TestToolDefinition.test_tool_definition_schema: ToolDefinition#test_tool_definition_schema().
  TestToolDefinition.test_analysis_type_enum: ToolDefinition#test_analysis_type_enum().
  TestArgumentValidation.test_validate_arguments_valid_minimal: ArgumentValidation#test_validate_arguments_valid_minimal().
  TestArgumentValidation.test_validate_arguments_valid_complete: ArgumentValidation#test_validate_arguments_valid_complete().
  TestArgumentValidation.test_validate_arguments_missing_file_path: ArgumentValidation#test_validate_arguments_missing_file_path().
  TestArgumentValidation.test_validate_arguments_invalid_file_path_type: ArgumentValidation#test_validate_arguments_invalid_file_path_type().
  TestArgumentValidation.test_validate_arguments_empty_file_path: ArgumentValidation#test_validate_arguments_empty_file_path().
  TestArgumentValidation.test_validate_arguments_invalid_language_type: ArgumentValidation#test_validate_arguments_invalid_language_type().
  TestArgumentValidation.test_validate_arguments_invalid_analysis_type: ArgumentValidation#test_validate_arguments_invalid_analysis_type().
  TestArgumentValidation.test_validate_arguments_invalid_include_ast_type: ArgumentValidation#test_validate_arguments_invalid_include_ast_type().
  TestArgumentValidation.test_validate_arguments_invalid_include_queries_type: ArgumentValidation#test_validate_arguments_invalid_include_queries_type().
  TestExecution.test_execute_unsupported_language: Execution#test_execute_unsupported_language().
  TestMetricsExtraction.test_extract_universal_basic_metrics: MetricsExtraction#test_extract_universal_basic_metrics().
  TestMetricsExtraction.test_extract_universal_detailed_metrics: MetricsExtraction#test_extract_universal_detailed_metrics().
  TestMetricsExtraction.test_extract_universal_structure_info: MetricsExtraction#test_extract_universal_structure_info().
  TestMetricsExtraction.test_extract_universal_comprehensive_metrics: MetricsExtraction#test_extract_universal_comprehensive_metrics().
  TestUniversalAnalyzeToolInitialization: UniversalAnalyzeToolInitialization#
  TestToolDefinition: ToolDefinition#
  TestArgumentValidation: ArgumentValidation#
  TestExecution: Execution#
  TestMetricsExtraction: MetricsExtraction#
  TestAvailableQueries: AvailableQueries#
  TestEdgeCases: EdgeCases#
---
# Module: [`tests/unit/cli/test_universal_analyze_tool_comprehensive.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py)

## Classes
### `TestArgumentValidation`
- def: [`tests/unit/cli/test_universal_analyze_tool_comprehensive.py:83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L83)
- doc: Test argument validation
- signature: `class TestArgumentValidation:`
- members:
  - `test_validate_arguments_empty_file_path(self)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L121) — Test validation fails with empty file_path
  - `test_validate_arguments_invalid_analysis_type(self)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L137) — Test validation fails with invalid analysis_type
  - `test_validate_arguments_invalid_file_path_type(self)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L113) — Test validation fails with non-string file_path
  - `test_validate_arguments_invalid_include_ast_type(self)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L149) — Test validation fails with non-boolean include_ast
  - `test_validate_arguments_invalid_include_queries_type(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L157) — Test validation fails with non-boolean include_queries
  - `test_validate_arguments_invalid_language_type(self)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L129) — Test validation fails with non-string language
  - `test_validate_arguments_missing_file_path(self)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L105) — Test validation fails without file_path
  - `test_validate_arguments_valid_complete(self)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L92) — Test validation with all arguments
  - `test_validate_arguments_valid_minimal(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L86) — Test validation with minimal valid arguments
- uses (calls/refs, reference-scoped): [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`validate_arguments`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool.validate_arguments)

### `TestAvailableQueries`
- def: [`tests/unit/cli/test_universal_analyze_tool_comprehensive.py:551`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L551)
- doc: Test available queries functionality
- signature: `class TestAvailableQueries:`
- members:
  - `test_get_available_queries_error_handling(self)` — [`L570`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L570) — Test error handling when getting queries fails
  - `test_get_available_queries_python(self)` — [`L555`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L555) — Test getting available queries for Python
- uses (calls/refs, reference-scoped): [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`analysis_engine`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool.analysis_engine), [`_get_available_queries`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool._get_available_queries)

### `TestEdgeCases`
- def: [`tests/unit/cli/test_universal_analyze_tool_comprehensive.py:586`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L586)
- doc: Test edge cases and error handling
- signature: `class TestEdgeCases:`
- members:
  - `test_execute_with_analysis_failure(self, tmp_path)` — [`L656`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L656) — Test execution when analysis fails
  - `test_execute_with_empty_file(self, tmp_path)` — [`L623`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L623) — Test execution with empty file
  - `test_execute_with_special_characters_in_path(self, tmp_path)` — [`L590`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L590) — Test execution with special characters in file path
- uses (calls/refs, reference-scoped): [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool.execute), [`analysis_engine`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool.analysis_engine)

### `TestExecution`
- def: [`tests/unit/cli/test_universal_analyze_tool_comprehensive.py:170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L170)
- doc: Test tool execution
- signature: `class TestExecution:`
- members:
  - `test_execute_basic_analysis_python(self, mock_supported, mock_detect, tmp_path)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L250) — Test basic analysis execution for Python
  - `test_execute_detailed_analysis(self, mock_supported, mock_detect, tmp_path)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L294) — Test detailed analysis execution
  - `test_execute_file_not_found(self, tmp_path)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L183) — Test execution fails when file doesn't exist
  - `test_execute_invalid_analysis_type(self, tmp_path)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L228) — Test execution fails with invalid analysis_type
  - `test_execute_language_detection_failure(self, tmp_path)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L192) — Test execution fails when language detection fails
  - `test_execute_metrics_analysis(self, mock_supported, mock_detect, tmp_path)` — [`L453`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L453) — Test metrics analysis type
  - `test_execute_missing_file_path(self)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L174) — Test execution fails without file_path
  - `test_execute_structure_analysis(self, mock_supported, mock_detect, tmp_path)` — [`L413`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L413) — Test structure analysis type
  - `test_execute_unsupported_language(self, tmp_path)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L205) — O3 (round-30 dogfood): an explicit ``language`` override that
  - `test_execute_with_include_ast(self, mock_supported, mock_detect, tmp_path)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L334) — Test execution with include_ast option
  - `test_execute_with_include_queries(self, mock_supported, mock_detect, tmp_path)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L374) — Test execution with include_queries option
- uses (calls/refs, reference-scoped): [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`AnalysisError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#AnalysisError), [`execute`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool.execute), [`analysis_engine`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool.analysis_engine)

### `TestMetricsExtraction`
- def: [`tests/unit/cli/test_universal_analyze_tool_comprehensive.py:486`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L486)
- doc: Test metrics extraction methods
- signature: `class TestMetricsExtraction:`
- members:
  - `test_extract_universal_basic_metrics(self)` — [`L489`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L489) — Test basic metrics extraction from universal analyzer
  - `test_extract_universal_comprehensive_metrics(self)` — [`L534`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L534) — Test comprehensive metrics extraction
  - `test_extract_universal_detailed_metrics(self)` — [`L507`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L507) — Test detailed metrics extraction
  - `test_extract_universal_structure_info(self)` — [`L521`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L521) — Test structure info extraction
- uses (calls/refs, reference-scoped): [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`_extract_universal_comprehensive_metrics`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool._extract_universal_comprehensive_metrics), [`_extract_universal_basic_metrics`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool._extract_universal_basic_metrics), [`_extract_universal_detailed_metrics`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool._extract_universal_detailed_metrics), [`_extract_universal_structure_info`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool._extract_universal_structure_info)

### `TestToolDefinition`
- def: [`tests/unit/cli/test_universal_analyze_tool_comprehensive.py:41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L41)
- doc: Test tool definition and schema
- signature: `class TestToolDefinition:`
- members:
  - `test_analysis_type_enum(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L68) — Test analysis_type has correct enum values
  - `test_get_tool_definition_structure(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L44) — Test tool definition has correct structure
  - `test_tool_definition_schema(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L54) — Test input schema structure
- uses (calls/refs, reference-scoped): [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool.get_tool_definition)

### `TestUniversalAnalyzeToolInitialization`
- def: [`tests/unit/cli/test_universal_analyze_tool_comprehensive.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L17)
- doc: Test UniversalAnalyzeTool initialization
- signature: `class TestUniversalAnalyzeToolInitialization:`
- members:
  - `test_init_with_project_root(self, tmp_path)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L27) — Test initialization with project root
  - `test_init_without_project_root(self)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L20) — Test initialization without project root
  - `test_set_project_path(self, tmp_path)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_universal_analyze_tool_comprehensive.py#L33) — Test setting project path
- uses (calls/refs, reference-scoped): [`project_root`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.project_root), [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`path_resolver`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.path_resolver), [`set_project_path`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.set_project_path), [`security_validator`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.security_validator), [`analysis_engine`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool.analysis_engine)

