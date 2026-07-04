---
title: 'Module: tests/unit/core/test_queries_cpp.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_queries_cpp.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_queries_cpp`/TestCppQueries#
symbols:
  TestCppQueries.test_query_consistency: test_query_consistency().
  TestCppQueries.test_query_aliases: test_query_aliases().
  TestCppQueries.test_get_cpp_query_valid: test_get_cpp_query_valid().
  TestCppQueries.test_get_cpp_query_invalid: test_get_cpp_query_invalid().
  TestCppQueries.test_get_cpp_query_description_valid: test_get_cpp_query_description_valid().
  TestCppQueries.test_get_cpp_query_description_invalid: test_get_cpp_query_description_invalid().
  TestCppQueries.test_get_query_valid: test_get_query_valid().
  TestCppQueries.test_get_query_invalid: test_get_query_invalid().
  TestCppQueries.test_get_all_queries: test_get_all_queries().
  TestCppQueries.test_list_queries: test_list_queries().
  TestCppQueries.test_get_available_cpp_queries: test_get_available_cpp_queries().
  TestCppQueries.test_cpp_queries_structure: test_cpp_queries_structure().
  TestCppQueries.test_cpp_query_descriptions_structure: test_cpp_query_descriptions_structure().
  TestCppQueries.test_all_queries_structure: test_all_queries_structure().
  TestCppQueries.test_template_queries: test_template_queries().
  TestCppQueries.test_namespace_queries: test_namespace_queries().
  TestCppQueries.test_access_specifier_queries: test_access_specifier_queries().
  TestCppQueries.test_inheritance_queries: test_inheritance_queries().
  TestCppQueries.test_modern_cpp_queries: test_modern_cpp_queries().
  TestCppQueries.test_exception_handling_queries: test_exception_handling_queries().
  TestCppQueries.test_operator_friend_queries: test_operator_friend_queries().
  TestCppQueries.test_virtual_destructor_constructor_queries: test_virtual_destructor_constructor_queries().
  TestCppQueries.test_name_extraction_queries: test_name_extraction_queries().
  TestCppQueries: ''
---
# Module: [`tests/unit/core/test_queries_cpp.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py)

## Classes
### `TestCppQueries`
- def: [`tests/unit/core/test_queries_cpp.py:21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L21)
- doc: Test C++ queries functionality
- signature: `class TestCppQueries:`
- members:
  - `test_access_specifier_queries(self)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L197) — Test C++ access specifier queries
  - `test_all_queries_structure(self)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L126) — Test ALL_QUERIES dictionary structure
  - `test_cpp_queries_structure(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L88) — Test CPP_QUERIES dictionary structure
  - `test_cpp_query_descriptions_structure(self)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L109) — Test CPP_QUERY_DESCRIPTIONS dictionary structure
  - `test_exception_handling_queries(self)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L236) — Test C++ exception handling queries
  - `test_get_all_queries(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L63) — Test getting all queries
  - `test_get_available_cpp_queries(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L80) — Test getting available C++ queries
  - `test_get_cpp_query_description_invalid(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L44) — Test getting description for invalid query returns default
  - `test_get_cpp_query_description_valid(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L39) — Test getting description for valid query
  - `test_get_cpp_query_invalid(self)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L31) — Test getting an invalid C++ query raises ValueError
  - `test_get_cpp_query_valid(self)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L24) — Test getting a valid C++ query
  - `test_get_query_invalid(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L55) — Test getting invalid query through ALL_QUERIES interface
  - `test_get_query_valid(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L49) — Test getting query through ALL_QUERIES interface
  - `test_inheritance_queries(self)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L209) — Test C++ inheritance queries
  - `test_list_queries(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L72) — Test listing all query names
  - `test_modern_cpp_queries(self)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L217) — Test modern C++ feature queries
  - `test_name_extraction_queries(self)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L268) — Test C++ name-only extraction queries
  - `test_namespace_queries(self)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L183) — Test C++ namespace-specific queries
  - `test_operator_friend_queries(self)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L247) — Test C++ operator overloading and friend queries
  - `test_query_aliases(self)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L138) — Test that query aliases work correctly
  - `test_query_consistency(self)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L160) — Test consistency between CPP_QUERIES and ALL_QUERIES
  - `test_template_queries(self)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L169) — Test C++ template-specific queries
  - `test_virtual_destructor_constructor_queries(self)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_cpp.py#L256) — Test C++ virtual, destructor, constructor queries
- uses (calls/refs, reference-scoped): [`CPP_QUERIES`](../../../tree_sitter_analyzer/queries/cpp.md#CPP_QUERIES.CPP_QUERIES), [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/cpp.md#ALL_QUERIES), [`CPP_QUERY_DESCRIPTIONS`](../../../tree_sitter_analyzer/queries/cpp.md#CPP_QUERY_DESCRIPTIONS.CPP_QUERY_DESCRIPTIONS), [`list_queries`](../../../tree_sitter_analyzer/queries/cpp.md#list_queries), [`get_cpp_query`](../../../tree_sitter_analyzer/queries/cpp.md#get_cpp_query), [`get_cpp_query_description`](../../../tree_sitter_analyzer/queries/cpp.md#get_cpp_query_description), [`get_available_cpp_queries`](../../../tree_sitter_analyzer/queries/cpp.md#get_available_cpp_queries), [`get_query`](../../../tree_sitter_analyzer/queries/cpp.md#get_query), [`get_all_queries`](../../../tree_sitter_analyzer/queries/cpp.md#get_all_queries)

