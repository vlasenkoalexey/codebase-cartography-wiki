---
title: 'Module: tests/unit/languages/test_html_plugin_advanced.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_html_plugin_advanced.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_html_plugin_advanced`/
symbols:
  get_tree_for_code: get_tree_for_code().
  LINK_IMAGE_CODE: LINK_IMAGE_CODE.
  SCRIPT_STYLE_CODE: SCRIPT_STYLE_CODE.
  COMPLEX_STRUCTURE_CODE: COMPLEX_STRUCTURE_CODE.
  TestHtmlLinkImageRecognition.test_extract_a_tag: TestHtmlLinkImageRecognition#test_extract_a_tag().
  TestHtmlLinkImageRecognition.test_extract_external_link: TestHtmlLinkImageRecognition#test_extract_external_link().
  TestHtmlLinkImageRecognition.test_extract_internal_link: TestHtmlLinkImageRecognition#test_extract_internal_link().
  TestHtmlLinkImageRecognition.test_extract_anchor_link: TestHtmlLinkImageRecognition#test_extract_anchor_link().
  TestHtmlLinkImageRecognition.test_extract_img_tag: TestHtmlLinkImageRecognition#test_extract_img_tag().
  TestHtmlLinkImageRecognition.test_extract_image_with_alt: TestHtmlLinkImageRecognition#test_extract_image_with_alt().
  TestHtmlLinkImageRecognition.test_extract_image_with_dimensions: TestHtmlLinkImageRecognition#test_extract_image_with_dimensions().
  TestHtmlLinkImageRecognition.test_extract_picture_tag: TestHtmlLinkImageRecognition#test_extract_picture_tag().
  TestHtmlLinkImageRecognition.test_extract_svg_tag: TestHtmlLinkImageRecognition#test_extract_svg_tag().
  TestHtmlScriptStyleRecognition.test_extract_script_tag: TestHtmlScriptStyleRecognition#test_extract_script_tag().
  TestHtmlScriptStyleRecognition.test_extract_style_tag: TestHtmlScriptStyleRecognition#test_extract_style_tag().
  TestHtmlScriptStyleRecognition.test_extract_link_tag: TestHtmlScriptStyleRecognition#test_extract_link_tag().
  TestHtmlScriptStyleRecognition.test_extract_meta_tag: TestHtmlScriptStyleRecognition#test_extract_meta_tag().
  TestHtmlScriptStyleRecognition.test_extract_title_tag: TestHtmlScriptStyleRecognition#test_extract_title_tag().
  TestHtmlScriptStyleRecognition.test_extract_script_with_src: TestHtmlScriptStyleRecognition#test_extract_script_with_src().
  TestHtmlScriptStyleRecognition.test_extract_style_with_href: TestHtmlScriptStyleRecognition#test_extract_style_with_href().
  TestHtmlComplexStructures.test_extract_nested_elements: TestHtmlComplexStructures#test_extract_nested_elements().
  TestHtmlComplexStructures.test_extract_parent_child_relationships: TestHtmlComplexStructures#test_extract_parent_child_relationships().
  TestHtmlComplexStructures.test_extract_multiple_classes: TestHtmlComplexStructures#test_extract_multiple_classes().
  TestHtmlComplexStructures.test_extract_doctype: TestHtmlComplexStructures#test_extract_doctype().
  TestHtmlComplexStructures.test_extract_html_tag: TestHtmlComplexStructures#test_extract_html_tag().
  TestHtmlComplexStructures.test_extract_head_tag: TestHtmlComplexStructures#test_extract_head_tag().
  TestHtmlComplexStructures.test_extract_body_tag: TestHtmlComplexStructures#test_extract_body_tag().
  TestHtmlQueryAccuracy.test_tag_query_accuracy: TestHtmlQueryAccuracy#test_tag_query_accuracy().
  TestHtmlQueryAccuracy.test_attribute_query_accuracy: TestHtmlQueryAccuracy#test_attribute_query_accuracy().
  TestHtmlQueryAccuracy.test_form_query_accuracy: TestHtmlQueryAccuracy#test_form_query_accuracy().
  TestHtmlQueryAccuracy.test_table_query_accuracy: TestHtmlQueryAccuracy#test_table_query_accuracy().
  TestHtmlQueryAccuracy.test_link_query_accuracy: TestHtmlQueryAccuracy#test_link_query_accuracy().
  TestHtmlQueryAccuracy.test_image_query_accuracy: TestHtmlQueryAccuracy#test_image_query_accuracy().
  TestHtmlQueryAccuracy.test_no_false_positives: TestHtmlQueryAccuracy#test_no_false_positives().
  TestHtmlQueryAccuracy.test_no_false_negatives: TestHtmlQueryAccuracy#test_no_false_negatives().
  TestHtmlQueryAccuracy.test_line_number_accuracy: TestHtmlQueryAccuracy#test_line_number_accuracy().
  TestHtmlQueryAccuracy.test_element_classification_accuracy: TestHtmlQueryAccuracy#test_element_classification_accuracy().
  TAG_CODE: TAG_CODE.
  ATTRIBUTE_CODE: ATTRIBUTE_CODE.
  FORM_CODE: FORM_CODE.
  TABLE_CODE: TABLE_CODE.
  TestHtmlLinkImageRecognition: TestHtmlLinkImageRecognition#
  TestHtmlScriptStyleRecognition: TestHtmlScriptStyleRecognition#
  TestHtmlComplexStructures: TestHtmlComplexStructures#
  TestHtmlQueryAccuracy: TestHtmlQueryAccuracy#
---
# Module: [`tests/unit/languages/test_html_plugin_advanced.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py)

## Classes
### `TestHtmlComplexStructures`
- def: [`tests/unit/languages/test_html_plugin_advanced.py:574`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L574)
- doc: Test extraction of complex HTML structures.
- signature: `class TestHtmlComplexStructures:`
- members:
  - `test_extract_body_tag(self)` — [`L653`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L653) — Test extraction of body tag.
  - `test_extract_doctype(self)` — [`L620`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L620) — Test extraction of DOCTYPE.
  - `test_extract_head_tag(self)` — [`L642`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L642) — Test extraction of head tag.
  - `test_extract_html_tag(self)` — [`L631`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L631) — Test extraction of html tag.
  - `test_extract_multiple_classes(self)` — [`L602`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L602) — Test extraction of elements with multiple classes.
  - `test_extract_nested_elements(self)` — [`L577`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L577) — Test extraction of nested elements.
  - `test_extract_parent_child_relationships(self)` — [`L588`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L588) — Test extraction of parent-child relationships.
- uses (calls/refs, reference-scoped): [`HtmlPlugin`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin.create_extractor), [`extract_html_elements`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_html_elements)  (2 test-only)

### `TestHtmlLinkImageRecognition`
- def: [`tests/unit/languages/test_html_plugin_advanced.py:323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L323)
- doc: Test HTML link and image recognition and extraction.
- signature: `class TestHtmlLinkImageRecognition:`
- members:
  - `test_extract_a_tag(self)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L326) — Test extraction of anchor tag.
  - `test_extract_anchor_link(self)` — [`L379`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L379) — Test extraction of anchor link.
  - `test_extract_external_link(self)` — [`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L337) — Test extraction of external link.
  - `test_extract_image_with_alt(self)` — [`L411`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L411) — Test extraction of image with alt text.
  - `test_extract_image_with_dimensions(self)` — [`L430`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L430) — Test extraction of image with dimensions.
  - `test_extract_img_tag(self)` — [`L400`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L400) — Test extraction of img tag.
  - `test_extract_internal_link(self)` — [`L358`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L358) — Test extraction of internal link.
  - `test_extract_picture_tag(self)` — [`L456`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L456) — Test extraction of picture tag.
  - `test_extract_svg_tag(self)` — [`L467`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L467) — Test extraction of svg tag.
- uses (calls/refs, reference-scoped): [`HtmlPlugin`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin.create_extractor), [`extract_html_elements`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_html_elements)  (2 test-only)

### `TestHtmlQueryAccuracy`
- def: [`tests/unit/languages/test_html_plugin_advanced.py:665`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L665)
- doc: Test accuracy of HTML queries.
- signature: `class TestHtmlQueryAccuracy:`
- members:
  - `test_attribute_query_accuracy(self)` — [`L713`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L713) — Test that attribute query accurately identifies attributes.
  - `test_element_classification_accuracy(self)` — [`L887`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L887) — Test that element classification is accurate.
  - `test_form_query_accuracy(self)` — [`L739`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L739) — Test that form query accurately identifies form elements.
  - `test_image_query_accuracy(self)` — [`L771`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L771) — Test that image query accurately identifies images.
  - `test_line_number_accuracy(self)` — [`L806`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L806) — Test that line numbers are accurate.
  - `test_link_query_accuracy(self)` — [`L759`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L759) — Test that link query accurately identifies links.
  - `test_no_false_negatives(self)` — [`L794`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L794) — Test that queries don't miss elements.
  - `test_no_false_positives(self)` — [`L783`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L783) — Test that queries don't produce false positives.
  - `test_table_query_accuracy(self)` — [`L749`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L749) — Test that table query accurately identifies table elements.
  - `test_tag_query_accuracy(self)` — [`L668`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L668) — Test that tag query accurately identifies tags.
- uses (calls/refs, reference-scoped): [`HtmlPlugin`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin.create_extractor), [`extract_html_elements`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_html_elements)  (6 test-only)

### `TestHtmlScriptStyleRecognition`
- def: [`tests/unit/languages/test_html_plugin_advanced.py:479`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L479)
- doc: Test HTML script and style recognition and extraction.
- signature: `class TestHtmlScriptStyleRecognition:`
- members:
  - `test_extract_link_tag(self)` — [`L504`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L504) — Test extraction of link tag.
  - `test_extract_meta_tag(self)` — [`L515`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L515) — Test extraction of meta tag.
  - `test_extract_script_tag(self)` — [`L482`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L482) — Test extraction of script tag.
  - `test_extract_script_with_src(self)` — [`L537`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L537) — Test extraction of script with src attribute.
  - `test_extract_style_tag(self)` — [`L493`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L493) — Test extraction of style tag.
  - `test_extract_style_with_href(self)` — [`L555`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L555) — Test extraction of link with href attribute.
  - `test_extract_title_tag(self)` — [`L526`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L526) — Test extraction of title tag.
- uses (calls/refs, reference-scoped): [`HtmlPlugin`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin.create_extractor), [`extract_html_elements`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_html_elements)  (2 test-only)

## Functions
- `get_tree_for_code(code: str, plugin: HtmlPlugin)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L308) — Helper to parse HTML code and return tree.

## Module values
- `ATTRIBUTE_CODE` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L44)
- `COMPLEX_STRUCTURE_CODE` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L261)
- `FORM_CODE` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L85)
- `LINK_IMAGE_CODE` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L191)
- `SCRIPT_STYLE_CODE` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L217)
- `TABLE_CODE` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L137)
- `TAG_CODE` — [`L5`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin_advanced.py#L5)

