---
title: 'Module: tree_sitter_analyzer/_route_cache.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_route_cache.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._route_cache`/
symbols:
  RouteCache._conn: RouteCache#_conn().
  RouteCache._local: RouteCache#_local.
  RouteCache: RouteCache#
  RouteCache.get: RouteCache#get().
  RouteCache.put: RouteCache#put().
  RouteCache.get_by_stat: RouteCache#get_by_stat().
  RouteCache.bulk_get_by_stat: RouteCache#bulk_get_by_stat().
  RouteCache.stats: RouteCache#stats().
  RouteCache._enforce_scanner_version: RouteCache#_enforce_scanner_version().
  RouteCache.freshness_key: RouteCache#freshness_key().
  RouteCache.bulk_put: RouteCache#bulk_put().
  _SCANNER_VERSION: _SCANNER_VERSION.
  _ROUTE_CACHE_SCHEMA: _ROUTE_CACHE_SCHEMA.
  RouteCache.db_path: RouteCache#db_path.
  RouteCache._hash: RouteCache#_hash().
  RouteCache.stat_mtime: RouteCache#stat_mtime().
  RouteCache.__init__: RouteCache#__init__().
---
# Module: [`tree_sitter_analyzer/_route_cache.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_cache.py)

## Classes
### `RouteCache`
- def: [`tree_sitter_analyzer/_route_cache.py:54`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_cache.py#L54)
- doc: SQLite-backed cache for per-file route detection.
- signature: `class RouteCache:`
- members:
  - `_enforce_scanner_version(self, expected: int)` — [`L76`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_cache.py#L76) — Clear the cache when its stored scanner version disagrees with ``expected``.
  - `bulk_get_by_stat(self, paths_with_mtimes: list[tuple[str, int]])` — [`L173`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_cache.py#L173) — Return ``{file_path: routes}`` for every (path, mtime) pair whose
  - `bulk_put(self, records: list[tuple[str, str, int, list[dict[str, Any]]]])` — [`L219`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_cache.py#L219) — Insert/update many cache rows in one transaction.
  - `freshness_key(self, file_path: str)` — [`L123`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_cache.py#L123) — Return ``(content_hash, mtime_ns)`` for the file, or ``None`` on read error.
  - `get(self, file_path: str, content_hash: str)` — [`L133`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_cache.py#L133)
  - `get_by_stat(self, file_path: str, mtime_ns: int)` — [`L147`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_cache.py#L147) — Fast path: trust the OS mtime as the freshness signal, skipping
  - `put(self, file_path: str, content_hash: str, mtime_ns: int, routes: list[dict[str, Any]])` — [`L245`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_cache.py#L245)
  - `stat_mtime(self, file_path: str)` — [`L166`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_cache.py#L166) — Return the file's mtime_ns or None if it cannot be stat'd.
  - `stats(self)` — [`L265`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_cache.py#L265)
  - `db_path` — [`L64`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_cache.py#L64)
- protocol/private: `__init__`[`L63`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_cache.py#L63), `_conn`[`L109`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_cache.py#L109), `_hash`[`L120`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_cache.py#L120), `_local`[`L66`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_cache.py#L66)
- uses (calls/refs, reference-scoped): [`_SCANNER_VERSION`](_route_cache.md#_SCANNER_VERSION), [`_ROUTE_CACHE_SCHEMA`](_route_cache.md#_ROUTE_CACHE_SCHEMA)
- used by: [`_detect_all_cached`](route_detector.md#RouteDetector._detect_all_cached), [`_cache`](route_detector.md#RouteDetector._cache), [`cache_stats`](route_detector.md#RouteDetector.cache_stats)  (4 test-only)

## Module values
- `_ROUTE_CACHE_SCHEMA` — [`L36`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_cache.py#L36)
- `_SCANNER_VERSION` — [`L34`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_cache.py#L34)

