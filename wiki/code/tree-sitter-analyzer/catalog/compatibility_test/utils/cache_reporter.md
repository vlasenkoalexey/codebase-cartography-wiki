---
title: 'Module: compatibility_test/utils/cache_reporter.py'
type: catalog
provenance: extracted
module: compatibility_test/utils/cache_reporter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `compatibility_test.utils.cache_reporter`/
symbols:
  CacheReporter.generate_cache_report: CacheReporter#generate_cache_report().
  generate_cache_report: generate_cache_report().
  markdown: markdown.
  CacheReporter: CacheReporter#
  report: report.
  reporter: reporter.
  CacheReporter.format_report_for_markdown: CacheReporter#format_report_for_markdown().
  CacheReporter._generate_summary: CacheReporter#_generate_summary().
  CacheReporter._generate_details: CacheReporter#_generate_details().
  CacheReporter._generate_recommendations: CacheReporter#_generate_recommendations().
  CacheReporter._analyze_cache_impact: CacheReporter#_analyze_cache_impact().
  logger: logger.
  CacheReporter.__init__: CacheReporter#__init__().
  CacheReporter.project_root: CacheReporter#project_root.
---
# Module: [`compatibility_test/utils/cache_reporter.py`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_reporter.py)

## Classes
### `CacheReporter`
- def: [`compatibility_test/utils/cache_reporter.py:15`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_reporter.py#L15)
- doc: キャッシュ状態のレポート生成クラス
- signature: `class CacheReporter:`
- members:
  - `__init__(self, project_root: str | None = None)` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_reporter.py#L20) — 初期化
  - `_analyze_cache_impact(self, cache_stats: dict[str, Any])` — [`L233`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_reporter.py#L233) — キャッシュがテストに与える影響を分析
  - `_generate_details(self, cache_stats: dict[str, Any])` — [`L111`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_reporter.py#L111) — 詳細情報を生成
  - `_generate_recommendations(self, cache_stats: dict[str, Any])` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_reporter.py#L173) — 推奨事項を生成
  - `_generate_summary(self, cache_stats: dict[str, Any])` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_reporter.py#L49) — サマリー情報を生成
  - `format_report_for_markdown(self, report: dict[str, Any])` — [`L313`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_reporter.py#L313) — レポートをMarkdown形式でフォーマット
  - `generate_cache_report(self, cache_stats: dict[str, Any])` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_reporter.py#L29) — キャッシュ統計からレポートを生成
  - `project_root` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_reporter.py#L27)
- used by: [`_generate_cache_report_content`](../scripts/run_compatibility_test.md#StandardizedCompatibilityTester._generate_cache_report_content), [`generate_cache_report`](cache_reporter.md#generate_cache_report), [`markdown`](cache_reporter.md#markdown), [`cache_reporter`](../scripts/run_compatibility_test.md#StandardizedCompatibilityTester.cache_reporter), [`reporter`](cache_reporter.md#reporter)

## Functions
- `generate_cache_report(project_root: str | None = None)` — [`L413`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_reporter.py#L413) — 便利関数：キャッシュレポートを生成

## Module values
- `logger` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_reporter.py#L12)
- `markdown` — [`L449`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_reporter.py#L449)
- `report` — [`L446`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_reporter.py#L446)
- `reporter` — [`L448`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_reporter.py#L448)

