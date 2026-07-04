---
title: 'Module: collect_project_metrics.py'
type: catalog
provenance: extracted
module: collect_project_metrics.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 collect_project_metrics/
symbols:
  main: main().
  collect_file_metrics: collect_file_metrics().
  collect_line_metrics: collect_line_metrics().
  is_project_file: is_project_file().
  count_lines_in_file: count_lines_in_file().
  analyze_project_structure: analyze_project_structure().
  check_dependencies: check_dependencies().
---
# Module: [`collect_project_metrics.py`](../../../../raw/code/tree-sitter-analyzer/collect_project_metrics.py)

## Functions
- `analyze_project_structure()` — [`L128`](../../../../raw/code/tree-sitter-analyzer/collect_project_metrics.py#L128) — プロジェクト構造を分析
- `check_dependencies()` — [`L147`](../../../../raw/code/tree-sitter-analyzer/collect_project_metrics.py#L147) — 依存関係を確認
- `collect_file_metrics()` — [`L46`](../../../../raw/code/tree-sitter-analyzer/collect_project_metrics.py#L46) — ファイルメトリクスを収集
- `collect_line_metrics(py_files, test_files)` — [`L79`](../../../../raw/code/tree-sitter-analyzer/collect_project_metrics.py#L79) — 行数メトリクスを収集
- `count_lines_in_file(filepath)` — [`L26`](../../../../raw/code/tree-sitter-analyzer/collect_project_metrics.py#L26) — ファイルの行数を数える
- `is_project_file(filepath)` — [`L10`](../../../../raw/code/tree-sitter-analyzer/collect_project_metrics.py#L10) — プロジェクト固有のファイルかどうかを判定
- `main()` — [`L173`](../../../../raw/code/tree-sitter-analyzer/collect_project_metrics.py#L173) — メイン関数

