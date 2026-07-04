---
title: 'Module: tree_sitter_analyzer/languages/typescript_plugin/_traversal_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/typescript_plugin/_traversal_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.typescript_plugin._traversal_helpers`/
symbols:
  traverse_and_extract_iterative: traverse_and_extract_iterative().
  _process_target_node: _process_target_node().
  _append_element: _append_element().
  ExtractorMap.ExtractorMap: ExtractorMap.ExtractorMap.
  ElementCache.ElementCache: ElementCache.ElementCache.
  _container_node_types: _container_node_types().
  _should_skip_node: _should_skip_node().
  _extend_stack: _extend_stack().
---
# Module: [`tree_sitter_analyzer/languages/typescript_plugin/_traversal_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_traversal_helpers.py)

## Functions
- `_append_element(results: list[Any], element: Any)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_traversal_helpers.py#L140)
- `_container_node_types()` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_traversal_helpers.py#L66)
- `_extend_stack(current_node: tree_sitter.Node, depth: int, node_stack: list[tuple[tree_sitter.Node, int]])` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_traversal_helpers.py#L149)
- `_process_target_node(current_node: tree_sitter.Node, extractors: ExtractorMap, results: list[Any], element_type: str, processed_nodes: set[int], element_cache: ElementCache)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_traversal_helpers.py#L111)
- `_should_skip_node(depth: int, node_type: str, target_node_types: set[str], container_node_types: set[str])` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_traversal_helpers.py#L98)
- `traverse_and_extract_iterative(root_node: tree_sitter.Node | None, extractors: ExtractorMap, results: list[Any], element_type: str, processed_nodes: set[int], element_cache: ElementCache, max_depth: int = 50)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_traversal_helpers.py#L18) — Iterative node traversal and extraction with caching.

## Module values
- `ElementCache` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_traversal_helpers.py#L15)
- `ExtractorMap` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_traversal_helpers.py#L14)

