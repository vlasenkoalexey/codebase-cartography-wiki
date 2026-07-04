---
title: 'Module: tests/unit/core/test_queries_sql.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_queries_sql.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_queries_sql`/TestSQLQuer
symbols:
  TestSQLQueries.test_sql_queries_exist: ies#test_sql_queries_exist().
  TestSQLQueryIntegration.test_query_service_with_sql_file: yIntegration#test_query_service_with_sql_file().
  TestSQLQueryIntegration.test_sql_query_execution: yIntegration#test_sql_query_execution().
  TestSQLQueryIntegration.test_sql_error_queries: yIntegration#test_sql_error_queries().
  TestSQLQueries.test_get_sql_query: ies#test_get_sql_query().
  TestSQLQueries.test_get_sql_query_description: ies#test_get_sql_query_description().
  TestSQLQueries.test_get_query_compatibility: ies#test_get_query_compatibility().
  TestSQLQueries.test_get_all_queries: ies#test_get_all_queries().
  TestSQLQueries.test_list_queries: ies#test_list_queries().
  TestSQLQueries.test_get_available_sql_queries: ies#test_get_available_sql_queries().
  TestSQLQueries.test_query_aliases: ies#test_query_aliases().
  TestSQLQueries.test_basic_sql_queries: ies#test_basic_sql_queries().
  TestSQLQueries.test_detailed_sql_queries: ies#test_detailed_sql_queries().
  TestSQLQueries.test_constraint_queries: ies#test_constraint_queries().
  TestSQLQueries.test_join_queries: ies#test_join_queries().
  TestSQLQueries.test_function_queries: ies#test_function_queries().
  TestSQLQueries.test_error_handling_queries: ies#test_error_handling_queries().
  TestSQLQueries.test_name_only_queries: ies#test_name_only_queries().
  TestSQLQueries.test_advanced_sql_features: ies#test_advanced_sql_features().
  TestSQLQueries.test_data_type_queries: ies#test_data_type_queries().
  TestSQLQueries.test_comment_queries: ies#test_comment_queries().
  TestSQLQueryIntegration.query_service: yIntegration#query_service().
  TestSQLQueries: ies#
  TestSQLQueryIntegration: yIntegration#
  TestSQLQueryIntegration.sample_sql_file: yIntegration#sample_sql_file().
---
# Module: [`tests/unit/core/test_queries_sql.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py)

## Classes
### `TestSQLQueries`
- def: [`tests/unit/core/test_queries_sql.py:25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L25)
- doc: Test SQL query definitions and functionality.
- signature: `class TestSQLQueries:`
- members:
  - `test_advanced_sql_features(self)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L235) — Test advanced SQL feature queries.
  - `test_basic_sql_queries(self)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L117) — Test basic SQL query patterns.
  - `test_comment_queries(self)` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L270) — Test comment extraction queries.
  - `test_constraint_queries(self)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L158) — Test constraint-related queries.
  - `test_data_type_queries(self)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L253) — Test data type queries.
  - `test_detailed_sql_queries(self)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L139) — Test detailed SQL query patterns.
  - `test_error_handling_queries(self)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L205) — Test error handling queries for tree-sitter-sql ERROR nodes.
  - `test_function_queries(self)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L191) — Test function-related queries.
  - `test_get_all_queries(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L68) — Test getting all queries.
  - `test_get_available_sql_queries(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L91) — Test getting available SQL queries.
  - `test_get_query_compatibility(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L58) — Test compatibility with generic query interface.
  - `test_get_sql_query(self)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L38) — Test getting SQL queries by name.
  - `test_get_sql_query_description(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L49) — Test getting SQL query descriptions.
  - `test_join_queries(self)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L176) — Test JOIN-related queries.
  - `test_list_queries(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L81) — Test listing all query names.
  - `test_name_only_queries(self)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L218) — Test name-only extraction queries.
  - `test_query_aliases(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L99) — Test that query aliases work correctly.
  - `test_sql_queries_exist(self)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L28) — Test that SQL queries are properly defined.
- uses (calls/refs, reference-scoped): [`get_sql_query`](../../../tree_sitter_analyzer/queries/sql.md#get_sql_query), [`SQL_QUERIES`](../../../tree_sitter_analyzer/queries/sql.md#SQL_QUERIES.SQL_QUERIES), [`list_queries`](../../../tree_sitter_analyzer/queries/sql.md#list_queries), [`SQL_QUERY_DESCRIPTIONS`](../../../tree_sitter_analyzer/queries/sql.md#SQL_QUERY_DESCRIPTIONS.SQL_QUERY_DESCRIPTIONS), [`get_sql_query_description`](../../../tree_sitter_analyzer/queries/sql.md#get_sql_query_description), [`get_available_sql_queries`](../../../tree_sitter_analyzer/queries/sql.md#get_available_sql_queries), [`get_all_queries`](../../../tree_sitter_analyzer/queries/sql.md#get_all_queries), [`get_query`](../../../tree_sitter_analyzer/queries/sql.md#get_query)

### `TestSQLQueryIntegration`
- def: [`tests/unit/core/test_queries_sql.py:286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L286)
- doc: Test SQL queries with actual SQL parsing.
- signature: `class TestSQLQueryIntegration:`
- members:
  - `query_service(self)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L295) — Create QueryService instance.
  - `sample_sql_file(self)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L290) — Get path to sample SQL file.
  - `test_query_service_with_sql_file(self, query_service: QueryService, sample_sql_file: Path)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L299) — Test QueryService with SQL file.
  - `test_sql_error_queries(self, query_service: QueryService, sample_sql_file: Path)` — [`L339`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L339) — Test error handling queries.
  - `test_sql_query_execution(self, query_service: QueryService, sample_sql_file: Path)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_sql.py#L319) — Test executing various SQL queries.
- uses (calls/refs, reference-scoped): [`QueryService`](../../../tree_sitter_analyzer/core/query_service.md#QueryService), [`execute_query`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.execute_query)

