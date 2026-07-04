---
title: 'Module: tree_sitter_analyzer/core/cache_service.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/core/cache_service.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.core.cache_service`/Cache
symbols:
  CacheService.set: Service#set().
  CacheService.get: Service#get().
  CacheService: Service#
  CacheService.get_stats: Service#get_stats().
  CacheService.clear: Service#clear().
  CacheService.invalidate_pattern: Service#invalidate_pattern().
  CacheService._stats: Service#_stats.
  CacheService._l1_cache: Service#_l1_cache.
  CacheService._l2_cache: Service#_l2_cache.
  CacheService.size: Service#size().
  CacheEntry: Entry#
  CacheEntry.value: Entry#value.
  CacheService.__del__: Service#__del__().
  CacheEntry.expires_at: Entry#expires_at.
  CacheEntry.is_expired: Entry#is_expired().
  CacheService._l3_cache: Service#_l3_cache.
  CacheEntry.created_at: Entry#created_at.
  CacheService._lock: Service#_lock.
  CacheService.generate_cache_key: Service#generate_cache_key().
  CacheEntry.access_count: Entry#access_count.
  CacheService._default_ttl: Service#_default_ttl.
  CacheService._invalidate_keys_in_cache: Service#_invalidate_keys_in_cache().
  CacheService.__init__: Service#__init__().
---
# Module: [`tree_sitter_analyzer/core/cache_service.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py)

## Classes
### `CacheEntry`
- def: [`tree_sitter_analyzer/core/cache_service.py:27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L27)
- doc: Cache Entry
- signature: `class CacheEntry:`
- members:
  - `is_expired(self)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L45) — Expiration check
  - `access_count` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L43)
  - `created_at` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L41)
  - `expires_at` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L42)
  - `value` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L40)
- used by: [`set`](cache_service.md#CacheService.set), [`get`](cache_service.md#CacheService.get), [`_l1_cache`](cache_service.md#CacheService._l1_cache), [`_l2_cache`](cache_service.md#CacheService._l2_cache), [`_l3_cache`](cache_service.md#CacheService._l3_cache)  (5 test-only)

### `CacheService`
- def: [`tree_sitter_analyzer/core/cache_service.py:57`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L57)
- doc: Unified Cache Service
- signature: `class CacheService:`
- members:
  - `__del__(self)` — [`L330`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L330) — デストラクタ - リソースクリーンアップ
  - `__init__(self, l1_maxsize: int = 100, l2_maxsize: int = 1000, l3_maxsize: int = 10000, ttl_seconds: int = 3600)` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L72) — Initialization
  - `_invalidate_keys_in_cache(cache: Any, pattern: str)` — [`L314`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L314) — Remove every key in ``cache`` that contains ``pattern``.
  - `clear(self)` — [`L215`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L215) — 全キャッシュをクリア
  - `generate_cache_key(self, file_path: str, language: str, options: dict[str, Any])` — [`L266`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L266) — キャッシュキーを生成
  - `get(self, key: str)` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L117) — キャッシュから値を取得
  - `get_stats(self)` — [`L244`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L244) — キャッシュ統計を取得
  - `invalidate_pattern(self, pattern: str)` — [`L292`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L292) — パターンに一致するキーを無効化
  - `set(self, key: str, value: Any, ttl_seconds: int | None = None)` — [`L171`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L171) — キャッシュに値を設定
  - `size(self)` — [`L234`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L234) — キャッシュサイズを取得
- protocol/private: `_default_ttl`[`L110`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L110), `_l1_cache`[`L89`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L89), `_l2_cache`[`L90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L90), `_l3_cache`[`L93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L93), `_lock`[`L96`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L96), `_stats`[`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/cache_service.py#L99)
- uses (calls/refs, reference-scoped): [`log_debug`](../utils/logging.md#log_debug), [`log_info`](../utils/logging.md#log_info), [`CacheEntry`](cache_service.md#CacheEntry), [`value`](cache_service.md#CacheEntry.value), [`expires_at`](cache_service.md#CacheEntry.expires_at), [`is_expired`](cache_service.md#CacheEntry.is_expired), [`created_at`](cache_service.md#CacheEntry.created_at), [`access_count`](cache_service.md#CacheEntry.access_count)
- used by: [`_ensure_initialized`](analysis_engine.md#UnifiedAnalysisEngine._ensure_initialized), [`MCP_UTILS_CAPABILITIES`](../mcp/utils/__init__.md#MCP_UTILS_CAPABILITIES), [`clear_all_caches`](../mcp/utils/__init__.md#BackwardCompatibleCacheManager.clear_all_caches), [`get_cache_stats`](../mcp/utils/__init__.md#BackwardCompatibleCacheManager.get_cache_stats), [`__init__`](../mcp/utils/__init__.md#BackwardCompatibleCacheManager.__init__)  (41 test-only)

