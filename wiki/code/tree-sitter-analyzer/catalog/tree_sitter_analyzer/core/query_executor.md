---
title: 'Module: tree_sitter_analyzer/core/query_executor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/core/query_executor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.core.query_executor`/
symbols:
  execute_ts_query: execute_ts_query().
  resolve_query_string: resolve_query_string().
  process_captures: process_captures().
  logger: logger.
---
# Module: [`tree_sitter_analyzer/core/query_executor.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_executor.py)

## Functions
- `execute_ts_query(tree: Any, language_obj: Any, query_string: str, root_node: Any, fallback_fn: Any, query_key: str | None, language: str, content: str)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_executor.py#L36) — Execute a tree-sitter query with plugin fallback.
- `process_captures(captures: list[tuple[Any, str]], content: str, create_result_fn: Any)` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_executor.py#L60) — Convert capture tuples into result dicts.
- `resolve_query_string(language: str, query_key: str | None, query_string: str | None)` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_executor.py#L12) — Resolve query_key or query_string into a concrete query string.

## Module values
- `logger` — [`L9`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_executor.py#L9)

