---
title: 'Module: tests/unit/core/test_query_loader_coverage_supplement.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_query_loader_coverage_supplement.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_query_loader_coverage_supplement`/TestQueryLoaderUncovered#
symbols:
  TestQueryLoaderUncovered.test_refresh_cache_clears_all: test_refresh_cache_clears_all().
  TestQueryLoaderUncovered.test_load_language_queries_failed_language_returns_empty: test_load_language_queries_failed_language_returns_empty().
  TestQueryLoaderUncovered.test_load_language_queries_cache_hit: test_load_language_queries_cache_hit().
  TestQueryLoaderUncovered.test_load_language_queries_generic_exception: test_load_language_queries_generic_exception().
  TestQueryLoaderUncovered.test_get_all_queries_for_language_with_dict_entries: test_get_all_queries_for_language_with_dict_entries().
  TestQueryLoaderUncovered.test_is_language_supported_failed_returns_false: test_is_language_supported_failed_returns_false().
  TestQueryLoaderUncovered.test_load_language_queries_import_error_fallback: test_load_language_queries_import_error_fallback().
  TestQueryLoaderUncovered.test_load_language_queries_module_with_get_all_queries: test_load_language_queries_module_with_get_all_queries().
  TestQueryLoaderUncovered.test_load_language_queries_module_with_ALL_QUERIES: test_load_language_queries_module_with_ALL_QUERIES().
  TestQueryLoaderUncovered.test_load_language_queries_directory_fallback: test_load_language_queries_directory_fallback().
  TestQueryLoaderUncovered.test_is_language_supported_unknown_returns_false: test_is_language_supported_unknown_returns_false().
  TestQueryLoaderUncovered.test_preload_languages_mixed: test_preload_languages_mixed().
  TestQueryLoaderUncovered.test_preload_languages_exception_handling: test_preload_languages_exception_handling().
  TestQueryLoaderUncovered: ''
---
# Module: [`tests/unit/core/test_query_loader_coverage_supplement.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader_coverage_supplement.py)

## Classes
### `TestQueryLoaderUncovered`
- def: [`tests/unit/core/test_query_loader_coverage_supplement.py:9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader_coverage_supplement.py#L9)
- doc: Targets: lines 67, 81-91, 101-105, 178-184, 209-224, 229-236
- signature: `class TestQueryLoaderUncovered:`
- members:
  - `test_get_all_queries_for_language_with_dict_entries(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader_coverage_supplement.py#L78) — Lines 199-212: get_all_queries_for_language with dict query_info.
  - `test_is_language_supported_failed_returns_false(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader_coverage_supplement.py#L100) — Lines 223-224: _failed_languages returns False.
  - `test_is_language_supported_unknown_returns_false(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader_coverage_supplement.py#L106) — Line 225: unknown language returns False.
  - `test_load_language_queries_cache_hit(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader_coverage_supplement.py#L19) — Lines 69-70: _loaded_queries cache hit.
  - `test_load_language_queries_directory_fallback(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader_coverage_supplement.py#L64) — Lines 83-91: dir() fallback with string/dict attributes.
  - `test_load_language_queries_failed_language_returns_empty(self)` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader_coverage_supplement.py#L12) — Line 67: _failed_languages cache hit returns {}.
  - `test_load_language_queries_generic_exception(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader_coverage_supplement.py#L34) — Lines 101-105: generic Exception handling.
  - `test_load_language_queries_import_error_fallback(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader_coverage_supplement.py#L26) — Lines 97-100: ImportError fallback.
  - `test_load_language_queries_module_with_ALL_QUERIES(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader_coverage_supplement.py#L53) — Lines 81-82: module with ALL_QUERIES dict.
  - `test_load_language_queries_module_with_get_all_queries(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader_coverage_supplement.py#L42) — Lines 79-80: module with get_all_queries().
  - `test_preload_languages_exception_handling(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader_coverage_supplement.py#L123) — Line 233-234: exception during preload.
  - `test_preload_languages_mixed(self)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader_coverage_supplement.py#L111) — Lines 229-236: preload_languages with mixed success/failure.
  - `test_refresh_cache_clears_all(self)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader_coverage_supplement.py#L89) — Lines 216-219: refresh_cache().
- uses (calls/refs, reference-scoped): [`load_language_queries`](../../../tree_sitter_analyzer/query_loader.md#QueryLoader.load_language_queries), [`QueryLoader`](../../../tree_sitter_analyzer/query_loader.md#QueryLoader), [`_loaded_queries`](../../../tree_sitter_analyzer/query_loader.md#QueryLoader._loaded_queries), [`is_language_supported`](../../../tree_sitter_analyzer/query_loader.md#QueryLoader.is_language_supported), [`refresh_cache`](../../../tree_sitter_analyzer/query_loader.md#QueryLoader.refresh_cache), [`_failed_languages`](../../../tree_sitter_analyzer/query_loader.md#QueryLoader._failed_languages), [`get_all_queries_for_language`](../../../tree_sitter_analyzer/query_loader.md#QueryLoader.get_all_queries_for_language), [`_query_modules`](../../../tree_sitter_analyzer/query_loader.md#QueryLoader._query_modules), [`preload_languages`](../../../tree_sitter_analyzer/query_loader.md#QueryLoader.preload_languages)

