---
title: 'Module: tests/unit/languages/test_css_plugin_enhanced_features.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_css_plugin_enhanced_features.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_css_plugin_enhanced_features`/
symbols:
  get_tree_for_code: get_tree_for_code().
  ANIMATION_CODE: ANIMATION_CODE.
  TestCssAnimationRecognition.test_extract_keyframes: TestCssAnimationRecognition#test_extract_keyframes().
  TestCssAnimationRecognition.test_extract_multiple_keyframes: TestCssAnimationRecognition#test_extract_multiple_keyframes().
  TestCssAnimationRecognition.test_extract_keyframes_name: TestCssAnimationRecognition#test_extract_keyframes_name().
  TestCssAnimationRecognition.test_extract_animation_properties: TestCssAnimationRecognition#test_extract_animation_properties().
  TestCssAnimationRecognition.test_extract_transition_properties: TestCssAnimationRecognition#test_extract_transition_properties().
  TestCssAnimationRecognition.test_keyframes_keyframes: TestCssAnimationRecognition#test_keyframes_keyframes().
  TestCssVariableRecognition.test_extract_root_variables: TestCssVariableRecognition#test_extract_root_variables().
  TestCssVariableRecognition.test_extract_variable_usage: TestCssVariableRecognition#test_extract_variable_usage().
  TestCssVariableRecognition.test_extract_variable_fallback: TestCssVariableRecognition#test_extract_variable_fallback().
  TestCssVariableRecognition.test_extract_local_variables: TestCssVariableRecognition#test_extract_local_variables().
  TestCssVariableRecognition.test_variable_naming: TestCssVariableRecognition#test_variable_naming().
  TestCssComplexStructures.test_extract_import_rules: TestCssComplexStructures#test_extract_import_rules().
  TestCssComplexStructures.test_extract_layer_rules: TestCssComplexStructures#test_extract_layer_rules().
  TestCssComplexStructures.test_extract_grid_template_areas: TestCssComplexStructures#test_extract_grid_template_areas().
  TestCssComplexStructures.test_extract_multiple_backgrounds: TestCssComplexStructures#test_extract_multiple_backgrounds().
  TestCssComplexStructures.test_extract_complex_box_shadow: TestCssComplexStructures#test_extract_complex_box_shadow().
  TestCssComplexStructures.test_extract_not_selector: TestCssComplexStructures#test_extract_not_selector().
  TestCssQueryAccuracy.test_selector_query_accuracy: TestCssQueryAccuracy#test_selector_query_accuracy().
  TestCssQueryAccuracy.test_property_query_accuracy: TestCssQueryAccuracy#test_property_query_accuracy().
  TestCssQueryAccuracy.test_media_query_accuracy: TestCssQueryAccuracy#test_media_query_accuracy().
  TestCssQueryAccuracy.test_keyframes_query_accuracy: TestCssQueryAccuracy#test_keyframes_query_accuracy().
  TestCssQueryAccuracy.test_variable_query_accuracy: TestCssQueryAccuracy#test_variable_query_accuracy().
  TestCssQueryAccuracy.test_no_false_positives: TestCssQueryAccuracy#test_no_false_positives().
  TestCssQueryAccuracy.test_no_false_negatives: TestCssQueryAccuracy#test_no_false_negatives().
  TestCssQueryAccuracy.test_line_number_accuracy: TestCssQueryAccuracy#test_line_number_accuracy().
  TestCssQueryAccuracy.test_element_classification_accuracy: TestCssQueryAccuracy#test_element_classification_accuracy().
  VARIABLE_CODE: VARIABLE_CODE.
  COMPLEX_STRUCTURE_CODE: COMPLEX_STRUCTURE_CODE.
  PROPERTY_CODE: PROPERTY_CODE.
  SELECTOR_CODE: SELECTOR_CODE.
  MEDIA_QUERY_CODE: MEDIA_QUERY_CODE.
  TestCssAnimationRecognition: TestCssAnimationRecognition#
  TestCssVariableRecognition: TestCssVariableRecognition#
  TestCssComplexStructures: TestCssComplexStructures#
  TestCssQueryAccuracy: TestCssQueryAccuracy#
---
# Module: [`tests/unit/languages/test_css_plugin_enhanced_features.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py)

## Classes
### `TestCssAnimationRecognition`
- def: [`tests/unit/languages/test_css_plugin_enhanced_features.py:364`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L364)
- doc: Test CSS animation recognition and extraction.
- signature: `class TestCssAnimationRecognition:`
- members:
  - `test_extract_animation_properties(self)` — [`L396`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L396) — Test extraction of animation properties.
  - `test_extract_keyframes(self)` — [`L367`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L367) — Test extraction of @keyframes.
  - `test_extract_keyframes_name(self)` — [`L385`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L385) — Test that keyframes name is captured.
  - `test_extract_multiple_keyframes(self)` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L376) — Test extraction of multiple @keyframes.
  - `test_extract_transition_properties(self)` — [`L408`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L408) — Test extraction of transition properties.
  - `test_keyframes_keyframes(self)` — [`L419`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L419) — Test that keyframes percentages are captured.
- uses (calls/refs, reference-scoped): [`CssPlugin`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin), [`extract_css_rules`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_css_rules), [`create_extractor`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin.create_extractor)  (2 test-only)

### `TestCssComplexStructures`
- def: [`tests/unit/languages/test_css_plugin_enhanced_features.py:494`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L494)
- doc: Test extraction of complex CSS structures.
- signature: `class TestCssComplexStructures:`
- members:
  - `test_extract_complex_box_shadow(self)` — [`L547`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L547) — Test extraction of complex box-shadow.
  - `test_extract_grid_template_areas(self)` — [`L519`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L519) — Test extraction of grid-template-areas.
  - `test_extract_import_rules(self)` — [`L497`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L497) — Test extraction of @import rules.
  - `test_extract_layer_rules(self)` — [`L508`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L508) — Test extraction of @layer rules.
  - `test_extract_multiple_backgrounds(self)` — [`L533`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L533) — Test extraction of multiple backgrounds.
  - `test_extract_not_selector(self)` — [`L559`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L559) — Test extraction of :not() selector.
- uses (calls/refs, reference-scoped): [`CssPlugin`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin), [`extract_css_rules`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_css_rules), [`create_extractor`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin.create_extractor)  (2 test-only)

### `TestCssQueryAccuracy`
- def: [`tests/unit/languages/test_css_plugin_enhanced_features.py:571`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L571)
- doc: Test accuracy of CSS queries.
- signature: `class TestCssQueryAccuracy:`
- members:
  - `test_element_classification_accuracy(self)` — [`L671`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L671) — Test that element classification is accurate.
  - `test_keyframes_query_accuracy(self)` — [`L617`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L617) — Test that keyframes query accurately identifies animations.
  - `test_line_number_accuracy(self)` — [`L656`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L656) — Test that line numbers are accurate.
  - `test_media_query_accuracy(self)` — [`L608`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L608) — Test that media query is accurately captured.
  - `test_no_false_negatives(self)` — [`L645`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L645) — Test that queries don't miss elements.
  - `test_no_false_positives(self)` — [`L635`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L635) — Test that queries don't produce false positives.
  - `test_property_query_accuracy(self)` — [`L596`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L596) — Test that property query accurately identifies properties.
  - `test_selector_query_accuracy(self)` — [`L574`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L574) — Test that selector query accurately identifies selectors.
  - `test_variable_query_accuracy(self)` — [`L626`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L626) — Test that variable query accurately identifies variables.
- uses (calls/refs, reference-scoped): [`CssPlugin`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin), [`extract_css_rules`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_css_rules), [`create_extractor`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin.create_extractor)  (6 test-only)

### `TestCssVariableRecognition`
- def: [`tests/unit/languages/test_css_plugin_enhanced_features.py:431`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L431)
- doc: Test CSS variable recognition and extraction.
- signature: `class TestCssVariableRecognition:`
- members:
  - `test_extract_local_variables(self)` — [`L470`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L470) — Test extraction of local variables.
  - `test_extract_root_variables(self)` — [`L434`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L434) — Test extraction of :root variables.
  - `test_extract_variable_fallback(self)` — [`L457`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L457) — Test extraction of variable fallback.
  - `test_extract_variable_usage(self)` — [`L445`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L445) — Test extraction of variable usage with var().
  - `test_variable_naming(self)` — [`L481`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L481) — Test that variable names are captured.
- uses (calls/refs, reference-scoped): [`CssPlugin`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin), [`extract_css_rules`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_css_rules), [`create_extractor`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin.create_extractor)  (2 test-only)

## Functions
- `get_tree_for_code(code: str, plugin: CssPlugin)` — [`L349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L349) — Helper to parse CSS code and return tree.

## Module values
- `ANIMATION_CODE` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L161)
- `COMPLEX_STRUCTURE_CODE` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L256)
- `MEDIA_QUERY_CODE` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L124)
- `PROPERTY_CODE` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L65)
- `SELECTOR_CODE` — [`L5`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L5)
- `VARIABLE_CODE` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin_enhanced_features.py#L215)

