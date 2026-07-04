---
title: 'Module: scripts/update_readme_stats.py'
type: catalog
provenance: extracted
module: scripts/update_readme_stats.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.update_readme_stats`/
symbols:
  ReadmeStatsUpdater.run: ReadmeStatsUpdater#run().
  ReadmeStatsUpdater._fallback_test_count: ReadmeStatsUpdater#_fallback_test_count().
  ReadmeStatsUpdater.get_test_count: ReadmeStatsUpdater#get_test_count().
  ReadmeStatsUpdater.update_test_badges: ReadmeStatsUpdater#update_test_badges().
  ReadmeStatsUpdater.update_quality_metrics: ReadmeStatsUpdater#update_quality_metrics().
  main: main().
  ReadmeStatsUpdater.project_root: ReadmeStatsUpdater#project_root.
  ReadmeStatsUpdater.readme_files: ReadmeStatsUpdater#readme_files.
  ReadmeStatsUpdater: ReadmeStatsUpdater#
  ReadmeStatsUpdater.__init__: ReadmeStatsUpdater#__init__().
---
# Module: [`scripts/update_readme_stats.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/update_readme_stats.py)

## Classes
### `ReadmeStatsUpdater`
- def: [`scripts/update_readme_stats.py:17`](../../../../../raw/code/tree-sitter-analyzer/scripts/update_readme_stats.py#L17)
- doc: README統計情報更新クラス
- signature: `class ReadmeStatsUpdater:`
- members:
  - `_fallback_test_count(self)` — [`L63`](../../../../../raw/code/tree-sitter-analyzer/scripts/update_readme_stats.py#L63) — フォールバック: testsディレクトリからテストファイル数を推定
  - `get_test_count(self)` — [`L24`](../../../../../raw/code/tree-sitter-analyzer/scripts/update_readme_stats.py#L24) — pytestを実行してテスト数を取得
  - `run(self)` — [`L241`](../../../../../raw/code/tree-sitter-analyzer/scripts/update_readme_stats.py#L241) — メイン実行関数
  - `update_quality_metrics(self, test_count: int)` — [`L121`](../../../../../raw/code/tree-sitter-analyzer/scripts/update_readme_stats.py#L121) — 品質指標の記述を更新
  - `update_test_badges(self, test_count: int)` — [`L77`](../../../../../raw/code/tree-sitter-analyzer/scripts/update_readme_stats.py#L77) — 全READMEファイルのテスト数バッジを更新
  - `project_root` — [`L21`](../../../../../raw/code/tree-sitter-analyzer/scripts/update_readme_stats.py#L21)
  - `readme_files` — [`L22`](../../../../../raw/code/tree-sitter-analyzer/scripts/update_readme_stats.py#L22)
- protocol/private: `__init__`[`L20`](../../../../../raw/code/tree-sitter-analyzer/scripts/update_readme_stats.py#L20)
- used by: [`main`](update_readme_stats.md#main)

## Functions
- `main()` — [`L261`](../../../../../raw/code/tree-sitter-analyzer/scripts/update_readme_stats.py#L261) — メイン関数

