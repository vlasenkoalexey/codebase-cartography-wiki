---
title: 'Module: tree_sitter_analyzer/utils/tree_sitter_compat.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/utils/tree_sitter_compat.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.utils.tree_sitter_compat`/
symbols:
  get_node_text_safe: get_node_text_safe().
  TreeSitterQueryCompat: TreeSitterQueryCompat#
  TreeSitterQueryCompat.safe_execute_query: TreeSitterQueryCompat#safe_execute_query().
  TreeSitterQueryCompat.execute_query: TreeSitterQueryCompat#execute_query().
  log_api_info: log_api_info().
  create_query_safely: create_query_safely().
  count_nodes_iterative: count_nodes_iterative().
  logger: logger.
  TreeSitterQueryCompat._execute_old_api: TreeSitterQueryCompat#_execute_old_api().
  TreeSitterQueryCompat._execute_modern_api: TreeSitterQueryCompat#_execute_modern_api().
  TreeSitterQueryCompat._execute_legacy_api: TreeSitterQueryCompat#_execute_legacy_api().
  TreeSitterQueryCompat._execute_newest_api: TreeSitterQueryCompat#_execute_newest_api().
---
# Module: [`tree_sitter_analyzer/utils/tree_sitter_compat.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/tree_sitter_compat.py)

## Classes
### `TreeSitterQueryCompat`
- def: [`tree_sitter_analyzer/utils/tree_sitter_compat.py:24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/tree_sitter_compat.py#L24)
- doc: Tree-sitter query execution wrapper for modern API.
- signature: `class TreeSitterQueryCompat:`
- members:
  - `_execute_legacy_api(query: Any, root_node: Any)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/tree_sitter_compat.py#L62) — Execute query using legacy API (tree-sitter < 0.20)
  - `_execute_modern_api(query: Any, root_node: Any)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/tree_sitter_compat.py#L57) — Execute query using modern API (tree-sitter 0.20+)
  - `_execute_newest_api(query: Any, root_node: Any)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/tree_sitter_compat.py#L52) — Execute query using newest API (tree-sitter 0.25+) with QueryCursor
  - `_execute_old_api(query: Any, root_node: Any)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/tree_sitter_compat.py#L67) — Execute query using very old API (tree-sitter < 0.19)
  - `execute_query(language: Any, query_string: str, root_node: Any)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/tree_sitter_compat.py#L32) — Execute a tree-sitter query using the modern API.
  - `safe_execute_query(language: Any, query_string: str, root_node: Any, fallback_result: list[tuple[Any, str]] | None = None)` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/tree_sitter_compat.py#L72) — Safely execute a query with fallback handling.
- uses (calls/refs, reference-scoped): [`logger`](tree_sitter_compat.md#logger), [`execute_old_api`](_tree_sitter_compat_helpers.md#execute_old_api), [`execute_query_compat`](_tree_sitter_compat_helpers.md#execute_query_compat), [`execute_legacy_api`](_tree_sitter_compat_helpers.md#execute_legacy_api), [`execute_modern_api`](_tree_sitter_compat_helpers.md#execute_modern_api), [`execute_newest_api`](_tree_sitter_compat_helpers.md#execute_newest_api)
- used by: [`execute_query`](../core/query.md#QueryExecutor.execute_query), [`_query_imports`](../languages/python_plugin/_import_helpers.md#_query_imports), [`_query_class_body_nodes`](../languages/python_plugin/_import_helpers.md#_query_class_body_nodes), [`execute_query_string`](../core/query.md#QueryExecutor.execute_query_string), [`execute_query_with_language_name`](../core/query.md#QueryExecutor.execute_query_with_language_name), [`execute_ts_query`](../core/query_executor.md#execute_ts_query)  (41 test-only)

## Functions
- `count_nodes_iterative(root_node: Any)` — [`L169`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/tree_sitter_compat.py#L169) — Count total number of nodes in a tree using iterative traversal.
- `create_query_safely(language: Any, query_string: str)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/tree_sitter_compat.py#L99) — Safely create a tree-sitter query object.
- `get_node_text_safe(node: Any, source_code: str, encoding: str = "utf-8")` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/tree_sitter_compat.py#L119) — Safely extract text from a tree-sitter node. — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
- `log_api_info()` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/tree_sitter_compat.py#L138) — Log information about available tree-sitter APIs.

## Module values
- `logger` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/tree_sitter_compat.py#L21)

