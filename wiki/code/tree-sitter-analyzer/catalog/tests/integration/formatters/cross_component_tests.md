---
title: 'Module: tests/integration/formatters/cross_component_tests.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/cross_component_tests.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters.cross_component_tests`/
symbols:
  CrossComponentFormatValidator.validate_cross_component_consistency: CrossComponentFormatValidator#validate_cross_component_consistency().
  CrossComponentFormatValidator._analyze_consistency: CrossComponentFormatValidator#_analyze_consistency().
  CrossComponentFormatValidator.collect_direct_result: CrossComponentFormatValidator#collect_direct_result().
  CrossComponentFormatValidator.collect_mcp_result: CrossComponentFormatValidator#collect_mcp_result().
  TestCrossComponentFormatValidation.test_cli_integration_when_available: TestCrossComponentFormatValidation#test_cli_integration_when_available().
  TestCrossComponentFormatValidation.test_direct_library_consistency: TestCrossComponentFormatValidation#test_direct_library_consistency().
  TestFormatContractValidation.test_format_contract_compliance: TestFormatContractValidation#test_format_contract_compliance().
  CrossComponentFormatValidator.collect_cli_result: CrossComponentFormatValidator#collect_cli_result().
  TestCrossComponentFormatValidation.validator: TestCrossComponentFormatValidation#validator().
  CrossComponentFormatValidator: CrossComponentFormatValidator#
  CrossComponentFormatValidator.project_root: CrossComponentFormatValidator#project_root.
  CrossComponentFormatValidator.collect_api_result: CrossComponentFormatValidator#collect_api_result().
  CrossComponentFormatValidator._check_metadata_consistency: CrossComponentFormatValidator#_check_metadata_consistency().
  CrossComponentFormatValidator._find_output_differences: CrossComponentFormatValidator#_find_output_differences().
  pytestmark: pytestmark.
  CrossComponentFormatValidator.__init__: CrossComponentFormatValidator#__init__().
  CrossComponentFormatValidator.results: CrossComponentFormatValidator#results.
  TestCrossComponentFormatValidation: TestCrossComponentFormatValidation#
  TestCrossComponentFormatValidation.test_file: TestCrossComponentFormatValidation#test_file().
  TestCrossComponentFormatValidation.test_mcp_api_consistency: TestCrossComponentFormatValidation#test_mcp_api_consistency().
  TestCrossComponentFormatValidation.test_all_interfaces_consistency: TestCrossComponentFormatValidation#test_all_interfaces_consistency().
  TestCrossComponentFormatValidation.test_metadata_consistency: TestCrossComponentFormatValidation#test_metadata_consistency().
  TestCrossComponentFormatValidation.test_format_regression_across_interfaces: TestCrossComponentFormatValidation#test_format_regression_across_interfaces().
  TestFormatContractValidation: TestFormatContractValidation#
  TestFormatContractValidation.test_error_handling_consistency: TestFormatContractValidation#test_error_handling_consistency().
---
# Module: [`tests/integration/formatters/cross_component_tests.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py)

## Classes
### `CrossComponentFormatValidator`
- def: [`tests/integration/formatters/cross_component_tests.py:42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L42)
- doc: Validator for cross-component format consistency
- signature: `class CrossComponentFormatValidator:`
- members:
  - `_analyze_consistency(self, results: dict[str, dict[str, Any]])` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L206) — Analyze consistency across interface results
  - `_check_metadata_consistency(self, results: dict[str, dict[str, Any]])` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L277) — Check consistency of metadata across interfaces
  - `_find_output_differences(self, outputs: dict[str, str])` — [`L306`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L306) — Find specific differences between outputs
  - `collect_api_result(self, file_path: str, format_type: str, language: str | None = None)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L69) — Collect result from API interface
  - `collect_cli_result(self, file_path: str, format_type: str, language: str | None = None)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L92) — Collect result from CLI interface
  - `collect_direct_result(self, file_path: str, format_type: str, language: str | None = None)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L132) — Collect result from direct library usage
  - `collect_mcp_result(self, file_path: str, format_type: str, language: str | None = None)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L49) — Collect result from MCP interface
  - `validate_cross_component_consistency(self, file_path: str, format_type: str, language: str | None = None)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L164) — Validate consistency across all interfaces
  - `project_root` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L46)
  - `results` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L47)
- protocol/private: `__init__`[`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L45)
- uses (calls/refs, reference-scoped): [`UnifiedAnalysisEngine`](../../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine), [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`FormatterRegistry`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute), [`get_formatter_for_language`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry.get_formatter_for_language), [`analyze_file`](../../../tree_sitter_analyzer/core/_analysis_engine_file_mixin.md#UnifiedAnalysisEngineFileMixin.analyze_file)  (3 test-only)
- used by: (2 test-only callers)

### `TestCrossComponentFormatValidation`
- def: [`tests/integration/formatters/cross_component_tests.py:349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L349)
- doc: Test cross-component format validation
- signature: `class TestCrossComponentFormatValidation:`
- members:
  - `test_all_interfaces_consistency(self, test_file, validator)` — [`L458`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L458) — Test consistency across all available interfaces
  - `test_cli_integration_when_available(self, test_file, validator)` — [`L513`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L513) — Test CLI integration when CLI is available
  - `test_direct_library_consistency(self, test_file, validator)` — [`L554`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L554) — Test direct library usage consistency
  - `test_file(self)` — [`L353`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L353) — Create a test file for cross-component testing
  - `test_format_regression_across_interfaces(self, test_file, validator)` — [`L591`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L591) — Test that format regressions are detected across all interfaces
  - `test_mcp_api_consistency(self, test_file, validator)` — [`L425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L425) — Test consistency between MCP and API interfaces
  - `test_metadata_consistency(self, test_file, validator)` — [`L489`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L489) — Test metadata consistency across interfaces
  - `validator(self, test_file)` — [`L419`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L419) — Create cross-component validator
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `TestFormatContractValidation`
- def: [`tests/integration/formatters/cross_component_tests.py:623`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L623)
- doc: Test format contracts across components
- signature: `class TestFormatContractValidation:`
- members:
  - `test_error_handling_consistency(self, validator)` — [`L681`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L681) — Test that error handling is consistent across interfaces
  - `test_format_contract_compliance(self, test_file)` — [`L627`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L627) — Test that all interfaces comply with format contracts
- uses (calls/refs, reference-scoped): (2 test-only callers)

## Module values
- `pytestmark` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/cross_component_tests.py#L33)

