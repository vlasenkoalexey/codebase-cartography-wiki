---
title: 'Module: tree_sitter_analyzer/languages/markdown_plugin/_misc_inline_extractor_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/markdown_plugin/_misc_inline_extractor_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.markdown_plugin._misc_inline_extractor_helpers`/
symbols:
  _append_text_format_match: _append_text_format_match().
  _extract_inline_code_spans_process_items: _extract_inline_code_spans_process_items().
  _extract_strikethrough_elements_process_items: _extract_strikethrough_elements_process_items().
  _append_inline_html_match: _append_inline_html_match().
  _extract_inline_html_process_items: _extract_inline_html_process_items().
  TextFormatMatchContext.match: TextFormatMatchContext#match.
  TextFormatMatchContext.element_type: TextFormatMatchContext#element_type.
  TextFormatMatchContext: TextFormatMatchContext#
  TextFormatMatchContext.node: TextFormatMatchContext#node.
  TextFormatMatchContext.raw_text: TextFormatMatchContext#raw_text.
  TextFormatMatchContext.formatting_elements: TextFormatMatchContext#formatting_elements.
  TextFormatMatchContext.label: TextFormatMatchContext#label.
  TextFormatMatchContext.content_group: TextFormatMatchContext#content_group.
  _match_start_line: _match_start_line().
---
# Module: [`tree_sitter_analyzer/languages/markdown_plugin/_misc_inline_extractor_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_inline_extractor_helpers.py)

## Classes
### `TextFormatMatchContext`
- def: [`tree_sitter_analyzer/languages/markdown_plugin/_misc_inline_extractor_helpers.py:15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_inline_extractor_helpers.py#L15)
- doc: Inputs needed to append an inline text formatting match.
- signature: `class TextFormatMatchContext:`
- members:
  - `content_group` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_inline_extractor_helpers.py#L24)
  - `element_type` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_inline_extractor_helpers.py#L23)
  - `formatting_elements` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_inline_extractor_helpers.py#L21)
  - `label` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_inline_extractor_helpers.py#L22)
  - `match` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_inline_extractor_helpers.py#L20)
  - `node` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_inline_extractor_helpers.py#L18)
  - `raw_text` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_inline_extractor_helpers.py#L19)
- used by: [`_append_text_format_match`](_misc_inline_extractor_helpers.md#_append_text_format_match), [`_extract_inline_code_spans_process_items`](_misc_inline_extractor_helpers.md#_extract_inline_code_spans_process_items), [`_extract_strikethrough_elements_process_items`](_misc_inline_extractor_helpers.md#_extract_strikethrough_elements_process_items)

## Functions
- `_append_inline_html_match(node: Any, raw_text: str, match: re.Match[str], html_elements: list[Any])` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_inline_extractor_helpers.py#L46)
- `_append_text_format_match(context: TextFormatMatchContext)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_inline_extractor_helpers.py#L126)
- `_extract_inline_code_spans_process_items(root_node: Any, formatting_elements: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_inline_extractor_helpers.py#L70)
- `_extract_inline_html_process_items(root_node: Any, html_elements: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_inline_extractor_helpers.py#L27)
- `_extract_strikethrough_elements_process_items(root_node: Any, formatting_elements: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_inline_extractor_helpers.py#L98)
- `_match_start_line(node: Any, raw_text: str, match: re.Match[str])` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_inline_extractor_helpers.py#L144)

