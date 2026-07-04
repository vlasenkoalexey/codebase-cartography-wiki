---
title: 'Module: tests/integration/mcp/test_tools/test_analyze_scale_tool.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_tools/test_analyze_scale_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_tools.test_analyze_scale_tool`/TestAnalyzeScaleTool
symbols:
  TestAnalyzeScaleToolEnhanced.tool: Enhanced#tool.
  TestAnalyzeScaleToolEnhanced.test_execute_with_java_file: Enhanced#test_execute_with_java_file().
  TestAnalyzeScaleToolEnhanced.test_execute_without_guidance: Enhanced#test_execute_without_guidance().
  TestAnalyzeScaleToolEnhanced.test_execute_with_details: Enhanced#test_execute_with_details().
  TestAnalyzeScaleToolEnhanced.test_tool_schema_structure: Enhanced#test_tool_schema_structure().
  TestAnalyzeScaleToolEnhanced.test_validate_arguments_valid: Enhanced#test_validate_arguments_valid().
  TestAnalyzeScaleToolEnhanced.test_validate_arguments_missing_required: Enhanced#test_validate_arguments_missing_required().
  TestAnalyzeScaleToolEnhanced.test_validate_arguments_invalid_types: Enhanced#test_validate_arguments_invalid_types().
  TestAnalyzeScaleToolEnhanced.test_execute_with_nonexistent_file: Enhanced#test_execute_with_nonexistent_file().
  TestAnalyzeScaleToolEnhanced.test_execute_with_missing_file_path: Enhanced#test_execute_with_missing_file_path().
  TestAnalyzeScaleToolEnhanced.test_file_metrics_calculation: Enhanced#test_file_metrics_calculation().
  TestAnalyzeScaleToolEnhanced.test_llm_guidance_generation: Enhanced#test_llm_guidance_generation().
  TestAnalyzeScaleToolEnhanced.test_tool_definition: Enhanced#test_tool_definition().
  TestAnalyzeScaleToolIntegration.test_integration_with_advanced_analyzer: Integration#test_integration_with_advanced_analyzer().
  TestAnalyzeScaleToolIntegration.test_language_detection_integration: Integration#test_language_detection_integration().
  TestAnalyzeScaleToolPerformance.test_performance_monitoring_integration: Performance#test_performance_monitoring_integration().
  TestAnalyzeScaleToolErrorHandling.test_invalid_file_path: ErrorHandling#test_invalid_file_path().
  TestAnalyzeScaleToolErrorHandling.test_unsupported_language: ErrorHandling#test_unsupported_language().
  TestAnalyzeScaleToolErrorHandling.test_file_metrics_error_handling: ErrorHandling#test_file_metrics_error_handling().
  TestAnalyzeScaleToolEnhanced.sample_java_code: Enhanced#sample_java_code.
  TestAnalyzeScaleToolErrorHandling.tool: ErrorHandling#tool.
  TestAnalyzeScaleToolIntegration.setup_method: Integration#setup_method().
  TestAnalyzeScaleToolPerformance.setup_method: Performance#setup_method().
  TestAnalyzeScaleToolErrorHandling.setup_method: ErrorHandling#setup_method().
  TestAnalyzeScaleToolIntegration.tool: Integration#tool.
  TestAnalyzeScaleToolPerformance.tool: Performance#tool.
  TestAnalyzeScaleToolEnhanced: Enhanced#
  TestAnalyzeScaleToolEnhanced.setup_method: Enhanced#setup_method().
  TestAnalyzeScaleToolIntegration: Integration#
  TestAnalyzeScaleToolPerformance: Performance#
  TestAnalyzeScaleToolErrorHandling: ErrorHandling#
---
# Module: [`tests/integration/mcp/test_tools/test_analyze_scale_tool.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py)

## Classes
### `TestAnalyzeScaleToolEnhanced`
- def: [`tests/integration/mcp/test_tools/test_analyze_scale_tool.py:18`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L18)
- doc: Test enhanced analyze_code_scale tool functionality
- signature: `class TestAnalyzeScaleToolEnhanced:`
- members:
  - `setup_method(self)` — [`L21`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L21) — Set up test fixtures
  - `test_execute_with_details(self)` — [`L235`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L235) — Test executing analysis with detailed information
  - `test_execute_with_java_file(self)` — [`L128`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L128) — Test executing enhanced analysis on a real Java file
  - `test_execute_with_missing_file_path(self)` — [`L271`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L271) — Test error handling for missing file_path argument
  - `test_execute_with_nonexistent_file(self)` — [`L265`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L265) — Test error handling for nonexistent file
  - `test_execute_without_guidance(self)` — [`L206`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L206) — Test executing analysis without LLM guidance
  - `test_file_metrics_calculation(self)` — [`L278`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L278) — Test file metrics calculation functionality
  - `test_llm_guidance_generation(self)` — [`L317`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L317) — Test LLM guidance generation
  - `test_tool_definition(self)` — [`L356`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L356) — Test tool definition structure
  - `test_tool_schema_structure(self)` — [`L74`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L74) — Test that enhanced tool schema has required structure
  - `test_validate_arguments_invalid_types(self)` — [`L116`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L116) — Test argument validation with invalid types
  - `test_validate_arguments_missing_required(self)` — [`L107`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L107) — Test argument validation with missing required field
  - `test_validate_arguments_valid(self)` — [`L93`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L93) — Test argument validation with valid arguments
  - `sample_java_code` — [`L24`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L24)
  - `tool` — [`L23`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L23)
- uses (calls/refs, reference-scoped): [`AnalyzeScaleTool`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool.execute), [`_calculate_file_metrics`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool._calculate_file_metrics), [`get_tool_definition`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool.get_tool_definition), [`get_tool_schema`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool.get_tool_schema), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool.validate_arguments), [`_generate_llm_guidance`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool._generate_llm_guidance)

### `TestAnalyzeScaleToolErrorHandling`
- def: [`tests/integration/mcp/test_tools/test_analyze_scale_tool.py:480`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L480)
- doc: Test error handling in enhanced analyze_code_scale tool
- signature: `class TestAnalyzeScaleToolErrorHandling:`
- members:
  - `setup_method(self)` — [`L483`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L483) — Set up test fixtures
  - `test_file_metrics_error_handling(self)` — [`L512`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L512) — Test error handling in file metrics calculation
  - `test_invalid_file_path(self)` — [`L488`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L488) — Test handling of invalid file paths
  - `test_unsupported_language(self)` — [`L494`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L494) — Test handling of unsupported language
  - `tool` — [`L485`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L485)
- uses (calls/refs, reference-scoped): [`AnalyzeScaleTool`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool.execute), [`_calculate_file_metrics`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool._calculate_file_metrics)

### `TestAnalyzeScaleToolIntegration`
- def: [`tests/integration/mcp/test_tools/test_analyze_scale_tool.py:373`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L373)
- doc: Test integration with existing analyzer components
- signature: `class TestAnalyzeScaleToolIntegration:`
- members:
  - `setup_method(self)` — [`L376`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L376) — Set up test fixtures
  - `test_integration_with_advanced_analyzer(self)` — [`L381`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L381) — Test integration with AdvancedAnalyzer
  - `test_language_detection_integration(self)` — [`L417`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L417) — Test integration with language detection
  - `tool` — [`L378`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L378)
- uses (calls/refs, reference-scoped): [`AnalyzeScaleTool`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool.execute)

### `TestAnalyzeScaleToolPerformance`
- def: [`tests/integration/mcp/test_tools/test_analyze_scale_tool.py:445`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L445)
- doc: Test performance characteristics of enhanced analyze_code_scale tool
- signature: `class TestAnalyzeScaleToolPerformance:`
- members:
  - `setup_method(self)` — [`L448`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L448) — Set up test fixtures
  - `test_performance_monitoring_integration(self)` — [`L453`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L453) — Test that performance monitoring is properly integrated
  - `tool` — [`L450`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_analyze_scale_tool.py#L450)
- uses (calls/refs, reference-scoped): [`AnalyzeScaleTool`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool.execute)

