---
title: 'Module: tree_sitter_analyzer/languages/html_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/html_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.html_helpers`/
symbols:
  create_markup_element: create_markup_element().
  parse_attribute: parse_attribute().
  extract_html_tag_name: extract_html_tag_name().
  extract_html_attributes: extract_html_attributes().
  _extract_tag_name_from_children: _extract_tag_name_from_children().
  extract_node_text: extract_node_text().
  classify_element: classify_element().
  _iter_typed_children: _iter_typed_children().
  _parse_attribute_children: _parse_attribute_children().
  _iter_attribute_nodes: _iter_attribute_nodes().
  _parse_attribute_text: _parse_attribute_text().
  _extract_tag_name_from_text: _extract_tag_name_from_text().
---
# Module: [`tree_sitter_analyzer/languages/html_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_helpers.py)

## Functions
- `_extract_tag_name_from_children(node: Any, get_node_text: Callable[..., str])` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_helpers.py#L149)
- `_extract_tag_name_from_text(node_text: str)` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_helpers.py#L164)
- `_iter_attribute_nodes(node: Any)` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_helpers.py#L172)
- `_iter_typed_children(node: Any)` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_helpers.py#L118)
- `_parse_attribute_children(attr_node: Any, get_node_text: Callable[..., str])` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_helpers.py#L124)
- `_parse_attribute_text(attr_text: str)` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_helpers.py#L141)
- `classify_element(tag_name: str, element_categories: dict[str, list[str]])` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_helpers.py#L39) — Classify HTML element based on tag name.
- `create_markup_element(node: Any, get_node_text: Callable[..., str], element_categories: dict[str, list[str]], parent: MarkupElement | None)` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_helpers.py#L80) — Create MarkupElement from tree-sitter node. — documented in [tree_sitter_analyzer-models-markup_models](../../../concepts/tree_sitter_analyzer-models-markup_models.md)
- `extract_html_attributes(node: Any, get_node_text: Callable[..., str])` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_helpers.py#L65) — Extract attributes from HTML element node.
- `extract_html_tag_name(node: Any, get_node_text: Callable[..., str])` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_helpers.py#L52) — Extract tag name from HTML element node.
- `extract_node_text(node: Any, source_code: str)` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_helpers.py#L10) — Extract text content from a tree-sitter node.
- `parse_attribute(attr_node: Any, get_node_text: Callable[..., str])` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_helpers.py#L24) — Parse individual attribute node.

