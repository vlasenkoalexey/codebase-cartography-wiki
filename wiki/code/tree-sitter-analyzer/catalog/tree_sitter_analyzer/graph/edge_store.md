---
title: 'Module: tree_sitter_analyzer/graph/edge_store.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/graph/edge_store.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.graph.edge_store`/
symbols:
  EdgeKind: EdgeKind#
  symbol_node: symbol_node().
  Edge: Edge#
  EdgeKind.CALLS: EdgeKind#CALLS.
  EdgeStore: EdgeStore#
  EdgeStore.upsert_edges: EdgeStore#upsert_edges().
  parse_node_id: parse_node_id().
  EdgeStore.get_neighbors: EdgeStore#get_neighbors().
  EdgeStore.get_edges: EdgeStore#get_edges().
  NodeRef.name: NodeRef#name.
  _bfs_call_edges: _bfs_call_edges().
  _edge_real_columns: _edge_real_columns().
  Edge.metadata: Edge#metadata.
  _edge_from_row: _edge_from_row().
  EdgeStore._conn: EdgeStore#_conn.
  NodeRef.file_path: NodeRef#file_path.
  EdgeStore.close: EdgeStore#close().
  _direct_callers: _direct_callers().
  EdgeStore.get_inheritance_tree: EdgeStore#get_inheritance_tree().
  Edge.to_dict: Edge#to_dict().
  _call_edge_entry: _call_edge_entry().
  EdgeKind.EXTENDS: EdgeKind#EXTENDS.
  NodeRef.line: NodeRef#line.
  _direct_callees: _direct_callees().
  EdgeStore.has_edges: EdgeStore#has_edges().
  Edge.target_node_id: Edge#target_node_id.
  EdgeStore.conn: EdgeStore#conn().
  EdgeStore.replace_edges_for_file: EdgeStore#replace_edges_for_file().
  EdgeStore.query_callers: EdgeStore#query_callers().
  EDGE_STORE_SCHEMA: EDGE_STORE_SCHEMA.
  EdgeStore.query_callees: EdgeStore#query_callees().
  Edge.source_node_id: Edge#source_node_id.
  NodeRef: NodeRef#
  _matches_callee: _matches_callee().
  backfill_edge_name_columns: backfill_edge_name_columns().
  Edge.normalized_kind: Edge#normalized_kind().
  ensure_edge_schema: ensure_edge_schema().
  file_node: file_node().
  Subgraph.to_dict: Subgraph#to_dict().
  _row_col: _row_col().
  EdgeStore.ensure_schema: EdgeStore#ensure_schema().
  Edge.line: Edge#line.
  EdgeStore._commit_if_owned: EdgeStore#_commit_if_owned().
  Subgraph.edges: Subgraph#edges.
  EdgeStore.backfill_name_columns: EdgeStore#backfill_name_columns().
  class_node: class_node().
  Edge.kind: Edge#kind.
  Subgraph.nodes: Subgraph#nodes.
  _callers_by_name: _callers_by_name().
  _callees_by_name: _callees_by_name().
  EdgeStore._owns_conn: EdgeStore#_owns_conn.
  _kind_value: _kind_value().
  EdgeKind.IMPLEMENTS: EdgeKind#IMPLEMENTS.
  Edge.provenance: Edge#provenance.
  Subgraph: Subgraph#
  EDGE_STORE_SCHEMA_STATEMENTS.EDGE_STORE_SCHEMA_STATEMENTS: EDGE_STORE_SCHEMA_STATEMENTS.EDGE_STORE_SCHEMA_STATEMENTS.
  EdgeKind.IMPORTS: EdgeKind#IMPORTS.
  EdgeKind.REFERENCES: EdgeKind#REFERENCES.
  EdgeKind.CONTAINS: EdgeKind#CONTAINS.
  module_node: module_node().
  _as_int: _as_int().
  _edge_query_with_kind: _edge_query_with_kind().
  _edge_query_without_kind: _edge_query_without_kind().
  _EDGE_NAME_COLUMNS._EDGE_NAME_COLUMNS: _EDGE_NAME_COLUMNS._EDGE_NAME_COLUMNS.
  EdgeKind.OVERRIDES: EdgeKind#OVERRIDES.
  EdgeKind.TYPE_OF: EdgeKind#TYPE_OF.
  EdgeKind.RETURNS: EdgeKind#RETURNS.
  EdgeKind.INSTANTIATES: EdgeKind#INSTANTIATES.
  EdgeKind.DECORATES: EdgeKind#DECORATES.
  EdgeStore.__init__: EdgeStore#__init__().
---
# Module: [`tree_sitter_analyzer/graph/edge_store.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py)

## Classes
### `Edge`
- def: [`tree_sitter_analyzer/graph/edge_store.py:34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L34) — documented in [tree_sitter_analyzer-ast_cache](../../../concepts/tree_sitter_analyzer-ast_cache.md)
- doc: One directed relationship between two indexed code nodes.
- signature: `class Edge:`
- members:
  - `normalized_kind(self)` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L44)
  - `to_dict(self)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L47)
  - `kind` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L39)
  - `line` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L40)
  - `metadata` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L42)
  - `provenance` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L41)
  - `source_node_id` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L37)
  - `target_node_id` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L38)
- uses (calls/refs, reference-scoped): [`EdgeKind`](edge_store.md#EdgeKind)
- used by: [`write_graph_edges_for_file`](../_ast_cache_write.md#write_graph_edges_for_file), [`upsert_edges`](edge_store.md#EdgeStore.upsert_edges), [`get_neighbors`](edge_store.md#EdgeStore.get_neighbors), [`get_edges`](edge_store.md#EdgeStore.get_edges), [`_bfs_call_edges`](edge_store.md#_bfs_call_edges), [`_edge_real_columns`](edge_store.md#_edge_real_columns), [`_edge_from_row`](edge_store.md#_edge_from_row), [`_resolved_edge`](../_ast_cache_unresolved.md#_resolved_edge), [`_direct_callers`](edge_store.md#_direct_callers), [`get_inheritance_tree`](edge_store.md#EdgeStore.get_inheritance_tree), [`_call_edge_entry`](edge_store.md#_call_edge_entry), [`_direct_callees`](edge_store.md#_direct_callees), [`replace_edges_for_file`](edge_store.md#EdgeStore.replace_edges_for_file), [`to_dict`](edge_store.md#Subgraph.to_dict), [`_row_col`](edge_store.md#_row_col), [`edges`](edge_store.md#Subgraph.edges)  (15 test-only)

### `EdgeKind`  ·  implements/extends Enum, str
- def: [`tree_sitter_analyzer/graph/edge_store.py:17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L17) — documented in [tree_sitter_analyzer-ast_cache](../../../concepts/tree_sitter_analyzer-ast_cache.md)
- doc: Supported code relationship edge kinds.
- signature: `class EdgeKind(str, Enum):`
- members:
  - `CALLS` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L20) — documented in [tree_sitter_analyzer-ast_cache](../../../concepts/tree_sitter_analyzer-ast_cache.md)
  - `CONTAINS` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L25)
  - `DECORATES` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L30)
  - `EXTENDS` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L22)
  - `IMPLEMENTS` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L23)
  - `IMPORTS` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L21)
  - `INSTANTIATES` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L29)
  - `OVERRIDES` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L26)
  - `REFERENCES` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L24)
  - `RETURNS` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L28)
  - `TYPE_OF` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L27)
- used by: [`write_graph_edges_for_file`](../_ast_cache_write.md#write_graph_edges_for_file), [`get_neighbors`](edge_store.md#EdgeStore.get_neighbors), [`resolve_unresolved_refs`](../_ast_cache_unresolved.md#resolve_unresolved_refs), [`_build_edges_from_edge_store`](../class_hierarchy.md#ClassHierarchy._build_edges_from_edge_store), [`get_edges`](edge_store.md#EdgeStore.get_edges), [`has_call_edges`](../ast_cache.md#ASTCache.has_call_edges), [`query_callees`](../ast_cache.md#ASTCache.query_callees), [`_get_call_graph`](../mcp/tools/codegraph_context_tool.md#CodeGraphContextTool._get_call_graph), [`_call_refs`](../_ast_cache_unresolved.md#_call_refs), [`query_callers`](../ast_cache.md#ASTCache.query_callers), [`_resolved_edge`](../_ast_cache_unresolved.md#_resolved_edge), [`_candidate_symbols`](../_ast_cache_unresolved.md#_candidate_symbols), [`_update_call_edge_resolution`](../_ast_cache_unresolved.md#_update_call_edge_resolution), [`get_inheritance_tree`](edge_store.md#EdgeStore.get_inheritance_tree), [`_parent_refs`](../_ast_cache_unresolved.md#_parent_refs), [`has_edges`](edge_store.md#EdgeStore.has_edges), [`normalized_kind`](edge_store.md#Edge.normalized_kind), [`kind`](edge_store.md#Edge.kind), [`_callees_by_name`](edge_store.md#_callees_by_name), [`_callers_by_name`](edge_store.md#_callers_by_name), [`_kind_value`](edge_store.md#_kind_value)  (25 test-only)

### `EdgeStore`
- def: [`tree_sitter_analyzer/graph/edge_store.py:194`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L194) — documented in [tree_sitter_analyzer-ast_cache](../../../concepts/tree_sitter_analyzer-ast_cache.md)
- doc: CRUD and traversal API for the unified `edges` table.
- signature: `class EdgeStore:`
- members:
  - `backfill_name_columns(self)` — [`L286`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L286) — Populate caller_name/callee_name/file_path for pre-v10 rows.
  - `close(self)` — [`L220`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L220)
  - `conn(self)` — [`L213`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L213)
  - `ensure_schema(self)` — [`L216`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L216)
  - `get_edges(self, node_id: str, kind: EdgeKind | str | None = None, direction: str = "outgoing")` — [`L338`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L338) — Return edges touching ``node_id`` in one direction or both. — documented in [tree_sitter_analyzer-graph-edge_store](../../../concepts/tree_sitter_analyzer-graph-edge_store.md)
  - `get_inheritance_tree(self, class_name: str)` — [`L390`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L390) — Return inheritance edges whose target is ``class_name``.
  - `get_neighbors(self, node_id: str, depth: int = 2, kinds: list[EdgeKind | str] | None = None)` — [`L354`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L354) — Breadth-first outgoing traversal from ``node_id``. — documented in [tree_sitter_analyzer-graph-edge_store](../../../concepts/tree_sitter_analyzer-graph-edge_store.md)
  - `has_edges(self, kind: EdgeKind | str | None = None)` — [`L326`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L326) — Return true when the store contains at least one edge. — documented in [tree_sitter_analyzer-graph-edge_store](../../../concepts/tree_sitter_analyzer-graph-edge_store.md)
  - `query_callees(self, caller_name: str, caller_file: str | None = None, max_depth: int = 1)` — [`L428`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L428) — Return callees of ``caller_name`` from unified CALLS edges.
  - `query_callers(self, callee_name: str, callee_file: str | None = None, max_depth: int = 1)` — [`L413`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L413) — Return callers of ``callee_name`` from unified CALLS edges.
  - `replace_edges_for_file(self, file_path: str, edges: list[Edge], *, preserve_calls: bool = False)` — [`L224`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L224) — Replace all edges whose source belongs to ``file_path``. — documented in [tree_sitter_analyzer-graph-edge_store](../../../concepts/tree_sitter_analyzer-graph-edge_store.md)
  - `upsert_edges(self, edges: list[Edge])` — [`L291`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L291) — documented in [tree_sitter_analyzer-graph-edge_store](../../../concepts/tree_sitter_analyzer-graph-edge_store.md)
- protocol/private: `__init__`[`L197`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L197), `_commit_if_owned`[`L322`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L322), `_conn`[`L205`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L205), `_owns_conn`[`L203`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L203)
- uses (calls/refs, reference-scoped): [`EdgeKind`](edge_store.md#EdgeKind), [`Edge`](edge_store.md#Edge), [`_bfs_call_edges`](edge_store.md#_bfs_call_edges), [`_edge_real_columns`](edge_store.md#_edge_real_columns), [`metadata`](edge_store.md#Edge.metadata), [`_edge_from_row`](edge_store.md#_edge_from_row), [`to_dict`](edge_store.md#Edge.to_dict), [`EXTENDS`](edge_store.md#EdgeKind.EXTENDS), [`target_node_id`](edge_store.md#Edge.target_node_id), [`source_node_id`](edge_store.md#Edge.source_node_id), [`backfill_edge_name_columns`](edge_store.md#backfill_edge_name_columns), [`ensure_edge_schema`](edge_store.md#ensure_edge_schema), [`file_node`](edge_store.md#file_node), [`normalized_kind`](edge_store.md#Edge.normalized_kind), [`line`](edge_store.md#Edge.line), [`edges`](edge_store.md#Subgraph.edges), [`class_node`](edge_store.md#class_node), [`nodes`](edge_store.md#Subgraph.nodes), [`_kind_value`](edge_store.md#_kind_value), [`IMPLEMENTS`](edge_store.md#EdgeKind.IMPLEMENTS), [`provenance`](edge_store.md#Edge.provenance), [`Subgraph`](edge_store.md#Subgraph), [`_edge_query_with_kind`](edge_store.md#_edge_query_with_kind), [`_edge_query_without_kind`](edge_store.md#_edge_query_without_kind)
- used by: [`write_graph_edges_for_file`](../_ast_cache_write.md#write_graph_edges_for_file), [`resolve_unresolved_refs`](../_ast_cache_unresolved.md#resolve_unresolved_refs), [`_build_edges_from_edge_store`](../class_hierarchy.md#ClassHierarchy._build_edges_from_edge_store), [`has_call_edges`](../ast_cache.md#ASTCache.has_call_edges), [`query_callees`](../ast_cache.md#ASTCache.query_callees), [`query_callers`](../ast_cache.md#ASTCache.query_callers), [`_get_edge_store`](../mcp/tools/codegraph_context_tool.md#CodeGraphContextTool._get_edge_store)  (23 test-only)

### `NodeRef`
- def: [`tree_sitter_analyzer/graph/edge_store.py:73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L73)
- doc: Parsed node id components used by graph read paths.
- signature: `class NodeRef:`
- members:
  - `file_path` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L76)
  - `line` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L78)
  - `name` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L77)
- used by: [`parse_node_id`](edge_store.md#parse_node_id), [`_add_placeholder_node`](../knowledge_graph/builder.md#KnowledgeGraphBuilder._add_placeholder_node), [`_build_edges_from_edge_store`](../class_hierarchy.md#ClassHierarchy._build_edges_from_edge_store), [`_bfs_call_edges`](edge_store.md#_bfs_call_edges), [`_edge_real_columns`](edge_store.md#_edge_real_columns), [`_direct_callers`](edge_store.md#_direct_callers), [`_update_call_edge_resolution`](../_ast_cache_unresolved.md#_update_call_edge_resolution), [`_call_edge_entry`](edge_store.md#_call_edge_entry), [`_direct_callees`](edge_store.md#_direct_callees), [`_matches_callee`](edge_store.md#_matches_callee), [`backfill_edge_name_columns`](edge_store.md#backfill_edge_name_columns)  (1 test-only)

### `Subgraph`
- def: [`tree_sitter_analyzer/graph/edge_store.py:59`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L59)
- doc: A small reachable graph slice.
- signature: `class Subgraph:`
- members:
  - `to_dict(self)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L65)
  - `edges` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L63)
  - `nodes` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L62)
- uses (calls/refs, reference-scoped): [`Edge`](edge_store.md#Edge), [`to_dict`](edge_store.md#Edge.to_dict)
- used by: [`get_neighbors`](edge_store.md#EdgeStore.get_neighbors)  (4 test-only)

## Functions
- `_as_int(value: Any, default: int = 0)` — [`L516`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L516)
- `_bfs_call_edges(conn: sqlite3.Connection, start_name: str, start_file: str | None, max_depth: int, direction: str)` — [`L592`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L592)
- `_call_edge_entry(row: sqlite3.Row, edge: Edge, source: NodeRef, target: NodeRef, depth: int)` — [`L748`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L748)
- `_callees_by_name(conn: sqlite3.Connection, caller_name: str, bare: str)` — [`L657`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L657) — CALLS rows whose caller matches ``caller_name``/``bare`` (index-backed).
- `_callers_by_name(conn: sqlite3.Connection, callee_name: str)` — [`L634`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L634) — CALLS rows whose callee matches ``callee_name`` (index-backed pushdown).
- `_direct_callees(conn: sqlite3.Connection, caller_name: str, caller_file: str | None)` — [`L705`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L705)
- `_direct_callers(conn: sqlite3.Connection, callee_name: str, callee_file: str | None)` — [`L674`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L674)
- `_edge_from_row(row: sqlite3.Row)` — [`L577`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L577) — documented in [tree_sitter_analyzer-graph-edge_store](../../../concepts/tree_sitter_analyzer-graph-edge_store.md)
- `_edge_query_with_kind(direction: str, node_id: str, kind_value: str)` — [`L531`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L531)
- `_edge_query_without_kind(direction: str, node_id: str)` — [`L555`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L555)
- `_edge_real_columns(edge: Edge)` — [`L485`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L485) — Derive every promoted real-column value for one ``Edge``. — documented in [tree_sitter_analyzer-graph-edge_store](../../../concepts/tree_sitter_analyzer-graph-edge_store.md)
- `_kind_value(kind: EdgeKind | str | None)` — [`L525`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L525)
- `_matches_callee(row: sqlite3.Row, target: NodeRef, callee_name: str)` — [`L742`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L742)
- `_row_col(row: sqlite3.Row, column: str, meta_key: str, edge: Edge)` — [`L723`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L723) — Read a promoted real column, falling back to the metadata JSON.
- `backfill_edge_name_columns(conn: sqlite3.Connection)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L173) — Populate caller_name/callee_name/file_path for pre-v10 rows.
- `class_node(class_name: str)` — [`L460`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L460)
- `ensure_edge_schema(conn: sqlite3.Connection)` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L156) — Create the ``edges`` table + indexes; ALTER legacy tables for new columns.
- `file_node(file_path: str)` — [`L452`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L452)
- `module_node(module_path: str)` — [`L456`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L456)
- `parse_node_id(node_id: str)` — [`L464`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L464) — Parse a stable node id into file/name/line components. — documented in [tree_sitter_analyzer-uml_export](../../../concepts/tree_sitter_analyzer-uml_export.md)
- `symbol_node(file_path: str, name: str, line: int | None = None)` — [`L444`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L444) — Build a stable file-scoped symbol node id. — documented in [tree_sitter_analyzer-ast_cache](../../../concepts/tree_sitter_analyzer-ast_cache.md)

## Module values
- `EDGE_STORE_SCHEMA` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L113)
- `EDGE_STORE_SCHEMA_STATEMENTS` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L81)
- `_EDGE_NAME_COLUMNS` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/graph/edge_store.py#L120)

