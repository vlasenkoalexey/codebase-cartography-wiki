---
title: 'Module: tree_sitter_analyzer/_ast_cache_graph.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_ast_cache_graph.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._ast_cache_graph`/
symbols:
  bfs_callers: bfs_callers().
  bfs_callees: bfs_callees().
  _EDGE_SELECT: _EDGE_SELECT.
  _CALLS_PREDICATE: _CALLS_PREDICATE.
  _fetch_caller_rows: _fetch_caller_rows().
  _fetch_callee_rows: _fetch_callee_rows().
  _bfs_traverse: _bfs_traverse().
  _caller_key: _caller_key().
  _caller_entry: _caller_entry().
  _caller_next_hop: _caller_next_hop().
  _callee_key: _callee_key().
  _callee_entry: _callee_entry().
  _callee_next_hop: _callee_next_hop().
---
# Module: [`tree_sitter_analyzer/_ast_cache_graph.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_graph.py)

## Functions
- `_bfs_traverse(conn: sqlite3.Connection, start_name: str, start_file: str | None, max_depth: int, fetch_rows: Callable, make_key: Callable, make_entry: Callable, next_hop: Callable)` — [`L162`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_graph.py#L162) — BFS traversal over the unified ``edges`` table in either direction.
- `_callee_entry(row: Any, depth: int)` — [`L138`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_graph.py#L138)
- `_callee_key(row: Any)` — [`L134`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_graph.py#L134)
- `_callee_next_hop(row: Any)` — [`L153`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_graph.py#L153)
- `_caller_entry(row: Any, depth: int)` — [`L116`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_graph.py#L116)
- `_caller_key(row: Any)` — [`L112`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_graph.py#L112)
- `_caller_next_hop(row: Any)` — [`L130`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_graph.py#L130)
- `_fetch_callee_rows(conn: sqlite3.Connection, name: str, file_: str | None)` — [`L73`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_graph.py#L73) — Return rows where *name*/*file_* is the caller (i.e. rows with callees).
- `_fetch_caller_rows(conn: sqlite3.Connection, name: str, file_: str | None)` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_graph.py#L39) — Return rows where *name*/*file_* is the callee (i.e. rows with callers).
- `bfs_callees(conn: sqlite3.Connection, caller_name: str, caller_file: str | None, max_depth: int)` — [`L239`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_graph.py#L239) — BFS traversal returning all callees of ``caller_name``.
- `bfs_callers(conn: sqlite3.Connection, callee_name: str, callee_file: str | None, max_depth: int)` — [`L208`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_graph.py#L208) — BFS traversal returning all callers of ``callee_name``.

## Module values
- `_CALLS_PREDICATE` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_graph.py#L32)
- `_EDGE_SELECT` — [`L25`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_graph.py#L25)

