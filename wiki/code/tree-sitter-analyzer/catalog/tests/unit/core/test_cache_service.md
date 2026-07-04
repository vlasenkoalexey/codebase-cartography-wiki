---
title: 'Module: tests/unit/core/test_cache_service.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_cache_service.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_cache_service`/TestCache
symbols:
  TestCacheServiceEdgeCases.test_l2_cache_hit_promotes_to_l1: ServiceEdgeCases#test_l2_cache_hit_promotes_to_l1().
  TestCacheServiceEdgeCases.test_l3_cache_hit_promotes_to_l1_and_l2: ServiceEdgeCases#test_l3_cache_hit_promotes_to_l1_and_l2().
  TestCacheEntry.test_cache_entry_initialization: Entry#test_cache_entry_initialization().
  TestCacheEntry.test_cache_entry_defaults: Entry#test_cache_entry_defaults().
  TestCacheEntry.test_is_expired_with_expiration: Entry#test_is_expired_with_expiration().
  TestCacheEntry.test_is_expired_without_expiration: Entry#test_is_expired_without_expiration().
  TestCacheEntry.test_is_expired_future: Entry#test_is_expired_future().
  TestCacheServiceClear.test_clear_all_caches: ServiceClear#test_clear_all_caches().
  TestCacheServiceClear.test_clear_resets_stats: ServiceClear#test_clear_resets_stats().
  TestCacheServiceSet.test_set_and_get: ServiceSet#test_set_and_get().
  TestCacheServiceStats.test_get_stats_comprehensive: ServiceStats#test_get_stats_comprehensive().
  TestCacheServiceStats.test_hit_rate_calculation: ServiceStats#test_hit_rate_calculation().
  TestCacheServiceStats.test_l1_l2_l3_hit_tracking: ServiceStats#test_l1_l2_l3_hit_tracking().
  TestCacheServiceInvalidatePattern.test_invalidate_pattern: ServiceInvalidatePattern#test_invalidate_pattern().
  TestCacheServiceHierarchical.test_cache_promotion_l2_to_l1: ServiceHierarchical#test_cache_promotion_l2_to_l1().
  TestCacheServiceHierarchical.test_cache_promotion_l3_to_l2: ServiceHierarchical#test_cache_promotion_l3_to_l2().
  TestCacheServiceHierarchical.test_multiple_cache_tiers: ServiceHierarchical#test_multiple_cache_tiers().
  TestCacheServiceInit.test_cache_service_default_initialization: ServiceInit#test_cache_service_default_initialization().
  TestCacheServiceInit.test_cache_service_custom_sizes: ServiceInit#test_cache_service_custom_sizes().
  TestCacheServiceGet.test_get_cache_miss: ServiceGet#test_get_cache_miss().
  TestCacheServiceGet.test_get_l1_hit: ServiceGet#test_get_l1_hit().
  TestCacheServiceGet.test_get_expired_entry: ServiceGet#test_get_expired_entry().
  TestCacheServiceSet.test_set_with_custom_ttl: ServiceSet#test_set_with_custom_ttl().
  TestCacheServiceSet.test_set_overwrites_existing: ServiceSet#test_set_overwrites_existing().
  TestCacheServiceSet.test_set_unserializable_value: ServiceSet#test_set_unserializable_value().
  TestCacheServiceSize.test_size_with_entries: ServiceSize#test_size_with_entries().
  TestCacheServiceInvalidatePattern.test_invalidate_pattern_no_matches: ServiceInvalidatePattern#test_invalidate_pattern_no_matches().
  TestCacheServiceInvalidatePattern.test_invalidate_pattern_all: ServiceInvalidatePattern#test_invalidate_pattern_all().
  TestCacheServiceThreadSafety.test_concurrent_sets: ServiceThreadSafety#test_concurrent_sets().
  TestCacheServiceThreadSafety.test_concurrent_gets: ServiceThreadSafety#test_concurrent_gets().
  TestCacheServiceEdgeCases.test_large_value: ServiceEdgeCases#test_large_value().
  TestCacheServiceEdgeCases.test_complex_value: ServiceEdgeCases#test_complex_value().
  TestCacheServiceEdgeCases.test_cache_eviction: ServiceEdgeCases#test_cache_eviction().
  TestCacheServiceInit.test_cache_service_stats_initialization: ServiceInit#test_cache_service_stats_initialization().
  TestCacheServiceGet.test_get_empty_key: ServiceGet#test_get_empty_key().
  TestCacheServiceGet.test_get_none_key: ServiceGet#test_get_none_key().
  TestCacheServiceSet.test_set_empty_key: ServiceSet#test_set_empty_key().
  TestCacheServiceSet.test_set_none_key: ServiceSet#test_set_none_key().
  TestCacheServiceSize.test_size_empty_cache: ServiceSize#test_size_empty_cache().
  TestCacheServiceStats.test_hit_rate_no_requests: ServiceStats#test_hit_rate_no_requests().
  TestCacheServiceGenerateKey.test_generate_cache_key_basic: ServiceGenerateKey#test_generate_cache_key_basic().
  TestCacheServiceGenerateKey.test_generate_cache_key_consistent: ServiceGenerateKey#test_generate_cache_key_consistent().
  TestCacheServiceGenerateKey.test_generate_cache_key_different_inputs: ServiceGenerateKey#test_generate_cache_key_different_inputs().
  TestCacheServiceThreadSafety.set_value: ServiceThreadSafety#set_value().
  TestCacheServiceThreadSafety.get_value: ServiceThreadSafety#get_value().
  TestCacheServiceSet.test_set_unserializable_value.UnserializableClass: ServiceSet#test_set_unserializable_value().UnserializableClass#
  TestCacheEntry: Entry#
  TestCacheServiceInit: ServiceInit#
  TestCacheServiceGet: ServiceGet#
  TestCacheServiceSet: ServiceSet#
  TestCacheServiceClear: ServiceClear#
  TestCacheServiceSize: ServiceSize#
  TestCacheServiceStats: ServiceStats#
  TestCacheServiceGenerateKey: ServiceGenerateKey#
  TestCacheServiceInvalidatePattern: ServiceInvalidatePattern#
  TestCacheServiceHierarchical: ServiceHierarchical#
  TestCacheServiceThreadSafety: ServiceThreadSafety#
  TestCacheServiceEdgeCases: ServiceEdgeCases#
---
# Module: [`tests/unit/core/test_cache_service.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py)

## Classes
### `TestCacheEntry`
- def: [`tests/unit/core/test_cache_service.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L18)
- doc: Test cases for CacheEntry dataclass.
- signature: `class TestCacheEntry:`
- members:
  - `test_cache_entry_defaults(self)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L38) — Test CacheEntry with default values.
  - `test_cache_entry_initialization(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L21) — Test CacheEntry initialization.
  - `test_is_expired_future(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L64) — Test is_expired with future expiration.
  - `test_is_expired_with_expiration(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L47) — Test is_expired with expiration time.
  - `test_is_expired_without_expiration(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L56) — Test is_expired without expiration time.
- uses (calls/refs, reference-scoped): [`CacheEntry`](../../../tree_sitter_analyzer/core/cache_service.md#CacheEntry), [`value`](../../../tree_sitter_analyzer/core/cache_service.md#CacheEntry.value), [`expires_at`](../../../tree_sitter_analyzer/core/cache_service.md#CacheEntry.expires_at), [`is_expired`](../../../tree_sitter_analyzer/core/cache_service.md#CacheEntry.is_expired), [`created_at`](../../../tree_sitter_analyzer/core/cache_service.md#CacheEntry.created_at), [`access_count`](../../../tree_sitter_analyzer/core/cache_service.md#CacheEntry.access_count)

### `TestCacheServiceClear`
- def: [`tests/unit/core/test_cache_service.py:240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L240)
- doc: Test cases for cache clear operations.
- signature: `class TestCacheServiceClear:`
- members:
  - `test_clear_all_caches(self)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L244) — Test clearing all caches.
  - `test_clear_resets_stats(self)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L261) — Test that clear resets statistics.
- uses (calls/refs, reference-scoped): [`set`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.set), [`get`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.get), [`CacheService`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService), [`get_stats`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.get_stats), [`clear`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.clear), [`size`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.size)

### `TestCacheServiceEdgeCases`
- def: [`tests/unit/core/test_cache_service.py:550`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L550)
- doc: Test cases for edge cases and error handling.
- signature: `class TestCacheServiceEdgeCases:`
- members:
  - `test_cache_eviction(self)` — [`L581`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L581) — Test cache eviction when size limit is reached.
  - `test_complex_value(self)` — [`L566`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L566) — Test caching a complex nested value.
  - `test_l2_cache_hit_promotes_to_l1(self)` — [`L595`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L595) — Test L2 cache hit promotes entry to L1.
  - `test_l3_cache_hit_promotes_to_l1_and_l2(self)` — [`L612`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L612) — Test L3 cache hit promotes entry to L1 and L2.
  - `test_large_value(self)` — [`L554`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L554) — Test caching a large value.
- uses (calls/refs, reference-scoped): [`set`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.set), [`get`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.get), [`CacheService`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService), [`get_stats`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.get_stats), [`_l1_cache`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService._l1_cache), [`_l2_cache`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService._l2_cache)

### `TestCacheServiceGenerateKey`
- def: [`tests/unit/core/test_cache_service.py:362`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L362)
- doc: Test cases for cache key generation.
- signature: `class TestCacheServiceGenerateKey:`
- members:
  - `test_generate_cache_key_basic(self)` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L365) — Test basic cache key generation.
  - `test_generate_cache_key_consistent(self)` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L376) — Test that same inputs generate same key.
  - `test_generate_cache_key_different_inputs(self)` — [`L389`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L389) — Test that different inputs generate different keys.
- uses (calls/refs, reference-scoped): [`CacheService`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService), [`generate_cache_key`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.generate_cache_key)

### `TestCacheServiceGet`
- def: [`tests/unit/core/test_cache_service.py:114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L114)
- doc: Test cases for cache get operations.
- signature: `class TestCacheServiceGet:`
- members:
  - `test_get_cache_miss(self)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L118) — Test get with cache miss.
  - `test_get_empty_key(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L157) — Test get with empty key.
  - `test_get_expired_entry(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L142) — Test get with expired entry.
  - `test_get_l1_hit(self)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L129) — Test get with L1 cache hit.
  - `test_get_none_key(self)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L165) — Test get with None key.
- uses (calls/refs, reference-scoped): [`get`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.get), [`CacheService`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService), [`get_stats`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.get_stats)

### `TestCacheServiceHierarchical`
- def: [`tests/unit/core/test_cache_service.py:460`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L460)
- doc: Test cases for hierarchical cache behavior.
- signature: `class TestCacheServiceHierarchical:`
- members:
  - `test_cache_promotion_l2_to_l1(self)` — [`L464`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L464) — Test cache promotion from L2 to L1.
  - `test_cache_promotion_l3_to_l2(self)` — [`L482`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L482) — Test cache promotion from L3 to L2.
  - `test_multiple_cache_tiers(self)` — [`L499`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L499) — Test that values are stored in all tiers.
- uses (calls/refs, reference-scoped): [`set`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.set), [`get`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.get), [`CacheService`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService), [`get_stats`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.get_stats)

### `TestCacheServiceInit`
- def: [`tests/unit/core/test_cache_service.py:74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L74)
- doc: Test cases for CacheService initialization.
- signature: `class TestCacheServiceInit:`
- members:
  - `test_cache_service_custom_sizes(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L86) — Test CacheService with custom cache sizes.
  - `test_cache_service_default_initialization(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L77) — Test CacheService with default parameters.
  - `test_cache_service_stats_initialization(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L98) — Test that stats are properly initialized.
- uses (calls/refs, reference-scoped): [`CacheService`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService), [`get_stats`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.get_stats), [`size`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.size)

### `TestCacheServiceInvalidatePattern`
- def: [`tests/unit/core/test_cache_service.py:405`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L405)
- doc: Test cases for pattern-based cache invalidation.
- signature: `class TestCacheServiceInvalidatePattern:`
- members:
  - `test_invalidate_pattern(self)` — [`L409`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L409) — Test invalidating entries by pattern.
  - `test_invalidate_pattern_all(self)` — [`L445`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L445) — Test invalidating all entries with wildcard pattern.
  - `test_invalidate_pattern_no_matches(self)` — [`L433`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L433) — Test invalidating with no matching pattern.
- uses (calls/refs, reference-scoped): [`set`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.set), [`get`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.get), [`CacheService`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService), [`invalidate_pattern`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.invalidate_pattern)

### `TestCacheServiceSet`
- def: [`tests/unit/core/test_cache_service.py:173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L173)
- doc: Test cases for cache set operations.
- signature: `class TestCacheServiceSet:`
- members:
  - `test_set_and_get(self)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L177) — Test basic set and get operations.
  - `test_set_empty_key(self)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L210) — Test set with empty key.
  - `test_set_none_key(self)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L218) — Test set with None key.
  - `test_set_overwrites_existing(self)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L199) — Test that set overwrites existing value.
  - `test_set_unserializable_value(self)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L226) — Test set with unserializable value.
  - `test_set_with_custom_ttl(self)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L189) — Test set with custom TTL.
- uses (calls/refs, reference-scoped): [`set`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.set), [`get`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.get), [`CacheService`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService), [`get_stats`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.get_stats)  (1 test-only)

### `TestCacheServiceSize`
- def: [`tests/unit/core/test_cache_service.py:280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L280)
- doc: Test cases for cache size operations.
- signature: `class TestCacheServiceSize:`
- members:
  - `test_size_empty_cache(self)` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L284) — Test size of empty cache.
  - `test_size_with_entries(self)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L291) — Test size with cache entries.
- uses (calls/refs, reference-scoped): [`set`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.set), [`CacheService`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService), [`size`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.size)

### `TestCacheServiceStats`
- def: [`tests/unit/core/test_cache_service.py:303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L303)
- doc: Test cases for cache statistics.
- signature: `class TestCacheServiceStats:`
- members:
  - `test_get_stats_comprehensive(self)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L307) — Test comprehensive statistics.
  - `test_hit_rate_calculation(self)` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L324) — Test hit rate calculation.
  - `test_hit_rate_no_requests(self)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L341) — Test hit rate with no requests.
  - `test_l1_l2_l3_hit_tracking(self)` — [`L349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L349) — Test tracking of L1, L2, L3 hits.
- uses (calls/refs, reference-scoped): [`set`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.set), [`get`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.get), [`CacheService`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService), [`get_stats`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.get_stats)

### `TestCacheServiceThreadSafety`
- def: [`tests/unit/core/test_cache_service.py:513`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L513)
- doc: Test cases for thread safety.
- signature: `class TestCacheServiceThreadSafety:`
- members:
  - `get_value()` — [`L539`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L539)
  - `set_value(i: int)` — [`L521`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L521)
  - `test_concurrent_gets(self)` — [`L532`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L532) — Test concurrent get operations.
  - `test_concurrent_sets(self)` — [`L517`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L517) — Test concurrent set operations.
- uses (calls/refs, reference-scoped): [`set`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.set), [`get`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.get), [`CacheService`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService), [`get_stats`](../../../tree_sitter_analyzer/core/cache_service.md#CacheService.get_stats)

### `UnserializableClass`
- def: [`tests/unit/core/test_cache_service.py:231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_cache_service.py#L231)
- signature: `class UnserializableClass:`
- used by: (1 test-only callers)

