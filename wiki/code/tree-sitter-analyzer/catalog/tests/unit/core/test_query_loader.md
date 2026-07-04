---
title: 'Module: tests/unit/core/test_query_loader.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_query_loader.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_query_loader`/test_
symbols:
  test_refresh_cache: refresh_cache().
  test_get_common_queries: get_common_queries().
  test_empty_language_name: empty_language_name().
  test_caching_behavior: caching_behavior().
  test_list_queries_for_language: list_queries_for_language().
  test_get_all_queries_for_language: get_all_queries_for_language().
  test_convenience_functions: convenience_functions().
  test_none_parameters: none_parameters().
  test_query_loader_instance: query_loader_instance().
  test_list_supported_languages: list_supported_languages().
  test_load_language_queries_java: load_language_queries_java().
  test_load_language_queries_javascript: load_language_queries_javascript().
  test_load_language_queries_python: load_language_queries_python().
  test_load_language_queries_typescript: load_language_queries_typescript().
  test_load_language_queries_unknown: load_language_queries_unknown().
  test_get_query_valid: get_query_valid().
  test_get_query_invalid: get_query_invalid().
  test_get_query_description: get_query_description().
  test_load_language_queries_import_error: load_language_queries_import_error().
  test_load_language_queries_missing_attributes: load_language_queries_missing_attributes().
  test_is_language_supported_function: is_language_supported_function().
---
# Module: [`tests/unit/core/test_query_loader.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py)

## Functions
- `test_caching_behavior()` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L263) — Test that queries are properly cached
- `test_convenience_functions()` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L205) — Test convenience functions
- `test_empty_language_name()` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L249) — Test handling of empty language names
- `test_get_all_queries_for_language()` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L166) — Test getting all queries with descriptions
- `test_get_common_queries()` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L138) — Test getting common queries across languages
- `test_get_query_description()` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L115) — Test getting query descriptions
- `test_get_query_invalid()` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L106) — Test getting an invalid query
- `test_get_query_valid()` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L92) — Test getting a valid query
- `test_is_language_supported_function()` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L157) — Test standalone is_language_supported function
- `test_list_queries_for_language()` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L126) — Test listing queries for specific languages
- `test_list_supported_languages()` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L27) — Test listing supported languages
- `test_load_language_queries_import_error(mocker)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L222) — Test handling of import errors when loading queries
- `test_load_language_queries_java()` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L38) — Test loading Java queries
- `test_load_language_queries_javascript()` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L49) — Test loading JavaScript queries
- `test_load_language_queries_missing_attributes(mocker)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L232) — Test handling when query module lacks expected attributes
- `test_load_language_queries_python()` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L61) — Test loading Python queries
- `test_load_language_queries_typescript()` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L73) — Test loading TypeScript queries
- `test_load_language_queries_unknown()` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L85) — Test loading queries for unknown language
- `test_none_parameters()` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L256) — Test handling of None parameters
- `test_query_loader_instance()` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L21) — Test that query loader instance is properly initialized
- `test_refresh_cache()` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_loader.py#L185) — Test cache refresh functionality

