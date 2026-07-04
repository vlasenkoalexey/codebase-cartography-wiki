---
title: 'Module: tree_sitter_analyzer/core/_query_execution.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/core/_query_execution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.core._query_execution`/
symbols:
  execute_query_by_name: execute_query_by_name().
  _execute_query_string: _execute_query_string().
  execute_query_by_explicit_language: execute_query_by_explicit_language().
  execute_raw_query_string: execute_raw_query_string().
  _input_error: _input_error().
  _language_name_from_object: _language_name_from_object().
  logger: logger.
  _process_captures_or_error: _process_captures_or_error().
  _success_result: _success_result().
  SafeExecuteQuery: SafeExecuteQuery.
---
# Module: [`tree_sitter_analyzer/core/_query_execution.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_execution.py)

## Functions
- `_execute_query_string(executor: Any, tree: Any, language: Any, query_string: str, source_code: str, safe_execute_query: SafeExecuteQuery, start_time: float, query_name: str | None = None, query_string_field: str | None = None)` — [`L160`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_execution.py#L160)
- `_input_error(executor: Any, tree: Any, language: Any, query_name: str | None = None)` — [`L133`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_execution.py#L133)
- `_language_name_from_object(language: Any)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_execution.py#L146)
- `_process_captures_or_error(executor: Any, captures: Any, source_code: str, query_name: str | None = None)` — [`L205`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_execution.py#L205)
- `_success_result(processed_captures: list[dict[str, Any]], query_string: str, execution_time: float, query_name: str | None = None, query_string_field: str | None = None)` — [`L222`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_execution.py#L222)
- `execute_query_by_explicit_language(executor: Any, tree: Any, language: Any, query_name: str, source_code: str, language_name: str, safe_execute_query: SafeExecuteQuery)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_execution.py#L57) — Execute a named query using a caller-provided language name.
- `execute_query_by_name(executor: Any, tree: Any, language: Any, query_name: str, source_code: str, safe_execute_query: SafeExecuteQuery)` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_execution.py#L15) — Execute a named query while preserving QueryExecutor's legacy contract.
- `execute_raw_query_string(executor: Any, tree: Any, language: Any, query_string: str, source_code: str, safe_execute_query: SafeExecuteQuery)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_execution.py#L100) — Execute a raw tree-sitter query string.

## Module values
- `SafeExecuteQuery` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_execution.py#L12)
- `logger` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_execution.py#L10)

