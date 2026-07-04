---
title: 'Module: tests/unit/languages/test_yaml_element_properties.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_yaml_element_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_yaml_element_properties`/
symbols:
  TestYAMLElementProperties.test_property_9_output_schema_consistency_attributes: TestYAMLElementProperties#test_property_9_output_schema_consistency_attributes().
  TestYAMLElementProperties.test_property_9_output_schema_consistency_json_serialization: TestYAMLElementProperties#test_property_9_output_schema_consistency_json_serialization().
  TestYAMLElementProperties.test_property_9_output_schema_consistency_defaults: TestYAMLElementProperties#test_property_9_output_schema_consistency_defaults().
  TestYAMLElementProperties.test_property_9_output_schema_consistency_type_values: TestYAMLElementProperties#test_property_9_output_schema_consistency_type_values().
  yaml_element_types: yaml_element_types.
  yaml_value_types: yaml_value_types.
  yaml_keys: yaml_keys.
  line_numbers: line_numbers.
  nesting_levels: nesting_levels.
  document_indices: document_indices.
  anchor_names: anchor_names.
  yaml_scalar_values: yaml_scalar_values.
  child_counts: child_counts.
  _assert_base_element_attrs: _assert_base_element_attrs().
  _assert_yaml_specific_attrs: _assert_yaml_specific_attrs().
  _assert_summary_required_fields: _assert_summary_required_fields().
  _assert_json_roundtrip: _assert_json_roundtrip().
  TestYAMLElementProperties: TestYAMLElementProperties#
---
# Module: [`tests/unit/languages/test_yaml_element_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_properties.py)

## Classes
### `TestYAMLElementProperties`
- def: [`tests/unit/languages/test_yaml_element_properties.py:125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_properties.py#L125)
- doc: Property-based tests for YAMLElement data model.
- signature: `class TestYAMLElementProperties:`
- members:
  - `test_property_9_output_schema_consistency_attributes(self, name: str, start_line: int, end_line_offset: int, raw_text: str, element_type: str, key: str | None, value: str | None, value_type: str | None, anchor_name: str | None, alias_target: str | None, nesting_level: int, document_index: int, child_count: int | None)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_properties.py#L144) — Feature: yaml-language-support, Property 9: Output Schema Consistency
  - `test_property_9_output_schema_consistency_defaults(self, start_line: int, end_line_offset: int)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_properties.py#L334) — Feature: yaml-language-support, Property 9: Output Schema Consistency
  - `test_property_9_output_schema_consistency_json_serialization(self, name: str, start_line: int, end_line_offset: int, raw_text: str, element_type: str, key: str | None, value: str | None, value_type: str | None, nesting_level: int, document_index: int)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_properties.py#L276) — Feature: yaml-language-support, Property 9: Output Schema Consistency
  - `test_property_9_output_schema_consistency_type_values(self, element_type: str, value_type: str | None)` — [`L382`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_properties.py#L382) — Feature: yaml-language-support, Property 9: Output Schema Consistency
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`to_summary_item`](../../../tree_sitter_analyzer/models/markup_models.md#YAMLElement.to_summary_item), [`YAMLElement`](../../../tree_sitter_analyzer/models/markup_models.md#YAMLElement), [`element_type`](../../../tree_sitter_analyzer/models/markup_models.md#YAMLElement.element_type), [`value_type`](../../../tree_sitter_analyzer/models/markup_models.md#YAMLElement.value_type), [`document_index`](../../../tree_sitter_analyzer/models/markup_models.md#YAMLElement.document_index), [`key`](../../../tree_sitter_analyzer/models/markup_models.md#YAMLElement.key), [`nesting_level`](../../../tree_sitter_analyzer/models/markup_models.md#YAMLElement.nesting_level), [`value`](../../../tree_sitter_analyzer/models/markup_models.md#YAMLElement.value), [`alias_target`](../../../tree_sitter_analyzer/models/markup_models.md#YAMLElement.alias_target), [`anchor_name`](../../../tree_sitter_analyzer/models/markup_models.md#YAMLElement.anchor_name), [`child_count`](../../../tree_sitter_analyzer/models/markup_models.md#YAMLElement.child_count), [`language`](../../../tree_sitter_analyzer/models/markup_models.md#YAMLElement.language)  (13 test-only)

## Functions
- `_assert_base_element_attrs(element)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_properties.py#L73) — Assert that base CodeElement attributes are present.
- `_assert_json_roundtrip(summary: dict)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_properties.py#L111) — Assert that summary is JSON-serializable and round-trips correctly.
- `_assert_summary_required_fields(summary: dict)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_properties.py#L101) — Assert that a to_summary_item() result has required fields.
- `_assert_yaml_specific_attrs(element)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_properties.py#L86) — Assert that YAML-specific attributes are present.

## Module values
- `anchor_names` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_properties.py#L59)
- `child_counts` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_properties.py#L56)
- `document_indices` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_properties.py#L53)
- `line_numbers` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_properties.py#L47)
- `nesting_levels` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_properties.py#L50)
- `yaml_element_types` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_properties.py#L20)
- `yaml_keys` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_properties.py#L29)
- `yaml_scalar_values` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_properties.py#L40)
- `yaml_value_types` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_element_properties.py#L24)

