---
title: 'Module: tests/unit/languages/test_css_plugin_enhanced_selectors.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_css_plugin_enhanced_selectors.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_css_plugin_enhanced_selectors`/
symbols:
  get_tree_for_code: get_tree_for_code().
  PROPERTY_CODE: PROPERTY_CODE.
  SELECTOR_CODE: SELECTOR_CODE.
  TestCssSelectorRecognition.test_extract_simple_class_selector: TestCssSelectorRecognition#test_extract_simple_class_selector().
  TestCssSelectorRecognition.test_extract_id_selector: TestCssSelectorRecognition#test_extract_id_selector().
  TestCssSelectorRecognition.test_extract_element_selector: TestCssSelectorRecognition#test_extract_element_selector().
  TestCssSelectorRecognition.test_extract_attribute_selector: TestCssSelectorRecognition#test_extract_attribute_selector().
  TestCssSelectorRecognition.test_extract_pseudo_class_selector: TestCssSelectorRecognition#test_extract_pseudo_class_selector().
  TestCssSelectorRecognition.test_extract_pseudo_element_selector: TestCssSelectorRecognition#test_extract_pseudo_element_selector().
  TestCssSelectorRecognition.test_extract_combinator_selector: TestCssSelectorRecognition#test_extract_combinator_selector().
  TestCssSelectorRecognition.test_selector_complexity: TestCssSelectorRecognition#test_selector_complexity().
  TestCssPropertyRecognition.test_extract_layout_properties: TestCssPropertyRecognition#test_extract_layout_properties().
  TestCssPropertyRecognition.test_extract_typography_properties: TestCssPropertyRecognition#test_extract_typography_properties().
  TestCssPropertyRecognition.test_extract_box_model_properties: TestCssPropertyRecognition#test_extract_box_model_properties().
  TestCssPropertyRecognition.test_extract_background_properties: TestCssPropertyRecognition#test_extract_background_properties().
  TestCssPropertyRecognition.test_extract_flexbox_properties: TestCssPropertyRecognition#test_extract_flexbox_properties().
  TestCssPropertyRecognition.test_extract_grid_properties: TestCssPropertyRecognition#test_extract_grid_properties().
  TestCssPropertyRecognition.test_property_values: TestCssPropertyRecognition#test_property_values().
  TestCssRuleRecognition.test_extract_simple_rule: TestCssRuleRecognition#test_extract_simple_rule().
  TestCssRuleRecognition.test_extract_multiple_rules: TestCssRuleRecognition#test_extract_multiple_rules().
  TestCssRuleRecognition.test_rule_selector: TestCssRuleRecognition#test_rule_selector().
  TestCssRuleRecognition.test_rule_properties: TestCssRuleRecognition#test_rule_properties().
  TestCssRuleRecognition.test_rule_line_numbers: TestCssRuleRecognition#test_rule_line_numbers().
  TestCssMediaQueryRecognition.test_extract_simple_media_query: TestCssMediaQueryRecognition#test_extract_simple_media_query().
  TestCssMediaQueryRecognition.test_extract_max_width_media_query: TestCssMediaQueryRecognition#test_extract_max_width_media_query().
  TestCssMediaQueryRecognition.test_extract_min_width_media_query: TestCssMediaQueryRecognition#test_extract_min_width_media_query().
  TestCssMediaQueryRecognition.test_extract_combined_media_query: TestCssMediaQueryRecognition#test_extract_combined_media_query().
  TestCssMediaQueryRecognition.test_extract_print_media_query: TestCssMediaQueryRecognition#test_extract_print_media_query().
  TestCssMediaQueryRecognition.test_extract_prefers_color_scheme_media_query: TestCssMediaQueryRecognition#test_extract_prefers_color_scheme_media_query().
  MEDIA_QUERY_CODE: MEDIA_QUERY_CODE.
  COMPLEX_STRUCTURE_CODE: COMPLEX_STRUCTURE_CODE.
  TestCssSelectorRecognition: TestCssSelectorRecognition#
  TestCssPropertyRecognition: TestCssPropertyRecognition#
  TestCssRuleRecognition: TestCssRuleRecognition#
  TestCssMediaQueryRecognition: TestCssMediaQueryRecognition#
---
# Module: [`tests/unit/languages/test_css_plugin_enhanced_selectors.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py)

## Classes
### `TestCssMediaQueryRecognition`
- def: [`tests/unit/languages/test_css_plugin_enhanced_selectors.py:509`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L509)
- doc: Test CSS media query recognition and extraction.
- signature: `class TestCssMediaQueryRecognition:`
- members:
  - `test_extract_combined_media_query(self)` — [`L539`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L539) — Test extraction of combined media query.
  - `test_extract_max_width_media_query(self)` — [`L521`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L521) — Test extraction of max-width media query.
  - `test_extract_min_width_media_query(self)` — [`L530`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L530) — Test extraction of min-width media query.
  - `test_extract_prefers_color_scheme_media_query(self)` — [`L557`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L557) — Test extraction of prefers-color-scheme media query.
  - `test_extract_print_media_query(self)` — [`L548`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L548) — Test extraction of print media query.
  - `test_extract_simple_media_query(self)` — [`L512`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L512) — Test extraction of simple media query.
- uses (calls/refs, reference-scoped): [`CssPlugin`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin), [`extract_css_rules`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_css_rules), [`create_extractor`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin.create_extractor)  (2 test-only)

### `TestCssPropertyRecognition`
- def: [`tests/unit/languages/test_css_plugin_enhanced_selectors.py:374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L374)
- doc: Test CSS property recognition and extraction.
- signature: `class TestCssPropertyRecognition:`
- members:
  - `test_extract_background_properties(self)` — [`L411`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L411) — Test extraction of background properties.
  - `test_extract_box_model_properties(self)` — [`L399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L399) — Test extraction of box model properties.
  - `test_extract_flexbox_properties(self)` — [`L421`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L421) — Test extraction of flexbox properties.
  - `test_extract_grid_properties(self)` — [`L431`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L431) — Test extraction of grid properties.
  - `test_extract_layout_properties(self)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L377) — Test extraction of layout properties.
  - `test_extract_typography_properties(self)` — [`L387`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L387) — Test extraction of typography properties.
  - `test_property_values(self)` — [`L441`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L441) — Test that property values are extracted.
- uses (calls/refs, reference-scoped): [`CssPlugin`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin), [`extract_css_rules`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_css_rules), [`create_extractor`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin.create_extractor)  (2 test-only)

### `TestCssRuleRecognition`
- def: [`tests/unit/languages/test_css_plugin_enhanced_selectors.py:454`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L454)
- doc: Test CSS rule recognition and extraction.
- signature: `class TestCssRuleRecognition:`
- members:
  - `test_extract_multiple_rules(self)` — [`L465`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L465) — Test extraction of multiple CSS rules.
  - `test_extract_simple_rule(self)` — [`L457`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L457) — Test extraction of simple CSS rule.
  - `test_rule_line_numbers(self)` — [`L498`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L498) — Test that rule line numbers are accurate.
  - `test_rule_properties(self)` — [`L483`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L483) — Test that rule properties are captured.
  - `test_rule_selector(self)` — [`L473`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L473) — Test that rule selector is captured.
- uses (calls/refs, reference-scoped): [`CssPlugin`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin), [`extract_css_rules`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_css_rules), [`create_extractor`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin.create_extractor)  (3 test-only)

### `TestCssSelectorRecognition`
- def: [`tests/unit/languages/test_css_plugin_enhanced_selectors.py:269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L269)
- doc: Test CSS selector recognition and extraction.
- signature: `class TestCssSelectorRecognition:`
- members:
  - `test_extract_attribute_selector(self)` — [`L302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L302) — Test extraction of attribute selector.
  - `test_extract_combinator_selector(self)` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L344) — Test extraction of combinator selector.
  - `test_extract_element_selector(self)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L292) — Test extraction of element selector.
  - `test_extract_id_selector(self)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L282) — Test extraction of ID selector.
  - `test_extract_pseudo_class_selector(self)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L320) — Test extraction of pseudo-class selector.
  - `test_extract_pseudo_element_selector(self)` — [`L332`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L332) — Test extraction of pseudo-element selector.
  - `test_extract_simple_class_selector(self)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L272) — Test extraction of simple class selector.
  - `test_selector_complexity(self)` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L361) — Test that complex selectors are handled.
- uses (calls/refs, reference-scoped): [`CssPlugin`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin), [`extract_css_rules`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_css_rules), [`create_extractor`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin.create_extractor)  (3 test-only)

## Functions
- `get_tree_for_code(code: str, plugin: CssPlugin)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L254) — Helper to parse CSS code and return tree.

## Module values
- `COMPLEX_STRUCTURE_CODE` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L161)
- `MEDIA_QUERY_CODE` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L124)
- `PROPERTY_CODE` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L65)
- `SELECTOR_CODE` — [`L5`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_selectors.py#L5)

