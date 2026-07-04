---
title: 'Module: tree_sitter_analyzer/call_path.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/call_path.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.call_path`/
symbols:
  CallPathResult.paths: CallPathResult#paths.
  CallPathFinder._fallback_graph: CallPathFinder#_fallback_graph().
  CallPathFinder.find_path: CallPathFinder#find_path().
  CallPathFinder: CallPathFinder#
  CallPathFinder._bidirectional_sql: CallPathFinder#_bidirectional_sql().
  CallPathFinder._bfs_sql_forward: CallPathFinder#_bfs_sql_forward().
  CallPathFinder._bfs_sql_backward: CallPathFinder#_bfs_sql_backward().
  CallPathResult.to_dict: CallPathResult#to_dict().
  CallPathFinder._try_get_cache: CallPathFinder#_try_get_cache().
  _make_chain: _make_chain().
  CallChain: CallChain#
  CallChain.hops: CallChain#hops.
  CallPathResult.data_source: CallPathResult#data_source.
  CallPathFinder._bfs_graph_backward: CallPathFinder#_bfs_graph_backward().
  CallPathResult: CallPathResult#
  CallPathFinder._bfs_graph_forward: CallPathFinder#_bfs_graph_forward().
  CallChain.to_dict: CallChain#to_dict().
  CallChain.total_hops: CallChain#total_hops.
  CallPathResult.source: CallPathResult#source.
  CallPathResult.target: CallPathResult#target.
  _path_signature: _path_signature().
  CallChain.files_crossed: CallChain#files_crossed.
  _bfs_sql_core: _bfs_sql_core().
  _bfs_graph_core: _bfs_graph_core().
  CallPathFinder._query_forward_edges: CallPathFinder#_query_forward_edges().
  CallPathFinder._query_backward_edges: CallPathFinder#_query_backward_edges().
  CallPathResult.truncated: CallPathResult#truncated.
  _files_in_chain: _files_in_chain().
  logger: logger.
  _FORWARD_EDGE_SELECT: _FORWARD_EDGE_SELECT.
  _BACKWARD_EDGE_SELECT: _BACKWARD_EDGE_SELECT.
  CallPathFinder._cache: CallPathFinder#_cache.
  _target_match: _target_match().
  _lookup_in_visited: _lookup_in_visited().
  CallPathFinder._project_root: CallPathFinder#_project_root.
  _fwd_state: _fwd_state().
  _fwd_hop: _fwd_hop().
  _bwd_state: _bwd_state().
  _bwd_hop: _bwd_hop().
  _graph_fwd_state: _graph_fwd_state().
  _graph_fwd_hop: _graph_fwd_hop().
  _graph_bwd_state: _graph_bwd_state().
  _graph_bwd_hop: _graph_bwd_hop().
  CallPathFinder._data_source: CallPathFinder#_data_source.
  CallPathFinder.__init__: CallPathFinder#__init__().
---
# Module: [`tree_sitter_analyzer/call_path.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py)

## Classes
### `CallChain`
- def: [`tree_sitter_analyzer/call_path.py:277`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L277)
- doc: A single call chain from source to target.
- signature: `class CallChain:`
- members:
  - `to_dict(self)` — [`L284`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L284)
  - `files_crossed` — [`L282`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L282)
  - `hops` — [`L280`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L280)
  - `total_hops` — [`L281`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L281)
- used by: [`paths`](call_path.md#CallPathResult.paths), [`_fallback_graph`](call_path.md#CallPathFinder._fallback_graph), [`_bidirectional_sql`](call_path.md#CallPathFinder._bidirectional_sql), [`execute`](mcp/tools/call_path_tool.md#CodeGraphCallPathTool.execute), [`to_dict`](call_path.md#CallPathResult.to_dict), [`_make_chain`](call_path.md#_make_chain), [`_bfs_graph_backward`](call_path.md#CallPathFinder._bfs_graph_backward), [`_bfs_graph_forward`](call_path.md#CallPathFinder._bfs_graph_forward)  (13 test-only)

### `CallPathFinder`
- def: [`tree_sitter_analyzer/call_path.py:353`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L353)
- doc: Find execution paths between two functions via BFS on call edges.
- signature: `class CallPathFinder:`
- members:
  - `find_path(self, source_function: str, target_function: str, source_file: str | None = None, target_file: str | None = None, max_depth: int = 10, max_paths: int = 5, direction: str = "forward")` — [`L386`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L386) — Find call paths from *source_function* to *target_function*.
- protocol/private: `__init__`[`L366`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L366), `_bfs_graph_backward`[`L812`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L812), `_bfs_graph_forward`[`L788`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L788), `_bfs_sql_backward`[`L491`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L491), `_bfs_sql_forward`[`L462`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L462), `_bidirectional_sql`[`L520`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L520), `_cache`[`L368`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L368), `_data_source`[`L369`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L369), `_fallback_graph`[`L701`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L701), `_project_root`[`L367`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L367), `_query_backward_edges`[`L673`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L673), `_query_forward_edges`[`L640`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L640), `_try_get_cache`[`L371`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L371)
- uses (calls/refs, reference-scoped): [`ASTCache`](ast_cache.md#ASTCache), [`close`](ast_cache.md#ASTCache.close), [`CallGraph`](call_graph.md#CallGraph), [`build`](call_graph.md#CallGraph.build), [`paths`](call_path.md#CallPathResult.paths), [`get_stats`](ast_cache.md#ASTCache.get_stats), [`has_call_edges`](ast_cache.md#ASTCache.has_call_edges), [`_make_chain`](call_path.md#_make_chain), [`CallChain`](call_path.md#CallChain), [`data_source`](call_path.md#CallPathResult.data_source), [`hops`](call_path.md#CallChain.hops), [`CallPathResult`](call_path.md#CallPathResult), [`_path_signature`](call_path.md#_path_signature), [`source`](call_path.md#CallPathResult.source), [`target`](call_path.md#CallPathResult.target), [`_bfs_graph_core`](call_path.md#_bfs_graph_core), [`_bfs_sql_core`](call_path.md#_bfs_sql_core), [`truncated`](call_path.md#CallPathResult.truncated), [`logger`](call_path.md#logger), [`_BACKWARD_EDGE_SELECT`](call_path.md#_BACKWARD_EDGE_SELECT), [`_FORWARD_EDGE_SELECT`](call_path.md#_FORWARD_EDGE_SELECT), [`_lookup_in_visited`](call_path.md#_lookup_in_visited), [`_bwd_hop`](call_path.md#_bwd_hop), [`_bwd_state`](call_path.md#_bwd_state), [`_fwd_hop`](call_path.md#_fwd_hop), [`_fwd_state`](call_path.md#_fwd_state), [`_graph_bwd_hop`](call_path.md#_graph_bwd_hop), [`_graph_bwd_state`](call_path.md#_graph_bwd_state), [`_graph_fwd_hop`](call_path.md#_graph_fwd_hop), [`_graph_fwd_state`](call_path.md#_graph_fwd_state)
- used by: [`sequence_diagram`](uml_export.md#UMLExporter.sequence_diagram), [`execute`](mcp/tools/call_path_tool.md#CodeGraphCallPathTool.execute), [`_enrich_with_bodies`](mcp/tools/call_path_tool.md#CodeGraphCallPathTool._enrich_with_bodies), [`_get_finder`](mcp/tools/call_path_tool.md#CodeGraphCallPathTool._get_finder), [`__init__`](mcp/tools/call_path_tool.md#CodeGraphCallPathTool.__init__)  (25 test-only)

### `CallPathResult`
- def: [`tree_sitter_analyzer/call_path.py:293`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L293)
- doc: Result of a call path search.
- signature: `class CallPathResult:`
- members:
  - `to_dict(self)` — [`L302`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L302)
  - `data_source` — [`L299`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L299)
  - `paths` — [`L298`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L298)
  - `source` — [`L296`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L296)
  - `target` — [`L297`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L297)
  - `truncated` — [`L300`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L300)
- uses (calls/refs, reference-scoped): [`CallChain`](call_path.md#CallChain), [`to_dict`](call_path.md#CallChain.to_dict)
- used by: [`sequence_diagram`](uml_export.md#UMLExporter.sequence_diagram), [`_fallback_graph`](call_path.md#CallPathFinder._fallback_graph), [`find_path`](call_path.md#CallPathFinder.find_path), [`_bidirectional_sql`](call_path.md#CallPathFinder._bidirectional_sql), [`_bfs_sql_backward`](call_path.md#CallPathFinder._bfs_sql_backward), [`_bfs_sql_forward`](call_path.md#CallPathFinder._bfs_sql_forward), [`execute`](mcp/tools/call_path_tool.md#CodeGraphCallPathTool.execute)  (25 test-only)

## Functions
- `_bfs_graph_core(get_neighbors: Callable, start_name: str, start_file: str | None, target_key: tuple[str, str | None], max_depth: int, max_paths: int, paths: list[Any], state_fn: Callable, hop_fn: Callable, prepend: bool)` — [`L244`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L244) — BFS over an in-memory CallGraph in one direction.
- `_bfs_sql_core(conn: sqlite3.Connection, start_name: str, start_file: str | None, target_key: tuple[str, str | None], max_depth: int, max_paths: int, query_fn: Callable, state_fn: Callable, hop_fn: Callable, prepend: bool)` — [`L210`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L210) — BFS over the unified ``edges`` table in one direction (forward/backward).
- `_bwd_hop(current_name: str, current_file: str | None, row: dict[str, Any])` — [`L98`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L98) — Build a hop dict for a backward (caller direction) step.
- `_bwd_state(row: dict[str, Any])` — [`L93`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L93) — Extract the next (name, file) state from a backward-edge row.
- `_files_in_chain(hops: list[dict[str, Any]])` — [`L313`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L313)
- `_fwd_hop(current_name: str, current_file: str | None, row: dict[str, Any])` — [`L70`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L70) — Build a hop dict for a forward (callee direction) step.
- `_fwd_state(row: dict[str, Any])` — [`L60`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L60) — Extract the next (name, file) state from a forward-edge row.
- `_graph_bwd_hop(current_name: str, current_file: str | None, caller: dict[str, Any])` — [`L145`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L145)
- `_graph_bwd_state(caller: dict[str, Any])` — [`L141`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L141)
- `_graph_fwd_hop(current_name: str, current_file: str | None, callee: dict[str, Any])` — [`L124`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L124)
- `_graph_fwd_state(callee: dict[str, Any])` — [`L120`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L120)
- `_lookup_in_visited(state: tuple[str, str | None], visited: dict[tuple[str, str | None], list[dict[str, Any]]])` — [`L176`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L176) — Lookup *state* in *visited*, also accepting a name-only (file=None) wildcard.
- `_make_chain(path: list[dict[str, Any]])` — [`L322`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L322) — Construct a CallChain from a hop list.
- `_path_signature(path: list[dict[str, Any]])` — [`L329`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L329) — Stable signature for a hop list, used to dedup equivalent paths.
- `_target_match(name: str, file_: str | None, target: tuple[str, str | None])` — [`L162`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L162) — Return True when (name, file_) matches the target (name, file) pair.

## Module values
- `_BACKWARD_EDGE_SELECT` — [`L46`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L46)
- `_FORWARD_EDGE_SELECT` — [`L38`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L38)
- `logger` — [`L25`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_path.py#L25)

