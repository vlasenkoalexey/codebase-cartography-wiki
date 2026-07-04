---
title: 'Module: tests/unit/core/test_core_search_cache.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_core_search_cache.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_core_search_cache`/TestSearchCache
symbols:
  TestSearchCacheGlobalFunctions.test_global_cache_functions: GlobalFunctions#test_global_cache_functions().
  TestSearchCacheInit.test_cache_initialization: Init#test_cache_initialization().
  TestSearchCacheClear.test_cache_clear: Clear#test_cache_clear().
  TestSearchCacheBasicOperations.test_cache_basic_operations: BasicOperations#test_cache_basic_operations().
  TestSearchCacheLRU.test_cache_lru_eviction: LRU#test_cache_lru_eviction().
  TestSearchCacheStatistics.test_cache_statistics_accuracy: Statistics#test_cache_statistics_accuracy().
  TestSearchCacheFormatCompatibility.test_bug_reproduction_scenario: FormatCompatibility#test_bug_reproduction_scenario().
  TestSearchCacheBasicOperations.test_cache_key_generation: BasicOperations#test_cache_key_generation().
  TestSearchCacheBasicOperations.test_cache_with_path_normalization: BasicOperations#test_cache_with_path_normalization().
  TestSearchCacheTTL.test_cache_ttl_expiration: TTL#test_cache_ttl_expiration().
  TestSearchCacheThreadSafety.test_cache_thread_safety_structure: ThreadSafety#test_cache_thread_safety_structure().
  TestSearchCacheFormatCompatibility.test_total_only_should_not_return_for_detailed_request: FormatCompatibility#test_total_only_should_not_return_for_detailed_request().
  TestSearchCacheFormatCompatibility.test_format_compatibility_validation: FormatCompatibility#test_format_compatibility_validation().
  TestSearchCacheFormatCompatibility.test_correct_format_cache_hit: FormatCompatibility#test_correct_format_cache_hit().
  TestSearchCacheFormatCompatibility.test_cross_format_derivation_still_works: FormatCompatibility#test_cross_format_derivation_still_works().
  TestSearchCacheFormatCompatibility.test_unknown_format_prevents_primitive_return: FormatCompatibility#test_unknown_format_prevents_primitive_return().
  TestSearchCacheInit.clear_cache_between_tests: Init#clear_cache_between_tests().
  TestSearchCacheBasicOperations.clear_cache_between_tests: BasicOperations#clear_cache_between_tests().
  TestSearchCacheTTL.clear_cache_between_tests: TTL#clear_cache_between_tests().
  TestSearchCacheLRU.clear_cache_between_tests: LRU#clear_cache_between_tests().
  TestSearchCacheClear.clear_cache_between_tests: Clear#clear_cache_between_tests().
  TestSearchCacheStatistics.clear_cache_between_tests: Statistics#clear_cache_between_tests().
  TestSearchCacheGlobalFunctions.clear_cache_between_tests: GlobalFunctions#clear_cache_between_tests().
  TestSearchCacheThreadSafety.clear_cache_between_tests: ThreadSafety#clear_cache_between_tests().
  TestSearchCacheFormatCompatibility.clear_cache_between_tests: FormatCompatibility#clear_cache_between_tests().
  TestSearchCacheInit: Init#
  TestSearchCacheBasicOperations: BasicOperations#
  TestSearchCacheTTL: TTL#
  TestSearchCacheLRU: LRU#
  TestSearchCacheClear: Clear#
  TestSearchCacheStatistics: Statistics#
  TestSearchCacheGlobalFunctions: GlobalFunctions#
  TestSearchCacheThreadSafety: ThreadSafety#
  TestSearchCacheFormatCompatibility: FormatCompatibility#
---
# Module: [`tests/unit/core/test_core_search_cache.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py)

## Classes
### `TestSearchCacheBasicOperations`
- def: [`tests/unit/core/test_core_search_cache.py:48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L48)
- doc: SearchCache 基本操作测试
- signature: `class TestSearchCacheBasicOperations:`
- members:
  - `clear_cache_between_tests(self)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L52) — Clear cache before each test to avoid interference
  - `test_cache_basic_operations(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L58) — Test basic cache set/get operations
  - `test_cache_key_generation(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L79) — Test cache key generation
  - `test_cache_with_path_normalization(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L99) — Test cache key generation with path normalization
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`get`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get), [`clear_cache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#clear_cache), [`get_stats`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get_stats), [`create_cache_key`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.create_cache_key)

### `TestSearchCacheClear`
- def: [`tests/unit/core/test_core_search_cache.py:185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L185)
- doc: SearchCache 清除测试
- signature: `class TestSearchCacheClear:`
- members:
  - `clear_cache_between_tests(self)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L189) — Clear cache before each test to avoid interference
  - `test_cache_clear(self)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L195) — Test cache clearing functionality
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`get`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get), [`clear_cache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#clear_cache), [`get_stats`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get_stats), [`clear`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.clear)

### `TestSearchCacheFormatCompatibility`
- def: [`tests/unit/core/test_core_search_cache.py:300`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L300)
- doc: SearchCache 格式兼容性测试 (bug fix tests)
- signature: `class TestSearchCacheFormatCompatibility:`
- members:
  - `clear_cache_between_tests(self)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L304) — Clear cache before each test to avoid interference
  - `test_bug_reproduction_scenario(self)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L412) — Reproduce the exact bug scenario from the roo_task document.
  - `test_correct_format_cache_hit(self)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L356) — Test that correctly formatted cached results are returned.
  - `test_cross_format_derivation_still_works(self)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L374) — Test that cross-format derivation still works after the fix.
  - `test_format_compatibility_validation(self)` — [`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L333) — Test the _is_format_compatible method with various scenarios.
  - `test_total_only_should_not_return_for_detailed_request(self)` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L310) — Test that cached total_only results (integers) are not returned
  - `test_unknown_format_prevents_primitive_return(self)` — [`L449`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L449) — Test that unknown formats prevent primitive data return (the main bug).
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`clear_cache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#clear_cache), [`get_compatible_result`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get_compatible_result), [`_is_format_compatible`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._is_format_compatible), [`create_cache_key`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.create_cache_key)

### `TestSearchCacheGlobalFunctions`
- def: [`tests/unit/core/test_core_search_cache.py:251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L251)
- doc: SearchCache 全局函数测试
- signature: `class TestSearchCacheGlobalFunctions:`
- members:
  - `clear_cache_between_tests(self)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L255) — Clear cache before each test to avoid interference
  - `test_global_cache_functions(self)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L261) — Test global cache configuration functions
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`get`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get), [`clear_cache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#clear_cache), [`get_default_cache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#get_default_cache), [`configure_cache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#configure_cache), [`ttl_seconds`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.ttl_seconds), [`max_size`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.max_size)

### `TestSearchCacheInit`
- def: [`tests/unit/core/test_core_search_cache.py:22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L22)
- doc: SearchCache 初始化测试
- signature: `class TestSearchCacheInit:`
- members:
  - `clear_cache_between_tests(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L26) — Clear cache before each test to avoid interference
  - `test_cache_initialization(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L32) — Test SearchCache initialization
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`clear_cache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#clear_cache), [`get_stats`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get_stats), [`cache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.cache), [`ttl_seconds`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.ttl_seconds), [`max_size`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.max_size)

### `TestSearchCacheLRU`
- def: [`tests/unit/core/test_core_search_cache.py:141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L141)
- doc: SearchCache LRU 驱逐测试
- signature: `class TestSearchCacheLRU:`
- members:
  - `clear_cache_between_tests(self)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L145) — Clear cache before each test to avoid interference
  - `test_cache_lru_eviction(self)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L151) — Test LRU eviction when cache is full
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`get`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get), [`clear_cache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#clear_cache), [`get_stats`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get_stats)

### `TestSearchCacheStatistics`
- def: [`tests/unit/core/test_core_search_cache.py:219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L219)
- doc: SearchCache 统计测试
- signature: `class TestSearchCacheStatistics:`
- members:
  - `clear_cache_between_tests(self)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L223) — Clear cache before each test to avoid interference
  - `test_cache_statistics_accuracy(self)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L229) — Test cache statistics are accurately tracked
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`get`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get), [`clear_cache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#clear_cache), [`get_stats`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get_stats)

### `TestSearchCacheTTL`
- def: [`tests/unit/core/test_core_search_cache.py:112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L112)
- doc: SearchCache TTL 过期测试
- signature: `class TestSearchCacheTTL:`
- members:
  - `clear_cache_between_tests(self)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L116) — Clear cache before each test to avoid interference
  - `test_cache_ttl_expiration(self)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L122) — Test TTL-based cache expiration
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`get`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache.get), [`clear_cache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#clear_cache)

### `TestSearchCacheThreadSafety`
- def: [`tests/unit/core/test_core_search_cache.py:281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L281)
- doc: SearchCache 线程安全测试
- signature: `class TestSearchCacheThreadSafety:`
- members:
  - `clear_cache_between_tests(self)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L285) — Clear cache before each test to avoid interference
  - `test_cache_thread_safety_structure(self)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_core_search_cache.py#L291) — Test that cache has thread safety mechanisms in place
- uses (calls/refs, reference-scoped): [`SearchCache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache), [`clear_cache`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#clear_cache), [`_lock`](../../../tree_sitter_analyzer/mcp/utils/search_cache.md#SearchCache._lock)

