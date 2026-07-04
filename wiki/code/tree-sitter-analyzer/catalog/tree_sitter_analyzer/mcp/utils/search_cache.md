---
title: 'Module: tree_sitter_analyzer/mcp/utils/search_cache.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/search_cache.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.search_cache`/
symbols:
  SearchCache: SearchCache#
  SearchCache.get: SearchCache#get().
  clear_cache: clear_cache().
  SearchCache.get_stats: SearchCache#get_stats().
  get_default_cache: get_default_cache().
  SearchCache.get_compatible_result: SearchCache#get_compatible_result().
  SearchCache._is_format_compatible: SearchCache#_is_format_compatible().
  SearchCache.clear: SearchCache#clear().
  SearchCache.create_cache_key: SearchCache#create_cache_key().
  SearchCache.cache: SearchCache#cache.
  SearchCache.set: SearchCache#set().
  configure_cache: configure_cache().
  SearchCache._derive_file_list_result: SearchCache#_derive_file_list_result().
  SearchCache._hits: SearchCache#_hits.
  SearchCache._misses: SearchCache#_misses.
  SearchCache._access_times: SearchCache#_access_times.
  SearchCache._cleanup_expired: SearchCache#_cleanup_expired().
  SearchCache._evict_one_lru_entry: SearchCache#_evict_one_lru_entry().
  SearchCache._evictions: SearchCache#_evictions.
  SearchCache.ttl_seconds: SearchCache#ttl_seconds.
  SearchCache.max_size: SearchCache#max_size.
  SearchCache._lock: SearchCache#_lock.
  logger: logger.
  SearchCache._is_expired: SearchCache#_is_expired().
  _default_cache: _default_cache.
  SearchCache._derive_count_key_from_cache_key: SearchCache#_derive_count_key_from_cache_key().
  SearchCache._can_derive_file_list: SearchCache#_can_derive_file_list().
  _default_cache_lock: _default_cache_lock.
  SearchCache.__init__: SearchCache#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/utils/search_cache.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py)

## Classes
### `SearchCache`
- def: [`tree_sitter_analyzer/mcp/utils/search_cache.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L20)
- doc: Thread-safe in-memory search result cache with TTL and LRU eviction
- signature: `class SearchCache:`
- members:
  - `__init__(self, max_size: int = 1000, ttl_seconds: int = 3600)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L23) — Initialize the search cache.
  - `_can_derive_file_list(self, count_result: dict[str, Any])` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L167) — Check if a count result contains file count data that can derive file lists.
  - `_cleanup_expired(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L46) — Remove expired entries (should be called with lock held)
  - `_derive_count_key_from_cache_key(self, cache_key: str)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L155) — Try to derive what the count_only cache key would be for this search.
  - `_derive_file_list_result(self, count_result: dict[str, Any], requested_format: str)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L175) — Derive file list result from count data.
  - `_evict_one_lru_entry(self)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L222) — Evict the least-recently-used cache entry.
  - `_is_expired(self, timestamp: float)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L42) — Check if a cache entry is expired
  - `_is_format_compatible(self, cached_result: Any, requested_format: str)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L123) — Check if a cached result is compatible with the requested format.
  - `clear(self)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L244) — Clear all cached results
  - `create_cache_key(self, query: str, roots: list[str], **params: Any)` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L277) — Create a deterministic cache key for search parameters.
  - `get(self, cache_key: str)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L62) — Get cached result if valid.
  - `get_compatible_result(self, cache_key: str, requested_format: str)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L89) — Get cached result and try to derive compatible formats.
  - `get_stats(self)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L254) — Get cache statistics
  - `set(self, cache_key: str, data: dict[str, Any] | Any)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L203) — Set cached result.
  - `cache` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L31)
  - `max_size` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L32)
  - `ttl_seconds` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L33)
- protocol/private: `_access_times`[`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L35), `_evictions`[`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L40), `_hits`[`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L38), `_lock`[`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L34), `_misses`[`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L39)
- uses (calls/refs, reference-scoped): [`create_file_summary_from_count_data`](../tools/fd_rg_result_utils.md#create_file_summary_from_count_data), [`extract_file_list_from_count_data`](../tools/fd_rg_result_utils.md#extract_file_list_from_count_data), [`logger`](search_cache.md#logger)
- used by: [`clear_cache`](search_cache.md#clear_cache), [`get_default_cache`](search_cache.md#get_default_cache), [`get_cache_stats`](../../../compatibility_test/utils/cache_manager.md#CacheManager.get_cache_stats), [`configure_cache`](search_cache.md#configure_cache), [`_check_cache`](../tools/search_content_tool.md#SearchContentTool._check_cache), [`_make_cache_key`](../tools/search_content_tool.md#SearchContentTool._make_cache_key)  (78 test-only)

## Functions
- `clear_cache()` — [`L353`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L353) — Clear the default search cache
- `configure_cache(max_size: int = 1000, ttl_seconds: int = 3600)` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L347) — Configure the default search cache
- `get_default_cache()` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L338) — Get the default search cache instance

## Module values
- `_default_cache` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L334)
- `_default_cache_lock` — [`L335`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L335)
- `logger` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/search_cache.py#L17)

