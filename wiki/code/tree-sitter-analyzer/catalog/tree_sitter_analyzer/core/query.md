---
title: 'Module: tree_sitter_analyzer/core/query.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/core/query.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.core.query`/
symbols:
  QueryExecutor: QueryExecutor#
  QueryExecutor.execute_query: QueryExecutor#execute_query().
  QueryExecutor._execution_stats: QueryExecutor#_execution_stats.
  QueryExecutor._query_loader: QueryExecutor#_query_loader.
  QueryExecutor.get_available_queries: QueryExecutor#get_available_queries().
  get_available_queries: get_available_queries().
  QueryExecutor.execute_query_string: QueryExecutor#execute_query_string().
  QueryExecutor.get_query_statistics: QueryExecutor#get_query_statistics().
  QueryExecutor.validate_query: QueryExecutor#validate_query().
  QueryExecutor.execute_query_with_language_name: QueryExecutor#execute_query_with_language_name().
  QueryExecutor.get_query_description: QueryExecutor#get_query_description().
  QueryExecutor._process_captures: QueryExecutor#_process_captures().
  QueryExecutor.execute_multiple_queries: QueryExecutor#execute_multiple_queries().
  get_query_description: get_query_description().
  QueryExecutor._create_result_dict: QueryExecutor#_create_result_dict().
  QueryExecutor._create_error_result: QueryExecutor#_create_error_result().
  logger: logger.
  query_loader: query_loader.
  loader: loader.
  QueryExecutor.reset_statistics: QueryExecutor#reset_statistics().
  QueryExecutor.execution_stats: QueryExecutor#execution_stats().
  QueryExecutor.create_error_result: QueryExecutor#create_error_result.
  QueryExecutor.query_loader: QueryExecutor#query_loader().
  QueryExecutor.process_captures: QueryExecutor#process_captures().
  get_all_queries_for_language: get_all_queries_for_language().
  QueryExecutor.__init__: QueryExecutor#__init__().
---
# Module: [`tree_sitter_analyzer/core/query.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py)

## Classes
### `QueryExecutor`
- def: [`tree_sitter_analyzer/core/query.py:32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L32)
- doc: Tree-sitter query executor for the new architecture.
- signature: `class QueryExecutor:`
- members:
  - `__init__(self)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L40) — Initialize the QueryExecutor.
  - `_create_error_result(self, error_message: str, query_name: str | None = None, **kwargs: Any)` — [`L192`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L192) — Create an error result dictionary.
  - `_create_result_dict(self, node: Node, capture_name: str, source_code: str)` — [`L176`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L176) — Create a result dictionary from a Tree-sitter node.
  - `_process_captures(self, captures: Any, source_code: str)` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L161) — Process query captures into standardized format.
  - `execute_multiple_queries(self, tree: Tree, language: Language, query_names: list[str], source_code: str)` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L138) — Execute multiple queries and return combined results.
  - `execute_query(self, tree: Tree | None, language: Language | None, query_name: str, source_code: str)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L51) — Execute a predefined query by name.
  - `execute_query_string(self, tree: Tree | None, language: Language | None, query_string: str, source_code: str)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L110) — Execute a query string directly.
  - `execute_query_with_language_name(self, tree: Tree | None, language: Language | None, query_name: str, source_code: str, language_name: str)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L79) — Execute a predefined query by name with explicit language name.
  - `execution_stats(self)` — [`L212`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L212) — Return the live execution stats dict (mutable reference).
  - `get_available_queries(self, language: str)` — [`L225`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L225) — Get available queries for a language.
  - `get_query_description(self, language: str, query_name: str)` — [`L244`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L244) — Get description for a specific query.
  - `get_query_statistics(self)` — [`L291`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L291) — Get query execution statistics.
  - `process_captures(self, captures: Any, source_code: str)` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L221) — Public alias for _process_captures used by companion helpers.
  - `query_loader(self)` — [`L217`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L217) — Return the query loader instance.
  - `reset_statistics(self)` — [`L300`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L300) — Reset query execution statistics.
  - `validate_query(self, language: str, query_string: str)` — [`L261`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L261) — Validate a query string for a specific language.
  - `create_error_result` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L209)
- protocol/private: `_execution_stats`[`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L43), `_query_loader`[`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L42)
- uses (calls/refs, reference-scoped): [`get_node_text_safe`](../utils/tree_sitter_compat.md#get_node_text_safe), [`TreeSitterQueryCompat`](../utils/tree_sitter_compat.md#TreeSitterQueryCompat), [`load_language`](../language_loader.md#LanguageLoader.load_language), [`get_query_loader`](../query_loader.md#get_query_loader), [`get_loader`](../language_loader.md#get_loader), [`safe_execute_query`](../utils/tree_sitter_compat.md#TreeSitterQueryCompat.safe_execute_query), [`execute_query_by_name`](_query_execution.md#execute_query_by_name), [`get_query_description`](../query_loader.md#QueryLoader.get_query_description), [`execute_query_by_explicit_language`](_query_execution.md#execute_query_by_explicit_language), [`execute_raw_query_string`](_query_execution.md#execute_raw_query_string), [`create_query_safely`](../utils/tree_sitter_compat.md#create_query_safely), [`process_captures`](_query_results.md#process_captures), [`create_result_dict`](_query_results.md#create_result_dict), [`get_all_queries_for_language`](../query_loader.md#QueryLoader.get_all_queries_for_language), [`create_error_result`](_query_results.md#create_error_result), [`logger`](query.md#logger), [`query_statistics`](_query_results.md#query_statistics)
- used by: [`_ensure_initialized`](analysis_engine.md#UnifiedAnalysisEngine._ensure_initialized)  (88 test-only)

## Functions
- `get_all_queries_for_language(language: str)` — [`L365`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L365) — Get all available queries for a specific language.
- `get_available_queries(language: str | None = None)` — [`L311`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L311) — Get available queries for a language (module-level function).
- `get_query_description(language: str, query_name: str)` — [`L337`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L337) — Get description for a specific query (module-level function).

## Module values
- `loader` — [`L394`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L394)
- `logger` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L29)
- `query_loader` — [`L360`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query.py#L360)

