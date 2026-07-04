---
title: 'Module: tests/unit/languages/test_markdown_plugin_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_markdown_plugin_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_markdown_plugin_coverage`/
symbols:
  _setup_extractor: _setup_extractor().
  TestMarkdownElementAttributes.test_all_attributes_set: TestMarkdownElementAttributes#test_all_attributes_set().
  TestMarkdownElementAttributes.test_default_attributes: TestMarkdownElementAttributes#test_default_attributes().
  _make_node: _make_node().
  TestPublicExtractMethods.test_extract_links_delegates: TestPublicExtractMethods#test_extract_links_delegates().
  TestPublicExtractMethods.test_extract_images_delegates: TestPublicExtractMethods#test_extract_images_delegates().
  TestPublicExtractMethods.test_extract_text_formatting: TestPublicExtractMethods#test_extract_text_formatting().
  TestPublicExtractMethods.test_extract_footnotes: TestPublicExtractMethods#test_extract_footnotes().
  TestPublicExtractMethods.test_extract_lists: TestPublicExtractMethods#test_extract_lists().
  TestPublicExtractMethods.test_extract_tables: TestPublicExtractMethods#test_extract_tables().
  TestPublicExtractMethods.test_extract_html_elements: TestPublicExtractMethods#test_extract_html_elements().
  TestPublicExtractMethods.test_extract_horizontal_rules: TestPublicExtractMethods#test_extract_horizontal_rules().
  TestPublicExtractMethods._mk_tree: TestPublicExtractMethods#_mk_tree().
  TestExtractFootnoteElements.test_footnote_reference: TestExtractFootnoteElements#test_footnote_reference().
  TestExtractFootnoteElements.test_footnote_definition: TestExtractFootnoteElements#test_footnote_definition().
  TestExtractFootnoteElements.test_footnote_no_match: TestExtractFootnoteElements#test_footnote_no_match().
  TestExtractInlineImages.test_inline_image: TestExtractInlineImages#test_inline_image().
  TestExtractInlineImages.test_inline_image_no_inline: TestExtractInlineImages#test_inline_image_no_inline().
  TestExtractImageRefDefs.test_image_ref_by_usage: TestExtractImageRefDefs#test_image_ref_by_usage().
  TestExtractImageRefDefs.test_image_ref_by_url_extension: TestExtractImageRefDefs#test_image_ref_by_url_extension().
  TestExtractImageRefDefs.test_image_ref_no_match: TestExtractImageRefDefs#test_image_ref_no_match().
  TestExtractInlineLinks.test_inline_link: TestExtractInlineLinks#test_inline_link().
  TestExtractInlineLinks.test_inline_link_no_inline: TestExtractInlineLinks#test_inline_link_no_inline().
  TestExtractInlineLinks.test_inline_link_with_title: TestExtractInlineLinks#test_inline_link_with_title().
  TestAnalyzeFile.test_empty_source: TestAnalyzeFile#test_empty_source().
  TestExtractFootnoteElements: TestExtractFootnoteElements#
  TestExtractInlineImages: TestExtractInlineImages#
  TestExtractImageRefDefs: TestExtractImageRefDefs#
  TestExtractInlineLinks: TestExtractInlineLinks#
  TestPublicExtractMethods: TestPublicExtractMethods#
  TestAnalyzeFile: TestAnalyzeFile#
  TestMarkdownElementAttributes: TestMarkdownElementAttributes#
---
# Module: [`tests/unit/languages/test_markdown_plugin_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py)

## Classes
### `TestAnalyzeFile`
- def: [`tests/unit/languages/test_markdown_plugin_coverage.py:424`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L424)
- signature: `class TestAnalyzeFile:`
- members:
  - `test_empty_source(self)` — [`L425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L425)
- uses (calls/refs, reference-scoped): [`MarkdownPlugin`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin), [`extract_all_elements`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_all_elements), [`create_extractor`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin.create_extractor)

### `TestExtractFootnoteElements`
- def: [`tests/unit/languages/test_markdown_plugin_coverage.py:64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L64)
- signature: `class TestExtractFootnoteElements:`
- members:
  - `test_footnote_definition(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L84)
  - `test_footnote_no_match(self)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L103)
  - `test_footnote_reference(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L65)
- uses (calls/refs, reference-scoped): [`_extract_footnote_elements`](../../../tree_sitter_analyzer/languages/markdown_plugin/private_extraction.md#MarkdownMiscPrivateExtractionMixin._extract_footnote_elements)  (2 test-only)

### `TestExtractImageRefDefs`
- def: [`tests/unit/languages/test_markdown_plugin_coverage.py:160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L160)
- signature: `class TestExtractImageRefDefs:`
- members:
  - `test_image_ref_by_url_extension(self)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L185)
  - `test_image_ref_by_usage(self)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L161)
  - `test_image_ref_no_match(self)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L206)
- uses (calls/refs, reference-scoped): [`_extract_image_reference_definitions`](../../../tree_sitter_analyzer/languages/markdown_plugin/private_extraction.md#MarkdownLinkImagePrivateExtractionMixin._extract_image_reference_definitions)  (2 test-only)

### `TestExtractInlineImages`
- def: [`tests/unit/languages/test_markdown_plugin_coverage.py:126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L126)
- signature: `class TestExtractInlineImages:`
- members:
  - `test_inline_image(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L127)
  - `test_inline_image_no_inline(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L147)
- uses (calls/refs, reference-scoped): [`_extract_inline_images`](../../../tree_sitter_analyzer/languages/markdown_plugin/private_extraction.md#MarkdownLinkImagePrivateExtractionMixin._extract_inline_images)  (2 test-only)

### `TestExtractInlineLinks`
- def: [`tests/unit/languages/test_markdown_plugin_coverage.py:229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L229)
- signature: `class TestExtractInlineLinks:`
- members:
  - `test_inline_link(self)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L230)
  - `test_inline_link_no_inline(self)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L249)
  - `test_inline_link_with_title(self)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L256)
- uses (calls/refs, reference-scoped): [`_extract_inline_links`](../../../tree_sitter_analyzer/languages/markdown_plugin/private_extraction.md#MarkdownLinkImagePrivateExtractionMixin._extract_inline_links)  (2 test-only)

### `TestMarkdownElementAttributes`
- def: [`tests/unit/languages/test_markdown_plugin_coverage.py:438`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L438)
- signature: `class TestMarkdownElementAttributes:`
- members:
  - `test_all_attributes_set(self)` — [`L439`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L439)
  - `test_default_attributes(self)` — [`L474`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L474)
- uses (calls/refs, reference-scoped): [`MarkdownElement`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement), [`text`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement.text), [`line_count`](../../../tree_sitter_analyzer/models/base.md#CodeElement.line_count), [`alt`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement.alt), [`alt_text`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement.alt_text), [`column_count`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement.column_count), [`item_count`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement.item_count), [`list_type`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement.list_type), [`row_count`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement.row_count), [`url`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement.url), [`is_checked`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement.is_checked), [`language_info`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement.language_info), [`level`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement.level), [`title`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement.title)

### `TestPublicExtractMethods`
- def: [`tests/unit/languages/test_markdown_plugin_coverage.py:280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L280)
- doc: Test public extract_* methods that delegate to private _extract_* methods.
- signature: `class TestPublicExtractMethods:`
- members:
  - `test_extract_footnotes(self)` — [`L335`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L335)
  - `test_extract_horizontal_rules(self)` — [`L406`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L406)
  - `test_extract_html_elements(self)` — [`L391`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L391)
  - `test_extract_images_delegates(self)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L305)
  - `test_extract_links_delegates(self)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L290)
  - `test_extract_lists(self)` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L350)
  - `test_extract_tables(self)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L378)
  - `test_extract_text_formatting(self)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L320)
- protocol/private: `_mk_tree`[`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L283)
- uses (calls/refs, reference-scoped): [`extract_images`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownInlineExtractionMixin.extract_images), [`extract_links`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownInlineExtractionMixin.extract_links), [`source_code`](../../../tree_sitter_analyzer/languages/markdown_plugin/extractor.md#MarkdownElementExtractor.source_code), [`extract_footnotes`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownInlineExtractionMixin.extract_footnotes), [`extract_horizontal_rules`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownBlockExtractionMixin.extract_horizontal_rules), [`extract_html_elements`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownBlockExtractionMixin.extract_html_elements), [`extract_text_formatting`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownInlineExtractionMixin.extract_text_formatting), [`extract_lists`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownBlockExtractionMixin.extract_lists), [`extract_tables`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownBlockExtractionMixin.extract_tables)  (2 test-only)

## Functions
- `_make_node(node_type, start_point=(0, 0), end_point=None, children=None, text="", start_byte=0, end_byte=None)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L23)
- `_setup_extractor(source_code, content_lines=None)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage.py#L47)

