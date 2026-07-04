---
title: 'Module: tests/unit/core/test_query_service.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_query_service.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_query_service`/
symbols:
  TestQueryServiceInit.test_query_service_init_default: TestQueryServiceInit#test_query_service_init_default().
  TestQueryServiceInit.test_query_service_init_with_project_root: TestQueryServiceInit#test_query_service_init_with_project_root().
  TestQueryServiceNoLanguageObject.test_execute_query_no_language_obj: TestQueryServiceNoLanguageObject#test_execute_query_no_language_obj().
  TestQueryServiceQueryExceptionFallback.test_execute_query_query_exception_uses_plugin_fallback: TestQueryServiceQueryExceptionFallback#test_execute_query_query_exception_uses_plugin_fallback().
  TestQueryServiceQueryExceptionFallback.test_execute_query_empty_captures_uses_plugin_fallback: TestQueryServiceQueryExceptionFallback#test_execute_query_empty_captures_uses_plugin_fallback().
  TestQueryServicePluginQueryInternalPaths.test_plugin_query_with_elements_having_line_info: TestQueryServicePluginQueryInternalPaths#test_plugin_query_with_elements_having_line_info().
  TestQueryServicePluginQueryInternalPaths.test_plugin_query_strategy_exception_falls_to_categories: TestQueryServicePluginQueryInternalPaths#test_plugin_query_strategy_exception_falls_to_categories().
  TestQueryServicePluginQueryInternalPaths.test_plugin_query_categories_exception_falls_to_fallback: TestQueryServicePluginQueryInternalPaths#test_plugin_query_categories_exception_falls_to_fallback().
  TestQueryServicePluginQueryInternalPaths.test_plugin_query_no_matching_key_in_categories: TestQueryServicePluginQueryInternalPaths#test_plugin_query_no_matching_key_in_categories().
  TestQueryServiceExecuteQuery.test_execute_query_with_query_key: TestQueryServiceExecuteQuery#test_execute_query_with_query_key().
  TestQueryServiceExecuteQuery.test_execute_query_with_query_string: TestQueryServiceExecuteQuery#test_execute_query_with_query_string().
  TestQueryServiceExecuteQuery.test_execute_query_with_filter: TestQueryServiceExecuteQuery#test_execute_query_with_filter().
  TestQueryServiceExecuteQuery.test_execute_query_no_query_params: TestQueryServiceExecuteQuery#test_execute_query_no_query_params().
  TestQueryServiceExecuteQuery.test_execute_query_both_query_params: TestQueryServiceExecuteQuery#test_execute_query_both_query_params().
  TestQueryServiceExecuteQuery.test_execute_query_invalid_query_key: TestQueryServiceExecuteQuery#test_execute_query_invalid_query_key().
  TestQueryServiceExecuteQuery.test_execute_query_file_not_found: TestQueryServiceExecuteQuery#test_execute_query_file_not_found().
  TestQueryServiceCreateResultDict.test_create_result_dict: TestQueryServiceCreateResultDict#test_create_result_dict().
  TestQueryServiceCreateResultDict.test_create_result_dict_with_source_code: TestQueryServiceCreateResultDict#test_create_result_dict_with_source_code().
  TestQueryServiceGetAvailableQueries.test_get_available_queries: TestQueryServiceGetAvailableQueries#test_get_available_queries().
  TestQueryServiceGetAvailableQueries.test_get_available_queries_unsupported_language: TestQueryServiceGetAvailableQueries#test_get_available_queries_unsupported_language().
  TestQueryServiceGetQueryDescription.test_get_query_description: TestQueryServiceGetQueryDescription#test_get_query_description().
  TestQueryServiceGetQueryDescription.test_get_query_description_invalid_query: TestQueryServiceGetQueryDescription#test_get_query_description_invalid_query().
  TestQueryServiceExecutePluginQuery.test_execute_plugin_query_with_plugin: TestQueryServiceExecutePluginQuery#test_execute_plugin_query_with_plugin().
  TestQueryServiceExecutePluginQuery.test_execute_plugin_query_without_plugin: TestQueryServiceExecutePluginQuery#test_execute_plugin_query_without_plugin().
  TestQueryServiceFallbackQueryExecution.test_fallback_query_execution_function: TestQueryServiceFallbackQueryExecution#test_fallback_query_execution_function().
  TestQueryServiceFallbackQueryExecution.test_fallback_query_execution_class: TestQueryServiceFallbackQueryExecution#test_fallback_query_execution_class().
  TestQueryServiceFallbackQueryExecution.test_fallback_query_execution_no_matches: TestQueryServiceFallbackQueryExecution#test_fallback_query_execution_no_matches().
  TestQueryServiceReadFileAsync.test_read_file_async: TestQueryServiceReadFileAsync#test_read_file_async().
  TestQueryServiceEdgeCases.test_execute_query_empty_results: TestQueryServiceEdgeCases#test_execute_query_empty_results().
  TestQueryServiceEdgeCases.test_create_result_dict_missing_attributes: TestQueryServiceEdgeCases#test_create_result_dict_missing_attributes().
  TestQueryServiceGetQueryDescriptionException.test_get_query_description_exception_returns_none: TestQueryServiceGetQueryDescriptionException#test_get_query_description_exception_returns_none().
  TestQueryServiceFallbackAdditionalPaths.test_fallback_method: TestQueryServiceFallbackAdditionalPaths#test_fallback_method().
  TestQueryServiceFallbackAdditionalPaths.test_fallback_variable: TestQueryServiceFallbackAdditionalPaths#test_fallback_variable().
  TestQueryServiceFallbackAdditionalPaths.test_fallback_import: TestQueryServiceFallbackAdditionalPaths#test_fallback_import().
  TestQueryServiceFallbackAdditionalPaths.test_fallback_header: TestQueryServiceFallbackAdditionalPaths#test_fallback_header().
  TestQueryServiceFallbackAdditionalPaths.test_fallback_plural_forms: TestQueryServiceFallbackAdditionalPaths#test_fallback_plural_forms().
  TestQueryServiceFallbackAdditionalPaths.test_fallback_none_query_key: TestQueryServiceFallbackAdditionalPaths#test_fallback_none_query_key().
  query_service: query_service().
  TestQueryServiceInit: TestQueryServiceInit#
  TestQueryServiceExecuteQuery: TestQueryServiceExecuteQuery#
  TestQueryServiceCreateResultDict: TestQueryServiceCreateResultDict#
  TestQueryServiceGetAvailableQueries: TestQueryServiceGetAvailableQueries#
  TestQueryServiceGetQueryDescription: TestQueryServiceGetQueryDescription#
  TestQueryServiceExecutePluginQuery: TestQueryServiceExecutePluginQuery#
  TestQueryServiceFallbackQueryExecution: TestQueryServiceFallbackQueryExecution#
  TestQueryServiceReadFileAsync: TestQueryServiceReadFileAsync#
  TestQueryServiceEdgeCases: TestQueryServiceEdgeCases#
  TestQueryServiceNoLanguageObject: TestQueryServiceNoLanguageObject#
  TestQueryServiceQueryExceptionFallback: TestQueryServiceQueryExceptionFallback#
  TestQueryServiceGetQueryDescriptionException: TestQueryServiceGetQueryDescriptionException#
  TestQueryServicePluginQueryInternalPaths: TestQueryServicePluginQueryInternalPaths#
  TestQueryServiceFallbackAdditionalPaths: TestQueryServiceFallbackAdditionalPaths#
  temp_file: temp_file().
---
# Module: [`tests/unit/core/test_query_service.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py)

## Classes
### `TestQueryServiceCreateResultDict`
- def: [`tests/unit/core/test_query_service.py:120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L120)
- doc: Tests for QueryService._create_result_dict method.
- signature: `class TestQueryServiceCreateResultDict:`
- members:
  - `test_create_result_dict(self, query_service: QueryService)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L123) — Test creating result dictionary from node.
  - `test_create_result_dict_with_source_code(self, query_service: QueryService)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L144) — Test creating result dictionary with source code.
- uses (calls/refs, reference-scoped): [`QueryService`](../../../tree_sitter_analyzer/core/query_service.md#QueryService), [`_create_result_dict`](../../../tree_sitter_analyzer/core/query_service.md#QueryService._create_result_dict)

### `TestQueryServiceEdgeCases`
- def: [`tests/unit/core/test_query_service.py:299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L299)
- doc: Tests for edge cases and error handling.
- signature: `class TestQueryServiceEdgeCases:`
- members:
  - `test_create_result_dict_missing_attributes(self, query_service: QueryService)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L314) — Test creating result dict with node missing attributes.
  - `test_execute_query_empty_results(self, query_service: QueryService, temp_file: Path)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L303) — Test executing query that returns no results.
- uses (calls/refs, reference-scoped): [`QueryService`](../../../tree_sitter_analyzer/core/query_service.md#QueryService), [`execute_query`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.execute_query), [`_create_result_dict`](../../../tree_sitter_analyzer/core/query_service.md#QueryService._create_result_dict)

### `TestQueryServiceExecutePluginQuery`
- def: [`tests/unit/core/test_query_service.py:197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L197)
- doc: Tests for QueryService._execute_plugin_query method.
- signature: `class TestQueryServiceExecutePluginQuery:`
- members:
  - `test_execute_plugin_query_with_plugin(self, query_service: QueryService)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L200) — Test executing plugin query with available plugin.
  - `test_execute_plugin_query_without_plugin(self, query_service: QueryService)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L212) — Test executing plugin query without available plugin.
- uses (calls/refs, reference-scoped): [`QueryService`](../../../tree_sitter_analyzer/core/query_service.md#QueryService), [`_execute_plugin_query`](../../../tree_sitter_analyzer/core/query_service.md#QueryService._execute_plugin_query)

### `TestQueryServiceExecuteQuery`
- def: [`tests/unit/core/test_query_service.py:36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L36)
- doc: Tests for QueryService.execute_query method.
- signature: `class TestQueryServiceExecuteQuery:`
- members:
  - `test_execute_query_both_query_params(self, query_service: QueryService, temp_file: Path)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L85) — Test executing query with both query_key and query_string raises ValueError.
  - `test_execute_query_file_not_found(self, query_service: QueryService)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L110) — Test executing query on non-existent file raises FileNotFoundError.
  - `test_execute_query_invalid_query_key(self, query_service: QueryService, temp_file: Path)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L100) — Test executing query with invalid query_key raises ValueError.
  - `test_execute_query_no_query_params(self, query_service: QueryService, temp_file: Path)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L75) — Test executing query without query parameters raises ValueError.
  - `test_execute_query_with_filter(self, query_service: QueryService, temp_file: Path)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L62) — Test executing query with filter expression.
  - `test_execute_query_with_query_key(self, query_service: QueryService, temp_file: Path)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L40) — Test executing query with query_key.
  - `test_execute_query_with_query_string(self, query_service: QueryService, temp_file: Path)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L50) — Test executing query with custom query_string.
- uses (calls/refs, reference-scoped): [`QueryService`](../../../tree_sitter_analyzer/core/query_service.md#QueryService), [`execute_query`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.execute_query)

### `TestQueryServiceFallbackAdditionalPaths`
- def: [`tests/unit/core/test_query_service.py:547`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L547)
- doc: Additional tests for _fallback_query_execution to cover missing branches.
- signature: `class TestQueryServiceFallbackAdditionalPaths:`
- members:
  - `test_fallback_header(self)` — [`L586`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L586) — Test fallback for heading nodes.
  - `test_fallback_import(self)` — [`L574`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L574) — Test fallback for import nodes.
  - `test_fallback_method(self)` — [`L550`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L550) — Test fallback for method nodes.
  - `test_fallback_none_query_key(self)` — [`L629`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L629) — Test fallback with None query_key returns empty list.
  - `test_fallback_plural_forms(self)` — [`L598`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L598) — Test fallback for plural query keys (functions, classes, methods, variables, imports, headers).
  - `test_fallback_variable(self)` — [`L562`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L562) — Test fallback for variable nodes.
- uses (calls/refs, reference-scoped): [`QueryService`](../../../tree_sitter_analyzer/core/query_service.md#QueryService), [`_fallback_query_execution`](../../../tree_sitter_analyzer/core/query_service.md#QueryService._fallback_query_execution)

### `TestQueryServiceFallbackQueryExecution`
- def: [`tests/unit/core/test_query_service.py:225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L225)
- doc: Tests for QueryService._fallback_query_execution method.
- signature: `class TestQueryServiceFallbackQueryExecution:`
- members:
  - `test_fallback_query_execution_class(self, query_service: QueryService)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L248) — Test fallback query execution for class nodes.
  - `test_fallback_query_execution_function(self, query_service: QueryService)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L228) — Test fallback query execution for function nodes.
  - `test_fallback_query_execution_no_matches(self, query_service: QueryService)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L265) — Test fallback query execution with no matches.
- uses (calls/refs, reference-scoped): [`QueryService`](../../../tree_sitter_analyzer/core/query_service.md#QueryService), [`_fallback_query_execution`](../../../tree_sitter_analyzer/core/query_service.md#QueryService._fallback_query_execution)

### `TestQueryServiceGetAvailableQueries`
- def: [`tests/unit/core/test_query_service.py:164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L164)
- doc: Tests for QueryService.get_available_queries method.
- signature: `class TestQueryServiceGetAvailableQueries:`
- members:
  - `test_get_available_queries(self, query_service: QueryService)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L167) — Test getting available queries for language.
  - `test_get_available_queries_unsupported_language(self, query_service: QueryService)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L173) — Test getting available queries for unsupported language.
- uses (calls/refs, reference-scoped): [`QueryService`](../../../tree_sitter_analyzer/core/query_service.md#QueryService), [`get_available_queries`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.get_available_queries)

### `TestQueryServiceGetQueryDescription`
- def: [`tests/unit/core/test_query_service.py:181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L181)
- doc: Tests for QueryService.get_query_description method.
- signature: `class TestQueryServiceGetQueryDescription:`
- members:
  - `test_get_query_description(self, query_service: QueryService)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L184) — Test getting query description.
  - `test_get_query_description_invalid_query(self, query_service: QueryService)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L189) — Test getting description for invalid query.
- uses (calls/refs, reference-scoped): [`QueryService`](../../../tree_sitter_analyzer/core/query_service.md#QueryService), [`get_query_description`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.get_query_description)

### `TestQueryServiceGetQueryDescriptionException`
- def: [`tests/unit/core/test_query_service.py:437`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L437)
- doc: Test get_query_description exception handling.
- signature: `class TestQueryServiceGetQueryDescriptionException:`
- members:
  - `test_get_query_description_exception_returns_none(self)` — [`L440`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L440) — Test that exception in get_query_description returns None.
- uses (calls/refs, reference-scoped): [`QueryService`](../../../tree_sitter_analyzer/core/query_service.md#QueryService), [`get_query_description`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.get_query_description)

### `TestQueryServiceInit`
- def: [`tests/unit/core/test_query_service.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L17)
- doc: Tests for QueryService initialization.
- signature: `class TestQueryServiceInit:`
- members:
  - `test_query_service_init_default(self)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L20) — Test QueryService initialization with default project_root.
  - `test_query_service_init_with_project_root(self)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L28) — Test QueryService initialization with project_root.
- uses (calls/refs, reference-scoped): [`QueryService`](../../../tree_sitter_analyzer/core/query_service.md#QueryService), [`plugin_manager`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.plugin_manager), [`parser`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.parser), [`project_root`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.project_root)

### `TestQueryServiceNoLanguageObject`
- def: [`tests/unit/core/test_query_service.py:330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L330)
- doc: Test execute_query when tree has no language object.
- signature: `class TestQueryServiceNoLanguageObject:`
- members:
  - `test_execute_query_no_language_obj(self)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L334) — Test that missing language object raises Exception.
- uses (calls/refs, reference-scoped): [`QueryService`](../../../tree_sitter_analyzer/core/query_service.md#QueryService), [`execute_query`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.execute_query), [`parser`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.parser)

### `TestQueryServicePluginQueryInternalPaths`
- def: [`tests/unit/core/test_query_service.py:451`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L451)
- doc: Test _execute_plugin_query internal code paths.
- signature: `class TestQueryServicePluginQueryInternalPaths:`
- members:
  - `test_plugin_query_categories_exception_falls_to_fallback(self)` — [`L505`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L505) — Test that element categories exception falls to basic fallback.
  - `test_plugin_query_no_matching_key_in_categories(self)` — [`L526`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L526) — Test when query_key is not in element categories.
  - `test_plugin_query_strategy_exception_falls_to_categories(self)` — [`L480`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L480) — Test that plugin strategy exception falls back to element categories.
  - `test_plugin_query_with_elements_having_line_info(self)` — [`L454`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L454) — Test plugin query when plugin returns elements with start_line/end_line.
- uses (calls/refs, reference-scoped): [`QueryService`](../../../tree_sitter_analyzer/core/query_service.md#QueryService), [`_execute_plugin_query`](../../../tree_sitter_analyzer/core/query_service.md#QueryService._execute_plugin_query), [`plugin_manager`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.plugin_manager)

### `TestQueryServiceQueryExceptionFallback`
- def: [`tests/unit/core/test_query_service.py:363`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L363)
- doc: Test execute_query fallback when tree-sitter query fails.
- signature: `class TestQueryServiceQueryExceptionFallback:`
- members:
  - `test_execute_query_empty_captures_uses_plugin_fallback(self)` — [`L402`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L402) — Test that empty captures from query triggers plugin fallback.
  - `test_execute_query_query_exception_uses_plugin_fallback(self)` — [`L367`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L367) — Test that query exception triggers plugin fallback path.
- uses (calls/refs, reference-scoped): [`QueryService`](../../../tree_sitter_analyzer/core/query_service.md#QueryService), [`execute_query`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.execute_query), [`parser`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.parser)

### `TestQueryServiceReadFileAsync`
- def: [`tests/unit/core/test_query_service.py:285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L285)
- doc: Tests for QueryService._read_file_async method.
- signature: `class TestQueryServiceReadFileAsync:`
- members:
  - `test_read_file_async(self, query_service: QueryService, temp_file: Path)` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L289) — Test async file reading.
- uses (calls/refs, reference-scoped): [`QueryService`](../../../tree_sitter_analyzer/core/query_service.md#QueryService), [`_read_file_async`](../../../tree_sitter_analyzer/core/query_service.md#QueryService._read_file_async)

## Functions
- `query_service()` — [`L642`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L642) — Create a QueryService instance for testing.
- `temp_file()` — [`L648`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service.py#L648) — Create a temporary Python file for testing.

