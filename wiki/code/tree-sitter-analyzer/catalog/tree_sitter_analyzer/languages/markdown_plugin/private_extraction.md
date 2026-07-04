---
title: 'Module: tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.markdown_plugin.private_extraction`/
symbols:
  MarkdownBlockPrivateExtractionMixin._extract_pipe_tables: MarkdownBlockPrivateExtractionMixin#_extract_pipe_tables().
  MarkdownBlockPrivateExtractionMixin._extract_setext_headers: MarkdownBlockPrivateExtractionMixin#_extract_setext_headers().
  MarkdownExtractorStateMixin._get_node_text_optimized: MarkdownExtractorStateMixin#_get_node_text_optimized().
  MarkdownBlockPrivateExtractionMixin._extract_list_items: MarkdownBlockPrivateExtractionMixin#_extract_list_items().
  MarkdownPrivateExtractionMixin: MarkdownPrivateExtractionMixin#
  MarkdownBlockPrivateExtractionMixin._extract_fenced_code_blocks: MarkdownBlockPrivateExtractionMixin#_extract_fenced_code_blocks().
  MarkdownLinkImagePrivateExtractionMixin._extract_autolinks: MarkdownLinkImagePrivateExtractionMixin#_extract_autolinks().
  MarkdownMiscPrivateExtractionMixin._extract_emphasis_elements: MarkdownMiscPrivateExtractionMixin#_extract_emphasis_elements().
  MarkdownBlockPrivateExtractionMixin._extract_indented_code_blocks: MarkdownBlockPrivateExtractionMixin#_extract_indented_code_blocks().
  MarkdownMiscPrivateExtractionMixin._extract_inline_html: MarkdownMiscPrivateExtractionMixin#_extract_inline_html().
  MarkdownBlockPrivateExtractionMixin._extract_atx_headers: MarkdownBlockPrivateExtractionMixin#_extract_atx_headers().
  MarkdownLinkImagePrivateExtractionMixin._extract_inline_links: MarkdownLinkImagePrivateExtractionMixin#_extract_inline_links().
  MarkdownLinkImagePrivateExtractionMixin._extract_reference_images: MarkdownLinkImagePrivateExtractionMixin#_extract_reference_images().
  MarkdownLinkImagePrivateExtractionMixin._extract_image_reference_definitions: MarkdownLinkImagePrivateExtractionMixin#_extract_image_reference_definitions().
  MarkdownMiscPrivateExtractionMixin._extract_strikethrough_elements: MarkdownMiscPrivateExtractionMixin#_extract_strikethrough_elements().
  MarkdownMiscPrivateExtractionMixin._extract_footnote_elements: MarkdownMiscPrivateExtractionMixin#_extract_footnote_elements().
  MarkdownLinkImagePrivateExtractionMixin._extract_inline_images: MarkdownLinkImagePrivateExtractionMixin#_extract_inline_images().
  MarkdownLinkImagePrivateExtractionMixin._extract_reference_links: MarkdownLinkImagePrivateExtractionMixin#_extract_reference_links().
  MarkdownLinkImagePrivateExtractionMixin._extract_link_reference_definitions: MarkdownLinkImagePrivateExtractionMixin#_extract_link_reference_definitions().
  MarkdownMiscPrivateExtractionMixin._extract_thematic_breaks: MarkdownMiscPrivateExtractionMixin#_extract_thematic_breaks().
  MarkdownMiscPrivateExtractionMixin._extract_block_quotes: MarkdownMiscPrivateExtractionMixin#_extract_block_quotes().
  MarkdownMiscPrivateExtractionMixin._extract_html_blocks: MarkdownMiscPrivateExtractionMixin#_extract_html_blocks().
  MarkdownMiscPrivateExtractionMixin._extract_inline_code_spans: MarkdownMiscPrivateExtractionMixin#_extract_inline_code_spans().
  MarkdownExtractorStateMixin._traverse_nodes: MarkdownExtractorStateMixin#_traverse_nodes().
  _count_pipe_table_rows: _count_pipe_table_rows().
  MarkdownExtractorStateMixin: MarkdownExtractorStateMixin#
  MarkdownBlockPrivateExtractionMixin: MarkdownBlockPrivateExtractionMixin#
  MarkdownLinkImagePrivateExtractionMixin: MarkdownLinkImagePrivateExtractionMixin#
  MarkdownMiscPrivateExtractionMixin: MarkdownMiscPrivateExtractionMixin#
  MarkdownExtractorStateMixin.reset_caches: MarkdownExtractorStateMixin#reset_caches.
  MarkdownExtractorStateMixin._reset_caches: MarkdownExtractorStateMixin#_reset_caches().
  _count_pipe_table_columns: _count_pipe_table_columns().
---
# Module: [`tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py)

## Classes
### `MarkdownBlockPrivateExtractionMixin`
- def: [`tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py:90`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L90)
- doc: Private extraction helpers for Markdown block elements.
- signature: `class MarkdownBlockPrivateExtractionMixin:`
- members:
  - `_extract_atx_headers(self, root_node: tree_sitter.Node, headers: list[MarkdownElement])` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L93) — Extract ATX-style headers (# ## ### etc.).
  - `_extract_fenced_code_blocks(self, root_node: tree_sitter.Node, code_blocks: list[MarkdownElement])` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L142) — Extract fenced code blocks.
  - `_extract_indented_code_blocks(self, root_node: tree_sitter.Node, code_blocks: list[MarkdownElement])` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L163) — Extract indented code blocks.
  - `_extract_list_items(self, root_node: tree_sitter.Node, lists: list[MarkdownElement])` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L190) — Extract lists.
  - `_extract_pipe_tables(self, root_node: tree_sitter.Node, tables: list[MarkdownElement])` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L219) — Extract pipe tables.
  - `_extract_setext_headers(self, root_node: tree_sitter.Node, headers: list[MarkdownElement])` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L126) — Extract Setext-style headers.
- uses (calls/refs, reference-scoped): [`log_debug`](../../utils/logging.md#log_debug), [`language`](../../models/base.md#CodeElement.language), [`MarkdownElement`](elements.md#MarkdownElement), [`MarkdownPrivateExtractionMixin`](private_extraction.md#MarkdownPrivateExtractionMixin), [`text`](elements.md#MarkdownElement.text), [`_build_markdown_list_element`](elements.md#_build_markdown_list_element), [`_build_markdown_code_block_element`](elements.md#_build_markdown_code_block_element), [`_build_markdown_heading_element`](elements.md#_build_markdown_heading_element), [`_summarize_fenced_code_block`](elements.md#_summarize_fenced_code_block), [`_summarize_markdown_list`](elements.md#_summarize_markdown_list), [`column_count`](elements.md#MarkdownElement.column_count), [`row_count`](elements.md#MarkdownElement.row_count), [`_count_pipe_table_rows`](private_extraction.md#_count_pipe_table_rows), [`_classify_markdown_list`](elements.md#_classify_markdown_list), [`_summarize_setext_header`](elements.md#_summarize_setext_header), [`_count_pipe_table_columns`](private_extraction.md#_count_pipe_table_columns)
- used by: [`MarkdownPrivateExtractionMixin`](private_extraction.md#MarkdownPrivateExtractionMixin)  (18 test-only)

### `MarkdownExtractorStateMixin`
- def: [`tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py:42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L42)
- doc: Shared state and traversal helpers for Markdown extraction.
- signature: `class MarkdownExtractorStateMixin:`
- members:
  - `_get_node_text_optimized(self, node: tree_sitter.Node)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L58) — Get node text with optimized caching using position-based keys.
  - `_reset_caches(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L45) — Reset performance caches and extraction tracking sets.
  - `_traverse_nodes(self, node: tree_sitter.Node)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L83) — Traverse all nodes in the tree.
  - `reset_caches` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L56)
- uses (calls/refs, reference-scoped): [`log_error`](../../utils/logging.md#log_error), [`MarkdownPrivateExtractionMixin`](private_extraction.md#MarkdownPrivateExtractionMixin), [`_extract_node_text_by_points`](node_text.md#_extract_node_text_by_points), [`_extract_node_text_by_bytes`](node_text.md#_extract_node_text_by_bytes)
- used by: [`MarkdownPrivateExtractionMixin`](private_extraction.md#MarkdownPrivateExtractionMixin)  (11 test-only)

### `MarkdownLinkImagePrivateExtractionMixin`
- def: [`tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py:250`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L250)
- doc: Private extraction adapters for Markdown links and images.
- signature: `class MarkdownLinkImagePrivateExtractionMixin:`
- protocol/private: `_extract_autolinks`[`L273`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L273), `_extract_image_reference_definitions`[`L300`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L300), `_extract_inline_images`[`L286`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L286), `_extract_inline_links`[`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L253), `_extract_link_reference_definitions`[`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L307), `_extract_reference_images`[`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L293), `_extract_reference_links`[`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L266)
- uses (calls/refs, reference-scoped): [`MarkdownElement`](elements.md#MarkdownElement), [`_extract_image_reference_definitions`](link_image_extractor.md#_extract_image_reference_definitions), [`MarkdownPrivateExtractionMixin`](private_extraction.md#MarkdownPrivateExtractionMixin), [`_extract_inline_images`](link_image_extractor.md#_extract_inline_images), [`_extract_reference_images`](link_image_extractor.md#_extract_reference_images), [`extract_md_link_reference_definitions`](link_image_extractor.md#extract_md_link_reference_definitions), [`_extract_autolinks`](link_image_extractor.md#_extract_autolinks), [`_extract_inline_links`](link_image_extractor.md#_extract_inline_links), [`_extract_reference_links`](link_image_extractor.md#_extract_reference_links)
- used by: [`MarkdownPrivateExtractionMixin`](private_extraction.md#MarkdownPrivateExtractionMixin)  (19 test-only)

### `MarkdownMiscPrivateExtractionMixin`
- def: [`tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py:316`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L316)
- doc: Private extraction adapters for miscellaneous Markdown elements.
- signature: `class MarkdownMiscPrivateExtractionMixin:`
- protocol/private: `_extract_block_quotes`[`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L319), `_extract_emphasis_elements`[`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L356), `_extract_footnote_elements`[`L386`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L386), `_extract_html_blocks`[`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L336), `_extract_inline_code_spans`[`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L366), `_extract_inline_html`[`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L346), `_extract_strikethrough_elements`[`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L376), `_extract_thematic_breaks`[`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L326)
- uses (calls/refs, reference-scoped): [`MarkdownElement`](elements.md#MarkdownElement), [`MarkdownPrivateExtractionMixin`](private_extraction.md#MarkdownPrivateExtractionMixin), [`extract_block_quotes`](misc_extractor.md#extract_block_quotes), [`extract_emphasis_elements`](misc_extractor.md#extract_emphasis_elements), [`extract_footnote_elements`](misc_extractor.md#extract_footnote_elements), [`extract_html_blocks`](misc_extractor.md#extract_html_blocks), [`extract_inline_code_spans`](misc_extractor.md#extract_inline_code_spans), [`extract_inline_html`](misc_extractor.md#extract_inline_html), [`extract_strikethrough_elements`](misc_extractor.md#extract_strikethrough_elements), [`extract_thematic_breaks`](misc_extractor.md#extract_thematic_breaks)
- used by: [`MarkdownPrivateExtractionMixin`](private_extraction.md#MarkdownPrivateExtractionMixin)  (16 test-only)

### `MarkdownPrivateExtractionMixin`  ·  implements/extends MarkdownBlockPrivateExtractionMixin, MarkdownExtractorStateMixin, MarkdownLinkImagePrivateExtractionMixin, MarkdownMiscPrivateExtractionMixin
- def: [`tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py:394`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L394)
- doc: Combined private extraction behavior for MarkdownElementExtractor.
- signature: `class MarkdownPrivateExtractionMixin(MarkdownExtractorStateMixin, MarkdownBlockPrivateExtractionMixin, MarkdownLinkImagePrivateExtractionMixin, MarkdownMiscPrivateExtractionMixin):`
- uses (calls/refs, reference-scoped): [`MarkdownElementExtractor`](extractor.md#MarkdownElementExtractor), [`MarkdownBlockPrivateExtractionMixin`](private_extraction.md#MarkdownBlockPrivateExtractionMixin), [`MarkdownExtractorStateMixin`](private_extraction.md#MarkdownExtractorStateMixin), [`MarkdownLinkImagePrivateExtractionMixin`](private_extraction.md#MarkdownLinkImagePrivateExtractionMixin), [`MarkdownMiscPrivateExtractionMixin`](private_extraction.md#MarkdownMiscPrivateExtractionMixin)
- used by: [`MarkdownElementExtractor`](extractor.md#MarkdownElementExtractor), [`TREE_SITTER_AVAILABLE`](extractor.md#TREE_SITTER_AVAILABLE), [`MarkdownBlockPrivateExtractionMixin`](private_extraction.md#MarkdownBlockPrivateExtractionMixin), [`MarkdownExtractorStateMixin`](private_extraction.md#MarkdownExtractorStateMixin), [`MarkdownLinkImagePrivateExtractionMixin`](private_extraction.md#MarkdownLinkImagePrivateExtractionMixin), [`MarkdownMiscPrivateExtractionMixin`](private_extraction.md#MarkdownMiscPrivateExtractionMixin)

## Functions
- `_count_pipe_table_columns(lines: list[str])` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L34) — Count columns from the first Markdown pipe table row.
- `_count_pipe_table_rows(lines: list[str])` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/private_extraction.py#L27) — Count non-separator rows in a Markdown pipe table.

