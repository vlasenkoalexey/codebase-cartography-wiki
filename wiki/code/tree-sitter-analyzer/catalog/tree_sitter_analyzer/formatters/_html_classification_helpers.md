---
title: 'Module: tree_sitter_analyzer/formatters/_html_classification_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_html_classification_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._html_classification_helpers`/
symbols:
  _add_classified_element: _add_classified_element().
  _add_classified_dict: _add_classified_dict().
  classify_html_elements: classify_html_elements().
  ClassifiedHtmlElements: ClassifiedHtmlElements#
  ClassifiedHtmlElements.markup_elements: ClassifiedHtmlElements#markup_elements.
  ClassifiedHtmlElements.style_elements: ClassifiedHtmlElements#style_elements.
  ClassifiedHtmlElements.other_elements: ClassifiedHtmlElements#other_elements.
---
# Module: [`tree_sitter_analyzer/formatters/_html_classification_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_classification_helpers.py)

## Classes
### `ClassifiedHtmlElements`
- def: [`tree_sitter_analyzer/formatters/_html_classification_helpers.py:11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_classification_helpers.py#L11)
- signature: `class ClassifiedHtmlElements:`
- members:
  - `markup_elements` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_classification_helpers.py#L12)
  - `other_elements` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_classification_helpers.py#L14)
  - `style_elements` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_classification_helpers.py#L13)
- used by: [`format`](html_formatter.md#HtmlFormatter.format), [`_add_classified_element`](_html_classification_helpers.md#_add_classified_element), [`_add_classified_dict`](_html_classification_helpers.md#_add_classified_dict), [`classify_html_elements`](_html_classification_helpers.md#classify_html_elements)

## Functions
- `_add_classified_dict(element: dict[str, Any], groups: ClassifiedHtmlElements, dict_to_markup: Callable[[dict[str, Any]], Any], dict_to_style: Callable[[dict[str, Any]], Any])` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_classification_helpers.py#L54)
- `_add_classified_element(element: CodeElement, groups: ClassifiedHtmlElements, dict_to_markup: Callable[[dict[str, Any]], Any], dict_to_style: Callable[[dict[str, Any]], Any], element_to_dict_fn: Callable[[CodeElement], dict[str, Any]])` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_classification_helpers.py#L35)
- `classify_html_elements(elements: list[CodeElement], dict_to_markup: Callable[[dict[str, Any]], Any], dict_to_style: Callable[[dict[str, Any]], Any], element_to_dict: Callable[[CodeElement], dict[str, Any]])` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_classification_helpers.py#L17)

