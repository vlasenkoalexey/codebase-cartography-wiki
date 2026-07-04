---
title: 'Module: tree_sitter_analyzer/_ast_cache_callgraph_state.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_ast_cache_callgraph_state.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._ast_cache_callgraph_state`/
symbols:
  clear_call_graph_built: clear_call_graph_built().
  mark_call_graph_built: mark_call_graph_built().
  call_graph_built: call_graph_built().
  logger: logger.
  _CREATE_DDL: _CREATE_DDL.
---
# Module: [`tree_sitter_analyzer/_ast_cache_callgraph_state.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_callgraph_state.py)

## Functions
- `call_graph_built(conn: sqlite3.Connection)` — [`L53`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_callgraph_state.py#L53) — Return True iff this cache holds a built call graph.
- `clear_call_graph_built(conn: sqlite3.Connection)` — [`L36`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_callgraph_state.py#L36) — Clear the marker before replacing the derived call graph.
- `mark_call_graph_built(conn: sqlite3.Connection)` — [`L19`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_callgraph_state.py#L19) — Record that the call-graph derivation completed for this cache.

## Module values
- `_CREATE_DDL` — [`L11`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_callgraph_state.py#L11)
- `logger` — [`L9`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_callgraph_state.py#L9)

