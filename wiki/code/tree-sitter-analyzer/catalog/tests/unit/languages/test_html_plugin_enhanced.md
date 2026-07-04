---
title: 'Module: tests/unit/languages/test_html_plugin_enhanced.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_html_plugin_enhanced.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_html_plugin_enhanced`/
symbols:
  get_tree_for_code: get_tree_for_code().
  FORM_CODE: FORM_CODE.
  ATTRIBUTE_CODE: ATTRIBUTE_CODE.
  TABLE_CODE: TABLE_CODE.
  TAG_CODE: TAG_CODE.
  TestHtmlTagRecognition.test_extract_structure_tags: TestHtmlTagRecognition#test_extract_structure_tags().
  TestHtmlTagRecognition.test_extract_heading_tags: TestHtmlTagRecognition#test_extract_heading_tags().
  TestHtmlTagRecognition.test_extract_text_tags: TestHtmlTagRecognition#test_extract_text_tags().
  TestHtmlTagRecognition.test_extract_div_tag: TestHtmlTagRecognition#test_extract_div_tag().
  TestHtmlTagRecognition.test_extract_span_tag: TestHtmlTagRecognition#test_extract_span_tag().
  TestHtmlTagRecognition.test_extract_paragraph_tag: TestHtmlTagRecognition#test_extract_paragraph_tag().
  TestHtmlTagRecognition.test_extract_list_tags: TestHtmlTagRecognition#test_extract_list_tags().
  TestHtmlTagRecognition.test_extract_inline_tags: TestHtmlTagRecognition#test_extract_inline_tags().
  TestHtmlAttributeRecognition.test_extract_id_attribute: TestHtmlAttributeRecognition#test_extract_id_attribute().
  TestHtmlAttributeRecognition.test_extract_class_attribute: TestHtmlAttributeRecognition#test_extract_class_attribute().
  TestHtmlAttributeRecognition.test_extract_data_attributes: TestHtmlAttributeRecognition#test_extract_data_attributes().
  TestHtmlAttributeRecognition.test_extract_style_attribute: TestHtmlAttributeRecognition#test_extract_style_attribute().
  TestHtmlAttributeRecognition.test_extract_event_attributes: TestHtmlAttributeRecognition#test_extract_event_attributes().
  TestHtmlAttributeRecognition.test_extract_href_attribute: TestHtmlAttributeRecognition#test_extract_href_attribute().
  TestHtmlAttributeRecognition.test_extract_src_attribute: TestHtmlAttributeRecognition#test_extract_src_attribute().
  TestHtmlAttributeRecognition.test_extract_alt_attribute: TestHtmlAttributeRecognition#test_extract_alt_attribute().
  TestHtmlAttributeRecognition.test_extract_multiple_attributes: TestHtmlAttributeRecognition#test_extract_multiple_attributes().
  TestHtmlFormRecognition.test_extract_form_tag: TestHtmlFormRecognition#test_extract_form_tag().
  TestHtmlFormRecognition.test_extract_input_tags: TestHtmlFormRecognition#test_extract_input_tags().
  TestHtmlFormRecognition.test_extract_text_input: TestHtmlFormRecognition#test_extract_text_input().
  TestHtmlFormRecognition.test_extract_password_input: TestHtmlFormRecognition#test_extract_password_input().
  TestHtmlFormRecognition.test_extract_checkbox_input: TestHtmlFormRecognition#test_extract_checkbox_input().
  TestHtmlFormRecognition.test_extract_radio_input: TestHtmlFormRecognition#test_extract_radio_input().
  TestHtmlFormRecognition.test_extract_select_tag: TestHtmlFormRecognition#test_extract_select_tag().
  TestHtmlFormRecognition.test_extract_option_tags: TestHtmlFormRecognition#test_extract_option_tags().
  TestHtmlFormRecognition.test_extract_textarea_tag: TestHtmlFormRecognition#test_extract_textarea_tag().
  TestHtmlFormRecognition.test_extract_button_tag: TestHtmlFormRecognition#test_extract_button_tag().
  TestHtmlFormRecognition.test_extract_label_tag: TestHtmlFormRecognition#test_extract_label_tag().
  TestHtmlTableRecognition.test_extract_table_tag: TestHtmlTableRecognition#test_extract_table_tag().
  TestHtmlTableRecognition.test_extract_thead_tag: TestHtmlTableRecognition#test_extract_thead_tag().
  TestHtmlTableRecognition.test_extract_tbody_tag: TestHtmlTableRecognition#test_extract_tbody_tag().
  TestHtmlTableRecognition.test_extract_tfoot_tag: TestHtmlTableRecognition#test_extract_tfoot_tag().
  TestHtmlTableRecognition.test_extract_tr_tag: TestHtmlTableRecognition#test_extract_tr_tag().
  TestHtmlTableRecognition.test_extract_th_tag: TestHtmlTableRecognition#test_extract_th_tag().
  TestHtmlTableRecognition.test_extract_td_tag: TestHtmlTableRecognition#test_extract_td_tag().
  TestHtmlTableRecognition.test_extract_caption_tag: TestHtmlTableRecognition#test_extract_caption_tag().
  TestHtmlTableRecognition.test_extract_table_attributes: TestHtmlTableRecognition#test_extract_table_attributes().
  LINK_IMAGE_CODE: LINK_IMAGE_CODE.
  SCRIPT_STYLE_CODE: SCRIPT_STYLE_CODE.
  COMPLEX_STRUCTURE_CODE: COMPLEX_STRUCTURE_CODE.
  TestHtmlTagRecognition: TestHtmlTagRecognition#
  TestHtmlAttributeRecognition: TestHtmlAttributeRecognition#
  TestHtmlFormRecognition: TestHtmlFormRecognition#
  TestHtmlTableRecognition: TestHtmlTableRecognition#
---
# Module: [`tests/unit/languages/test_html_plugin_enhanced.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py)

## Classes
### `TestHtmlAttributeRecognition`
- def: [`tests/unit/languages/test_html_plugin_enhanced.py:409`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L409)
- doc: Test HTML attribute recognition and extraction.
- signature: `class TestHtmlAttributeRecognition:`
- members:
  - `test_extract_alt_attribute(self)` — [`L501`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L501) — Test extraction of alt attribute.
  - `test_extract_class_attribute(self)` — [`L424`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L424) — Test extraction of class attribute.
  - `test_extract_data_attributes(self)` — [`L436`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L436) — Test extraction of data attributes.
  - `test_extract_event_attributes(self)` — [`L460`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L460) — Test extraction of event attributes.
  - `test_extract_href_attribute(self)` — [`L472`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L472) — Test extraction of href attribute.
  - `test_extract_id_attribute(self)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L412) — Test extraction of id attribute.
  - `test_extract_multiple_attributes(self)` — [`L518`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L518) — Test extraction of multiple attributes.
  - `test_extract_src_attribute(self)` — [`L484`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L484) — Test extraction of src attribute.
  - `test_extract_style_attribute(self)` — [`L448`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L448) — Test extraction of style attribute.
- uses (calls/refs, reference-scoped): [`HtmlPlugin`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin.create_extractor), [`extract_html_elements`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_html_elements)  (2 test-only)

### `TestHtmlFormRecognition`
- def: [`tests/unit/languages/test_html_plugin_enhanced.py:533`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L533)
- doc: Test HTML form element recognition and extraction.
- signature: `class TestHtmlFormRecognition:`
- members:
  - `test_extract_button_tag(self)` — [`L657`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L657) — Test extraction of button tag.
  - `test_extract_checkbox_input(self)` — [`L592`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L592) — Test extraction of checkbox input.
  - `test_extract_form_tag(self)` — [`L536`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L536) — Test extraction of form tag.
  - `test_extract_input_tags(self)` — [`L545`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L545) — Test extraction of input tags.
  - `test_extract_label_tag(self)` — [`L666`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L666) — Test extraction of label tag.
  - `test_extract_option_tags(self)` — [`L639`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L639) — Test extraction of option tags.
  - `test_extract_password_input(self)` — [`L573`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L573) — Test extraction of password input.
  - `test_extract_radio_input(self)` — [`L611`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L611) — Test extraction of radio input.
  - `test_extract_select_tag(self)` — [`L630`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L630) — Test extraction of select tag.
  - `test_extract_text_input(self)` — [`L554`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L554) — Test extraction of text input.
  - `test_extract_textarea_tag(self)` — [`L648`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L648) — Test extraction of textarea tag.
- uses (calls/refs, reference-scoped): [`HtmlPlugin`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin.create_extractor), [`extract_html_elements`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_html_elements)  (2 test-only)

### `TestHtmlTableRecognition`
- def: [`tests/unit/languages/test_html_plugin_enhanced.py:676`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L676)
- doc: Test HTML table element recognition and extraction.
- signature: `class TestHtmlTableRecognition:`
- members:
  - `test_extract_caption_tag(self)` — [`L742`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L742) — Test extraction of caption tag.
  - `test_extract_table_attributes(self)` — [`L751`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L751) — Test extraction of table attributes.
  - `test_extract_table_tag(self)` — [`L679`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L679) — Test extraction of table tag.
  - `test_extract_tbody_tag(self)` — [`L697`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L697) — Test extraction of tbody tag.
  - `test_extract_td_tag(self)` — [`L733`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L733) — Test extraction of td tag.
  - `test_extract_tfoot_tag(self)` — [`L706`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L706) — Test extraction of tfoot tag.
  - `test_extract_th_tag(self)` — [`L724`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L724) — Test extraction of th tag.
  - `test_extract_thead_tag(self)` — [`L688`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L688) — Test extraction of thead tag.
  - `test_extract_tr_tag(self)` — [`L715`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L715) — Test extraction of tr tag.
- uses (calls/refs, reference-scoped): [`HtmlPlugin`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin.create_extractor), [`extract_html_elements`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_html_elements)  (2 test-only)

### `TestHtmlTagRecognition`
- def: [`tests/unit/languages/test_html_plugin_enhanced.py:324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L324)
- doc: Test HTML tag recognition and extraction.
- signature: `class TestHtmlTagRecognition:`
- members:
  - `test_extract_div_tag(self)` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L354) — Test extraction of div tag.
  - `test_extract_heading_tags(self)` — [`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L336) — Test extraction of heading tags.
  - `test_extract_inline_tags(self)` — [`L394`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L394) — Test extraction of inline tags.
  - `test_extract_list_tags(self)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L383) — Test extraction of list tags.
  - `test_extract_paragraph_tag(self)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L374) — Test extraction of paragraph tag.
  - `test_extract_span_tag(self)` — [`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L363) — Test extraction of span tag.
  - `test_extract_structure_tags(self)` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L327) — Test extraction of structure tags.
  - `test_extract_text_tags(self)` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L345) — Test extraction of text tags.
- uses (calls/refs, reference-scoped): [`HtmlPlugin`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin.create_extractor), [`extract_html_elements`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_html_elements)  (2 test-only)

## Functions
- `get_tree_for_code(code: str, plugin: HtmlPlugin)` — [`L309`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L309) — Helper to parse HTML code and return tree.

## Module values
- `ATTRIBUTE_CODE` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L45)
- `COMPLEX_STRUCTURE_CODE` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L262)
- `FORM_CODE` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L86)
- `LINK_IMAGE_CODE` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L192)
- `SCRIPT_STYLE_CODE` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L218)
- `TABLE_CODE` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L138)
- `TAG_CODE` — [`L6`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_enhanced.py#L6)

