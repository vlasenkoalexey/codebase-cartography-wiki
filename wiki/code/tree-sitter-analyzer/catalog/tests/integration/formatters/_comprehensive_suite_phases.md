---
title: 'Module: tests/integration/formatters/_comprehensive_suite_phases.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/_comprehensive_suite_phases.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters._comprehensive_suite_phases`/
symbols:
  run_one_schema_validation_test: run_one_schema_validation_test().
  run_one_end_to_end_test: run_one_end_to_end_test().
  run_one_specification_compliance_test: run_one_specification_compliance_test().
  run_one_enhanced_assertion_test: run_one_enhanced_assertion_test().
  run_one_golden_master_test: run_one_golden_master_test().
  run_one_integration_test: run_one_integration_test().
  run_one_cross_component_test: run_one_cross_component_test().
  run_one_performance_test: run_one_performance_test().
  run_one_format_contract_test: run_one_format_contract_test().
  _format_phase_case: _format_phase_case().
  _language_phase_case: _language_phase_case().
  ComprehensiveSuitePhasesMixin._run_end_to_end_tests: ComprehensiveSuitePhasesMixin#_run_end_to_end_tests().
  ComprehensiveSuitePhasesMixin._run_specification_compliance_tests: ComprehensiveSuitePhasesMixin#_run_specification_compliance_tests().
  ComprehensiveSuitePhasesMixin._run_golden_master_tests: ComprehensiveSuitePhasesMixin#_run_golden_master_tests().
  ComprehensiveSuitePhasesMixin._run_schema_validation_tests: ComprehensiveSuitePhasesMixin#_run_schema_validation_tests().
  ComprehensiveSuitePhasesMixin._run_integration_tests: ComprehensiveSuitePhasesMixin#_run_integration_tests().
  ComprehensiveSuitePhasesMixin._run_cross_component_tests: ComprehensiveSuitePhasesMixin#_run_cross_component_tests().
  ComprehensiveSuitePhasesMixin._run_format_contract_tests: ComprehensiveSuitePhasesMixin#_run_format_contract_tests().
  ComprehensiveSuitePhasesMixin._run_enhanced_assertion_tests: ComprehensiveSuitePhasesMixin#_run_enhanced_assertion_tests().
  ComprehensiveSuitePhasesMixin._run_performance_tests: ComprehensiveSuitePhasesMixin#_run_performance_tests().
  ComprehensiveSuitePhasesMixin: ComprehensiveSuitePhasesMixin#
  _performance_is_acceptable: _performance_is_acceptable().
---
# Module: [`tests/integration/formatters/_comprehensive_suite_phases.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py)

## Classes
### `ComprehensiveSuitePhasesMixin`
- def: [`tests/integration/formatters/_comprehensive_suite_phases.py:23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L23)
- doc: Runs each validation phase behind the suite interface.
- signature: `class ComprehensiveSuitePhasesMixin:`
- members:
  - `_run_cross_component_tests(self, analyzer_function: callable, test_data_sources: list[dict[str, Any]])` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L97) — Run cross-component tests
  - `_run_end_to_end_tests(self, analyzer_function: callable, test_data_sources: list[dict[str, Any]])` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L78) — Run end-to-end tests
  - `_run_enhanced_assertion_tests(self, analyzer_function: callable, test_data_sources: list[dict[str, Any]])` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L156) — Run enhanced assertion tests
  - `_run_format_contract_tests(self, analyzer_function: callable, test_data_sources: list[dict[str, Any]])` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L138) — Run format contract tests
  - `_run_golden_master_tests(self, analyzer_function: callable, test_data_sources: list[dict[str, Any]])` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L26) — Run golden master tests
  - `_run_integration_tests(self, analyzer_function: callable, test_data_sources: list[dict[str, Any]])` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L60) — Run integration tests
  - `_run_performance_tests(self, analyzer_function: callable, test_data_sources: list[dict[str, Any]])` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L175) — Run performance tests
  - `_run_schema_validation_tests(self, analyzer_function: callable, test_data_sources: list[dict[str, Any]])` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L41) — Run schema validation tests
  - `_run_specification_compliance_tests(self, analyzer_function: callable, test_data_sources: list[dict[str, Any]])` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L115) — Run specification compliance tests
- uses (calls/refs, reference-scoped): (15 test-only callers)
- used by: (1 test-only callers)

## Functions
- `_format_phase_case(analyzer_function: callable, test_data: dict[str, Any], format_type: str, prefix: str, results: dict[str, Any])` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L190)
- `_language_phase_case(analyzer_function: callable, test_data: dict[str, Any], prefix: str, results: dict[str, Any])` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L207)
- `_performance_is_acceptable(performance_results: dict[str, Any])` — [`L413`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L413)
- `run_one_cross_component_test(case: PhaseCase)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L305)
- `run_one_end_to_end_test(case: PhaseCase)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L290)
- `run_one_enhanced_assertion_test(suite: Any, case: PhaseCase)` — [`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L368)
- `run_one_format_contract_test(case: PhaseCase)` — [`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L346)
- `run_one_golden_master_test(suite: Any, case: PhaseCase)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L222)
- `run_one_integration_test(case: PhaseCase)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L269)
- `run_one_performance_test(suite: Any, case: PhaseCase)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L390)
- `run_one_schema_validation_test(suite: Any, case: PhaseCase)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L251)
- `run_one_specification_compliance_test(case: PhaseCase)` — [`L325`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phases.py#L325)

