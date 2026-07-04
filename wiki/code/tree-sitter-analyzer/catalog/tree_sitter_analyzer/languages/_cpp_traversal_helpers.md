---
title: 'Module: tree_sitter_analyzer/languages/_cpp_traversal_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_cpp_traversal_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._cpp_traversal_helpers`/
symbols:
  traverse_and_extract_iterative: traverse_and_extract_iterative().
  _extract_node: _extract_node().
  _traversal_state: _traversal_state().
  CppTraversalState: CppTraversalState#
  CppTraversalState.processed_nodes: CppTraversalState#processed_nodes.
  CppTraversalState.element_cache: CppTraversalState#element_cache.
  CppTraversalState.extractors: CppTraversalState#extractors.
  CppTraversalState.results: CppTraversalState#results.
  _should_skip_node: _should_skip_node().
  CppTraversalState.element_type: CppTraversalState#element_type.
  _append_extracted: _append_extracted().
  _CONTAINER_NODE_TYPES: _CONTAINER_NODE_TYPES.
---
# Module: [`tree_sitter_analyzer/languages/_cpp_traversal_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_traversal_helpers.py)

## Classes
### `CppTraversalState`
- def: [`tree_sitter_analyzer/languages/_cpp_traversal_helpers.py:30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_traversal_helpers.py#L30)
- signature: `class CppTraversalState:`
- members:
  - `element_cache` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_traversal_helpers.py#L35)
  - `element_type` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_traversal_helpers.py#L33)
  - `extractors` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_traversal_helpers.py#L31)
  - `processed_nodes` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_traversal_helpers.py#L34)
  - `results` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_traversal_helpers.py#L32)
- used by: [`_traverse_and_extract_iterative`](cpp_plugin.md#CppElementExtractor._traverse_and_extract_iterative), [`traverse_and_extract_iterative`](_cpp_traversal_helpers.md#traverse_and_extract_iterative), [`_extract_node`](_cpp_traversal_helpers.md#_extract_node), [`_traversal_state`](_cpp_traversal_helpers.md#_traversal_state)

## Functions
- `_append_extracted(results: list[Any], element: Any)` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_traversal_helpers.py#L118)
- `_extract_node(node: Any, state: CppTraversalState)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_traversal_helpers.py#L81)
- `_should_skip_node(node: Any, depth: int, target_node_types: set[str])` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_traversal_helpers.py#L73)
- `_traversal_state(state: CppTraversalState | dict[str, Any], *legacy_args: Any)` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_traversal_helpers.py#L101)
- `traverse_and_extract_iterative(root_node: Any, state: CppTraversalState | dict[str, Any], *legacy_args: Any)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_traversal_helpers.py#L38) — Iterative node traversal and extraction with caching.

## Module values
- `_CONTAINER_NODE_TYPES` — [`L8`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_traversal_helpers.py#L8)

