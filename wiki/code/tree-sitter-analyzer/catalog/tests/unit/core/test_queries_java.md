---
title: 'Module: tests/unit/core/test_queries_java.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_queries_java.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_queries_java`/TestJavaQueries#
symbols:
  TestJavaQueries.test_query_consistency: test_query_consistency().
  TestJavaQueries.test_query_aliases: test_query_aliases().
  TestJavaQueries.test_get_java_query_valid: test_get_java_query_valid().
  TestJavaQueries.test_get_java_query_invalid: test_get_java_query_invalid().
  TestJavaQueries.test_get_java_query_description_valid: test_get_java_query_description_valid().
  TestJavaQueries.test_get_java_query_description_invalid: test_get_java_query_description_invalid().
  TestJavaQueries.test_get_query_valid: test_get_query_valid().
  TestJavaQueries.test_get_query_invalid: test_get_query_invalid().
  TestJavaQueries.test_get_all_queries: test_get_all_queries().
  TestJavaQueries.test_list_queries: test_list_queries().
  TestJavaQueries.test_get_available_java_queries: test_get_available_java_queries().
  TestJavaQueries.test_java_queries_structure: test_java_queries_structure().
  TestJavaQueries.test_java_query_descriptions_structure: test_java_query_descriptions_structure().
  TestJavaQueries.test_all_queries_structure: test_all_queries_structure().
  TestJavaQueries.test_spring_framework_queries: test_spring_framework_queries().
  TestJavaQueries.test_jpa_queries: test_jpa_queries().
  TestJavaQueries.test_detailed_queries: test_detailed_queries().
  TestJavaQueries.test_modifier_specific_queries: test_modifier_specific_queries().
  TestJavaQueries: ''
---
# Module: [`tests/unit/core/test_queries_java.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py)

## Classes
### `TestJavaQueries`
- def: [`tests/unit/core/test_queries_java.py:21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py#L21)
- doc: Test Java queries functionality
- signature: `class TestJavaQueries:`
- members:
  - `test_all_queries_structure(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py#L124) — Test ALL_QUERIES dictionary structure
  - `test_detailed_queries(self)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py#L168) — Test detailed information extraction queries
  - `test_get_all_queries(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py#L63) — Test getting all queries
  - `test_get_available_java_queries(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py#L80) — Test getting available Java queries
  - `test_get_java_query_description_invalid(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py#L44) — Test getting description for invalid query returns default
  - `test_get_java_query_description_valid(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py#L39) — Test getting description for valid query
  - `test_get_java_query_invalid(self)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py#L31) — Test getting an invalid Java query raises ValueError
  - `test_get_java_query_valid(self)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py#L24) — Test getting a valid Java query
  - `test_get_query_invalid(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py#L55) — Test getting invalid query through ALL_QUERIES interface
  - `test_get_query_valid(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py#L49) — Test getting query through ALL_QUERIES interface
  - `test_java_queries_structure(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py#L88) — Test JAVA_QUERIES dictionary structure
  - `test_java_query_descriptions_structure(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py#L106) — Test JAVA_QUERY_DESCRIPTIONS dictionary structure
  - `test_jpa_queries(self)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py#L160) — Test JPA specific queries
  - `test_list_queries(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py#L72) — Test listing all query names
  - `test_modifier_specific_queries(self)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py#L183) — Test modifier-specific queries
  - `test_query_aliases(self)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py#L137) — Test that query aliases work correctly
  - `test_query_consistency(self)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py#L192) — Test consistency between JAVA_QUERIES and ALL_QUERIES
  - `test_spring_framework_queries(self)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_java.py#L151) — Test Spring Framework specific queries
- uses (calls/refs, reference-scoped): [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/java.md#ALL_QUERIES), [`JAVA_QUERIES`](../../../tree_sitter_analyzer/queries/java.md#JAVA_QUERIES.JAVA_QUERIES), [`JAVA_QUERY_DESCRIPTIONS`](../../../tree_sitter_analyzer/queries/java.md#JAVA_QUERY_DESCRIPTIONS.JAVA_QUERY_DESCRIPTIONS), [`get_java_query`](../../../tree_sitter_analyzer/queries/java.md#get_java_query), [`get_java_query_description`](../../../tree_sitter_analyzer/queries/java.md#get_java_query_description), [`get_query`](../../../tree_sitter_analyzer/queries/java.md#get_query), [`get_all_queries`](../../../tree_sitter_analyzer/queries/java.md#get_all_queries), [`get_available_java_queries`](../../../tree_sitter_analyzer/queries/java.md#get_available_java_queries), [`list_queries`](../../../tree_sitter_analyzer/queries/java.md#list_queries)

