---
title: 'Module: tests/unit/languages/test_json_plugin.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_json_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_json_plugin`/
symbols:
  TestJSONExtraction.test_extracts_pairs_with_key_names: TestJSONExtraction#test_extracts_pairs_with_key_names().
  TestJSONExtraction.test_nested_object_is_extracted: TestJSONExtraction#test_nested_object_is_extracted().
  _parse: _parse().
  TestJSONExtraction.test_extracts_value_types: TestJSONExtraction#test_extracts_value_types().
  TestJSONExtraction.test_array_is_extracted: TestJSONExtraction#test_array_is_extracted().
  TestJSONExtraction.test_empty_object_does_not_crash: TestJSONExtraction#test_empty_object_does_not_crash().
  TestJSONExtraction.test_extract_elements_returns_json_elements_bucket: TestJSONExtraction#test_extract_elements_returns_json_elements_bucket().
  TestJSONExtraction.test_extract_with_none_tree_returns_empty: TestJSONExtraction#test_extract_with_none_tree_returns_empty().
  TestJSONPluginMetadata.test_language_name: TestJSONPluginMetadata#test_language_name().
  TestJSONPluginMetadata.test_file_extensions: TestJSONPluginMetadata#test_file_extensions().
  TestJSONPluginMetadata.test_is_applicable: TestJSONPluginMetadata#test_is_applicable().
  TestJSONPluginMetadata.test_create_extractor_is_fresh_instance: TestJSONPluginMetadata#test_create_extractor_is_fresh_instance().
  TestJSONExtraction: TestJSONExtraction#
  TestJSONPluginMetadata: TestJSONPluginMetadata#
---
# Module: [`tests/unit/languages/test_json_plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_json_plugin.py)

## Classes
### `TestJSONExtraction`
- def: [`tests/unit/languages/test_json_plugin.py:21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_json_plugin.py#L21)
- signature: `class TestJSONExtraction:`
- members:
  - `test_array_is_extracted(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_json_plugin.py#L56)
  - `test_empty_object_does_not_crash(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_json_plugin.py#L63)
  - `test_extract_elements_returns_json_elements_bucket(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_json_plugin.py#L22)
  - `test_extract_with_none_tree_returns_empty(self)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_json_plugin.py#L70)
  - `test_extracts_pairs_with_key_names(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_json_plugin.py#L29)
  - `test_extracts_value_types(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_json_plugin.py#L36)
  - `test_nested_object_is_extracted(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_json_plugin.py#L47)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`element_type`](../../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`extract_json_elements`](../../../tree_sitter_analyzer/languages/json_plugin.md#JSONElementExtractor.extract_json_elements), [`JSONPlugin`](../../../tree_sitter_analyzer/languages/json_plugin.md#JSONPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/json_plugin.md#JSONPlugin.create_extractor), [`extract_elements`](../../../tree_sitter_analyzer/languages/json_plugin.md#JSONElementExtractor.extract_elements)  (1 test-only)

### `TestJSONPluginMetadata`
- def: [`tests/unit/languages/test_json_plugin.py:76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_json_plugin.py#L76)
- signature: `class TestJSONPluginMetadata:`
- members:
  - `test_create_extractor_is_fresh_instance(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_json_plugin.py#L88)
  - `test_file_extensions(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_json_plugin.py#L80)
  - `test_is_applicable(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_json_plugin.py#L83)
  - `test_language_name(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_json_plugin.py#L77)
- uses (calls/refs, reference-scoped): [`is_applicable`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.is_applicable), [`JSONPlugin`](../../../tree_sitter_analyzer/languages/json_plugin.md#JSONPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/json_plugin.md#JSONPlugin.create_extractor), [`get_file_extensions`](../../../tree_sitter_analyzer/languages/json_plugin.md#JSONPlugin.get_file_extensions), [`get_language_name`](../../../tree_sitter_analyzer/languages/json_plugin.md#JSONPlugin.get_language_name)

## Functions
- `_parse(code: str)` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_json_plugin.py#L15)

