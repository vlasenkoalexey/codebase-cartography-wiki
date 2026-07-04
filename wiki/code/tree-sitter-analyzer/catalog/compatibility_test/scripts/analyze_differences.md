---
title: 'Module: compatibility_test/scripts/analyze_differences.py'
type: catalog
provenance: extracted
module: compatibility_test/scripts/analyze_differences.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `compatibility_test.scripts.analyze_differences`/
symbols:
  DifferenceAnalyzer.generate_analysis_report: DifferenceAnalyzer#generate_analysis_report().
  DifferenceAnalyzer.analyze_json_differences: DifferenceAnalyzer#analyze_json_differences().
  DifferenceAnalyzer.version_b_files: DifferenceAnalyzer#version_b_files.
  DifferenceAnalyzer.analyze_all_differences: DifferenceAnalyzer#analyze_all_differences().
  DifferenceAnalyzer.analyze_text_differences: DifferenceAnalyzer#analyze_text_differences().
  main: main().
  DifferenceAnalyzer.version_b_dir: DifferenceAnalyzer#version_b_dir.
  DifferenceAnalyzer.results_dir: DifferenceAnalyzer#results_dir.
  DifferenceAnalyzer.version_a: DifferenceAnalyzer#version_a.
  DifferenceAnalyzer.version_b: DifferenceAnalyzer#version_b.
  DifferenceAnalyzer.version_a_dir: DifferenceAnalyzer#version_a_dir.
  DifferenceAnalyzer.version_a_files: DifferenceAnalyzer#version_a_files.
  DifferenceAnalyzer: DifferenceAnalyzer#
  DifferenceAnalyzer.smart_compare: DifferenceAnalyzer#smart_compare.
  DifferenceAnalyzer.analysis_results: DifferenceAnalyzer#analysis_results.
  DifferenceAnalyzer.project_root: DifferenceAnalyzer#project_root.
  DifferenceAnalyzer.__init__: DifferenceAnalyzer#__init__().
  DifferenceAnalyzer.generate_normalized: DifferenceAnalyzer#generate_normalized.
---
# Module: [`compatibility_test/scripts/analyze_differences.py`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/analyze_differences.py)

## Classes
### `DifferenceAnalyzer`
- def: [`compatibility_test/scripts/analyze_differences.py:38`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/analyze_differences.py#L38)
- signature: `class DifferenceAnalyzer:`
- members:
  - `analyze_all_differences(self)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/analyze_differences.py#L113) — 全ての差分を分析
  - `analyze_json_differences(self, file_a: Path, file_b: Path)` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/analyze_differences.py#L63) — JSONファイルの構造的差分を分析
  - `analyze_text_differences(self, file_a: Path, file_b: Path)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/analyze_differences.py#L109) — テキストファイルの差分を分析
  - `generate_analysis_report(self, analysis_results: dict[str, Any])` — [`L136`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/analyze_differences.py#L136) — 分析レポートを生成
  - `analysis_results` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/analyze_differences.py#L61)
  - `generate_normalized` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/analyze_differences.py#L54)
  - `project_root` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/analyze_differences.py#L50)
  - `results_dir` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/analyze_differences.py#L56)
  - `smart_compare` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/analyze_differences.py#L53)
  - `version_a` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/analyze_differences.py#L48)
  - `version_a_dir` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/analyze_differences.py#L57)
  - `version_a_files` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/analyze_differences.py#L121)
  - `version_b` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/analyze_differences.py#L49)
  - `version_b_dir` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/analyze_differences.py#L58)
  - `version_b_files` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/analyze_differences.py#L124)
- protocol/private: `__init__`[`L39`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/analyze_differences.py#L39)
- uses (calls/refs, reference-scoped): [`compare_json_structure`](_analyze_differences_json_structure.md#compare_json_structure), [`determine_field_severity`](_analyze_differences_json_severity.md#determine_field_severity), [`analyze_common_files`](_analyze_differences_analysis.md#analyze_common_files), [`build_analysis_report_lines`](_analyze_differences_report.md#build_analysis_report_lines), [`analyze_text_difference`](_analyze_differences_json_text.md#analyze_text_difference), [`compare_performance_metrics`](_analyze_differences_json_metrics.md#compare_performance_metrics), [`configure_smart_comparison`](_analyze_differences_setup.md#configure_smart_comparison), [`determine_severity`](_analyze_differences_json_severity.md#determine_severity), [`load_json_pair`](_analyze_differences_json_text.md#load_json_pair), [`build_report_path`](_analyze_differences_report.md#build_report_path), [`generate_normalized_outputs`](_analyze_differences_analysis.md#generate_normalized_outputs), [`initial_analysis_results`](_analyze_differences_setup.md#initial_analysis_results), [`validate_version_dirs`](_analyze_differences_analysis.md#validate_version_dirs), [`write_report`](_analyze_differences_report.md#write_report)
- used by: [`main`](analyze_differences.md#main)  (3 test-only)

## Functions
- `main()` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/analyze_differences.py#L147) — メイン実行関数

