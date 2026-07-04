---
title: 'Module: tests/unit/languages/test_yaml_output_format_properties.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_yaml_output_format_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_yaml_output_format_properties`/
symbols:
  TestYAMLOutputFormatProperties.test_property_10_json_format_produces_valid_json: TestYAMLOutputFormatProperties#test_property_10_json_format_produces_valid_json().
  TestYAMLOutputFormatProperties.test_property_10_output_format_consistency: TestYAMLOutputFormatProperties#test_property_10_output_format_consistency().
  TestYAMLOutputFormatProperties.test_property_10_text_format_produces_valid_text: TestYAMLOutputFormatProperties#test_property_10_text_format_produces_valid_text().
  TestYAMLOutputFormatProperties.test_property_10_empty_result_handling: TestYAMLOutputFormatProperties#test_property_10_empty_result_handling().
  _assert_format_succeeds: _assert_format_succeeds().
  TestYAMLOutputFormatProperties.test_property_10_csv_format_produces_valid_csv: TestYAMLOutputFormatProperties#test_property_10_csv_format_produces_valid_csv().
  _build_basic_yaml_elements: _build_basic_yaml_elements().
  _build_mapping_yaml_elements: _build_mapping_yaml_elements().
  _make_yaml_analysis_result: _make_yaml_analysis_result().
  _parse_json_from_output: _parse_json_from_output().
  create_yaml_element_dict: create_yaml_element_dict().
  yaml_element_types: yaml_element_types.
  yaml_value_types: yaml_value_types.
  yaml_keys: yaml_keys.
  yaml_values: yaml_values.
  line_numbers: line_numbers.
  nesting_levels: nesting_levels.
  document_indices: document_indices.
  child_counts: child_counts.
  TestYAMLOutputFormatProperties: TestYAMLOutputFormatProperties#
---
# Module: [`tests/unit/languages/test_yaml_output_format_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py)

## Classes
### `TestYAMLOutputFormatProperties`
- def: [`tests/unit/languages/test_yaml_output_format_properties.py:157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L157)
- doc: Property-based tests for YAML output format support.
- signature: `class TestYAMLOutputFormatProperties:`
- members:
  - `test_property_10_csv_format_produces_valid_csv(self, file_path: str, mapping_count: int)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L264) — Feature: yaml-language-support, Property 10: Output Format Support
  - `test_property_10_empty_result_handling(self, file_path: str)` — [`L403`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L403) — Feature: yaml-language-support, Property 10: Output Format Support
  - `test_property_10_json_format_produces_valid_json(self, file_path: str, line_count: int, element_count: int)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L168) — Feature: yaml-language-support, Property 10: Output Format Support
  - `test_property_10_output_format_consistency(self, element_count: int)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L320) — Feature: yaml-language-support, Property 10: Output Format Support
  - `test_property_10_text_format_produces_valid_text(self, file_path: str, line_count: int, element_count: int)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L215) — Feature: yaml-language-support, Property 10: Output Format Support
- uses (calls/refs, reference-scoped): [`YAMLFormatter`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter), [`format_table`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter.format_table), [`format_advanced`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter.format_advanced), [`format_summary`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter.format_summary), [`format_structure`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter.format_structure)  (6 test-only)

## Functions
- `_assert_format_succeeds(result: str, context: str)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L120) — Assert that a formatter result is a non-empty string.
- `_build_basic_yaml_elements(element_count: int)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L51) — Build element_count basic YAML elements cycling through 4 types.
- `_build_mapping_yaml_elements(mapping_count: int)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L73) — Build mapping_count YAML mapping elements.
- `_make_yaml_analysis_result(file_path: str, line_count: int, elements: list)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L91) — Build a standard analysis_result dict for YAML formatter tests.
- `_parse_json_from_output(output: str, context: str)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L106) — Extract the first JSON object from formatter output and parse it.
- `create_yaml_element_dict(name: str, start_line: int, end_line: int, element_type: str, key: str | None = None, value: str | None = None, value_type: str | None = None, anchor_name: str | None = None, alias_target: str | None = None, nesting_level: int = 0, document_index: int = 0, child_count: int | None = None)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L126) — Create a dictionary representation of a YAML element.

## Module values
- `child_counts` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L48)
- `document_indices` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L47)
- `line_numbers` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L45)
- `nesting_levels` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L46)
- `yaml_element_types` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L21)
- `yaml_keys` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L29)
- `yaml_value_types` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L25)
- `yaml_values` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_output_format_properties.py#L39)

