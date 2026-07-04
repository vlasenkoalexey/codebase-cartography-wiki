---
title: 'Module: tree_sitter_analyzer/languages/markdown_plugin/elements.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/markdown_plugin/elements.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.markdown_plugin.elements`/
symbols:
  MarkdownElement: MarkdownElement#
  MarkdownElement.text: MarkdownElement#text.
  _build_markdown_list_element: _build_markdown_list_element().
  _build_markdown_heading_element: _build_markdown_heading_element().
  _summarize_fenced_code_block: _summarize_fenced_code_block().
  _build_markdown_code_block_element: _build_markdown_code_block_element().
  MarkdownElement.alt: MarkdownElement#alt.
  _summarize_markdown_list: _summarize_markdown_list().
  MarkdownElement.url: MarkdownElement#url.
  MarkdownElement.alt_text: MarkdownElement#alt_text.
  MarkdownElement.list_type: MarkdownElement#list_type.
  MarkdownElement.item_count: MarkdownElement#item_count.
  MarkdownElement.row_count: MarkdownElement#row_count.
  MarkdownElement.column_count: MarkdownElement#column_count.
  MarkdownElement.level: MarkdownElement#level.
  MarkdownElement.title: MarkdownElement#title.
  MarkdownElement.language_info: MarkdownElement#language_info.
  MarkdownElement.is_checked: MarkdownElement#is_checked.
  MarkdownElement.__init__: MarkdownElement#__init__().
  _is_pipe_table_separator: _is_pipe_table_separator().
  _classify_markdown_list: _classify_markdown_list().
  _summarize_setext_header: _summarize_setext_header().
  _is_task_list_item: _is_task_list_item().
  _extract_fenced_code_language: _extract_fenced_code_language().
  _extract_fenced_code_content_lines: _extract_fenced_code_content_lines().
---
# Module: [`tree_sitter_analyzer/languages/markdown_plugin/elements.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py)

## Classes
### `MarkdownElement`  ·  implements/extends CodeElement
- def: [`tree_sitter_analyzer/languages/markdown_plugin/elements.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L11) — documented in [tree_sitter_analyzer-plugins-base](../../../../concepts/tree_sitter_analyzer-plugins-base.md)
- doc: Markdown-specific code element.
- signature: `class MarkdownElement(CodeElement):`
- members:
  - `alt` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L48)
  - `alt_text` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L41)
  - `column_count` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L52)
  - `is_checked` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L44)
  - `item_count` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L50)
  - `language_info` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L43)
  - `level` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L39)
  - `list_type` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L49)
  - `row_count` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L51)
  - `text` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L46)
  - `title` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L42)
  - `url` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L40)
- protocol/private: `__init__`[`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L14)
- uses (calls/refs, reference-scoped): [`CodeElement`](../../models/base.md#CodeElement), [`element_type`](../../models/base.md#CodeElement.element_type)
- used by: [`CodeElement`](../../models/base.md#CodeElement), [`_append_text_format_match`](_misc_inline_extractor_helpers.md#_append_text_format_match), [`extract_images`](public_extraction.md#MarkdownInlineExtractionMixin.extract_images), [`extract_links`](public_extraction.md#MarkdownInlineExtractionMixin.extract_links), [`_append_image_reference_definition`](_image_reference_extractor_helpers.md#_append_image_reference_definition), [`_extract_pipe_tables`](private_extraction.md#MarkdownBlockPrivateExtractionMixin._extract_pipe_tables), [`_extract_block_quotes_process_items`](_misc_block_extractor_helpers.md#_extract_block_quotes_process_items), [`_extract_setext_headers`](private_extraction.md#MarkdownBlockPrivateExtractionMixin._extract_setext_headers), [`extract_blockquotes`](public_extraction.md#MarkdownBlockExtractionMixin.extract_blockquotes), [`extract_references`](public_extraction.md#MarkdownInlineExtractionMixin.extract_references), [`extract_footnotes`](public_extraction.md#MarkdownInlineExtractionMixin.extract_footnotes), [`extract_headers`](public_extraction.md#MarkdownBlockExtractionMixin.extract_headers), [`extract_horizontal_rules`](public_extraction.md#MarkdownBlockExtractionMixin.extract_horizontal_rules), [`extract_html_elements`](public_extraction.md#MarkdownBlockExtractionMixin.extract_html_elements), [`extract_text_formatting`](public_extraction.md#MarkdownInlineExtractionMixin.extract_text_formatting), [`_extract_list_items`](private_extraction.md#MarkdownBlockPrivateExtractionMixin._extract_list_items), [`extract_code_blocks`](public_extraction.md#MarkdownBlockExtractionMixin.extract_code_blocks), [`extract_lists`](public_extraction.md#MarkdownBlockExtractionMixin.extract_lists), [`extract_tables`](public_extraction.md#MarkdownBlockExtractionMixin.extract_tables), [`_append_inline_html_match`](_misc_inline_extractor_helpers.md#_append_inline_html_match), [`_extract_fenced_code_blocks`](private_extraction.md#MarkdownBlockPrivateExtractionMixin._extract_fenced_code_blocks), [`_extract_html_blocks_process_items`](_misc_block_extractor_helpers.md#_extract_html_blocks_process_items), [`_append_autolink_match`](_link_image_extractor_helpers.md#_append_autolink_match), [`_append_inline_link_match`](_link_image_extractor_helpers.md#_append_inline_link_match), [`_extract_autolinks`](private_extraction.md#MarkdownLinkImagePrivateExtractionMixin._extract_autolinks), [`_extract_inline_images`](link_image_extractor.md#_extract_inline_images), [`_extract_reference_images`](link_image_extractor.md#_extract_reference_images), [`_extract_emphasis_elements`](private_extraction.md#MarkdownMiscPrivateExtractionMixin._extract_emphasis_elements), [`_build_markdown_list_element`](elements.md#_build_markdown_list_element), [`_extract_emphasis_elements_process_items`](_misc_extractor_helpers.md#_extract_emphasis_elements_process_items), [`_extract_indented_code_blocks`](private_extraction.md#MarkdownBlockPrivateExtractionMixin._extract_indented_code_blocks), [`_extract_thematic_breaks_process_items`](_misc_block_extractor_helpers.md#_extract_thematic_breaks_process_items), [`_extract_inline_html`](private_extraction.md#MarkdownMiscPrivateExtractionMixin._extract_inline_html), [`extract_md_link_reference_definitions`](link_image_extractor.md#extract_md_link_reference_definitions), [`_append_footnote_definition`](_misc_extractor_helpers.md#_append_footnote_definition), [`_append_footnote_references`](_misc_extractor_helpers.md#_append_footnote_references), [`_append_reference_link_match`](_link_image_extractor_helpers.md#_append_reference_link_match), [`_extract_atx_headers`](private_extraction.md#MarkdownBlockPrivateExtractionMixin._extract_atx_headers), [`_extract_footnote_elements`](private_extraction.md#MarkdownMiscPrivateExtractionMixin._extract_footnote_elements), [`_extract_image_reference_definitions`](private_extraction.md#MarkdownLinkImagePrivateExtractionMixin._extract_image_reference_definitions)  (+13 more; 11 test-only)

## Functions
- `_build_markdown_code_block_element(node: tree_sitter.Node, raw_text: str, language_info: str | None, line_count: int)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L186) — Build a MarkdownElement for a fenced code block node.
- `_build_markdown_heading_element(node: tree_sitter.Node, raw_text: str, content: str, level: int)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L136) — Build a MarkdownElement for a heading node.
- `_build_markdown_list_element(node: tree_sitter.Node, raw_text: str, item_count: int, list_type: str, element_type: str)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L100) — Build a MarkdownElement for a list node.
- `_classify_markdown_list(is_task_list: bool, is_ordered: bool)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L91) — Return formatter list_type and element_type for a Markdown list.
- `_extract_fenced_code_content_lines(lines: list[str])` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L171) — Return lines between opening and closing triple-backtick fences.
- `_extract_fenced_code_language(lines: list[str])` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L164) — Return the fence language info when present.
- `_is_pipe_table_separator(line: str)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L55) — Return True for Markdown table separator rows like ``| --- | :---: |``.
- `_is_task_list_item(item_text: str)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L86) — Return whether item text uses GitHub-style task list markers.
- `_summarize_fenced_code_block(raw_text: str)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L157) — Return language info and content-line count for a fenced code block.
- `_summarize_markdown_list(node: tree_sitter.Node, get_node_text: Any)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L65) — Return item count plus task/ordered flags for a Markdown list node.
- `_summarize_setext_header(raw_text: str)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/elements.py#L121) — Return heading text and level for a Setext-style heading.

