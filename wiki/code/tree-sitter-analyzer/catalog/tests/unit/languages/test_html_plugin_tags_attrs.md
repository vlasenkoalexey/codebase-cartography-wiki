---
title: 'Module: tests/unit/languages/test_html_plugin_tags_attrs.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_html_plugin_tags_attrs.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_html_plugin_tags_attrs`/TestHtml
symbols:
  TestHtmlTagRecognition.test_extract_structure_tags: TagRecognition#test_extract_structure_tags().
  TestHtmlTagRecognition.test_extract_heading_tags: TagRecognition#test_extract_heading_tags().
  TestHtmlTagRecognition.test_extract_text_tags: TagRecognition#test_extract_text_tags().
  TestHtmlTagRecognition.test_extract_div_tag: TagRecognition#test_extract_div_tag().
  TestHtmlTagRecognition.test_extract_span_tag: TagRecognition#test_extract_span_tag().
  TestHtmlTagRecognition.test_extract_paragraph_tag: TagRecognition#test_extract_paragraph_tag().
  TestHtmlTagRecognition.test_extract_list_tags: TagRecognition#test_extract_list_tags().
  TestHtmlTagRecognition.test_extract_inline_tags: TagRecognition#test_extract_inline_tags().
  TestHtmlAttributeRecognition.test_extract_id_attribute: AttributeRecognition#test_extract_id_attribute().
  TestHtmlAttributeRecognition.test_extract_class_attribute: AttributeRecognition#test_extract_class_attribute().
  TestHtmlAttributeRecognition.test_extract_data_attributes: AttributeRecognition#test_extract_data_attributes().
  TestHtmlAttributeRecognition.test_extract_style_attribute: AttributeRecognition#test_extract_style_attribute().
  TestHtmlAttributeRecognition.test_extract_event_attributes: AttributeRecognition#test_extract_event_attributes().
  TestHtmlAttributeRecognition.test_extract_href_attribute: AttributeRecognition#test_extract_href_attribute().
  TestHtmlAttributeRecognition.test_extract_src_attribute: AttributeRecognition#test_extract_src_attribute().
  TestHtmlAttributeRecognition.test_extract_alt_attribute: AttributeRecognition#test_extract_alt_attribute().
  TestHtmlAttributeRecognition.test_extract_multiple_attributes: AttributeRecognition#test_extract_multiple_attributes().
  TestHtmlTagRecognition: TagRecognition#
  TestHtmlAttributeRecognition: AttributeRecognition#
---
# Module: [`tests/unit/languages/test_html_plugin_tags_attrs.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py)

## Classes
### `TestHtmlAttributeRecognition`
- def: [`tests/unit/languages/test_html_plugin_tags_attrs.py:118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py#L118)
- doc: Test HTML attribute recognition and extraction.
- signature: `class TestHtmlAttributeRecognition:`
- members:
  - `test_extract_alt_attribute(self)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py#L210) — Test extraction of alt attribute.
  - `test_extract_class_attribute(self)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py#L133) — Test extraction of class attribute.
  - `test_extract_data_attributes(self)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py#L145) — Test extraction of data attributes.
  - `test_extract_event_attributes(self)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py#L169) — Test extraction of event attributes.
  - `test_extract_href_attribute(self)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py#L181) — Test extraction of href attribute.
  - `test_extract_id_attribute(self)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py#L121) — Test extraction of id attribute.
  - `test_extract_multiple_attributes(self)` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py#L227) — Test extraction of multiple attributes.
  - `test_extract_src_attribute(self)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py#L193) — Test extraction of src attribute.
  - `test_extract_style_attribute(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py#L157) — Test extraction of style attribute.
- uses (calls/refs, reference-scoped): [`HtmlPlugin`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin.create_extractor), [`extract_html_elements`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_html_elements)  (2 test-only)

### `TestHtmlTagRecognition`
- def: [`tests/unit/languages/test_html_plugin_tags_attrs.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py#L11)
- doc: Test HTML tag recognition and extraction.
- signature: `class TestHtmlTagRecognition:`
- members:
  - `test_extract_div_tag(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py#L48) — Test extraction of div tag.
  - `test_extract_heading_tags(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py#L25) — Test extraction of heading tags.
  - `test_extract_inline_tags(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py#L91) — Test extraction of inline tags.
  - `test_extract_list_tags(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py#L79) — Test extraction of list tags.
  - `test_extract_paragraph_tag(self)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py#L69) — Test extraction of paragraph tag.
  - `test_extract_span_tag(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py#L58) — Test extraction of span tag.
  - `test_extract_structure_tags(self)` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py#L14) — Test extraction of structure tags.
  - `test_extract_text_tags(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_tags_attrs.py#L36) — Test extraction of text tags.
- uses (calls/refs, reference-scoped): [`HtmlPlugin`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin.create_extractor), [`extract_html_elements`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_html_elements)  (2 test-only)

