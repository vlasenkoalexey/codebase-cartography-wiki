---
title: 'Module: tests/unit/core/test_query_extended.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_query_extended.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_query_extended`/TestQueryExecutor
symbols:
  TestQueryExecutorConfiguration.test_query_executor_with_custom_settings: Configuration#test_query_executor_with_custom_settings().
  TestQueryExecutorPerformance.test_query_execution_with_timeout: Performance#test_query_execution_with_timeout().
  TestQueryExecutorEdgeCases.query_executor: EdgeCases#query_executor().
  TestQueryExecutorEdgeCases.test_execute_query_with_empty_query: EdgeCases#test_execute_query_with_empty_query().
  TestQueryExecutorEdgeCases.test_execute_query_with_invalid_syntax: EdgeCases#test_execute_query_with_invalid_syntax().
  TestQueryExecutorEdgeCases.test_execute_query_with_none_inputs: EdgeCases#test_execute_query_with_none_inputs().
  TestQueryExecutorEdgeCases.test_execute_query_with_malformed_tree: EdgeCases#test_execute_query_with_malformed_tree().
  TestQueryExecutorEdgeCases.test_execute_query_with_complex_queries: EdgeCases#test_execute_query_with_complex_queries().
  TestQueryExecutorEdgeCases.test_execute_query_with_large_tree: EdgeCases#test_execute_query_with_large_tree().
  TestQueryExecutorConfiguration.test_query_executor_initialization: Configuration#test_query_executor_initialization().
  TestQueryExecutorConfiguration.test_query_executor_error_handling_configuration: Configuration#test_query_executor_error_handling_configuration().
  TestQueryExecutorPerformance.query_executor: Performance#query_executor().
  TestQueryExecutorPerformance.test_concurrent_query_execution: Performance#test_concurrent_query_execution().
  TestQueryExecutorIntegration.query_executor: Integration#query_executor().
  TestQueryExecutorPerformance.execute_query: Performance#execute_query().
  TestQueryExecutorPerformance.slow_query: Performance#slow_query().
  TestQueryExecutorEdgeCases: EdgeCases#
  TestQueryExecutorEdgeCases.mock_tree: EdgeCases#mock_tree().
  TestQueryExecutorEdgeCases.mock_language: EdgeCases#mock_language().
  TestQueryExecutorConfiguration: Configuration#
  TestQueryExecutorPerformance: Performance#
  TestQueryExecutorPerformance.test_memory_usage_with_repeated_queries: Performance#test_memory_usage_with_repeated_queries().
  TestQueryExecutorIntegration: Integration#
  TestQueryExecutorIntegration.test_query_executor_with_real_tree_sitter_objects: Integration#test_query_executor_with_real_tree_sitter_objects().
  TestQueryExecutorIntegration.test_query_executor_error_recovery: Integration#test_query_executor_error_recovery().
---
# Module: [`tests/unit/core/test_query_extended.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py)

## Classes
### `TestQueryExecutorConfiguration`
- def: [`tests/unit/core/test_query_extended.py:203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L203)
- doc: Test QueryExecutor configuration and initialization.
- signature: `class TestQueryExecutorConfiguration:`
- members:
  - `test_query_executor_error_handling_configuration(self)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L231) — Test QueryExecutor error handling configuration.
  - `test_query_executor_initialization(self)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L206) — Test QueryExecutor initialization with different configurations.
  - `test_query_executor_with_custom_settings(self)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L223) — Test QueryExecutor with custom settings.
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`execute_query`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.execute_query)

### `TestQueryExecutorEdgeCases`
- def: [`tests/unit/core/test_query_extended.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L17)
- doc: Test edge cases and error conditions in QueryExecutor.
- signature: `class TestQueryExecutorEdgeCases:`
- members:
  - `mock_language(self)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L38) — Create a mock tree-sitter language.
  - `mock_tree(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L26) — Create a mock tree-sitter tree.
  - `query_executor(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L21) — Create a QueryExecutor instance for testing.
  - `test_execute_query_with_complex_queries(self, query_executor, mock_tree, mock_language)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L127) — Test executing complex queries.
  - `test_execute_query_with_empty_query(self, query_executor, mock_tree, mock_language)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L44) — Test executing an empty query.
  - `test_execute_query_with_invalid_syntax(self, query_executor, mock_tree, mock_language)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L61) — Test executing queries with invalid syntax.
  - `test_execute_query_with_large_tree(self, query_executor, mock_language)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L168) — Test executing query on a large tree structure.
  - `test_execute_query_with_malformed_tree(self, query_executor, mock_language)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L107) — Test executing query with malformed tree.
  - `test_execute_query_with_none_inputs(self, query_executor)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L84) — Test executing query with None inputs.
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`QueryError`](../../../tree_sitter_analyzer/_exceptions_core.md#QueryError)

### `TestQueryExecutorIntegration`
- def: [`tests/unit/core/test_query_extended.py:353`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L353)
- doc: Integration tests for QueryExecutor.
- signature: `class TestQueryExecutorIntegration:`
- members:
  - `query_executor(self)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L357) — Create a QueryExecutor instance for testing.
  - `test_query_executor_error_recovery(self, query_executor)` — [`L392`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L392) — Test QueryExecutor error recovery mechanisms.
  - `test_query_executor_with_real_tree_sitter_objects(self, query_executor)` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L361) — Test QueryExecutor with real tree-sitter objects (if available).
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor)

### `TestQueryExecutorPerformance`
- def: [`tests/unit/core/test_query_extended.py:249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L249)
- doc: Test QueryExecutor performance characteristics.
- signature: `class TestQueryExecutorPerformance:`
- members:
  - `execute_query()` — [`L273`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L273)
  - `query_executor(self)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L253) — Create a QueryExecutor instance for testing.
  - `slow_query(*args, **kwargs)` — [`L302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L302)
  - `test_concurrent_query_execution(self, query_executor)` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L257) — Test concurrent query execution.
  - `test_memory_usage_with_repeated_queries(self, query_executor)` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L321) — Test memory usage with repeated query execution.
  - `test_query_execution_with_timeout(self, query_executor)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_extended.py#L295) — Test query execution with timeout scenarios.
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`QueryError`](../../../tree_sitter_analyzer/_exceptions_core.md#QueryError)

