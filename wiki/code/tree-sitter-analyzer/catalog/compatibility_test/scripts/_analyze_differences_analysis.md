---
title: 'Module: compatibility_test/scripts/_analyze_differences_analysis.py'
type: catalog
provenance: extracted
module: compatibility_test/scripts/_analyze_differences_analysis.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `compatibility_test.scripts._analyze_differences_analysis`/
symbols:
  analyze_common_files: analyze_common_files().
  update_summary: update_summary().
  FileAnalyzer: FileAnalyzer.
  _analyze_one_file: _analyze_one_file().
  generate_normalized_outputs: generate_normalized_outputs().
  validate_version_dirs: validate_version_dirs().
  build_initial_results: build_initial_results().
  _is_identical_analysis: _is_identical_analysis().
  _update_change_severity_counts: _update_change_severity_counts().
  _update_performance_change_count: _update_performance_change_count().
---
# Module: [`compatibility_test/scripts/_analyze_differences_analysis.py`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_analysis.py)

## Functions
- `_analyze_one_file(analyzer: Any, filename: str, analyze_json: FileAnalyzer, analyze_text: FileAnalyzer)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_analysis.py#L99)
- `_is_identical_analysis(analysis: dict[str, Any])` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_analysis.py#L112)
- `_update_change_severity_counts(summary: dict[str, int], analysis: dict[str, Any])` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_analysis.py#L118)
- `_update_performance_change_count(summary: dict[str, int], analysis: dict[str, Any])` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_analysis.py#L127)
- `analyze_common_files(analyzer: Any, common_files: set[str], analyze_json: FileAnalyzer, analyze_text: FileAnalyzer)` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_analysis.py#L70) — Analyze every common output file and update summary counts.
- `build_initial_results(analyzer: Any, common_files: set[str])` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_analysis.py#L46) — Build the analysis result envelope.
- `generate_normalized_outputs(analyzer: Any)` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_analysis.py#L11) — Generate normalized files when requested.
- `update_summary(summary: dict[str, int], analysis: dict[str, Any])` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_analysis.py#L88) — Update aggregate counters for one file analysis.
- `validate_version_dirs(analyzer: Any)` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_analysis.py#L27) — Validate that both version result directories exist.

## Module values
- `FileAnalyzer` — [`L8`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_analysis.py#L8)

