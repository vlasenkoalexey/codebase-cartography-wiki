---
title: 'Module: tree_sitter_analyzer/formatters/_html_formatter_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_html_formatter_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._html_formatter_helpers`/
symbols:
  format_element_tree: format_element_tree().
  _markup_table_row: _markup_table_row().
  _style_table_row: _style_table_row().
  format_markup_elements: format_markup_elements().
  element_to_dict: element_to_dict().
  format_style_elements: format_style_elements().
  _markup_group_lines: _markup_group_lines().
  _style_group_lines: _style_group_lines().
  format_other_elements: format_other_elements().
  _group_by_element_class: _group_by_element_class().
  _markup_attributes_summary: _markup_attributes_summary().
  _key_attribute_summary: _key_attribute_summary().
  _style_properties_summary: _style_properties_summary().
  _other_element_values: _other_element_values().
---
# Module: [`tree_sitter_analyzer/formatters/_html_formatter_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_formatter_helpers.py)

## Functions
- `_group_by_element_class(elements: list[Any])` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_formatter_helpers.py#L83)
- `_key_attribute_summary(attributes: dict[str, Any])` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_formatter_helpers.py#L126)
- `_markup_attributes_summary(attributes: dict[str, Any])` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_formatter_helpers.py#L113)
- `_markup_group_lines(element_class: str, elements: list[MarkupElement])` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_formatter_helpers.py#L91)
- `_markup_table_row(element: MarkupElement)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_formatter_helpers.py#L104)
- `_other_element_values(element: Any)` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_formatter_helpers.py#L164)
- `_style_group_lines(element_class: str, elements: list[StyleElement])` — [`L136`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_formatter_helpers.py#L136)
- `_style_properties_summary(properties: dict[str, Any])` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_formatter_helpers.py#L156)
- `_style_table_row(element: StyleElement)` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_formatter_helpers.py#L149)
- `element_to_dict(element: CodeElement)` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_formatter_helpers.py#L72) — Convert generic CodeElement to dictionary.
- `format_element_tree(element: MarkupElement, depth: int)` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_formatter_helpers.py#L26) — Format element tree hierarchy.
- `format_markup_elements(elements: list[MarkupElement])` — [`L8`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_formatter_helpers.py#L8) — Format MarkupElement list with hierarchy.
- `format_other_elements(elements: list[Any])` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_formatter_helpers.py#L52) — Format non-HTML/CSS elements.
- `format_style_elements(elements: list[StyleElement])` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_formatter_helpers.py#L41) — Format StyleElement list.

