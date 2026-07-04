---
title: 'Module: tests/unit/languages/test_yaml_scalar_type_properties.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_yaml_scalar_type_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_yaml_scalar_type_properties`/
symbols:
  _extract_yaml_elements: _extract_yaml_elements().
  pytestmark: pytestmark.
  TestYAMLScalarTypeProperties.test_property_5_string_scalar_identification: TestYAMLScalarTypeProperties#test_property_5_string_scalar_identification().
  TestYAMLScalarTypeProperties.test_property_5_number_scalar_identification: TestYAMLScalarTypeProperties#test_property_5_number_scalar_identification().
  TestYAMLScalarTypeProperties.test_property_5_boolean_scalar_identification: TestYAMLScalarTypeProperties#test_property_5_boolean_scalar_identification().
  TestYAMLScalarTypeProperties.test_property_5_null_scalar_identification: TestYAMLScalarTypeProperties#test_property_5_null_scalar_identification().
  TestYAMLScalarTypeProperties: TestYAMLScalarTypeProperties#
---
# Module: [`tests/unit/languages/test_yaml_scalar_type_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_scalar_type_properties.py)

## Classes
### `TestYAMLScalarTypeProperties`
- def: [`tests/unit/languages/test_yaml_scalar_type_properties.py:44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_scalar_type_properties.py#L44)
- doc: Property-based tests for YAML scalar type identification.
- signature: `class TestYAMLScalarTypeProperties:`
- members:
  - `test_property_5_boolean_scalar_identification(self, key_name: str, bool_value: str)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_scalar_type_properties.py#L195) — Feature: yaml-language-support, Property 5: Scalar Type Identification
  - `test_property_5_null_scalar_identification(self, key_name: str, null_value: str)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_scalar_type_properties.py#L247) — Feature: yaml-language-support, Property 5: Scalar Type Identification
  - `test_property_5_number_scalar_identification(self, key_name: str, number_value: float | int)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_scalar_type_properties.py#L141) — Feature: yaml-language-support, Property 5: Scalar Type Identification
  - `test_property_5_string_scalar_identification(self, key_name: str, string_value: str)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_scalar_type_properties.py#L84) — Feature: yaml-language-support, Property 5: Scalar Type Identification
- uses (calls/refs, reference-scoped): (1 test-only callers)

## Functions
- `_extract_yaml_elements(yaml_content: str)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_scalar_type_properties.py#L28) — Parse YAML content and return extracted elements. Skips if library unavailable.

## Module values
- `pytestmark` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_scalar_type_properties.py#L23)

