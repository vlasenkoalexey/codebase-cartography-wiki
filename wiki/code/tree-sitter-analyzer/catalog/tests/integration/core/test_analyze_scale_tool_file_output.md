---
title: 'Module: tests/integration/core/test_analyze_scale_tool_file_output.py'
type: catalog
provenance: extracted
module: tests/integration/core/test_analyze_scale_tool_file_output.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.core.test_analyze_scale_tool_file_output`/TestAnalyzeScaleToolFileOutput#
symbols:
  TestAnalyzeScaleToolFileOutput.create_mock_analysis_result: create_mock_analysis_result().
  TestAnalyzeScaleToolFileOutput._named_annotation: _named_annotation().
  TestAnalyzeScaleToolFileOutput.analyze_scale_tool: analyze_scale_tool().
  TestAnalyzeScaleToolFileOutput.test_basic_analyze_scale_functionality: test_basic_analyze_scale_functionality().
  TestAnalyzeScaleToolFileOutput.test_include_details_functionality: test_include_details_functionality().
  TestAnalyzeScaleToolFileOutput.test_language_auto_detection: test_language_auto_detection().
  TestAnalyzeScaleToolFileOutput.test_complexity_hotspots_detection: test_complexity_hotspots_detection().
  TestAnalyzeScaleToolFileOutput.test_llm_guidance_generation: test_llm_guidance_generation().
  TestAnalyzeScaleToolFileOutput.test_disable_guidance: test_disable_guidance().
  TestAnalyzeScaleToolFileOutput.test_file_metrics_calculation: test_file_metrics_calculation().
  TestAnalyzeScaleToolFileOutput.test_comprehensive_analysis_workflow: test_comprehensive_analysis_workflow().
  TestAnalyzeScaleToolFileOutput: ''
  TestAnalyzeScaleToolFileOutput.temp_project_dir: temp_project_dir().
  TestAnalyzeScaleToolFileOutput.test_python_file_analysis: test_python_file_analysis().
  TestAnalyzeScaleToolFileOutput.test_error_handling_analysis_failure: test_error_handling_analysis_failure().
  TestAnalyzeScaleToolFileOutput.test_invalid_file_path: test_invalid_file_path().
  TestAnalyzeScaleToolFileOutput.test_unsupported_language: test_unsupported_language().
  TestAnalyzeScaleToolFileOutput.test_tool_definition_structure: test_tool_definition_structure().
  TestAnalyzeScaleToolFileOutput.test_argument_validation: test_argument_validation().
  TestAnalyzeScaleToolFileOutput.test_future_file_output_compatibility: test_future_file_output_compatibility().
---
# Module: [`tests/integration/core/test_analyze_scale_tool_file_output.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py)

## Classes
### `TestAnalyzeScaleToolFileOutput`
- def: [`tests/integration/core/test_analyze_scale_tool_file_output.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L20)
- doc: Test analyze_scale_tool functionality and prepare for file output features
- signature: `class TestAnalyzeScaleToolFileOutput:`
- members:
  - `_named_annotation(name)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L256) — Annotation mock with a real .name string.
  - `analyze_scale_tool(self, temp_project_dir)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L251) — Create AnalyzeScaleTool instance
  - `create_mock_analysis_result(self, file_type="java")` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L266) — Create mock analysis result
  - `temp_project_dir(self)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L24) — Create a temporary project directory with test files
  - `test_argument_validation(self, analyze_scale_tool)` — [`L637`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L637) — Test argument validation
  - `test_basic_analyze_scale_functionality(self, analyze_scale_tool, temp_project_dir)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L356) — Test basic analyze_scale functionality
  - `test_complexity_hotspots_detection(self, analyze_scale_tool, temp_project_dir)` — [`L494`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L494) — Test complexity hotspots detection
  - `test_comprehensive_analysis_workflow(self, analyze_scale_tool, temp_project_dir)` — [`L720`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L720) — Test comprehensive analysis workflow
  - `test_disable_guidance(self, analyze_scale_tool, temp_project_dir)` — [`L563`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L563) — Test disabling LLM guidance
  - `test_error_handling_analysis_failure(self, analyze_scale_tool, temp_project_dir)` — [`L580`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L580) — Test error handling when analysis fails
  - `test_file_metrics_calculation(self, analyze_scale_tool, temp_project_dir)` — [`L665`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L665) — Test file metrics calculation
  - `test_future_file_output_compatibility(self, analyze_scale_tool)` — [`L697`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L697) — Test that the tool structure is compatible with future file output features
  - `test_include_details_functionality(self, analyze_scale_tool, temp_project_dir)` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L418) — Test include_details functionality
  - `test_invalid_file_path(self, analyze_scale_tool, temp_project_dir)` — [`L595`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L595) — Test handling of invalid file path
  - `test_language_auto_detection(self, analyze_scale_tool, temp_project_dir)` — [`L473`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L473) — Test automatic language detection
  - `test_llm_guidance_generation(self, analyze_scale_tool, temp_project_dir)` — [`L532`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L532) — Test LLM guidance generation for different file sizes
  - `test_python_file_analysis(self, analyze_scale_tool, temp_project_dir)` — [`L446`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L446) — Test analysis of Python file
  - `test_tool_definition_structure(self, analyze_scale_tool)` — [`L612`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L612) — Test that tool definition has correct structure
  - `test_unsupported_language(self, analyze_scale_tool, temp_project_dir)` — [`L603`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_analyze_scale_tool_file_output.py#L603) — Test handling of unsupported language
- uses (calls/refs, reference-scoped): [`AnalyzeScaleTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool)

