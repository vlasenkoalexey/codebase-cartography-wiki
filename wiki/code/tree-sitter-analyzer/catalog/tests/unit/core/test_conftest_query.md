---
title: 'Module: tests/unit/core/test_conftest_query.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_conftest_query.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_conftest_query`/
symbols:
  TestQueryFixtures.test_query_service_initialized: TestQueryFixtures#test_query_service_initialized().
  TestQueryFixtures.test_executor_initialized: TestQueryFixtures#test_executor_initialized().
  TestQueryFixtures.test_query_executor_alias: TestQueryFixtures#test_query_executor_alias().
  TestQueryFixtures.test_query_filter_initialized: TestQueryFixtures#test_query_filter_initialized().
  executor: executor().
  query_executor: query_executor().
  query_service: query_service().
  query_filter: query_filter().
  mock_tree: mock_tree().
  mock_language: mock_language().
  temp_project_dir: temp_project_dir().
  temp_file: temp_file().
  TestQueryFixtures: TestQueryFixtures#
  TestQueryFixtures.test_query_filter_noop: TestQueryFixtures#test_query_filter_noop().
  TestQueryFixtures.test_temp_project_dir: TestQueryFixtures#test_temp_project_dir().
  TestQueryFixtures.test_temp_file: TestQueryFixtures#test_temp_file().
---
# Module: [`tests/unit/core/test_conftest_query.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_conftest_query.py)

## Classes
### `TestQueryFixtures`
- def: [`tests/unit/core/test_conftest_query.py:76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_conftest_query.py#L76)
- doc: Tests for query fixture functionality.
- signature: `class TestQueryFixtures:`
- members:
  - `test_executor_initialized(self, executor)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_conftest_query.py#L79) — Test that QueryExecutor fixture initializes correctly.
  - `test_query_executor_alias(self, query_executor)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_conftest_query.py#L91) — Test that query_executor alias fixture works.
  - `test_query_filter_initialized(self, query_filter)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_conftest_query.py#L111) — Test that QueryFilter fixture initializes correctly.
  - `test_query_filter_noop(self, query_filter)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_conftest_query.py#L117) — Test QueryFilter.filter_results with no filter returns all results.
  - `test_query_service_initialized(self, query_service)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_conftest_query.py#L102) — Test that QueryService fixture initializes correctly.
  - `test_temp_file(self, temp_file)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_conftest_query.py#L129) — Test that temp_file fixture creates a valid file.
  - `test_temp_project_dir(self, temp_project_dir)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_conftest_query.py#L123) — Test that temp_project_dir fixture creates a valid path.
- uses (calls/refs, reference-scoped): [`Parser`](../../../tree_sitter_analyzer/core/parser.md#Parser), [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`QueryService`](../../../tree_sitter_analyzer/core/query_service.md#QueryService), [`execute_query`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.execute_query), [`QueryFilter`](../../../tree_sitter_analyzer/core/query_filter.md#QueryFilter), [`filter_results`](../../../tree_sitter_analyzer/core/query_filter.md#QueryFilter.filter_results), [`execute_query`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.execute_query), [`execute_query_string`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.execute_query_string), [`get_available_queries`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.get_available_queries), [`parser`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.parser), [`execute_multiple_queries`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.execute_multiple_queries), [`project_root`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.project_root), [`execution_stats`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.execution_stats), [`get_filter_help`](../../../tree_sitter_analyzer/core/query_filter.md#QueryFilter.get_filter_help)

## Functions
- `executor()` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_conftest_query.py#L20) — Create a QueryExecutor instance.
- `mock_language()` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_conftest_query.py#L40) — Create a mock Language object.
- `mock_tree()` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_conftest_query.py#L32) — Create a mock Tree-sitter tree.
- `query_executor()` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_conftest_query.py#L26) — Create a QueryExecutor instance (alias).
- `query_filter()` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_conftest_query.py#L54) — Create a QueryFilter instance.
- `query_service()` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_conftest_query.py#L48) — Create a QueryService instance.
- `temp_file()` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_conftest_query.py#L67) — Create a temporary file for testing.
- `temp_project_dir()` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_conftest_query.py#L60) — Create a temporary project directory.

