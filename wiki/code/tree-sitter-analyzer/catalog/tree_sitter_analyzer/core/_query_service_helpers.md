---
title: 'Module: tree_sitter_analyzer/core/_query_service_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/core/_query_service_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.core._query_service_helpers`/
symbols:
  fallback_query_captures: fallback_query_captures().
  plugin_strategy_captures: plugin_strategy_captures().
  plugin_category_captures: plugin_category_captures().
  _element_to_capture: _element_to_capture().
  _walk_for_plugin_categories: _walk_for_plugin_categories().
  PluginQueryNode: PluginQueryNode#
  fallback_query_captures.walk_tree_basic: fallback_query_captures().walk_tree_basic().
  PluginQueryNode.text: PluginQueryNode#text.
  _node_matches_query: _node_matches_query().
  PluginQueryNode.start_point: PluginQueryNode#start_point.
  PluginQueryNode.end_point: PluginQueryNode#end_point.
  logger: logger.
  PluginQueryNode.__init__: PluginQueryNode#__init__().
---
# Module: [`tree_sitter_analyzer/core/_query_service_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_service_helpers.py)

## Classes
### `PluginQueryNode`
- def: [`tree_sitter_analyzer/core/_query_service_helpers.py:9`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_service_helpers.py#L9)
- doc: Small node shim for plugin elements returned without tree-sitter nodes.
- signature: `class PluginQueryNode:`
- members:
  - `end_point` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_service_helpers.py#L15)
  - `start_point` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_service_helpers.py#L14)
  - `text` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_service_helpers.py#L16)
- protocol/private: `__init__`[`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_service_helpers.py#L12)
- used by: [`_element_to_capture`](_query_service_helpers.md#_element_to_capture)  (6 test-only)

## Functions
- `_element_to_capture(element: Any, query_key: str | None)` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_service_helpers.py#L19)
- `_node_matches_query(node_type: str, query_key: str | None)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_service_helpers.py#L71)
- `_walk_for_plugin_categories(node: Any, node_types: list[str], query_key: str, captures: list[tuple[Any, str]])` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_service_helpers.py#L42)
- `fallback_query_captures(root_node: Any, query_key: str | None)` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_service_helpers.py#L88)
- `plugin_category_captures(plugin: Any, root_node: Any, query_key: str | None)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_service_helpers.py#L52)
- `plugin_strategy_captures(plugin: Any, query_key: str | None, source_code: str)` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_service_helpers.py#L25)
- `walk_tree_basic(node: Any)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_service_helpers.py#L93)

## Module values
- `logger` — [`L6`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_service_helpers.py#L6)

