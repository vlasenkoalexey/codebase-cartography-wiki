---
title: 'Module: tests/unit/languages/test_yaml_plugin_structure.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_yaml_plugin_structure.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_yaml_plugin_structure`/
symbols:
  TestYAMLAnchorAliasRecognition.test_extract_anchor_alias_shapes: TestYAMLAnchorAliasRecognition#test_extract_anchor_alias_shapes().
  TestYAMLKeyPairRecognition.test_extract_key_value_shapes: TestYAMLKeyPairRecognition#test_extract_key_value_shapes().
  TestYAMLListRecognition.test_extract_list_shapes: TestYAMLListRecognition#test_extract_list_shapes().
  TestYAMLNestedStructureRecognition.test_extract_nested_structure_shapes: TestYAMLNestedStructureRecognition#test_extract_nested_structure_shapes().
  get_tree_for_code: get_tree_for_code().
  TestYAMLKeyPairRecognition: TestYAMLKeyPairRecognition#
  TestYAMLListRecognition: TestYAMLListRecognition#
  TestYAMLNestedStructureRecognition: TestYAMLNestedStructureRecognition#
  TestYAMLAnchorAliasRecognition: TestYAMLAnchorAliasRecognition#
  KEY_VALUE_CODE: KEY_VALUE_CODE.
  LIST_CODE: LIST_CODE.
  NESTED_STRUCTURE_CODE: NESTED_STRUCTURE_CODE.
  ANCHOR_ALIAS_CODE: ANCHOR_ALIAS_CODE.
---
# Module: [`tests/unit/languages/test_yaml_plugin_structure.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_structure.py)

## Classes
### `TestYAMLAnchorAliasRecognition`
- def: [`tests/unit/languages/test_yaml_plugin_structure.py:247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_structure.py#L247)
- doc: Test YAML anchor and alias recognition and extraction.
- signature: `class TestYAMLAnchorAliasRecognition:`
- members:
  - `test_extract_anchor_alias_shapes(self)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_structure.py#L250) — Test anchors, aliases, merge keys, and list anchors in one parse.
- uses (calls/refs, reference-scoped): [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`element_type`](../../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`YAMLPlugin`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin), [`extract_yaml_elements`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLElementExtractor.extract_yaml_elements), [`YAML_AVAILABLE`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAML_AVAILABLE), [`extractor`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin.extractor), [`key`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.key), [`alias_target`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.alias_target), [`anchor_name`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.anchor_name)  (2 test-only)

### `TestYAMLKeyPairRecognition`
- def: [`tests/unit/languages/test_yaml_plugin_structure.py:156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_structure.py#L156)
- doc: Test YAML key-value pair recognition and extraction.
- signature: `class TestYAMLKeyPairRecognition:`
- members:
  - `test_extract_key_value_shapes(self)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_structure.py#L159) — Test representative key-value scalar shapes in one parse.
- uses (calls/refs, reference-scoped): [`element_type`](../../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`YAMLPlugin`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin), [`extract_yaml_elements`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLElementExtractor.extract_yaml_elements), [`YAML_AVAILABLE`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAML_AVAILABLE), [`extractor`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin.extractor), [`key`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.key), [`value_type`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.value_type), [`value`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.value)  (2 test-only)

### `TestYAMLListRecognition`
- def: [`tests/unit/languages/test_yaml_plugin_structure.py:205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_structure.py#L205)
- doc: Test YAML list recognition and extraction.
- signature: `class TestYAMLListRecognition:`
- members:
  - `test_extract_list_shapes(self)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_structure.py#L208) — Test representative list shapes in one parse.
- uses (calls/refs, reference-scoped): [`element_type`](../../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`YAMLPlugin`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin), [`extract_yaml_elements`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLElementExtractor.extract_yaml_elements), [`YAML_AVAILABLE`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAML_AVAILABLE), [`extractor`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin.extractor), [`key`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.key), [`value_type`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.value_type)  (2 test-only)

### `TestYAMLNestedStructureRecognition`
- def: [`tests/unit/languages/test_yaml_plugin_structure.py:225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_structure.py#L225)
- doc: Test YAML nested structure recognition and extraction.
- signature: `class TestYAMLNestedStructureRecognition:`
- members:
  - `test_extract_nested_structure_shapes(self)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_structure.py#L228) — Test nested mapping structure and nesting levels in one parse.
- uses (calls/refs, reference-scoped): [`element_type`](../../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`YAMLPlugin`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin), [`extract_yaml_elements`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLElementExtractor.extract_yaml_elements), [`YAML_AVAILABLE`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAML_AVAILABLE), [`extractor`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin.extractor), [`key`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.key), [`nesting_level`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.nesting_level)  (2 test-only)

## Functions
- `get_tree_for_code(code: str, plugin: YAMLPlugin)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_structure.py#L140) — Helper to parse YAML code and return tree.

## Module values
- `ANCHOR_ALIAS_CODE` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_structure.py#L99)
- `KEY_VALUE_CODE` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_structure.py#L10)
- `LIST_CODE` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_structure.py#L34)
- `NESTED_STRUCTURE_CODE` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_structure.py#L68)

