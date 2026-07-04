---
title: 'Module: tests/unit/languages/test_markdown_plugin_new_elements.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_markdown_plugin_new_elements.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_markdown_plugin_new_elements`/TestMarkdown
symbols:
  TestMarkdownNewElementsExtraction.extractor: NewElementsExtraction#extractor.
  TestMarkdownPluginNewElementsIntegration.test_analyze_file_with_new_elements: PluginNewElementsIntegration#test_analyze_file_with_new_elements().
  TestMarkdownNewElementsExtraction.test_extract_blockquotes_basic: NewElementsExtraction#test_extract_blockquotes_basic().
  TestMarkdownNewElementsExtraction.test_extract_horizontal_rules_basic: NewElementsExtraction#test_extract_horizontal_rules_basic().
  TestMarkdownNewElementsExtraction.test_extract_html_elements_basic: NewElementsExtraction#test_extract_html_elements_basic().
  TestMarkdownPluginNewElementsIntegration.plugin: PluginNewElementsIntegration#plugin.
  TestMarkdownNewElementsExtraction.test_extract_text_formatting_basic: NewElementsExtraction#test_extract_text_formatting_basic().
  TestMarkdownNewElementsExtraction.test_extract_footnotes_basic: NewElementsExtraction#test_extract_footnotes_basic().
  TestMarkdownPluginNewElementsIntegration.test_extract_elements_includes_new_elements: PluginNewElementsIntegration#test_extract_elements_includes_new_elements().
  TestMarkdownElementNewAttributes.test_markdown_element_blockquote_attributes: ElementNewAttributes#test_markdown_element_blockquote_attributes().
  TestMarkdownElementNewAttributes.test_markdown_element_html_attributes: ElementNewAttributes#test_markdown_element_html_attributes().
  TestMarkdownElementNewAttributes.test_markdown_element_formatting_attributes: ElementNewAttributes#test_markdown_element_formatting_attributes().
  TestMarkdownElementNewAttributes.test_markdown_element_footnote_attributes: ElementNewAttributes#test_markdown_element_footnote_attributes().
  TestMarkdownNewElementsExtraction.test_extract_blockquotes_empty: NewElementsExtraction#test_extract_blockquotes_empty().
  TestMarkdownNewElementsExtraction.test_extract_blockquotes_with_exception: NewElementsExtraction#test_extract_blockquotes_with_exception().
  TestMarkdownNewElementsExtraction.test_extract_horizontal_rules_with_exception: NewElementsExtraction#test_extract_horizontal_rules_with_exception().
  TestMarkdownNewElementsExtraction.test_extract_html_elements_with_exception: NewElementsExtraction#test_extract_html_elements_with_exception().
  TestMarkdownNewElementsExtraction.test_extract_text_formatting_with_exception: NewElementsExtraction#test_extract_text_formatting_with_exception().
  TestMarkdownNewElementsExtraction.test_extract_footnotes_with_exception: NewElementsExtraction#test_extract_footnotes_with_exception().
  TestMarkdownPluginNewElementsIntegration.test_get_supported_queries_includes_new_queries: PluginNewElementsIntegration#test_get_supported_queries_includes_new_queries().
  TestMarkdownNewElementsExtraction.plugin: NewElementsExtraction#plugin.
  TestMarkdownNewElementsExtraction: NewElementsExtraction#
  TestMarkdownNewElementsExtraction.setup_method: NewElementsExtraction#setup_method().
  TestMarkdownPluginNewElementsIntegration: PluginNewElementsIntegration#
  TestMarkdownPluginNewElementsIntegration.setup_method: PluginNewElementsIntegration#setup_method().
  TestMarkdownElementNewAttributes: ElementNewAttributes#
---
# Module: [`tests/unit/languages/test_markdown_plugin_new_elements.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py)

## Classes
### `TestMarkdownElementNewAttributes`
- def: [`tests/unit/languages/test_markdown_plugin_new_elements.py:531`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L531)
- doc: Test MarkdownElement with new attributes for new element types
- signature: `class TestMarkdownElementNewAttributes:`
- members:
  - `test_markdown_element_blockquote_attributes(self)` — [`L534`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L534) — Test MarkdownElement with blockquote-specific attributes
  - `test_markdown_element_footnote_attributes(self)` — [`L573`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L573) — Test MarkdownElement with footnote attributes
  - `test_markdown_element_formatting_attributes(self)` — [`L560`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L560) — Test MarkdownElement with text formatting attributes
  - `test_markdown_element_html_attributes(self)` — [`L547`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L547) — Test MarkdownElement with HTML-specific attributes
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`MarkdownElement`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement), [`element_type`](../../../tree_sitter_analyzer/models/base.md#CodeElement.element_type)

### `TestMarkdownNewElementsExtraction`
- def: [`tests/unit/languages/test_markdown_plugin_new_elements.py:24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L24)
- doc: Test new Markdown elements extraction functionality
- signature: `class TestMarkdownNewElementsExtraction:`
- members:
  - `setup_method(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L27) — Setup test fixtures
  - `test_extract_blockquotes_basic(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L32) — Test basic blockquote extraction
  - `test_extract_blockquotes_empty(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L68) — Test blockquote extraction with no blockquotes
  - `test_extract_blockquotes_with_exception(self)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L254) — Test blockquote extraction with exception handling
  - `test_extract_footnotes_basic(self)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L204) — Test basic footnote extraction
  - `test_extract_footnotes_with_exception(self)` — [`L332`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L332) — Test footnote extraction with exception handling
  - `test_extract_horizontal_rules_basic(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L81) — Test basic horizontal rule extraction
  - `test_extract_horizontal_rules_with_exception(self)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L274) — Test horizontal rule extraction with exception handling
  - `test_extract_html_elements_basic(self)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L121) — Test basic HTML element extraction
  - `test_extract_html_elements_with_exception(self)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L292) — Test HTML element extraction with exception handling
  - `test_extract_text_formatting_basic(self)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L160) — Test basic text formatting extraction
  - `test_extract_text_formatting_with_exception(self)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L312) — Test text formatting extraction with exception handling
  - `extractor` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L29)
  - `plugin` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L30)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`element_type`](../../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`MarkdownElementExtractor`](../../../tree_sitter_analyzer/languages/markdown_plugin/extractor.md#MarkdownElementExtractor), [`MarkdownPlugin`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin), [`extract_blockquotes`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownBlockExtractionMixin.extract_blockquotes), [`extract_footnotes`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownInlineExtractionMixin.extract_footnotes), [`extract_horizontal_rules`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownBlockExtractionMixin.extract_horizontal_rules), [`extract_html_elements`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownBlockExtractionMixin.extract_html_elements), [`extract_text_formatting`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownInlineExtractionMixin.extract_text_formatting)

### `TestMarkdownPluginNewElementsIntegration`
- def: [`tests/unit/languages/test_markdown_plugin_new_elements.py:353`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L353)
- doc: Integration tests for new Markdown elements in plugin
- signature: `class TestMarkdownPluginNewElementsIntegration:`
- members:
  - `setup_method(self)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L356) — Setup test fixtures
  - `test_analyze_file_with_new_elements(self)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L416) — Test analyze_file includes new elements in results
  - `test_extract_elements_includes_new_elements(self)` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L360) — Test that extract_elements includes new element types
  - `test_get_supported_queries_includes_new_queries(self)` — [`L405`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L405) — Test that get_supported_queries includes new query types
  - `plugin` — [`L358`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_new_elements.py#L358)
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`MarkdownElement`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement), [`MarkdownElementExtractor`](../../../tree_sitter_analyzer/languages/markdown_plugin/extractor.md#MarkdownElementExtractor), [`analyze_file`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin.analyze_file), [`extract_elements`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin.extract_elements), [`MarkdownPlugin`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin), [`get_supported_queries`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin.get_supported_queries)

