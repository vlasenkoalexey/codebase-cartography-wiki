---
title: 'Module: tree_sitter_analyzer/languages/markdown_plugin/extractor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/markdown_plugin/extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.markdown_plugin.extractor`/
symbols:
  MarkdownElementExtractor: MarkdownElementExtractor#
  MarkdownElementExtractor.source_code: MarkdownElementExtractor#source_code.
  TREE_SITTER_AVAILABLE: TREE_SITTER_AVAILABLE.
  MarkdownElementExtractor.content_lines: MarkdownElementExtractor#content_lines.
  MarkdownElementExtractor._node_text_cache: MarkdownElementExtractor#_node_text_cache.
  MarkdownElementExtractor._processed_nodes: MarkdownElementExtractor#_processed_nodes.
  MarkdownElementExtractor._element_cache: MarkdownElementExtractor#_element_cache.
  MarkdownElementExtractor._extracted_links: MarkdownElementExtractor#_extracted_links.
  MarkdownElementExtractor._extracted_images: MarkdownElementExtractor#_extracted_images.
  MarkdownElementExtractor.current_file: MarkdownElementExtractor#current_file.
  __all__: __all__.
  MarkdownElementExtractor.__init__: MarkdownElementExtractor#__init__().
  MarkdownElementExtractor._file_encoding: MarkdownElementExtractor#_file_encoding.
---
# Module: [`tree_sitter_analyzer/languages/markdown_plugin/extractor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/extractor.py)

## Classes
### `MarkdownElementExtractor`  ·  implements/extends ElementExtractor, MarkdownBlockExtractionMixin, MarkdownInlineExtractionMixin, MarkdownModelExtractionMixin, MarkdownPrivateExtractionMixin
- def: [`tree_sitter_analyzer/languages/markdown_plugin/extractor.py:35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/extractor.py#L35) — documented in [tree_sitter_analyzer-plugins-base](../../../../concepts/tree_sitter_analyzer-plugins-base.md)
- doc: Markdown-specific element extractor with comprehensive feature support.
- signature: `class MarkdownElementExtractor(MarkdownModelExtractionMixin, MarkdownBlockExtractionMixin, MarkdownInlineExtractionMixin, MarkdownPrivateExtractionMixin, ElementExtractor):`
- members:
  - `__init__(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/extractor.py#L44) — Initialize the Markdown element extractor.
  - `content_lines` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/extractor.py#L48)
  - `current_file` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/extractor.py#L46)
  - `source_code` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/extractor.py#L47)
- protocol/private: `_element_cache`[`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/extractor.py#L52), `_extracted_images`[`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/extractor.py#L56), `_extracted_links`[`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/extractor.py#L55), `_file_encoding`[`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/extractor.py#L53), `_node_text_cache`[`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/extractor.py#L50), `_processed_nodes`[`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/extractor.py#L51)
- uses (calls/refs, reference-scoped): [`ElementExtractor`](../../plugins/base.md#ElementExtractor), [`MarkdownPrivateExtractionMixin`](private_extraction.md#MarkdownPrivateExtractionMixin), [`MarkdownBlockExtractionMixin`](public_extraction.md#MarkdownBlockExtractionMixin), [`MarkdownInlineExtractionMixin`](public_extraction.md#MarkdownInlineExtractionMixin), [`MarkdownModelExtractionMixin`](public_extraction.md#MarkdownModelExtractionMixin)
- used by: [`ElementExtractor`](../../plugins/base.md#ElementExtractor), [`extract_elements`](plugin.md#MarkdownPlugin.extract_elements), [`_collect_markdown_elements`](plugin.md#MarkdownPlugin._collect_markdown_elements), [`TREE_SITTER_AVAILABLE`](plugin.md#TREE_SITTER_AVAILABLE), [`MarkdownPrivateExtractionMixin`](private_extraction.md#MarkdownPrivateExtractionMixin), [`create_extractor`](plugin.md#MarkdownPlugin.create_extractor), [`_extractor`](plugin.md#MarkdownPlugin._extractor), [`MarkdownBlockExtractionMixin`](public_extraction.md#MarkdownBlockExtractionMixin), [`MarkdownInlineExtractionMixin`](public_extraction.md#MarkdownInlineExtractionMixin), [`MarkdownModelExtractionMixin`](public_extraction.md#MarkdownModelExtractionMixin)  (54 test-only)

## Module values
- `TREE_SITTER_AVAILABLE` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/extractor.py#L13)
- `__all__` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/extractor.py#L27)

