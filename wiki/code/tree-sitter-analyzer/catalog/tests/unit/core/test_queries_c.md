---
title: 'Module: tests/unit/core/test_queries_c.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_queries_c.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_queries_c`/TestCQueries#
symbols:
  TestCQueries.test_query_consistency: test_query_consistency().
  TestCQueries.test_query_aliases: test_query_aliases().
  TestCQueries.test_get_c_query_valid: test_get_c_query_valid().
  TestCQueries.test_get_c_query_invalid: test_get_c_query_invalid().
  TestCQueries.test_get_c_query_description_valid: test_get_c_query_description_valid().
  TestCQueries.test_get_c_query_description_invalid: test_get_c_query_description_invalid().
  TestCQueries.test_get_query_valid: test_get_query_valid().
  TestCQueries.test_get_query_invalid: test_get_query_invalid().
  TestCQueries.test_get_all_queries: test_get_all_queries().
  TestCQueries.test_list_queries: test_list_queries().
  TestCQueries.test_get_available_c_queries: test_get_available_c_queries().
  TestCQueries.test_c_queries_structure: test_c_queries_structure().
  TestCQueries.test_c_query_descriptions_structure: test_c_query_descriptions_structure().
  TestCQueries.test_all_queries_structure: test_all_queries_structure().
  TestCQueries.test_specific_c_queries: test_specific_c_queries().
  TestCQueries.test_pointer_and_array_types: test_pointer_and_array_types().
  TestCQueries.test_string_and_comment_queries: test_string_and_comment_queries().
  TestCQueries.test_function_call_queries: test_function_call_queries().
  TestCQueries.test_sizeof_and_cast_queries: test_sizeof_and_cast_queries().
  TestCQueries: ''
---
# Module: [`tests/unit/core/test_queries_c.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py)

## Classes
### `TestCQueries`
- def: [`tests/unit/core/test_queries_c.py:21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L21)
- doc: Test C queries functionality
- signature: `class TestCQueries:`
- members:
  - `test_all_queries_structure(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L127) — Test ALL_QUERIES dictionary structure
  - `test_c_queries_structure(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L88) — Test C_QUERIES dictionary structure
  - `test_c_query_descriptions_structure(self)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L109) — Test C_QUERY_DESCRIPTIONS dictionary structure
  - `test_function_call_queries(self)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L231) — Test function call queries
  - `test_get_all_queries(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L63) — Test getting all queries
  - `test_get_available_c_queries(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L80) — Test getting available C queries
  - `test_get_c_query_description_invalid(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L44) — Test getting description for invalid query returns default
  - `test_get_c_query_description_valid(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L39) — Test getting description for valid query
  - `test_get_c_query_invalid(self)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L31) — Test getting an invalid C query raises ValueError
  - `test_get_c_query_valid(self)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L24) — Test getting a valid C query
  - `test_get_query_invalid(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L55) — Test getting invalid query through ALL_QUERIES interface
  - `test_get_query_valid(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L49) — Test getting query through ALL_QUERIES interface
  - `test_list_queries(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L72) — Test listing all query names
  - `test_pointer_and_array_types(self)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L209) — Test pointer and array type queries
  - `test_query_aliases(self)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L139) — Test that query aliases work correctly
  - `test_query_consistency(self)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L165) — Test consistency between C_QUERIES and ALL_QUERIES
  - `test_sizeof_and_cast_queries(self)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L240) — Test sizeof and cast expression queries
  - `test_specific_c_queries(self)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L176) — Test specific C query patterns
  - `test_string_and_comment_queries(self)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_c.py#L217) — Test string literal and comment queries
- uses (calls/refs, reference-scoped): [`C_QUERIES`](../../../tree_sitter_analyzer/queries/c.md#C_QUERIES.C_QUERIES), [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/c.md#ALL_QUERIES), [`C_QUERY_DESCRIPTIONS`](../../../tree_sitter_analyzer/queries/c.md#C_QUERY_DESCRIPTIONS.C_QUERY_DESCRIPTIONS), [`list_queries`](../../../tree_sitter_analyzer/queries/c.md#list_queries), [`get_c_query`](../../../tree_sitter_analyzer/queries/c.md#get_c_query), [`get_c_query_description`](../../../tree_sitter_analyzer/queries/c.md#get_c_query_description), [`get_available_c_queries`](../../../tree_sitter_analyzer/queries/c.md#get_available_c_queries), [`get_query`](../../../tree_sitter_analyzer/queries/c.md#get_query), [`get_all_queries`](../../../tree_sitter_analyzer/queries/c.md#get_all_queries)

