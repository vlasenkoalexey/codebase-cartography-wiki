---
title: 'Module: tree_sitter_analyzer/_api_query_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_api_query_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._api_query_helpers`/
symbols:
  filter_elements_by_type: filter_elements_by_type().
  group_captures_by_main_node: group_captures_by_main_node().
  query_execution_result: query_execution_result().
  _add_capture_to_group: _add_capture_to_group().
  query_captures_for_result: query_captures_for_result().
  _MAIN_CAPTURE_TYPES: _MAIN_CAPTURE_TYPES.
  _add_main_capture: _add_main_capture().
  _add_child_capture: _add_child_capture().
  _CLASS_FAMILY_TYPES: _CLASS_FAMILY_TYPES.
---
# Module: [`tree_sitter_analyzer/_api_query_helpers.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_query_helpers.py)

## Functions
- `_add_capture_to_group(capture: dict[str, Any], main_node_stack: list[tuple[dict[str, Any], dict[str, Any]]], results: list[dict[str, Any]])` — [`L28`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_query_helpers.py#L28)
- `_add_child_capture(capture_name: str, capture: dict[str, Any], parent_grouped: dict[str, Any])` — [`L66`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_query_helpers.py#L66)
- `_add_main_capture(capture: dict[str, Any], main_node_stack: list[tuple[dict[str, Any], dict[str, Any]]], results: list[dict[str, Any]])` — [`L45`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_query_helpers.py#L45)
- `filter_elements_by_type(elements: list[dict[str, Any]], element_types: list[str] | None)` — [`L128`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_query_helpers.py#L128) — Filter extracted elements by fuzzy type match.
- `group_captures_by_main_node(captures: list[dict[str, Any]])` — [`L9`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_query_helpers.py#L9) — Group flat query captures by their main nodes.
- `query_captures_for_result(result: dict[str, Any], query_name: str)` — [`L82`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_query_helpers.py#L82) — Extract raw captures from the API query result shape.
- `query_execution_result(result: dict[str, Any], query_name: str, file_path: str | Path)` — [`L92`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_query_helpers.py#L92) — Build the public API response for a query facade call.

## Module values
- `_CLASS_FAMILY_TYPES` — [`L123`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_query_helpers.py#L123)
- `_MAIN_CAPTURE_TYPES` — [`L6`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_query_helpers.py#L6)

