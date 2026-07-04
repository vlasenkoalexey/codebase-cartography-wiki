---
title: 'Module: tests/unit/languages/test_yaml_element_metadata_properties.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_yaml_element_metadata_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_yaml_element_metadata_properties`/
symbols:
  TestYAMLElementMetadataProperties.test_property_4_element_metadata_raw_text_accuracy: TestYAMLElementMetadataProperties#test_property_4_element_metadata_raw_text_accuracy().
  TestYAMLElementMetadataProperties.test_property_4_element_metadata_sequence_accuracy: TestYAMLElementMetadataProperties#test_property_4_element_metadata_sequence_accuracy().
  TestYAMLElementMetadataProperties.test_property_4_element_metadata_with_comments: TestYAMLElementMetadataProperties#test_property_4_element_metadata_with_comments().
  TestYAMLElementMetadataProperties.test_property_4_element_metadata_mixed_structures: TestYAMLElementMetadataProperties#test_property_4_element_metadata_mixed_structures().
  TestYAMLElementMetadataProperties.test_property_4_element_metadata_line_numbers: TestYAMLElementMetadataProperties#test_property_4_element_metadata_line_numbers().
  TestYAMLElementMetadataProperties.test_property_4_element_metadata_consistency: TestYAMLElementMetadataProperties#test_property_4_element_metadata_consistency().
  yaml_with_comments: yaml_with_comments().
  _yaml_word: _yaml_word().
  yaml_simple_mapping: yaml_simple_mapping().
  _yaml_comment: _yaml_comment().
  yaml_simple_sequence: yaml_simple_sequence().
  pytestmark: pytestmark.
  _YAML_TEXT_CHARS: _YAML_TEXT_CHARS.
  _YAML_COMMENT_CHARS: _YAML_COMMENT_CHARS.
  _yaml_scalar_value: _yaml_scalar_value().
  TestYAMLElementMetadataProperties: TestYAMLElementMetadataProperties#
---
# Module: [`tests/unit/languages/test_yaml_element_metadata_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_metadata_properties.py)

## Classes
### `TestYAMLElementMetadataProperties`
- def: [`tests/unit/languages/test_yaml_element_metadata_properties.py:119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_metadata_properties.py#L119)
- doc: Property-based tests for YAML element metadata completeness.
- signature: `class TestYAMLElementMetadataProperties:`
- members:
  - `test_property_4_element_metadata_consistency(self, num_keys: int)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_metadata_properties.py#L235) — Feature: yaml-language-support, Property 4: Element Metadata Completeness
  - `test_property_4_element_metadata_line_numbers(self, yaml_content: str)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_metadata_properties.py#L124) — Feature: yaml-language-support, Property 4: Element Metadata Completeness
  - `test_property_4_element_metadata_mixed_structures(self, mapping_count: int, sequence_count: int)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_metadata_properties.py#L274) — Feature: yaml-language-support, Property 4: Element Metadata Completeness
  - `test_property_4_element_metadata_raw_text_accuracy(self, yaml_content: str)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_metadata_properties.py#L142) — Feature: yaml-language-support, Property 4: Element Metadata Completeness
  - `test_property_4_element_metadata_sequence_accuracy(self, yaml_content: str)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_metadata_properties.py#L162) — Feature: yaml-language-support, Property 4: Element Metadata Completeness
  - `test_property_4_element_metadata_with_comments(self, yaml_content: str)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_metadata_properties.py#L197) — Feature: yaml-language-support, Property 4: Element Metadata Completeness
- uses (calls/refs, reference-scoped): [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`element_type`](../../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`extract_yaml_elements`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLElementExtractor.extract_yaml_elements), [`YAMLElementExtractor`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLElementExtractor)  (15 test-only)

## Functions
- `_yaml_comment()` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_metadata_properties.py#L54)
- `_yaml_scalar_value()` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_metadata_properties.py#L58) — Generate YAML scalar values used in property strategies.
- `_yaml_word()` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_metadata_properties.py#L50)
- `yaml_simple_mapping(draw)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_metadata_properties.py#L69) — Generate simple YAML mapping content.
- `yaml_simple_sequence(draw)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_metadata_properties.py#L89) — Generate simple YAML sequence content.
- `yaml_with_comments(draw)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_metadata_properties.py#L102) — Generate YAML content with comments.

## Module values
- `_YAML_COMMENT_CHARS` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_metadata_properties.py#L43)
- `_YAML_TEXT_CHARS` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_metadata_properties.py#L40)
- `pytestmark` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_metadata_properties.py#L36)

