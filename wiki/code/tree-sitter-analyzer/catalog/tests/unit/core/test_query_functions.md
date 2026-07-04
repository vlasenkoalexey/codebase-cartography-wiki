---
title: 'Module: tests/unit/core/test_query_functions.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_query_functions.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_query_functions`/Test
symbols:
  TestExecuteQueryWithRealParser.test_execute_query_with_real_python_code: ExecuteQueryWithRealParser#test_execute_query_with_real_python_code().
  TestExecuteQueryWithRealParser.test_execute_query_string_with_real_code: ExecuteQueryWithRealParser#test_execute_query_string_with_real_code().
  TestGetAvailableQueriesResponseFormats.test_get_available_queries_none_response: GetAvailableQueriesResponseFormats#test_get_available_queries_none_response().
  TestGetAvailableQueriesResponseFormats.test_get_available_queries_dict_response: GetAvailableQueriesResponseFormats#test_get_available_queries_dict_response().
  TestGetAvailableQueriesResponseFormats.test_get_available_queries_list_response: GetAvailableQueriesResponseFormats#test_get_available_queries_list_response().
  TestExecuteQueryLanguageNameEdgeCases.test_execute_query_with_empty_language_name: ExecuteQueryLanguageNameEdgeCases#test_execute_query_with_empty_language_name().
  TestExecuteQueryLanguageNameEdgeCases.test_execute_query_with_none_language_name_attr: ExecuteQueryLanguageNameEdgeCases#test_execute_query_with_none_language_name_attr().
  TestExecuteQueryLanguageNameEdgeCases.test_execute_query_with_language_name_string_none: ExecuteQueryLanguageNameEdgeCases#test_execute_query_with_language_name_string_none().
  TestExecuteQueryLanguageNameEdgeCases.test_execute_query_with_whitespace_language_name: ExecuteQueryLanguageNameEdgeCases#test_execute_query_with_whitespace_language_name().
  TestExecuteQueryEdgeCases.test_execute_query_with_empty_source_code: ExecuteQueryEdgeCases#test_execute_query_with_empty_source_code().
  TestExecuteQueryEdgeCases.test_execute_query_with_very_long_source_code: ExecuteQueryEdgeCases#test_execute_query_with_very_long_source_code().
  TestExecuteMultipleQueriesPartialFailures.test_execute_multiple_queries_with_partial_failures: ExecuteMultipleQueriesPartialFailures#test_execute_multiple_queries_with_partial_failures().
  TestProcessCapturesMixedFormats.test_process_captures_with_mixed_formats: ProcessCapturesMixedFormats#test_process_captures_with_mixed_formats().
  TestModuleLevelFunctions.test_get_available_queries_module_level: ModuleLevelFunctions#test_get_available_queries_module_level().
  TestModuleLevelFunctions.test_get_available_queries_with_language: ModuleLevelFunctions#test_get_available_queries_with_language().
  TestModuleLevelFunctions.test_get_query_description_module_level: ModuleLevelFunctions#test_get_query_description_module_level().
  TestDeprecatedFunctions.test_get_all_queries_for_language_deprecated: DeprecatedFunctions#test_get_all_queries_for_language_deprecated().
  TestExecuteMultipleQueriesPartialFailures.mock_execute: ExecuteMultipleQueriesPartialFailures#mock_execute().
  TestModuleLevelFunctions: ModuleLevelFunctions#
  TestGetAvailableQueriesResponseFormats: GetAvailableQueriesResponseFormats#
  TestExecuteQueryLanguageNameEdgeCases: ExecuteQueryLanguageNameEdgeCases#
  TestExecuteQueryEdgeCases: ExecuteQueryEdgeCases#
  TestProcessCapturesMixedFormats: ProcessCapturesMixedFormats#
  TestExecuteMultipleQueriesPartialFailures: ExecuteMultipleQueriesPartialFailures#
  TestDeprecatedFunctions: DeprecatedFunctions#
  TestExecuteQueryWithRealParser: ExecuteQueryWithRealParser#
---
# Module: [`tests/unit/core/test_query_functions.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py)

## Classes
### `TestDeprecatedFunctions`
- def: [`tests/unit/core/test_query_functions.py:278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L278)
- doc: Test deprecated functions.
- signature: `class TestDeprecatedFunctions:`
- members:
  - `test_get_all_queries_for_language_deprecated(self)` — [`L281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L281) — Test that get_all_queries_for_language shows deprecation warning.
- uses (calls/refs, reference-scoped): [`get_all_queries_for_language`](../../../tree_sitter_analyzer/core/query.md#get_all_queries_for_language)

### `TestExecuteMultipleQueriesPartialFailures`
- def: [`tests/unit/core/test_query_functions.py:252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L252)
- doc: Test execute_multiple_queries with partial failures.
- signature: `class TestExecuteMultipleQueriesPartialFailures:`
- members:
  - `mock_execute(tree, lang, query_name, code)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L262)
  - `test_execute_multiple_queries_with_partial_failures(self)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L255) — Test executing multiple queries where some fail.
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`execute_multiple_queries`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.execute_multiple_queries)

### `TestExecuteQueryEdgeCases`
- def: [`tests/unit/core/test_query_functions.py:182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L182)
- doc: Test execute_query with various edge cases.
- signature: `class TestExecuteQueryEdgeCases:`
- members:
  - `test_execute_query_with_empty_source_code(self)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L185) — Test executing query with empty source code.
  - `test_execute_query_with_very_long_source_code(self)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L201) — Test executing query with very long source code.
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`execute_query`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.execute_query), [`_query_loader`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor._query_loader)

### `TestExecuteQueryLanguageNameEdgeCases`
- def: [`tests/unit/core/test_query_functions.py:105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L105)
- doc: Test execute_query with edge case language names.
- signature: `class TestExecuteQueryLanguageNameEdgeCases:`
- members:
  - `test_execute_query_with_empty_language_name(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L108) — Test execute_query when language name is empty string.
  - `test_execute_query_with_language_name_string_none(self)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L145) — Test execute_query when language name is string 'None'.
  - `test_execute_query_with_none_language_name_attr(self)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L126) — Test execute_query when language.name is None.
  - `test_execute_query_with_whitespace_language_name(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L163) — Test execute_query when language name is whitespace.
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`execute_query`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.execute_query), [`_query_loader`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor._query_loader)

### `TestExecuteQueryWithRealParser`
- def: [`tests/unit/core/test_query_functions.py:291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L291)
- doc: Integration tests using real tree-sitter parsing.
- signature: `class TestExecuteQueryWithRealParser:`
- members:
  - `test_execute_query_string_with_real_code(self)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L314) — Test query string execution with real code.
  - `test_execute_query_with_real_python_code(self)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L294) — Test query execution with real Python code parsing.
- uses (calls/refs, reference-scoped): [`Parser`](../../../tree_sitter_analyzer/core/parser.md#Parser), [`tree`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.tree), [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`parse_code`](../../../tree_sitter_analyzer/core/parser.md#Parser.parse_code), [`success`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.success), [`execute_query_string`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.execute_query_string), [`execute_query_with_language_name`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.execute_query_with_language_name)

### `TestGetAvailableQueriesResponseFormats`
- def: [`tests/unit/core/test_query_functions.py:68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L68)
- doc: Test get_available_queries with different response formats.
- signature: `class TestGetAvailableQueriesResponseFormats:`
- members:
  - `test_get_available_queries_dict_response(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L80) — Test get_available_queries with dict response.
  - `test_get_available_queries_list_response(self)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L92) — Test get_available_queries with list response.
  - `test_get_available_queries_none_response(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L71) — Test get_available_queries with None response.
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`_query_loader`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor._query_loader), [`get_available_queries`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.get_available_queries)

### `TestModuleLevelFunctions`
- def: [`tests/unit/core/test_query_functions.py:13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L13)
- doc: 模块级别函数测试
- signature: `class TestModuleLevelFunctions:`
- members:
  - `test_get_available_queries_module_level(self, mock_loader)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L17) — 测试模块级别get_available_queries函数
  - `test_get_available_queries_with_language(self, mock_loader)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L35) — 测试带语言参数的get_available_queries
  - `test_get_query_description_module_level(self, mock_loader)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L53) — 测试模块级别get_query_description函数
- uses (calls/refs, reference-scoped): [`get_available_queries`](../../../tree_sitter_analyzer/core/query.md#get_available_queries), [`get_query_description`](../../../tree_sitter_analyzer/core/query.md#get_query_description)

### `TestProcessCapturesMixedFormats`
- def: [`tests/unit/core/test_query_functions.py:221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L221)
- doc: Test _process_captures with mixed formats.
- signature: `class TestProcessCapturesMixedFormats:`
- members:
  - `test_process_captures_with_mixed_formats(self)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_functions.py#L224) — Test processing captures with mixed tuple and dict formats.
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`_process_captures`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor._process_captures)

