---
title: 'Module: compatibility_test/scripts/_analyze_differences_report.py'
type: catalog
provenance: extracted
module: compatibility_test/scripts/_analyze_differences_report.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `compatibility_test.scripts._analyze_differences_report`/
symbols:
  build_analysis_report_lines: build_analysis_report_lines().
  _single_analysis_lines: _single_analysis_lines().
  _severity_section_lines: _severity_section_lines().
  _missing_file_lines: _missing_file_lines().
  _file_analysis_lines: _file_analysis_lines().
  _json_comparison_lines: _json_comparison_lines().
  build_report_path: build_report_path().
  write_report: write_report().
  _one_missing_side_lines: _one_missing_side_lines().
  _summary_lines: _summary_lines().
  _smart_json_analysis_lines: _smart_json_analysis_lines().
  _generic_diff_lines: _generic_diff_lines().
  _performance_diff_line: _performance_diff_line().
  _text_difference_lines: _text_difference_lines().
---
# Module: [`compatibility_test/scripts/_analyze_differences_report.py`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_report.py)

## Functions
- `_file_analysis_lines(analysis_results: dict[str, Any])` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_report.py#L105)
- `_generic_diff_lines(diff: dict[str, Any], include_values: bool)` — [`L192`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_report.py#L192)
- `_json_comparison_lines(analysis: dict[str, Any])` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_report.py#L158)
- `_missing_file_lines(analysis_results: dict[str, Any], version_a: str, version_b: str)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_report.py#L83)
- `_one_missing_side_lines(missing_files: list[str] | None, version: str)` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_report.py#L96)
- `_performance_diff_line(diff: dict[str, Any])` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_report.py#L200)
- `_severity_section_lines(differences: list[dict[str, Any]], severity: str, title: str)` — [`L175`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_report.py#L175)
- `_single_analysis_lines(analysis: dict[str, Any])` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_report.py#L114)
- `_smart_json_analysis_lines(analysis: dict[str, Any])` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_report.py#L127)
- `_summary_lines(report_title: str, analysis_results: dict[str, Any], version_a: str, version_b: str)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_report.py#L56)
- `_text_difference_lines(analysis: dict[str, Any])` — [`L206`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_report.py#L206)
- `build_analysis_report_lines(analysis_results: dict[str, Any], version_a: str, version_b: str, smart_compare: bool)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_report.py#L29) — Render the Markdown report lines.
- `build_report_path(project_root: Path, version_a: str, version_b: str, smart_compare: bool)` — [`L8`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_report.py#L8) — Build the timestamped report path.
- `write_report(report_file: Path, report_lines: list[str])` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_report.py#L47) — Write the report and return its string path.

