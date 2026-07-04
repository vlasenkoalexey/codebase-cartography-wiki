---
title: 'Module: tests/integration/formatters/_comprehensive_suite_reporting.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/_comprehensive_suite_reporting.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters._comprehensive_suite_reporting`/
symbols:
  _configuration_lines: _configuration_lines().
  _phase_results: _phase_results().
  _summary_header_lines: _summary_header_lines().
  _summary_report_lines: _summary_report_lines().
  update_test_counts: update_test_counts().
  _recommendation_lines: _recommendation_lines().
  generate_summary_report: generate_summary_report().
  _phase_result_lines: _phase_result_lines().
  save_comprehensive_results: save_comprehensive_results().
  _one_phase_result_lines: _one_phase_result_lines().
---
# Module: [`tests/integration/formatters/_comprehensive_suite_reporting.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_reporting.py)

## Functions
- `_configuration_lines(config: FormatTestSuiteConfig)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_reporting.py#L128)
- `_one_phase_result_lines(phase_name: str, phase_results: dict[str, Any])` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_reporting.py#L108)
- `_phase_result_lines(results: TestSuiteResults)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_reporting.py#L86)
- `_phase_results(results: TestSuiteResults)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_reporting.py#L94)
- `_recommendation_lines(results: TestSuiteResults)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_reporting.py#L149)
- `_summary_header_lines(results: TestSuiteResults)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_reporting.py#L69)
- `_summary_report_lines(config: FormatTestSuiteConfig, results: TestSuiteResults)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_reporting.py#L59)
- `generate_summary_report(results_dir: Path, config: FormatTestSuiteConfig, results: TestSuiteResults)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_reporting.py#L40) — Generate summary report.
- `save_comprehensive_results(results_dir: Path, results: TestSuiteResults)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_reporting.py#L24) — Save comprehensive test results.
- `update_test_counts(results: TestSuiteResults, phase_results: dict[str, Any])` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_reporting.py#L15) — Update test counts from phase results.

