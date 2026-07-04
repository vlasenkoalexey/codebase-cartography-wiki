---
title: 'Module: tests/unit/test_project_health_coverage_fields.py'
type: catalog
provenance: extracted
module: tests/unit/test_project_health_coverage_fields.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_project_health_coverage_fields`/
symbols:
  test_project_health_emits_coverage_fields: test_project_health_emits_coverage_fields().
  test_excluded_dirs_show_up_in_skip_reasons: test_excluded_dirs_show_up_in_skip_reasons().
  test_coverage_pct_is_consistent: test_coverage_pct_is_consistent().
  test_total_files_analyzed_matches_total_files_legacy: test_total_files_analyzed_matches_total_files_legacy().
  _make_project: _make_project().
---
# Module: [`tests/unit/test_project_health_coverage_fields.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_health_coverage_fields.py)

## Functions
- `_make_project(tmp_path: Path)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_health_coverage_fields.py#L30)
- `test_coverage_pct_is_consistent(tmp_path: Path)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_health_coverage_fields.py#L76) — coverage_pct must equal analyzed / scanned * 100, rounded to 0.1.
- `test_excluded_dirs_show_up_in_skip_reasons(tmp_path: Path)` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_health_coverage_fields.py#L60) — ``__pycache__/ignored.py`` must be counted as excluded_dir skip.
- `test_project_health_emits_coverage_fields(tmp_path: Path)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_health_coverage_fields.py#L40) — All five coverage-transparency fields must appear in the response.
- `test_total_files_analyzed_matches_total_files_legacy(tmp_path: Path)` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_health_coverage_fields.py#L91) — ``total_files_analyzed`` is the modern alias of the legacy ``total_files``.

