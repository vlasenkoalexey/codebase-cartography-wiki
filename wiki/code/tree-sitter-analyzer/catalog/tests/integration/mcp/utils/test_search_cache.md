---
title: 'Module: tests/integration/mcp/utils/test_search_cache.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/utils/test_search_cache.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.utils.test_search_cache`/Test
symbols:
  TestCacheClear.test_clear_all_data: CacheClear#test_clear_all_data().
  TestSearchCacheInitialization.test_cache_initialization_default: SearchCacheInitialization#test_cache_initialization_default().
  TestGlobalCacheFunctions.test_clear_default_cache: GlobalCacheFunctions#test_clear_default_cache().
  TestCacheGetSet.test_set_and_get_success: CacheGetSet#test_set_and_get_success().
  TestCacheGetSet.test_get_nonexistent_key: CacheGetSet#test_get_nonexistent_key().
  TestCacheLRUEviction.test_lru_eviction_when_full: CacheLRUEviction#test_lru_eviction_when_full().
  TestThreadSafety.test_concurrent_set_get_mixed: ThreadSafety#test_concurrent_set_get_mixed().
  TestGlobalCacheFunctions.test_configure_cache: GlobalCacheFunctions#test_configure_cache().
  TestCacheEdgeCases.test_get_with_expired_entry_removal: CacheEdgeCases#test_get_with_expired_entry_removal().
  TestSearchCacheInitialization.test_cache_initialization_custom: SearchCacheInitialization#test_cache_initialization_custom().
  TestCacheExpiration.test_cache_entry_expired: CacheExpiration#test_cache_entry_expired().
  TestCacheLRUEviction.test_update_existing_key_no_eviction: CacheLRUEviction#test_update_existing_key_no_eviction().
  TestCacheStatistics.test_get_stats_with_data: CacheStatistics#test_get_stats_with_data().
  TestCacheStatistics.test_hit_rate_calculation: CacheStatistics#test_hit_rate_calculation().
  TestCacheClear.test_clear_empty_cache: CacheClear#test_clear_empty_cache().
  TestThreadSafety.test_concurrent_get_operations: ThreadSafety#test_concurrent_get_operations().
  TestSearchCacheInitialization.test_cache_initialization_lock: SearchCacheInitialization#test_cache_initialization_lock().
  TestCacheGetSet.test_set_updates_existing_key: CacheGetSet#test_set_updates_existing_key().
  TestCacheGetSet.test_set_various_data_types: CacheGetSet#test_set_various_data_types().
  TestCacheExpiration.test_cache_entry_not_expired: CacheExpiration#test_cache_entry_not_expired().
  TestCacheExpiration.test_is_expired_true: CacheExpiration#test_is_expired_true().
  TestCacheExpiration.test_is_expired_false: CacheExpiration#test_is_expired_false().
  TestCacheExpiration.test_cleanup_expired_entries: CacheExpiration#test_cleanup_expired_entries().
  TestCacheLRUEviction.test_no_eviction_when_not_full: CacheLRUEviction#test_no_eviction_when_not_full().
  TestCacheStatistics.test_get_stats_empty_cache: CacheStatistics#test_get_stats_empty_cache().
  TestCacheStatistics.test_stats_includes_expired_count: CacheStatistics#test_stats_includes_expired_count().
  TestCacheKeyGeneration.test_create_cache_key_basic: CacheKeyGeneration#test_create_cache_key_basic().
  TestCacheKeyGeneration.test_create_cache_key_normalizes_query: CacheKeyGeneration#test_create_cache_key_normalizes_query().
  TestCacheKeyGeneration.test_create_cache_key_normalizes_roots: CacheKeyGeneration#test_create_cache_key_normalizes_roots().
  TestCacheKeyGeneration.test_create_cache_key_with_params: CacheKeyGeneration#test_create_cache_key_with_params().
  TestCacheKeyGeneration.test_create_cache_key_deterministic: CacheKeyGeneration#test_create_cache_key_deterministic().
  TestFormatCompatibility.test_is_format_compatible_total_only: FormatCompatibility#test_is_format_compatible_total_only().
  TestFormatCompatibility.test_is_format_compatible_count_only: FormatCompatibility#test_is_format_compatible_count_only().
  TestFormatCompatibility.test_is_format_compatible_summary: FormatCompatibility#test_is_format_compatible_summary().
  TestFormatCompatibility.test_is_format_compatible_normal: FormatCompatibility#test_is_format_compatible_normal().
  TestFormatCompatibility.test_is_format_compatible_unknown_format: FormatCompatibility#test_is_format_compatible_unknown_format().
  TestCompatibleResultDerivation.test_get_compatible_result_direct_hit: CompatibleResultDerivation#test_get_compatible_result_direct_hit().
  TestCompatibleResultDerivation.test_get_compatible_result_no_match: CompatibleResultDerivation#test_get_compatible_result_no_match().
  TestCompatibleResultDerivation.test_derive_count_key_from_cache_key: CompatibleResultDerivation#test_derive_count_key_from_cache_key().
  TestCompatibleResultDerivation.test_derive_count_key_adds_param: CompatibleResultDerivation#test_derive_count_key_adds_param().
  TestCompatibleResultDerivation.test_derive_count_key_none: CompatibleResultDerivation#test_derive_count_key_none().
  TestCompatibleResultDerivation.test_can_derive_file_list_true: CompatibleResultDerivation#test_can_derive_file_list_true().
  TestCompatibleResultDerivation.test_can_derive_file_list_false: CompatibleResultDerivation#test_can_derive_file_list_false().
  TestCompatibleResultDerivation.test_derive_file_list_result_summary: CompatibleResultDerivation#test_derive_file_list_result_summary().
  TestCompatibleResultDerivation.test_derive_file_list_result_file_list: CompatibleResultDerivation#test_derive_file_list_result_file_list().
  TestThreadSafety.test_concurrent_set_operations: ThreadSafety#test_concurrent_set_operations().
  TestCacheEdgeCases.test_set_with_zero_max_size: CacheEdgeCases#test_set_with_zero_max_size().
  TestCacheEdgeCases.test_set_with_zero_ttl: CacheEdgeCases#test_set_with_zero_ttl().
  TestCacheEdgeCases.test_empty_string_key: CacheEdgeCases#test_empty_string_key().
  TestCacheEdgeCases.test_very_long_key: CacheEdgeCases#test_very_long_key().
  TestCacheEdgeCases.test_cache_key_path_resolution_error: CacheEdgeCases#test_cache_key_path_resolution_error().
  TestCacheAccessTimeTracking.test_access_time_updated_on_get: CacheAccessTimeTracking#test_access_time_updated_on_get().
  TestCacheAccessTimeTracking.test_access_time_updated_on_set: CacheAccessTimeTracking#test_access_time_updated_on_set().
  TestGlobalCacheFunctions.test_get_default_cache_singleton: GlobalCacheFunctions#test_get_default_cache_singleton().
  TestSearchCacheInitialization: SearchCacheInitialization#
  TestCacheGetSet: CacheGetSet#
  TestCacheExpiration: CacheExpiration#
  TestCacheLRUEviction: CacheLRUEviction#
  TestCacheStatistics: CacheStatistics#
  TestCacheClear: CacheClear#
  TestCacheKeyGeneration: CacheKeyGeneration#
  TestFormatCompatibility: FormatCompatibility#
  TestCompatibleResultDerivation: CompatibleResultDerivation#
  TestThreadSafety: ThreadSafety#
  TestGlobalCacheFunctions: GlobalCacheFunctions#
  TestCacheEdgeCases: CacheEdgeCases#
  TestCacheAccessTimeTracking: CacheAccessTimeTracking#
---
# Module: [`tests/integration/mcp/utils/test_search_cache.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py)

## Classes
### `TestCacheAccessTimeTracking`
- def: [`tests/integration/mcp/utils/test_search_cache.py:532`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L532)
- doc: Tests for access time tracking for LRU.
- signature: `class TestCacheAccessTimeTracking:`
- members:
  - `test_access_time_updated_on_get(self)` — [`L535`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L535) — Test that access time is updated on get.
  - `test_access_time_updated_on_set(self)` — [`L549`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L549) — Test that access time is updated on set.
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`get`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get)

### `TestCacheClear`
- def: [`tests/integration/mcp/utils/test_search_cache.py:224`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L224)
- doc: Tests for cache clearing.
- signature: `class TestCacheClear:`
- members:
  - `test_clear_all_data(self)` — [`L227`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L227) — Test that clear removes all data.
  - `test_clear_empty_cache(self)` — [`L241`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L241) — Test clearing an empty cache.
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`get`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get), [`clear`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.clear), [`cache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.cache), [`_access_times`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._access_times), [`_hits`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._hits), [`_misses`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._misses), [`_evictions`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._evictions)

### `TestCacheEdgeCases`
- def: [`tests/integration/mcp/utils/test_search_cache.py:475`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L475)
- doc: Tests for edge cases.
- signature: `class TestCacheEdgeCases:`
- members:
  - `test_cache_key_path_resolution_error(self)` — [`L521`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L521) — Test cache key generation with path resolution error.
  - `test_empty_string_key(self)` — [`L506`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L506) — Test with empty string key.
  - `test_get_with_expired_entry_removal(self)` — [`L478`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L478) — Test that get removes expired entry.
  - `test_set_with_zero_max_size(self)` — [`L488`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L488) — Test cache with zero max size.
  - `test_set_with_zero_ttl(self)` — [`L497`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L497) — Test cache with zero TTL.
  - `test_very_long_key(self)` — [`L513`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L513) — Test with very long cache key.
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`get`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get), [`create_cache_key`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.create_cache_key), [`cache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.cache), [`_access_times`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._access_times), [`_evictions`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._evictions)

### `TestCacheExpiration`
- def: [`tests/integration/mcp/utils/test_search_cache.py:89`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L89)
- doc: Tests for TTL-based cache expiration.
- signature: `class TestCacheExpiration:`
- members:
  - `test_cache_entry_expired(self)` — [`L100`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L100) — Test that expired entries are removed.
  - `test_cache_entry_not_expired(self)` — [`L92`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L92) — Test that fresh entries are not expired.
  - `test_cleanup_expired_entries(self)` — [`L121`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L121) — Test that expired entries are cleaned up.
  - `test_is_expired_false(self)` — [`L115`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L115) — Test _is_expired returns False for fresh entry.
  - `test_is_expired_true(self)` — [`L109`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L109) — Test _is_expired returns True for expired entry.
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`get`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get), [`_misses`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._misses), [`_is_expired`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._is_expired)

### `TestCacheGetSet`
- def: [`tests/integration/mcp/utils/test_search_cache.py:47`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L47)
- doc: Tests for basic get/set operations.
- signature: `class TestCacheGetSet:`
- members:
  - `test_get_nonexistent_key(self)` — [`L59`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L59) — Test get with nonexistent key.
  - `test_set_and_get_success(self)` — [`L50`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L50) — Test successful set and get operations.
  - `test_set_updates_existing_key(self)` — [`L67`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L67) — Test that set updates existing key.
  - `test_set_various_data_types(self)` — [`L75`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L75) — Test storing different data types.
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`get`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get), [`_hits`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._hits), [`_misses`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._misses)

### `TestCacheKeyGeneration`
- def: [`tests/integration/mcp/utils/test_search_cache.py:248`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L248)
- doc: Tests for cache key generation.
- signature: `class TestCacheKeyGeneration:`
- members:
  - `test_create_cache_key_basic(self)` — [`L251`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L251) — Test basic cache key generation.
  - `test_create_cache_key_deterministic(self)` — [`L282`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L282) — Test that same parameters produce same key.
  - `test_create_cache_key_normalizes_query(self)` — [`L258`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L258) — Test that cache key normalizes query.
  - `test_create_cache_key_normalizes_roots(self)` — [`L265`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L265) — Test that cache key normalizes and sorts roots.
  - `test_create_cache_key_with_params(self)` — [`L272`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L272) — Test cache key with search parameters.
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`create_cache_key`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.create_cache_key)

### `TestCacheLRUEviction`
- def: [`tests/integration/mcp/utils/test_search_cache.py:135`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L135)
- doc: Tests for LRU (Least Recently Used) eviction.
- signature: `class TestCacheLRUEviction:`
- members:
  - `test_lru_eviction_when_full(self)` — [`L138`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L138) — Test that LRU entry is evicted when cache is full.
  - `test_no_eviction_when_not_full(self)` — [`L153`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L153) — Test that no eviction occurs when cache is not full.
  - `test_update_existing_key_no_eviction(self)` — [`L161`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L161) — Test that updating existing key doesn't trigger eviction.
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`get`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get), [`cache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.cache), [`_evictions`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._evictions)

### `TestCacheStatistics`
- def: [`tests/integration/mcp/utils/test_search_cache.py:173`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L173)
- doc: Tests for cache statistics tracking.
- signature: `class TestCacheStatistics:`
- members:
  - `test_get_stats_empty_cache(self)` — [`L176`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L176) — Test statistics for empty cache.
  - `test_get_stats_with_data(self)` — [`L187`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L187) — Test statistics with cache data.
  - `test_hit_rate_calculation(self)` — [`L201`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L201) — Test hit rate percentage calculation.
  - `test_stats_includes_expired_count(self)` — [`L214`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L214) — Test that stats count expired entries.
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`get`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get), [`get_stats`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get_stats)

### `TestCompatibleResultDerivation`
- def: [`tests/integration/mcp/utils/test_search_cache.py:332`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L332)
- doc: Tests for compatible result derivation.
- signature: `class TestCompatibleResultDerivation:`
- members:
  - `test_can_derive_file_list_false(self)` — [`L375`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L375) — Test checking if file list cannot be derived.
  - `test_can_derive_file_list_true(self)` — [`L369`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L369) — Test checking if file list can be derived.
  - `test_derive_count_key_adds_param(self)` — [`L355`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L355) — Test that derive count key adds count_only_matches.
  - `test_derive_count_key_from_cache_key(self)` — [`L348`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L348) — Test deriving count key from cache key.
  - `test_derive_count_key_none(self)` — [`L362`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L362) — Test derive count key returns None when not applicable.
  - `test_derive_file_list_result_file_list(self)` — [`L389`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L389) — Test deriving file list result for file_list format.
  - `test_derive_file_list_result_summary(self)` — [`L381`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L381) — Test deriving file list result for summary format.
  - `test_get_compatible_result_direct_hit(self)` — [`L335`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L335) — Test getting compatible result with direct cache hit.
  - `test_get_compatible_result_no_match(self)` — [`L342`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L342) — Test getting compatible result with no cache hit.
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`get_compatible_result`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get_compatible_result), [`_derive_file_list_result`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._derive_file_list_result), [`_can_derive_file_list`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._can_derive_file_list), [`_derive_count_key_from_cache_key`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._derive_count_key_from_cache_key)

### `TestFormatCompatibility`
- def: [`tests/integration/mcp/utils/test_search_cache.py:294`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L294)
- doc: Tests for format compatibility checking.
- signature: `class TestFormatCompatibility:`
- members:
  - `test_is_format_compatible_count_only(self)` — [`L303`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L303) — Test format compatibility for count_only.
  - `test_is_format_compatible_normal(self)` — [`L317`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L317) — Test format compatibility for normal format.
  - `test_is_format_compatible_summary(self)` — [`L310`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L310) — Test format compatibility for summary.
  - `test_is_format_compatible_total_only(self)` — [`L297`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L297) — Test format compatibility for total_only.
  - `test_is_format_compatible_unknown_format(self)` — [`L325`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L325) — Test format compatibility for unknown format.
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`_is_format_compatible`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._is_format_compatible)

### `TestGlobalCacheFunctions`
- def: [`tests/integration/mcp/utils/test_search_cache.py:448`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L448)
- doc: Tests for global cache functions.
- signature: `class TestGlobalCacheFunctions:`
- members:
  - `test_clear_default_cache(self)` — [`L464`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L464) — Test clearing the default cache.
  - `test_configure_cache(self)` — [`L457`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L457) — Test configuring the default cache.
  - `test_get_default_cache_singleton(self)` — [`L451`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L451) — Test that get_default_cache returns singleton.
- uses (calls/refs, reference-scoped): [`clear_cache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#clear_cache), [`get_default_cache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#get_default_cache), [`cache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.cache), [`configure_cache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#configure_cache), [`_hits`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._hits), [`_misses`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._misses), [`ttl_seconds`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.ttl_seconds), [`max_size`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.max_size)

### `TestSearchCacheInitialization`
- def: [`tests/integration/mcp/utils/test_search_cache.py:21`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L21)
- doc: Tests for SearchCache initialization.
- signature: `class TestSearchCacheInitialization:`
- members:
  - `test_cache_initialization_custom(self)` — [`L34`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L34) — Test cache initialization with custom parameters.
  - `test_cache_initialization_default(self)` — [`L24`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L24) — Test cache initialization with default parameters.
  - `test_cache_initialization_lock(self)` — [`L40`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L40) — Test that cache initializes with thread lock.
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`cache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.cache), [`_hits`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._hits), [`_misses`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._misses), [`_evictions`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._evictions), [`ttl_seconds`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.ttl_seconds), [`_lock`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._lock), [`max_size`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.max_size)

### `TestThreadSafety`
- def: [`tests/integration/mcp/utils/test_search_cache.py:400`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L400)
- doc: Tests for thread-safe operations.
- signature: `class TestThreadSafety:`
- members:
  - `test_concurrent_get_operations(self)` — [`L415`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L415) — Test that concurrent get operations are safe.
  - `test_concurrent_set_get_mixed(self)` — [`L428`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L428) — Test mixed concurrent set and get operations.
  - `test_concurrent_set_operations(self)` — [`L403`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/utils/test_search_cache.py#L403) — Test that concurrent set operations are safe.
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`get`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get), [`cache`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.cache), [`_hits`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._hits), [`_misses`](../../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._misses)

