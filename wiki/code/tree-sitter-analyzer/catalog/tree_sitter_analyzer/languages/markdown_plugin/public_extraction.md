---
title: 'Module: tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.markdown_plugin.public_extraction`/
symbols:
  MarkdownInlineExtractionMixin.extract_images: MarkdownInlineExtractionMixin#extract_images().
  MarkdownInlineExtractionMixin.extract_links: MarkdownInlineExtractionMixin#extract_links().
  MarkdownModelExtractionMixin.extract_functions: MarkdownModelExtractionMixin#extract_functions().
  MarkdownModelExtractionMixin.extract_classes: MarkdownModelExtractionMixin#extract_classes().
  MarkdownModelExtractionMixin.extract_variables: MarkdownModelExtractionMixin#extract_variables().
  MarkdownModelExtractionMixin.extract_imports: MarkdownModelExtractionMixin#extract_imports().
  MarkdownBlockExtractionMixin.extract_blockquotes: MarkdownBlockExtractionMixin#extract_blockquotes().
  MarkdownInlineExtractionMixin.extract_references: MarkdownInlineExtractionMixin#extract_references().
  MarkdownBlockExtractionMixin.extract_headers: MarkdownBlockExtractionMixin#extract_headers().
  MarkdownBlockExtractionMixin.extract_horizontal_rules: MarkdownBlockExtractionMixin#extract_horizontal_rules().
  MarkdownBlockExtractionMixin.extract_html_elements: MarkdownBlockExtractionMixin#extract_html_elements().
  MarkdownInlineExtractionMixin.extract_text_formatting: MarkdownInlineExtractionMixin#extract_text_formatting().
  MarkdownInlineExtractionMixin.extract_footnotes: MarkdownInlineExtractionMixin#extract_footnotes().
  _run_extractors: _run_extractors().
  MarkdownBlockExtractionMixin.extract_code_blocks: MarkdownBlockExtractionMixin#extract_code_blocks().
  MarkdownBlockExtractionMixin.extract_lists: MarkdownBlockExtractionMixin#extract_lists().
  MarkdownBlockExtractionMixin.extract_tables: MarkdownBlockExtractionMixin#extract_tables().
  _prepare_public_extraction: _prepare_public_extraction().
  _deduplicate_elements: _deduplicate_elements().
  MarkdownModelExtractionMixin: MarkdownModelExtractionMixin#
  MarkdownBlockExtractionMixin: MarkdownBlockExtractionMixin#
  MarkdownInlineExtractionMixin: MarkdownInlineExtractionMixin#
---
# Module: [`tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py)

## Classes
### `MarkdownBlockExtractionMixin`
- def: [`tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py:137`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L137)
- doc: Public extraction methods for block-level Markdown elements.
- signature: `class MarkdownBlockExtractionMixin:`
- members:
  - `extract_blockquotes(self, tree: tree_sitter.Tree, source_code: str)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L170) — Extract Markdown blockquotes.
  - `extract_code_blocks(self, tree: tree_sitter.Tree, source_code: str)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L155) — Extract Markdown code blocks.
  - `extract_headers(self, tree: tree_sitter.Tree, source_code: str)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L140) — Extract Markdown headers (H1-H6).
  - `extract_horizontal_rules(self, tree: tree_sitter.Tree, source_code: str)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L184) — Extract Markdown horizontal rules.
  - `extract_html_elements(self, tree: tree_sitter.Tree, source_code: str)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L198) — Extract HTML elements.
  - `extract_lists(self, tree: tree_sitter.Tree, source_code: str)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L212) — Extract Markdown lists.
  - `extract_tables(self, tree: tree_sitter.Tree, source_code: str)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L226) — Extract Markdown tables.
- uses (calls/refs, reference-scoped): [`log_debug`](../../utils/logging.md#log_debug), [`MarkdownElement`](elements.md#MarkdownElement), [`MarkdownElementExtractor`](extractor.md#MarkdownElementExtractor), [`_run_extractors`](public_extraction.md#_run_extractors), [`_prepare_public_extraction`](public_extraction.md#_prepare_public_extraction)
- used by: [`MarkdownElementExtractor`](extractor.md#MarkdownElementExtractor), [`extract_elements`](plugin.md#MarkdownPlugin.extract_elements), [`_collect_markdown_elements`](plugin.md#MarkdownPlugin._collect_markdown_elements), [`TREE_SITTER_AVAILABLE`](extractor.md#TREE_SITTER_AVAILABLE)  (23 test-only)

### `MarkdownInlineExtractionMixin`
- def: [`tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py:241`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L241)
- doc: Public extraction methods for inline Markdown elements.
- signature: `class MarkdownInlineExtractionMixin:`
- members:
  - `extract_footnotes(self, tree: tree_sitter.Tree, source_code: str)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L334) — Extract footnotes.
  - `extract_images(self, tree: tree_sitter.Tree, source_code: str)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L272) — Extract Markdown images.
  - `extract_links(self, tree: tree_sitter.Tree, source_code: str)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L244) — Extract Markdown links.
  - `extract_references(self, tree: tree_sitter.Tree, source_code: str)` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L296) — Extract Markdown reference definitions.
  - `extract_text_formatting(self, tree: tree_sitter.Tree, source_code: str)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L316) — Extract text formatting elements.
- uses (calls/refs, reference-scoped): [`log_debug`](../../utils/logging.md#log_debug), [`MarkdownElement`](elements.md#MarkdownElement), [`MarkdownElementExtractor`](extractor.md#MarkdownElementExtractor), [`_run_extractors`](public_extraction.md#_run_extractors), [`_prepare_public_extraction`](public_extraction.md#_prepare_public_extraction), [`extract_md_images`](link_image_extractor.md#extract_md_images), [`extract_md_links`](link_image_extractor.md#extract_md_links), [`extract_md_link_reference_definitions`](link_image_extractor.md#extract_md_link_reference_definitions), [`_deduplicate_elements`](public_extraction.md#_deduplicate_elements), [`alt_text`](elements.md#MarkdownElement.alt_text), [`url`](elements.md#MarkdownElement.url)
- used by: [`MarkdownElementExtractor`](extractor.md#MarkdownElementExtractor), [`extract_elements`](plugin.md#MarkdownPlugin.extract_elements), [`_collect_markdown_elements`](plugin.md#MarkdownPlugin._collect_markdown_elements), [`TREE_SITTER_AVAILABLE`](extractor.md#TREE_SITTER_AVAILABLE)  (17 test-only)

### `MarkdownModelExtractionMixin`
- def: [`tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py:69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L69)
- doc: Map Markdown elements into the generic analyzer model types.
- signature: `class MarkdownModelExtractionMixin:`
- members:
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L87) — Extract Markdown sections (code blocks act as 'classes').
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L72) — Extract Markdown elements (headers act as 'functions').
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L121) — Extract Markdown references and definitions.
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L102) — Extract Markdown links and images (act as 'variables').
- uses (calls/refs, reference-scoped): [`name`](../../models/base.md#CodeElement.name), [`start_line`](../../models/base.md#CodeElement.start_line), [`end_line`](../../models/base.md#CodeElement.end_line), [`language`](../../models/base.md#CodeElement.language), [`Function`](../../models/base.md#Function), [`raw_text`](../../models/base.md#CodeElement.raw_text), [`Class`](../../models/base.md#Class), [`Variable`](../../models/base.md#Variable), [`Import`](../../models/base.md#Import), [`MarkdownElementExtractor`](extractor.md#MarkdownElementExtractor)
- used by: [`MarkdownElementExtractor`](extractor.md#MarkdownElementExtractor), [`TREE_SITTER_AVAILABLE`](extractor.md#TREE_SITTER_AVAILABLE)  (8 test-only)

## Functions
- `_deduplicate_elements(elements: list[MarkdownElement], key_for: Callable[[MarkdownElement], tuple[str, str]])` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L53) — Return elements with duplicate display/url pairs removed.
- `_prepare_public_extraction(extractor: object, tree: object | None, source_code: str)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L26) — Set per-call extractor state and return the tree root, if available.
- `_run_extractors(root_node: object | None, error_context: str, *extractors: Callable[[object], None])` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/public_extraction.py#L38) — Run public extraction callbacks with consistent error logging.

