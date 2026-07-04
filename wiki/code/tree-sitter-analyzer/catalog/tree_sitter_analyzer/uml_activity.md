---
title: 'Module: tree_sitter_analyzer/uml_activity.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/uml_activity.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.uml_activity`/
symbols:
  build_activity_cfg: build_activity_cfg().
  ActivityCFG.nodes: ActivityCFG#nodes.
  CFGNode.kind: CFGNode#kind.
  _CFGWalker.build: _CFGWalker#build().
  _CFGWalker._add_node: _CFGWalker#_add_node().
  _CFGWalker._handle_if: _CFGWalker#_handle_if().
  _CFGWalker._add_edge: _CFGWalker#_add_edge().
  CFGNode: CFGNode#
  _CFGWalker._handle_statement: _CFGWalker#_handle_statement().
  _parse_file_for_activity: _parse_file_for_activity().
  CFGNode.node_id: CFGNode#node_id.
  _CFGWalker._walk_body: _CFGWalker#_walk_body().
  _CFGWalker._handle_try: _CFGWalker#_handle_try().
  _CFGWalker._handle_loop: _CFGWalker#_handle_loop().
  ActivityCFG.truncated: ActivityCFG#truncated.
  _node_text: _node_text().
  ActivityCFG.edges: ActivityCFG#edges.
  _find_function_node: _find_function_node().
  ActivityCFG.error: ActivityCFG#error.
  CFGNode.label: CFGNode#label.
  _condition_text: _condition_text().
  ActivityCFG: ActivityCFG#
  CFGEdge.source_id: CFGEdge#source_id.
  _CFGWalker: _CFGWalker#
  CFGEdge.label: CFGEdge#label.
  _CFGWalker._nodes: _CFGWalker#_nodes.
  CFGEdge.target_id: CFGEdge#target_id.
  _CFGWalker._pending_edge_label: _CFGWalker#_pending_edge_label.
  _CFGWalker._edges: _CFGWalker#_edges.
  _CFGWalker._new_id: _CFGWalker#_new_id().
  CFGEdge: CFGEdge#
  _CFGWalker._truncated: _CFGWalker#_truncated.
  _CFGWalker._counter: _CFGWalker#_counter.
  _CFGWalker._function_name: _CFGWalker#_function_name.
  _CFGWalker._max_nodes: _CFGWalker#_max_nodes.
  _CFGWalker.__init__: _CFGWalker#__init__().
  _CFG_NODE_TYPES._CFG_NODE_TYPES: _CFG_NODE_TYPES._CFG_NODE_TYPES.
---
# Module: [`tree_sitter_analyzer/uml_activity.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py)

## Classes
### `ActivityCFG`
- def: [`tree_sitter_analyzer/uml_activity.py:47`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L47)
- doc: Result of an activity-diagram walk.
- signature: `class ActivityCFG:`
- members:
  - `edges` — [`L51`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L51)
  - `error` — [`L53`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L53)
  - `nodes` — [`L50`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L50)
  - `truncated` — [`L52`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L52)
- uses (calls/refs, reference-scoped): [`CFGNode`](uml_activity.md#CFGNode), [`CFGEdge`](uml_activity.md#CFGEdge)
- used by: [`activity_diagram`](uml_export.md#UMLExporter.activity_diagram), [`build_activity_cfg`](uml_activity.md#build_activity_cfg), [`build`](uml_activity.md#_CFGWalker.build)  (30 test-only)

### `CFGEdge`
- def: [`tree_sitter_analyzer/uml_activity.py:38`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L38)
- doc: A directed edge between two CFG nodes.
- signature: `class CFGEdge:`
- members:
  - `label` — [`L43`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L43)
  - `source_id` — [`L41`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L41)
  - `target_id` — [`L42`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L42)
- used by: [`activity_diagram`](uml_export.md#UMLExporter.activity_diagram), [`_add_edge`](uml_activity.md#_CFGWalker._add_edge), [`edges`](uml_activity.md#ActivityCFG.edges), [`_edges`](uml_activity.md#_CFGWalker._edges)  (5 test-only)

### `CFGNode`
- def: [`tree_sitter_analyzer/uml_activity.py:27`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L27)
- doc: A single node in the control-flow graph.
- signature: `class CFGNode:`
- members:
  - `kind` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L32) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
  - `label` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L31)
  - `node_id` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L30) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
- used by: [`activity_diagram`](uml_export.md#UMLExporter.activity_diagram), [`build_activity_cfg`](uml_activity.md#build_activity_cfg), [`nodes`](uml_activity.md#ActivityCFG.nodes), [`build`](uml_activity.md#_CFGWalker.build), [`_add_node`](uml_activity.md#_CFGWalker._add_node), [`_handle_if`](uml_activity.md#_CFGWalker._handle_if), [`_add_edge`](uml_activity.md#_CFGWalker._add_edge), [`_handle_statement`](uml_activity.md#_CFGWalker._handle_statement), [`_handle_try`](uml_activity.md#_CFGWalker._handle_try), [`_walk_body`](uml_activity.md#_CFGWalker._walk_body), [`_handle_loop`](uml_activity.md#_CFGWalker._handle_loop), [`_nodes`](uml_activity.md#_CFGWalker._nodes)  (25 test-only)

### `_CFGWalker`
- def: [`tree_sitter_analyzer/uml_activity.py:202`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L202)
- doc: Stateful walker that builds a CFG from a tree-sitter function body.
- signature: `class _CFGWalker:`
- members:
  - `_handle_statement(self, node: Any, incoming: list[CFGNode])` — [`L289`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L289) — Process one AST node. Returns updated live set, or None to skip.
  - `_walk_body(self, body_node: Any, incoming: list[CFGNode])` — [`L274`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L274) — Walk statement children, threading incoming/outgoing node sets.
  - `build(self, func_node: Any)` — [`L240`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L240) — Walk function body and build the CFG. Returns ActivityCFG.
- protocol/private: `__init__`[`L205`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L205), `_add_edge`[`L233`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L233), `_add_node`[`L221`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L221), `_counter`[`L210`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L210), `_edges`[`L209`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L209), `_function_name`[`L206`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L206), `_handle_if`[`L319`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L319), `_handle_loop`[`L380`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L380), `_handle_try`[`L398`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L398), `_max_nodes`[`L207`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L207), `_new_id`[`L217`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L217), `_nodes`[`L208`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L208), `_pending_edge_label`[`L215`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L215), `_truncated`[`L211`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L211)
- uses (calls/refs, reference-scoped): [`nodes`](uml_activity.md#ActivityCFG.nodes), [`kind`](uml_activity.md#CFGNode.kind), [`CFGNode`](uml_activity.md#CFGNode), [`node_id`](uml_activity.md#CFGNode.node_id), [`_node_text`](uml_activity.md#_node_text), [`truncated`](uml_activity.md#ActivityCFG.truncated), [`edges`](uml_activity.md#ActivityCFG.edges), [`label`](uml_activity.md#CFGNode.label), [`_condition_text`](uml_activity.md#_condition_text), [`ActivityCFG`](uml_activity.md#ActivityCFG), [`CFGEdge`](uml_activity.md#CFGEdge)
- used by: [`build_activity_cfg`](uml_activity.md#build_activity_cfg)  (3 test-only)

## Functions
- `_condition_text(node: Any)` — [`L87`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L87) — Extract condition text from an if/while/for node.
- `_find_function_node(root: Any, function_name: str)` — [`L156`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L156) — DFS preorder search for a function_definition node named *function_name*.
- `_node_text(node: Any, max_len: int = 40)` — [`L73`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L73) — Decode a tree-sitter node's text, capped at max_len chars.
- `_parse_file_for_activity(file_path: str, language: str = "python")` — [`L132`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L132) — Parse *file_path* with tree-sitter and return (tree_root, source_bytes).
- `build_activity_cfg(function_name: str, file_path: str, max_nodes: int = 50, language: str = "python")` — [`L441`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L441) — Parse *file_path* and build a CFG for *function_name*. — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)

## Module values
- `_CFG_NODE_TYPES` — [`L61`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_activity.py#L61)

