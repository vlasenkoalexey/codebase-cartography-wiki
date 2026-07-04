---
title: 'Module: tree_sitter_analyzer/languages/_java_traversal_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_java_traversal_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._java_traversal_helpers`/
symbols:
  java_traverse_and_extract: java_traverse_and_extract().
  _process_field_batch: _process_field_batch().
  _flush_field_batch: _flush_field_batch().
  _append_element: _append_element().
  _should_skip_node: _should_skip_node().
  _process_matched_node: _process_matched_node().
  _flush_field_batch_if_ready: _flush_field_batch_if_ready().
  _process_field_node: _process_field_node().
  _JAVA_CONTAINER_NODES: _JAVA_CONTAINER_NODES.
  _push_children: _push_children().
---
# Module: [`tree_sitter_analyzer/languages/_java_traversal_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_traversal_helpers.py)

## Functions
- `_append_element(results: list[Any], element: Any)` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_traversal_helpers.py#L120)
- `_flush_field_batch(field_batch: list[Any], extractors: dict[str, Any], results: list[Any], processed_nodes: set[int], element_cache: dict[tuple[int, str], Any])` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_traversal_helpers.py#L150)
- `_flush_field_batch_if_ready(field_batch: list[Any], extractors: dict[str, Any], results: list[Any], processed_nodes: set[int], element_cache: dict[tuple[int, str], Any])` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_traversal_helpers.py#L138)
- `_process_field_batch(batch: list[Any], extractors: dict[str, Any], results: list[Any], processed_nodes: set[int], element_cache: dict[tuple[int, str], Any])` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_traversal_helpers.py#L165) — Process field nodes with caching.
- `_process_field_node(node: Any, extractors: dict[str, Any], results: list[Any], processed_nodes: set[int], element_cache: dict[tuple[int, str], Any])` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_traversal_helpers.py#L177)
- `_process_matched_node(node: Any, extractors: dict[str, Any], results: list[Any], element_type: str, processed_nodes: set[int], element_cache: dict[tuple[int, str], Any], field_batch: list[Any])` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_traversal_helpers.py#L87)
- `_push_children(node_stack: list[tuple[Any, int]], current_node: Any, depth: int)` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_traversal_helpers.py#L129)
- `_should_skip_node(depth: int, node_type: str, target_node_types: set[str])` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_traversal_helpers.py#L79)
- `java_traverse_and_extract(root_node: Any, extractors: dict[str, Any], results: list[Any], element_type: str, processed_nodes: set[int], element_cache: dict[tuple[int, str], Any], *, log_warning_func: Callable[[str], None], log_debug_func: Callable[[str], None])` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_traversal_helpers.py#L28) — Iterative node traversal and extraction with batch field processing.

## Module values
- `_JAVA_CONTAINER_NODES` — [`L6`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_traversal_helpers.py#L6)

