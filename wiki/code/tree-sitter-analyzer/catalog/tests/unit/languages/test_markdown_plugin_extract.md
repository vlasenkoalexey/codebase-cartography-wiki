---
title: 'Module: tests/unit/languages/test_markdown_plugin_extract.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_markdown_plugin_extract.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_markdown_plugin_extract`/
symbols:
  _make_node: _make_node().
  _setup_extractor: _setup_extractor().
  TestExtractAutolinks.test_autolink_duplicate_skip: TestExtractAutolinks#test_autolink_duplicate_skip().
  TestExtractAutolinks.test_autolink_url: TestExtractAutolinks#test_autolink_url().
  TestExtractAutolinks.test_autolink_mailto: TestExtractAutolinks#test_autolink_mailto().
  TestExtractAutolinks.test_autolink_email: TestExtractAutolinks#test_autolink_email().
  TestExtractAutolinks.test_autolink_no_inline_node: TestExtractAutolinks#test_autolink_no_inline_node().
  TestExtractAutolinks.test_autolink_empty_text: TestExtractAutolinks#test_autolink_empty_text().
  TestExtractReferenceImages.test_reference_image_basic: TestExtractReferenceImages#test_reference_image_basic().
  TestExtractReferenceImages.test_reference_image_empty_alt: TestExtractReferenceImages#test_reference_image_empty_alt().
  TestExtractReferenceImages.test_reference_image_no_inline: TestExtractReferenceImages#test_reference_image_no_inline().
  TestExtractInlineHTML.test_inline_html_tag: TestExtractInlineHTML#test_inline_html_tag().
  TestExtractInlineHTML.test_inline_html_br_tag: TestExtractInlineHTML#test_inline_html_br_tag().
  TestExtractInlineHTML.test_inline_html_not_autolink: TestExtractInlineHTML#test_inline_html_not_autolink().
  TestExtractInlineHTML.test_inline_html_no_inline: TestExtractInlineHTML#test_inline_html_no_inline().
  TestExtractPipeTables.test_pipe_table: TestExtractPipeTables#test_pipe_table().
  TestExtractPipeTables.test_pipe_table_no_pipe_node: TestExtractPipeTables#test_pipe_table_no_pipe_node().
  TestExtractEmphasisElements.test_bold: TestExtractEmphasisElements#test_bold().
  TestExtractEmphasisElements.test_bold_underscore: TestExtractEmphasisElements#test_bold_underscore().
  TestExtractEmphasisElements.test_italic: TestExtractEmphasisElements#test_italic().
  TestExtractEmphasisElements.test_italic_underscore: TestExtractEmphasisElements#test_italic_underscore().
  TestExtractEmphasisElements.test_no_inline: TestExtractEmphasisElements#test_no_inline().
  TestExtractStrikethrough.test_strikethrough: TestExtractStrikethrough#test_strikethrough().
  TestExtractStrikethrough.test_strikethrough_no_inline: TestExtractStrikethrough#test_strikethrough_no_inline().
  TestExtractStrikethrough.test_strikethrough_multiple: TestExtractStrikethrough#test_strikethrough_multiple().
  TestExecuteQueryStrategy.test_none_query: TestExecuteQueryStrategy#test_none_query().
  TestExecuteQueryStrategy.test_known_category: TestExecuteQueryStrategy#test_known_category().
  TestExecuteQueryStrategy.test_unknown_category_fallback_to_queries: TestExecuteQueryStrategy#test_unknown_category_fallback_to_queries().
  TestExecuteQueryStrategy.test_category_headers: TestExecuteQueryStrategy#test_category_headers().
  TestExecuteQueryStrategy.test_category_links: TestExecuteQueryStrategy#test_category_links().
  TestExecuteQueryStrategy.test_category_all_elements: TestExecuteQueryStrategy#test_category_all_elements().
  TestExtractAutolinks: TestExtractAutolinks#
  TestExtractReferenceImages: TestExtractReferenceImages#
  TestExtractInlineHTML: TestExtractInlineHTML#
  TestExecuteQueryStrategy: TestExecuteQueryStrategy#
  TestExtractPipeTables: TestExtractPipeTables#
  TestExtractEmphasisElements: TestExtractEmphasisElements#
  TestExtractStrikethrough: TestExtractStrikethrough#
---
# Module: [`tests/unit/languages/test_markdown_plugin_extract.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py)

## Classes
### `TestExecuteQueryStrategy`
- def: [`tests/unit/languages/test_markdown_plugin_extract.py:275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L275)
- signature: `class TestExecuteQueryStrategy:`
- members:
  - `test_category_all_elements(self)` — [`L302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L302)
  - `test_category_headers(self)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L292)
  - `test_category_links(self)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L297)
  - `test_known_category(self)` — [`L281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L281)
  - `test_none_query(self)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L276)
  - `test_unknown_category_fallback_to_queries(self)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L287)
- uses (calls/refs, reference-scoped): [`MarkdownPlugin`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin), [`execute_query_strategy`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin.execute_query_strategy)

### `TestExtractAutolinks`
- def: [`tests/unit/languages/test_markdown_plugin_extract.py:63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L63)
- signature: `class TestExtractAutolinks:`
- members:
  - `test_autolink_duplicate_skip(self)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L121)
  - `test_autolink_email(self)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L103)
  - `test_autolink_empty_text(self)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L148)
  - `test_autolink_mailto(self)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L85)
  - `test_autolink_no_inline_node(self)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L139)
  - `test_autolink_url(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L64)
- uses (calls/refs, reference-scoped): [`_extract_autolinks`](../../../tree_sitter_analyzer/languages/markdown_plugin/private_extraction.md#MarkdownLinkImagePrivateExtractionMixin._extract_autolinks), [`_extracted_links`](../../../tree_sitter_analyzer/languages/markdown_plugin/extractor.md#MarkdownElementExtractor._extracted_links)  (2 test-only)

### `TestExtractEmphasisElements`
- def: [`tests/unit/languages/test_markdown_plugin_extract.py:352`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L352)
- signature: `class TestExtractEmphasisElements:`
- members:
  - `test_bold(self)` — [`L353`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L353)
  - `test_bold_underscore(self)` — [`L372`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L372)
  - `test_italic(self)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L390)
  - `test_italic_underscore(self)` — [`L409`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L409)
  - `test_no_inline(self)` — [`L427`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L427)
- uses (calls/refs, reference-scoped): [`_extract_emphasis_elements`](../../../tree_sitter_analyzer/languages/markdown_plugin/private_extraction.md#MarkdownMiscPrivateExtractionMixin._extract_emphasis_elements)  (2 test-only)

### `TestExtractInlineHTML`
- def: [`tests/unit/languages/test_markdown_plugin_extract.py:211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L211)
- signature: `class TestExtractInlineHTML:`
- members:
  - `test_inline_html_br_tag(self)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L231)
  - `test_inline_html_no_inline(self)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L262)
  - `test_inline_html_not_autolink(self)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L245)
  - `test_inline_html_tag(self)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L212)
- uses (calls/refs, reference-scoped): [`_extract_inline_html`](../../../tree_sitter_analyzer/languages/markdown_plugin/private_extraction.md#MarkdownMiscPrivateExtractionMixin._extract_inline_html)  (2 test-only)

### `TestExtractPipeTables`
- def: [`tests/unit/languages/test_markdown_plugin_extract.py:313`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L313)
- signature: `class TestExtractPipeTables:`
- members:
  - `test_pipe_table(self)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L314)
  - `test_pipe_table_no_pipe_node(self)` — [`L339`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L339)
- uses (calls/refs, reference-scoped): [`_extract_pipe_tables`](../../../tree_sitter_analyzer/languages/markdown_plugin/private_extraction.md#MarkdownBlockPrivateExtractionMixin._extract_pipe_tables)  (2 test-only)

### `TestExtractReferenceImages`
- def: [`tests/unit/languages/test_markdown_plugin_extract.py:166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L166)
- signature: `class TestExtractReferenceImages:`
- members:
  - `test_reference_image_basic(self)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L167)
  - `test_reference_image_empty_alt(self)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L183)
  - `test_reference_image_no_inline(self)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L198)
- uses (calls/refs, reference-scoped): [`_extract_reference_images`](../../../tree_sitter_analyzer/languages/markdown_plugin/private_extraction.md#MarkdownLinkImagePrivateExtractionMixin._extract_reference_images)  (2 test-only)

### `TestExtractStrikethrough`
- def: [`tests/unit/languages/test_markdown_plugin_extract.py:440`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L440)
- signature: `class TestExtractStrikethrough:`
- members:
  - `test_strikethrough(self)` — [`L441`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L441)
  - `test_strikethrough_multiple(self)` — [`L467`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L467)
  - `test_strikethrough_no_inline(self)` — [`L460`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L460)
- uses (calls/refs, reference-scoped): [`_extract_strikethrough_elements`](../../../tree_sitter_analyzer/languages/markdown_plugin/private_extraction.md#MarkdownMiscPrivateExtractionMixin._extract_strikethrough_elements)  (2 test-only)

## Functions
- `_make_node(node_type, start_point=(0, 0), end_point=None, children=None, text="", start_byte=0, end_byte=None)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L22)
- `_setup_extractor(source_code, content_lines=None)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_extract.py#L46)

