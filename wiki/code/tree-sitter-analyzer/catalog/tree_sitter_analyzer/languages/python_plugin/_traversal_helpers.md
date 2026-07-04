---
title: 'Module: tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.python_plugin._traversal_helpers`/
symbols:
  run_iterative_traversal: run_iterative_traversal().
  _TraversalContext.run: _TraversalContext#run().
  _TraversalContext._is_cached_target: _TraversalContext#_is_cached_target().
  _TraversalContext._extract_uncached_target: _TraversalContext#_extract_uncached_target().
  _TraversalContext._should_visit_node_type: _TraversalContext#_should_visit_node_type().
  _TraversalContext.__post_init__: _TraversalContext#__post_init__().
  _TraversalContext.max_depth: _TraversalContext#max_depth.
  _TraversalContext._append_element: _TraversalContext#_append_element().
  _MAX_TRAVERSAL_DEPTH: _MAX_TRAVERSAL_DEPTH.
  TraversalRuntime: TraversalRuntime#
  _TraversalContext.element_cache: _TraversalContext#element_cache.
  _TraversalContext.processed_node_ids: _TraversalContext#processed_node_ids.
  _push_child_nodes: _push_child_nodes().
  _TraversalContext.extractors: _TraversalContext#extractors.
  _TraversalContext.results: _TraversalContext#results.
  _TraversalContext.target_node_types: _TraversalContext#target_node_types.
  TraversalRuntime.extractors: TraversalRuntime#extractors.
  TraversalRuntime.results: TraversalRuntime#results.
  TraversalRuntime.element_type: TraversalRuntime#element_type.
  TraversalRuntime.element_cache: TraversalRuntime#element_cache.
  TraversalRuntime.processed_node_ids: TraversalRuntime#processed_node_ids.
  TraversalRuntime.log_debug_fn: TraversalRuntime#log_debug_fn.
  TraversalRuntime.log_warning_fn: TraversalRuntime#log_warning_fn.
  _TraversalContext.element_type: _TraversalContext#element_type.
  _TraversalContext.log_warning_fn: _TraversalContext#log_warning_fn.
  _TraversalContext.processed_nodes: _TraversalContext#processed_nodes.
  _CONTAINER_NODE_TYPES: _CONTAINER_NODE_TYPES.
  _iter_child_nodes: _iter_child_nodes().
  _TraversalContext: _TraversalContext#
---
# Module: [`tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py)

## Classes
### `TraversalRuntime`
- def: [`tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py:31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L31)
- signature: `class TraversalRuntime:`
- members:
  - `element_cache` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L35)
  - `element_type` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L34)
  - `extractors` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L32)
  - `log_debug_fn` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L37)
  - `log_warning_fn` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L38)
  - `processed_node_ids` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L36)
  - `results` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L33)
- used by: [`run_iterative_traversal`](_traversal_helpers.md#run_iterative_traversal), [`_traverse_and_extract_iterative`](_core_extractor_mixin.md#PythonExtractorCoreMixin._traverse_and_extract_iterative)

### `_TraversalContext`
- def: [`tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py:61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L61)
- members:
  - `run(self, root_node: Any)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L75)
  - `element_cache` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L65)
  - `element_type` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L64)
  - `extractors` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L62)
  - `log_warning_fn` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L67)
  - `max_depth` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L70)
  - `processed_node_ids` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L66)
  - `processed_nodes` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L69)
  - `results` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L63)
  - `target_node_types` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L68)
- protocol/private: `__post_init__`[`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L72), `_append_element`[`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L138), `_extract_uncached_target`[`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L118), `_is_cached_target`[`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L101), `_should_visit_node_type`[`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L98)
- uses (calls/refs, reference-scoped): [`_MAX_TRAVERSAL_DEPTH`](_traversal_helpers.md#_MAX_TRAVERSAL_DEPTH), [`_push_child_nodes`](_traversal_helpers.md#_push_child_nodes), [`_CONTAINER_NODE_TYPES`](_traversal_helpers.md#_CONTAINER_NODE_TYPES)
- used by: [`run_iterative_traversal`](_traversal_helpers.md#run_iterative_traversal)

## Functions
- `_iter_child_nodes(current_node: Any)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L154)
- `_push_child_nodes(node_stack: list[tuple[Any, int]], current_node: Any, depth: int)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L147)
- `run_iterative_traversal(root_node: Any | None, runtime: TraversalRuntime)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L41) — Traverse the tree iteratively and append extracted elements.

## Module values
- `_CONTAINER_NODE_TYPES` — [`L9`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L9)
- `_MAX_TRAVERSAL_DEPTH` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.py#L27)

