---
title: 'Module: tests/integration/formatters/generate_regression_report.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/generate_regression_report.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters.generate_regression_report`/
symbols:
  RegressionReportGenerator.report_data: RegressionReportGenerator#report_data.
  main: main().
  RegressionReportGenerator._generate_html_content: RegressionReportGenerator#_generate_html_content().
  RegressionReportGenerator.generate_html_report: RegressionReportGenerator#generate_html_report().
  RegressionReportGenerator.generate_json_report: RegressionReportGenerator#generate_json_report().
  RegressionReportGenerator.add_test_failure: RegressionReportGenerator#add_test_failure().
  RegressionReportGenerator.add_format_change: RegressionReportGenerator#add_format_change().
  RegressionReportGenerator.add_recommendation: RegressionReportGenerator#add_recommendation().
  RegressionReportGenerator._generate_failures_section: RegressionReportGenerator#_generate_failures_section().
  RegressionReportGenerator._generate_changes_section: RegressionReportGenerator#_generate_changes_section().
  RegressionReportGenerator._generate_recommendations_section: RegressionReportGenerator#_generate_recommendations_section().
  RegressionReportGenerator.output_dir: RegressionReportGenerator#output_dir.
  RegressionReportGenerator: RegressionReportGenerator#
  RegressionReportGenerator._get_git_info: RegressionReportGenerator#_get_git_info().
  RegressionReportGenerator._get_environment_info: RegressionReportGenerator#_get_environment_info().
  RegressionReportGenerator.__init__: RegressionReportGenerator#__init__().
---
# Module: [`tests/integration/formatters/generate_regression_report.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/generate_regression_report.py)

## Classes
### `RegressionReportGenerator`
- def: [`tests/integration/formatters/generate_regression_report.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/generate_regression_report.py#L17)
- doc: Generates comprehensive format regression reports
- signature: `class RegressionReportGenerator:`
- members:
  - `__init__(self, output_dir: Path = None)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/generate_regression_report.py#L20) — Initialize regression report generator
  - `_generate_changes_section(self)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/generate_regression_report.py#L253) — Generate HTML for format changes section
  - `_generate_failures_section(self)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/generate_regression_report.py#L232) — Generate HTML for test failures section
  - `_generate_html_content(self)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/generate_regression_report.py#L153) — Generate HTML content for the report
  - `_generate_recommendations_section(self)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/generate_regression_report.py#L272) — Generate HTML for recommendations section
  - `_get_environment_info(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/generate_regression_report.py#L57) — Get environment information
  - `_get_git_info(self)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/generate_regression_report.py#L37) — Get current git information
  - `add_format_change(self, format_type: str, change_description: str, impact_level: str, affected_components: list[str])` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/generate_regression_report.py#L96) — Add a format change to the report
  - `add_recommendation(self, recommendation: str, priority: str = "medium")` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/generate_regression_report.py#L122) — Add a recommendation to the report
  - `add_test_failure(self, test_name: str, failure_type: str, expected: str, actual: str, diff: str | None = None)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/generate_regression_report.py#L67) — Add a test failure to the report
  - `generate_html_report(self)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/generate_regression_report.py#L138) — Generate HTML regression report
  - `generate_json_report(self)` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/generate_regression_report.py#L289) — Generate JSON regression report
  - `output_dir` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/generate_regression_report.py#L27)
  - `report_data` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/generate_regression_report.py#L28)
- used by: (1 test-only callers)

## Functions
- `main()` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/generate_regression_report.py#L304) — Main function to generate regression report

