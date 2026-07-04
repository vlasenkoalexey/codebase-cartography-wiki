---
title: 'Module: tests/integration/formatters/end_to_end_tests.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/end_to_end_tests.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters.end_to_end_tests`/Test
symbols:
  TestEndToEndFormatValidation.test_complete_pipeline_java_file: EndToEndFormatValidation#test_complete_pipeline_java_file().
  TestEndToEndFormatValidation.test_complete_pipeline_python_file: EndToEndFormatValidation#test_complete_pipeline_python_file().
  TestEndToEndFormatValidation.test_format_validation_with_edge_cases: EndToEndFormatValidation#test_format_validation_with_edge_cases().
  TestEndToEndFormatValidation.test_format_consistency_across_languages: EndToEndFormatValidation#test_format_consistency_across_languages().
  TestEndToEndFormatValidation.test_api_interface_format_validation: EndToEndFormatValidation#test_api_interface_format_validation().
  TestEndToEndFormatValidation.test_format_regression_detection: EndToEndFormatValidation#test_format_regression_detection().
  TestFormatStabilityValidation.test_format_output_deterministic: FormatStabilityValidation#test_format_output_deterministic().
  TestFormatStabilityValidation.test_format_metadata_consistency: FormatStabilityValidation#test_format_metadata_consistency().
  TestEndToEndFormatValidation.golden_master_manager: EndToEndFormatValidation#golden_master_manager().
  TestEndToEndFormatValidation: EndToEndFormatValidation#
  TestEndToEndFormatValidation.comprehensive_test_files: EndToEndFormatValidation#comprehensive_test_files().
  TestEndToEndFormatValidation.test_cli_interface_format_validation: EndToEndFormatValidation#test_cli_interface_format_validation().
  TestFormatStabilityValidation: FormatStabilityValidation#
---
# Module: [`tests/integration/formatters/end_to_end_tests.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/end_to_end_tests.py)

## Classes
### `TestEndToEndFormatValidation`
- def: [`tests/integration/formatters/end_to_end_tests.py:28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/end_to_end_tests.py#L28)
- doc: End-to-end format validation through complete pipeline
- signature: `class TestEndToEndFormatValidation:`
- members:
  - `comprehensive_test_files(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/end_to_end_tests.py#L32) — Create comprehensive test files for different languages
  - `golden_master_manager(self)` — [`L309`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/end_to_end_tests.py#L309) — Provide golden master manager
  - `test_api_interface_format_validation(self, comprehensive_test_files)` — [`L426`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/end_to_end_tests.py#L426) — Test format validation through API interface
  - `test_cli_interface_format_validation(self, comprehensive_test_files)` — [`L452`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/end_to_end_tests.py#L452) — Test format validation through CLI interface
  - `test_complete_pipeline_java_file(self, comprehensive_test_files, golden_master_manager)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/end_to_end_tests.py#L314) — Test complete pipeline: Java file → analysis → formatting → validation
  - `test_complete_pipeline_python_file(self, comprehensive_test_files, golden_master_manager)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/end_to_end_tests.py#L374) — Test complete pipeline: Python file → analysis → formatting → validation
  - `test_format_consistency_across_languages(self, comprehensive_test_files)` — [`L605`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/end_to_end_tests.py#L605) — Test format consistency across different programming languages
  - `test_format_regression_detection(self, comprehensive_test_files, golden_master_manager)` — [`L506`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/end_to_end_tests.py#L506) — Test that format changes are detected by regression tests
  - `test_format_validation_with_edge_cases(self, comprehensive_test_files)` — [`L537`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/end_to_end_tests.py#L537) — Test format validation with edge cases and boundary conditions
- uses (calls/refs, reference-scoped): [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute)  (9 test-only)

### `TestFormatStabilityValidation`
- def: [`tests/integration/formatters/end_to_end_tests.py:638`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/end_to_end_tests.py#L638)
- doc: Test format stability and consistency over time
- signature: `class TestFormatStabilityValidation:`
- members:
  - `test_format_metadata_consistency(self, comprehensive_test_files)` — [`L662`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/end_to_end_tests.py#L662) — Test that format metadata is consistent and accurate
  - `test_format_output_deterministic(self, comprehensive_test_files)` — [`L642`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/end_to_end_tests.py#L642) — Test that format output is deterministic (same input → same output)
- uses (calls/refs, reference-scoped): [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute)

