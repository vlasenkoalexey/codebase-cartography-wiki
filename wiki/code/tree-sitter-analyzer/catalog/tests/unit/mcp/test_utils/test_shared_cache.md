---
title: 'Module: tests/unit/mcp/test_utils/test_shared_cache.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_utils/test_shared_cache.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_utils.test_shared_cache`/
symbols:
  TestCacheClear.test_clear_all_caches: TestCacheClear#test_clear_all_caches().
  TestCacheIsolation.test_caches_are_independent: TestCacheIsolation#test_caches_are_independent().
  TestCacheIsolation.test_same_key_different_cache_types: TestCacheIsolation#test_same_key_different_cache_types().
  TestCachePersistence.test_cache_persists_across_operations: TestCachePersistence#test_cache_persists_across_operations().
  TestCacheClear.test_clear_preserves_singleton: TestCacheClear#test_clear_preserves_singleton().
  TestSharedCacheSingleton.test_initialization_called_once: TestSharedCacheSingleton#test_initialization_called_once().
  TestLanguageCache.test_set_and_get_language: TestLanguageCache#test_set_and_get_language().
  TestLanguageCache.test_set_language_overwrites: TestLanguageCache#test_set_language_overwrites().
  TestLanguageCache.test_language_cache_with_project_root: TestLanguageCache#test_language_cache_with_project_root().
  TestLanguageCache.test_language_cache_different_roots: TestLanguageCache#test_language_cache_different_roots().
  TestLanguageMetaCache.test_set_and_get_language_meta: TestLanguageMetaCache#test_set_and_get_language_meta().
  TestLanguageMetaCache.test_set_language_meta_overwrites: TestLanguageMetaCache#test_set_language_meta_overwrites().
  TestLanguageMetaCache.test_language_meta_cache_with_project_root: TestLanguageMetaCache#test_language_meta_cache_with_project_root().
  TestSecurityCache.test_set_and_get_security: TestSecurityCache#test_set_and_get_security().
  TestSecurityCache.test_set_security_overwrites: TestSecurityCache#test_set_security_overwrites().
  TestSecurityCache.test_security_cache_with_project_root: TestSecurityCache#test_security_cache_with_project_root().
  TestMetricsCache.test_set_and_get_metrics: TestMetricsCache#test_set_and_get_metrics().
  TestMetricsCache.test_set_metrics_overwrites: TestMetricsCache#test_set_metrics_overwrites().
  TestMetricsCache.test_metrics_cache_with_project_root: TestMetricsCache#test_metrics_cache_with_project_root().
  TestResolvedPathCache.test_set_and_get_resolved_path: TestResolvedPathCache#test_set_and_get_resolved_path().
  TestResolvedPathCache.test_set_resolved_path_overwrites: TestResolvedPathCache#test_set_resolved_path_overwrites().
  TestResolvedPathCache.test_resolved_path_cache_with_project_root: TestResolvedPathCache#test_resolved_path_cache_with_project_root().
  TestCacheWithSpecialCharacters.test_cache_key_with_spaces: TestCacheWithSpecialCharacters#test_cache_key_with_spaces().
  TestCacheWithSpecialCharacters.test_cache_key_with_special_chars: TestCacheWithSpecialCharacters#test_cache_key_with_special_chars().
  TestCacheWithSpecialCharacters.test_cache_key_with_unicode: TestCacheWithSpecialCharacters#test_cache_key_with_unicode().
  TestCacheEdgeCases.test_empty_string_key: TestCacheEdgeCases#test_empty_string_key().
  TestCacheEdgeCases.test_none_value: TestCacheEdgeCases#test_none_value().
  TestCacheEdgeCases.test_complex_dict_value: TestCacheEdgeCases#test_complex_dict_value().
  TestCacheEdgeCases.test_very_long_key: TestCacheEdgeCases#test_very_long_key().
  TestCacheEdgeCases.test_very_long_value: TestCacheEdgeCases#test_very_long_value().
  TestCachePersistence.test_multiple_sets_same_key: TestCachePersistence#test_multiple_sets_same_key().
  TestCacheThreadSafety.test_concurrent_sets_same_key: TestCacheThreadSafety#test_concurrent_sets_same_key().
  TestCacheThreadSafety.test_concurrent_different_keys: TestCacheThreadSafety#test_concurrent_different_keys().
  clear_shared_cache: clear_shared_cache().
  TestSharedCacheSingleton.test_get_shared_cache_returns_instance: TestSharedCacheSingleton#test_get_shared_cache_returns_instance().
  TestCacheKeyGeneration.test_make_key_with_project_root: TestCacheKeyGeneration#test_make_key_with_project_root().
  TestCacheKeyGeneration.test_make_key_without_project_root: TestCacheKeyGeneration#test_make_key_without_project_root().
  TestCacheKeyGeneration.test_make_key_consistent: TestCacheKeyGeneration#test_make_key_consistent().
  TestCacheKeyGeneration.test_make_key_differentiates_kinds: TestCacheKeyGeneration#test_make_key_differentiates_kinds().
  TestCacheKeyGeneration.test_make_key_differentiates_paths: TestCacheKeyGeneration#test_make_key_differentiates_paths().
  TestLanguageCache.test_get_language_not_set: TestLanguageCache#test_get_language_not_set().
  TestLanguageMetaCache.test_get_language_meta_not_set: TestLanguageMetaCache#test_get_language_meta_not_set().
  TestSecurityCache.test_get_security_not_set: TestSecurityCache#test_get_security_not_set().
  TestMetricsCache.test_get_metrics_not_set: TestMetricsCache#test_get_metrics_not_set().
  TestResolvedPathCache.test_get_resolved_path_not_set: TestResolvedPathCache#test_get_resolved_path_not_set().
  TestCacheThreadSafety.set_value: TestCacheThreadSafety#set_value().
  TestSharedCacheSingleton.test_singleton_returns_same_instance: TestSharedCacheSingleton#test_singleton_returns_same_instance().
  TestSharedCacheSingleton.test_get_shared_cache_singleton: TestSharedCacheSingleton#test_get_shared_cache_singleton().
  TestSharedCacheSingleton.test_multiple_instantiations_same_instance: TestSharedCacheSingleton#test_multiple_instantiations_same_instance().
  TestSharedCacheSingleton: TestSharedCacheSingleton#
  TestCacheKeyGeneration: TestCacheKeyGeneration#
  TestLanguageCache: TestLanguageCache#
  TestLanguageMetaCache: TestLanguageMetaCache#
  TestSecurityCache: TestSecurityCache#
  TestMetricsCache: TestMetricsCache#
  TestResolvedPathCache: TestResolvedPathCache#
  TestCacheClear: TestCacheClear#
  TestCacheIsolation: TestCacheIsolation#
  TestCacheWithSpecialCharacters: TestCacheWithSpecialCharacters#
  TestCacheEdgeCases: TestCacheEdgeCases#
  TestCachePersistence: TestCachePersistence#
  TestCacheThreadSafety: TestCacheThreadSafety#
---
# Module: [`tests/unit/mcp/test_utils/test_shared_cache.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py)

## Classes
### `TestCacheClear`
- def: [`tests/unit/mcp/test_utils/test_shared_cache.py:300`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L300)
- doc: Tests for cache clearing.
- signature: `class TestCacheClear:`
- members:
  - `test_clear_all_caches(self)` — [`L303`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L303) — Test that clear removes all cached data.
  - `test_clear_preserves_singleton(self)` — [`L331`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L331) — Test that clear preserves singleton instance.
- uses (calls/refs, reference-scoped): [`SharedCache`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache), [`get_language`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_language), [`set_language`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_language), [`get_security_validation`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_security_validation), [`get_language_meta`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_language_meta), [`get_metrics`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_metrics), [`set_security_validation`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_security_validation), [`clear`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.clear), [`set_metrics`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_metrics), [`get_resolved_path`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_resolved_path), [`set_language_meta`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_language_meta), [`set_resolved_path`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_resolved_path)

### `TestCacheEdgeCases`
- def: [`tests/unit/mcp/test_utils/test_shared_cache.py:403`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L403)
- doc: Tests for edge cases.
- signature: `class TestCacheEdgeCases:`
- members:
  - `test_complex_dict_value(self)` — [`L420`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L420) — Test cache with complex nested dict value.
  - `test_empty_string_key(self)` — [`L406`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L406) — Test cache with empty string key.
  - `test_none_value(self)` — [`L413`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L413) — Test cache with None value.
  - `test_very_long_key(self)` — [`L433`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L433) — Test cache with very long key.
  - `test_very_long_value(self)` — [`L441`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L441) — Test cache with very long value.
- uses (calls/refs, reference-scoped): [`SharedCache`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache), [`get_language`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_language), [`set_language`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_language), [`get_language_meta`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_language_meta), [`set_language_meta`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_language_meta)

### `TestCacheIsolation`
- def: [`tests/unit/mcp/test_utils/test_shared_cache.py:344`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L344)
- doc: Tests for cache isolation between different cache types.
- signature: `class TestCacheIsolation:`
- members:
  - `test_caches_are_independent(self)` — [`L347`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L347) — Test that different cache types don't interfere.
  - `test_same_key_different_cache_types(self)` — [`L364`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L364) — Test that same key in different cache types works correctly.
- uses (calls/refs, reference-scoped): [`SharedCache`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache), [`get_language`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_language), [`set_language`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_language), [`get_security_validation`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_security_validation), [`get_language_meta`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_language_meta), [`get_metrics`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_metrics), [`set_security_validation`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_security_validation), [`set_metrics`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_metrics), [`get_resolved_path`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_resolved_path), [`set_language_meta`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_language_meta), [`set_resolved_path`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_resolved_path)

### `TestCacheKeyGeneration`
- def: [`tests/unit/mcp/test_utils/test_shared_cache.py:63`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L63)
- doc: Tests for cache key generation.
- signature: `class TestCacheKeyGeneration:`
- members:
  - `test_make_key_consistent(self)` — [`L83`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L83) — Test that same parameters produce same key.
  - `test_make_key_differentiates_kinds(self)` — [`L90`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L90) — Test that different cache kinds produce different keys.
  - `test_make_key_differentiates_paths(self)` — [`L97`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L97) — Test that different paths produce different keys.
  - `test_make_key_with_project_root(self)` — [`L66`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L66) — Test key generation with project root.
  - `test_make_key_without_project_root(self)` — [`L74`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L74) — Test key generation without project root.
- uses (calls/refs, reference-scoped): [`SharedCache`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache), [`_make_key`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache._make_key)

### `TestCachePersistence`
- def: [`tests/unit/mcp/test_utils/test_shared_cache.py:450`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L450)
- doc: Tests for cache persistence across operations.
- signature: `class TestCachePersistence:`
- members:
  - `test_cache_persists_across_operations(self)` — [`L453`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L453) — Test that cache persists across multiple operations.
  - `test_multiple_sets_same_key(self)` — [`L466`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L466) — Test that multiple sets to same key work correctly.
- uses (calls/refs, reference-scoped): [`SharedCache`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache), [`get_language`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_language), [`set_language`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_language), [`get_metrics`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_metrics), [`set_metrics`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_metrics)

### `TestCacheThreadSafety`
- def: [`tests/unit/mcp/test_utils/test_shared_cache.py:478`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L478)
- doc: Tests for thread-safe cache operations.
- signature: `class TestCacheThreadSafety:`
- members:
  - `set_value(value)` — [`L488`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L488)
  - `test_concurrent_different_keys(self)` — [`L504`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L504) — Test concurrent sets to different keys.
  - `test_concurrent_sets_same_key(self)` — [`L481`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L481) — Test concurrent sets to same key.
- uses (calls/refs, reference-scoped): [`SharedCache`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache), [`get_language`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_language), [`set_language`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_language)

### `TestCacheWithSpecialCharacters`
- def: [`tests/unit/mcp/test_utils/test_shared_cache.py:376`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L376)
- doc: Tests for cache with special characters in keys.
- signature: `class TestCacheWithSpecialCharacters:`
- members:
  - `test_cache_key_with_spaces(self)` — [`L379`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L379) — Test cache with spaces in file path.
  - `test_cache_key_with_special_chars(self)` — [`L386`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L386) — Test cache with special characters in file path.
  - `test_cache_key_with_unicode(self)` — [`L394`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L394) — Test cache with unicode characters.
- uses (calls/refs, reference-scoped): [`SharedCache`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache), [`get_language`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_language), [`set_language`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_language)

### `TestLanguageCache`
- def: [`tests/unit/mcp/test_utils/test_shared_cache.py:105`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L105)
- doc: Tests for language detection cache.
- signature: `class TestLanguageCache:`
- members:
  - `test_get_language_not_set(self)` — [`L115`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L115) — Test getting language that was not set.
  - `test_language_cache_different_roots(self)` — [`L136`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L136) — Test that different project roots create separate caches.
  - `test_language_cache_with_project_root(self)` — [`L129`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L129) — Test language cache with project root.
  - `test_set_and_get_language(self)` — [`L108`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L108) — Test setting and getting language.
  - `test_set_language_overwrites(self)` — [`L121`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L121) — Test that set_language overwrites existing value.
- uses (calls/refs, reference-scoped): [`SharedCache`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache), [`get_language`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_language), [`set_language`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_language)

### `TestLanguageMetaCache`
- def: [`tests/unit/mcp/test_utils/test_shared_cache.py:149`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L149)
- doc: Tests for language metadata cache.
- signature: `class TestLanguageMetaCache:`
- members:
  - `test_get_language_meta_not_set(self)` — [`L160`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L160) — Test getting metadata that was not set.
  - `test_language_meta_cache_with_project_root(self)` — [`L178`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L178) — Test language metadata cache with project root.
  - `test_set_and_get_language_meta(self)` — [`L152`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L152) — Test setting and getting language metadata.
  - `test_set_language_meta_overwrites(self)` — [`L166`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L166) — Test that set_language_meta overwrites existing value.
- uses (calls/refs, reference-scoped): [`SharedCache`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache), [`get_language_meta`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_language_meta), [`set_language_meta`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_language_meta)

### `TestMetricsCache`
- def: [`tests/unit/mcp/test_utils/test_shared_cache.py:225`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L225)
- doc: Tests for metrics cache.
- signature: `class TestMetricsCache:`
- members:
  - `test_get_metrics_not_set(self)` — [`L236`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L236) — Test getting metrics that was not set.
  - `test_metrics_cache_with_project_root(self)` — [`L254`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L254) — Test metrics cache with project root.
  - `test_set_and_get_metrics(self)` — [`L228`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L228) — Test setting and getting metrics.
  - `test_set_metrics_overwrites(self)` — [`L242`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L242) — Test that set_metrics overwrites existing value.
- uses (calls/refs, reference-scoped): [`SharedCache`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache), [`get_metrics`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_metrics), [`set_metrics`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_metrics)

### `TestResolvedPathCache`
- def: [`tests/unit/mcp/test_utils/test_shared_cache.py:263`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L263)
- doc: Tests for resolved path cache.
- signature: `class TestResolvedPathCache:`
- members:
  - `test_get_resolved_path_not_set(self)` — [`L273`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L273) — Test getting resolved path that was not set.
  - `test_resolved_path_cache_with_project_root(self)` — [`L291`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L291) — Test resolved path cache with project root.
  - `test_set_and_get_resolved_path(self)` — [`L266`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L266) — Test setting and getting resolved path.
  - `test_set_resolved_path_overwrites(self)` — [`L279`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L279) — Test that set_resolved_path overwrites existing value.
- uses (calls/refs, reference-scoped): [`SharedCache`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache), [`get_resolved_path`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_resolved_path), [`set_resolved_path`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_resolved_path)

### `TestSecurityCache`
- def: [`tests/unit/mcp/test_utils/test_shared_cache.py:187`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L187)
- doc: Tests for security validation cache.
- signature: `class TestSecurityCache:`
- members:
  - `test_get_security_not_set(self)` — [`L198`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L198) — Test getting security that was not set.
  - `test_security_cache_with_project_root(self)` — [`L216`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L216) — Test security cache with project root.
  - `test_set_and_get_security(self)` — [`L190`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L190) — Test setting and getting security validation.
  - `test_set_security_overwrites(self)` — [`L204`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L204) — Test that set_security overwrites existing value.
- uses (calls/refs, reference-scoped): [`SharedCache`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache), [`get_security_validation`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_security_validation), [`set_security_validation`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_security_validation)

### `TestSharedCacheSingleton`
- def: [`tests/unit/mcp/test_utils/test_shared_cache.py:26`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L26)
- doc: Tests for SharedCache singleton pattern.
- signature: `class TestSharedCacheSingleton:`
- members:
  - `test_get_shared_cache_returns_instance(self)` — [`L35`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L35) — Test that get_shared_cache returns SharedCache instance.
  - `test_get_shared_cache_singleton(self)` — [`L40`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L40) — Test that get_shared_cache returns singleton.
  - `test_initialization_called_once(self)` — [`L53`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L53) — Test that initialization is called only once.
  - `test_multiple_instantiations_same_instance(self)` — [`L46`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L46) — Test that multiple instantiations return same instance.
  - `test_singleton_returns_same_instance(self)` — [`L29`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L29) — Test that singleton returns the same instance.
- uses (calls/refs, reference-scoped): [`SharedCache`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache), [`get_shared_cache`](../../../../tree_sitter_analyzer/_shared_cache.md#get_shared_cache), [`get_language`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.get_language), [`set_language`](../../../../tree_sitter_analyzer/_shared_cache.md#SharedCache.set_language)

## Functions
- `clear_shared_cache()` — [`L18`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_shared_cache.py#L18) — Fixture to clear shared cache before each test.

