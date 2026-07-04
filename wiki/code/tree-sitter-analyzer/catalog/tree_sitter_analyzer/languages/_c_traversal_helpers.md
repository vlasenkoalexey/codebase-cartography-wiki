---
title: 'Module: tree_sitter_analyzer/languages/_c_traversal_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_c_traversal_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._c_traversal_helpers`/
symbols:
  c_traverse_and_extract: c_traverse_and_extract().
  _depth_exceeded: _depth_exceeded().
  _should_visit_node: _should_visit_node().
  _process_target_node: _process_target_node().
  _append_extracted_element: _append_extracted_element().
  _push_children: _push_children().
  _C_CONTAINER_NODE_TYPES: _C_CONTAINER_NODE_TYPES.
---
# Module: [`tree_sitter_analyzer/languages/_c_traversal_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_traversal_helpers.py)

## Functions
- `_append_extracted_element(results: list[Any], element: Any)` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_traversal_helpers.py#L121)
- `_depth_exceeded(depth: int, max_depth: int)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_traversal_helpers.py#L83)
- `_process_target_node(node: Any, extractors: dict[str, Any], results: list[Any], element_type: str, processed_nodes: set[int], element_cache: dict[tuple[int, str], Any])` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_traversal_helpers.py#L96)
- `_push_children(node_stack: list[tuple[Any, int]], node: Any, depth: int)` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_traversal_helpers.py#L130)
- `_should_visit_node(node: Any, depth: int, target_node_types: set[str])` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_traversal_helpers.py#L90)
- `c_traverse_and_extract(root_node: Any, extractors: dict[str, Any], results: list[Any], element_type: str, processed_nodes: set[int], element_cache: dict[tuple[int, str], Any])` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_traversal_helpers.py#L40) — Iterative node traversal and extraction with caching for C.

## Module values
- `_C_CONTAINER_NODE_TYPES` — [`L7`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_traversal_helpers.py#L7)

