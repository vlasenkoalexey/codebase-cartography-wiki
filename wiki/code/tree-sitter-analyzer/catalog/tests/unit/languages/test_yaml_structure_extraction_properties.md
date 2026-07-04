---
title: 'Module: tests/unit/languages/test_yaml_structure_extraction_properties.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_yaml_structure_extraction_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_yaml_structure_extraction_properties`/
symbols:
  TestYAMLStructureExtractionProperties.test_property_2_structure_extraction_combined: TestYAMLStructureExtractionProperties#test_property_2_structure_extraction_combined().
  _extract_yaml_elements: _extract_yaml_elements().
  yaml_nested_content.generate_nested: yaml_nested_content().generate_nested().
  TestYAMLStructureExtractionProperties.test_property_2_structure_extraction_mappings: TestYAMLStructureExtractionProperties#test_property_2_structure_extraction_mappings().
  TestYAMLStructureExtractionProperties.test_property_2_structure_extraction_sequences: TestYAMLStructureExtractionProperties#test_property_2_structure_extraction_sequences().
  TestYAMLStructureExtractionProperties.test_property_2_structure_extraction_nested: TestYAMLStructureExtractionProperties#test_property_2_structure_extraction_nested().
  yaml_nested_content: yaml_nested_content().
  pytestmark: pytestmark.
  TestYAMLStructureExtractionProperties.test_property_2_structure_extraction_completeness_count: TestYAMLStructureExtractionProperties#test_property_2_structure_extraction_completeness_count().
  yaml_mapping_content: yaml_mapping_content().
  yaml_sequence_content: yaml_sequence_content().
  _group_by_level: _group_by_level().
  _assert_no_partial_overlap: _assert_no_partial_overlap().
  TestYAMLStructureExtractionProperties: TestYAMLStructureExtractionProperties#
---
# Module: [`tests/unit/languages/test_yaml_structure_extraction_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_structure_extraction_properties.py)

## Classes
### `TestYAMLStructureExtractionProperties`
- def: [`tests/unit/languages/test_yaml_structure_extraction_properties.py:193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_structure_extraction_properties.py#L193)
- doc: Property-based tests for YAML structure extraction.
- signature: `class TestYAMLStructureExtractionProperties:`
- members:
  - `test_property_2_structure_extraction_combined(self, mapping_content: str, sequence_content: str)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_structure_extraction_properties.py#L369) — Feature: yaml-language-support, Property 2: Structure Extraction Completeness
  - `test_property_2_structure_extraction_completeness_count(self, num_mappings: int, num_sequences: int)` — [`L414`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_structure_extraction_properties.py#L414) — Feature: yaml-language-support, Property 2: Structure Extraction Completeness
  - `test_property_2_structure_extraction_mappings(self, yaml_content: str)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_structure_extraction_properties.py#L198) — Feature: yaml-language-support, Property 2: Structure Extraction Completeness
  - `test_property_2_structure_extraction_nested(self, yaml_content: str)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_structure_extraction_properties.py#L312) — Feature: yaml-language-support, Property 2: Structure Extraction Completeness
  - `test_property_2_structure_extraction_sequences(self, yaml_content: str)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_structure_extraction_properties.py#L254) — Feature: yaml-language-support, Property 2: Structure Extraction Completeness
- uses (calls/refs, reference-scoped): (6 test-only callers)

## Functions
- `_assert_no_partial_overlap(level: int, level_elements: list)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_structure_extraction_properties.py#L173) — Assert that elements at a given nesting level do not partially overlap.
- `_extract_yaml_elements(yaml_content: str)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_structure_extraction_properties.py#L147) — Parse YAML and return extracted elements. Skips if library unavailable.
- `_group_by_level(elements)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_structure_extraction_properties.py#L163) — Group elements by nesting_level.
- `generate_nested(current_depth, indent="")` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_structure_extraction_properties.py#L93)
- `yaml_mapping_content(draw)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_structure_extraction_properties.py#L29) — Generate YAML content with mappings.
- `yaml_nested_content(draw)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_structure_extraction_properties.py#L89) — Generate YAML content with nested structures.
- `yaml_sequence_content(draw)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_structure_extraction_properties.py#L65) — Generate YAML content with sequences.

## Module values
- `pytestmark` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_structure_extraction_properties.py#L22)

