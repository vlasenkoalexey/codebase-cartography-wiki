---
title: 'Module: compatibility_test/utils/cache_manager.py'
type: catalog
provenance: extracted
module: compatibility_test/utils/cache_manager.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `compatibility_test.utils.cache_manager`/
symbols:
  CacheManager.get_cache_stats: CacheManager#get_cache_stats().
  CacheManager._clear_analysis_engine_cache: CacheManager#_clear_analysis_engine_cache().
  logger: logger.
  CacheManager.clear_all_caches: CacheManager#clear_all_caches().
  CacheManager: CacheManager#
  result: result.
  clear_all_caches: clear_all_caches().
  get_cache_status: get_cache_status().
  CacheManager._clear_search_content_cache: CacheManager#_clear_search_content_cache().
  stats: stats.
  CacheManager.force_disable_caches: CacheManager#force_disable_caches().
  CacheManager._clear_other_mcp_caches: CacheManager#_clear_other_mcp_caches().
  CacheManager.project_root: CacheManager#project_root.
  CacheManager.__init__: CacheManager#__init__().
  CacheManager.cache_stats: CacheManager#cache_stats.
---
# Module: [`compatibility_test/utils/cache_manager.py`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_manager.py)

## Classes
### `CacheManager`
- def: [`compatibility_test/utils/cache_manager.py:16`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_manager.py#L16)
- doc: tree-sitter-analyzerのキャッシュを統合管理するクラス
- signature: `class CacheManager:`
- members:
  - `__init__(self, project_root: str | None = None)` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_manager.py#L21) — 初期化
  - `_clear_analysis_engine_cache(self)` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_manager.py#L80) — UnifiedAnalysisEngine のキャッシュをクリア
  - `_clear_other_mcp_caches(self)` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_manager.py#L119) — その他のMCPツールのキャッシュをクリア
  - `_clear_search_content_cache(self)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_manager.py#L105) — SearchContentTool のキャッシュをクリア
  - `clear_all_caches(self)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_manager.py#L31) — 全てのキャッシュをクリア
  - `force_disable_caches(self)` — [`L166`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_manager.py#L166) — キャッシュを強制的に無効化（テスト用）
  - `get_cache_stats(self)` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_manager.py#L130) — 各キャッシュの統計情報を取得
  - `cache_stats` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_manager.py#L29)
  - `project_root` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_manager.py#L28)
- uses (calls/refs, reference-scoped): [`UnifiedAnalysisEngine`](../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine), [`get_analysis_engine`](../../tree_sitter_analyzer/core/analysis_engine.md#get_analysis_engine), [`clear_cache`](../../tree_sitter_analyzer/mcp/utils/search_cache.md#clear_cache), [`get_stats`](../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get_stats), [`get_default_cache`](../../tree_sitter_analyzer/mcp/utils/search_cache.md#get_default_cache), [`configure_cache`](../../tree_sitter_analyzer/mcp/utils/search_cache.md#configure_cache), [`logger`](cache_manager.md#logger), [`_instances`](../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine._instances), [`clear_cache`](../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine.clear_cache), [`get_cache_stats`](../../tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.md#UnifiedAnalysisEngineRuntimeMixin.get_cache_stats)
- used by: [`run_compatibility_test`](../scripts/run_compatibility_test.md#StandardizedCompatibilityTester.run_compatibility_test), [`run_version_tests`](../scripts/run_compatibility_test.md#StandardizedCompatibilityTester.run_version_tests), [`_generate_cache_report_content`](../scripts/run_compatibility_test.md#StandardizedCompatibilityTester._generate_cache_report_content), [`generate_cache_report`](cache_reporter.md#generate_cache_report), [`cache_manager`](../scripts/run_compatibility_test.md#StandardizedCompatibilityTester.cache_manager), [`clear_all_caches`](cache_manager.md#clear_all_caches), [`get_cache_status`](cache_manager.md#get_cache_status)

## Functions
- `clear_all_caches(project_root: str | None = None)` — [`L199`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_manager.py#L199) — 便利関数：全キャッシュをクリア
- `get_cache_status(project_root: str | None = None)` — [`L213`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_manager.py#L213) — 便利関数：キャッシュ状態を取得

## Module values
- `logger` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_manager.py#L13)
- `result` — [`L233`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_manager.py#L233)
- `stats` — [`L239`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/cache_manager.py#L239)

