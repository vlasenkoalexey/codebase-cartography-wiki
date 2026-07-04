---
title: 'Module: tests/unit/core/test_query_code_cross_language_compatibility.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_query_code_cross_language_compatibility.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_query_code_cross_language_compatibility`/
symbols:
  TestQueryCodeCrossLanguageCompatibility.test_cross_language_query_result_structure: TestQueryCodeCrossLanguageCompatibility#test_cross_language_query_result_structure().
  TestQueryCodeCrossLanguageCompatibility.create_temp_file: TestQueryCodeCrossLanguageCompatibility#create_temp_file().
  TestQueryCodeCrossLanguageCompatibility.test_javascript_query_consistency: TestQueryCodeCrossLanguageCompatibility#test_javascript_query_consistency().
  TestQueryCodeCrossLanguageCompatibility.test_typescript_query_consistency: TestQueryCodeCrossLanguageCompatibility#test_typescript_query_consistency().
  TestQueryCodeCrossLanguageCompatibility.test_python_query_consistency: TestQueryCodeCrossLanguageCompatibility#test_python_query_consistency().
  TestQueryCodeCrossLanguageCompatibility.test_java_query_consistency: TestQueryCodeCrossLanguageCompatibility#test_java_query_consistency().
  TestQueryCodeCrossLanguageCompatibility.test_javascript_functions_bug_fix: TestQueryCodeCrossLanguageCompatibility#test_javascript_functions_bug_fix().
  TestQueryCodeCrossLanguageCompatibility.test_manual_query_execution_fallback: TestQueryCodeCrossLanguageCompatibility#test_manual_query_execution_fallback().
  TestQueryCodeCrossLanguageCompatibility.JAVASCRIPT_CODE: TestQueryCodeCrossLanguageCompatibility#JAVASCRIPT_CODE.
  TestQueryCodeCrossLanguageCompatibility.query_service: TestQueryCodeCrossLanguageCompatibility#query_service().
  TestQueryCodeCrossLanguageCompatibility.TYPESCRIPT_CODE: TestQueryCodeCrossLanguageCompatibility#TYPESCRIPT_CODE.
  TestQueryCodeCrossLanguageCompatibility.PYTHON_CODE: TestQueryCodeCrossLanguageCompatibility#PYTHON_CODE.
  TestQueryCodeCrossLanguageCompatibility.JAVA_CODE: TestQueryCodeCrossLanguageCompatibility#JAVA_CODE.
  _assert_result_structure: _assert_result_structure().
  TestQueryCodeCrossLanguageCompatibility: TestQueryCodeCrossLanguageCompatibility#
---
# Module: [`tests/unit/core/test_query_code_cross_language_compatibility.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_code_cross_language_compatibility.py)

## Classes
### `TestQueryCodeCrossLanguageCompatibility`
- def: [`tests/unit/core/test_query_code_cross_language_compatibility.py:28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_code_cross_language_compatibility.py#L28)
- doc: Test cross-language query compatibility
- signature: `class TestQueryCodeCrossLanguageCompatibility:`
- members:
  - `create_temp_file(self, content: str, extension: str)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_code_cross_language_compatibility.py#L134) — Create temporary file with given content and extension
  - `query_service(self)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_code_cross_language_compatibility.py#L130) — Create QueryService instance
  - `test_cross_language_query_result_structure(self, query_service)` — [`L392`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_code_cross_language_compatibility.py#L392) — Test that all languages return consistent result structure
  - `test_java_query_consistency(self, query_service)` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_code_cross_language_compatibility.py#L310) — Test Java query consistency for singular/plural forms
  - `test_javascript_functions_bug_fix(self, query_service)` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_code_cross_language_compatibility.py#L345) — Specific test for the original JavaScript functions bug.
  - `test_javascript_query_consistency(self, query_service)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_code_cross_language_compatibility.py#L141) — Test JavaScript query consistency for singular/plural forms
  - `test_manual_query_execution_fallback(self, query_service)` — [`L434`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_code_cross_language_compatibility.py#L434) — Test that manual query execution fallback works correctly
  - `test_python_query_consistency(self, query_service)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_code_cross_language_compatibility.py#L258) — Test Python query consistency for singular/plural forms
  - `test_typescript_query_consistency(self, query_service)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_code_cross_language_compatibility.py#L191) — Test TypeScript query consistency for singular/plural forms
  - `JAVASCRIPT_CODE` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_code_cross_language_compatibility.py#L32)
  - `JAVA_CODE` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_code_cross_language_compatibility.py#L107)
  - `PYTHON_CODE` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_code_cross_language_compatibility.py#L89)
  - `TYPESCRIPT_CODE` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_code_cross_language_compatibility.py#L60)
- uses (calls/refs, reference-scoped): [`QueryService`](../../../tree_sitter_analyzer/core/query_service.md#QueryService)  (1 test-only)

## Functions
- `_assert_result_structure(result: dict, language: str)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_code_cross_language_compatibility.py#L17) — Assert one query result has the expected fields and types.

