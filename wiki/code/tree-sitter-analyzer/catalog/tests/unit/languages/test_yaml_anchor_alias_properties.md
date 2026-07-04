---
title: 'Module: tests/unit/languages/test_yaml_anchor_alias_properties.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_yaml_anchor_alias_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_yaml_anchor_alias_properties`/
symbols:
  _parse_and_extract_yaml: _parse_and_extract_yaml().
  yaml_with_anchor_and_alias: yaml_with_anchor_and_alias().
  TestYAMLAnchorAliasProperties.test_property_6_anchor_detection: TestYAMLAnchorAliasProperties#test_property_6_anchor_detection().
  TestYAMLAnchorAliasProperties.test_property_6_alias_detection: TestYAMLAnchorAliasProperties#test_property_6_alias_detection().
  TestYAMLAnchorAliasProperties.test_property_6_anchor_alias_correspondence: TestYAMLAnchorAliasProperties#test_property_6_anchor_alias_correspondence().
  TestYAMLAnchorAliasProperties.test_property_6_multiple_anchors_detection: TestYAMLAnchorAliasProperties#test_property_6_multiple_anchors_detection().
  TestYAMLAnchorAliasProperties.test_property_6_multiple_aliases_detection: TestYAMLAnchorAliasProperties#test_property_6_multiple_aliases_detection().
  TestYAMLAnchorAliasProperties.test_property_6_nested_anchor_detection: TestYAMLAnchorAliasProperties#test_property_6_nested_anchor_detection().
  TestYAMLAnchorAliasProperties.test_property_6_anchor_name_extraction_accuracy: TestYAMLAnchorAliasProperties#test_property_6_anchor_name_extraction_accuracy().
  TestYAMLAnchorAliasProperties.test_property_6_alias_target_extraction_accuracy: TestYAMLAnchorAliasProperties#test_property_6_alias_target_extraction_accuracy().
  yaml_with_multiple_anchors: yaml_with_multiple_anchors().
  valid_anchor_name: valid_anchor_name().
  yaml_with_nested_anchor: yaml_with_nested_anchor().
  pytestmark: pytestmark.
  _yaml_scalar_value_strategy: _yaml_scalar_value_strategy().
  TestYAMLAnchorAliasProperties: TestYAMLAnchorAliasProperties#
---
# Module: [`tests/unit/languages/test_yaml_anchor_alias_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_anchor_alias_properties.py)

## Classes
### `TestYAMLAnchorAliasProperties`
- def: [`tests/unit/languages/test_yaml_anchor_alias_properties.py:173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_anchor_alias_properties.py#L173)
- doc: Property-based tests for YAML anchor and alias detection.
- signature: `class TestYAMLAnchorAliasProperties:`
- members:
  - `test_property_6_alias_detection(self, yaml_data: tuple[str, str])` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_anchor_alias_properties.py#L232) — Feature: yaml-language-support, Property 6: Anchor and Alias Detection
  - `test_property_6_alias_target_extraction_accuracy(self, anchor_name: str, value: str)` — [`L506`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_anchor_alias_properties.py#L506) — Feature: yaml-language-support, Property 6: Anchor and Alias Detection
  - `test_property_6_anchor_alias_correspondence(self, yaml_data: tuple[str, str])` — [`L286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_anchor_alias_properties.py#L286) — Feature: yaml-language-support, Property 6: Anchor and Alias Detection
  - `test_property_6_anchor_detection(self, yaml_data: tuple[str, str])` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_anchor_alias_properties.py#L178) — Feature: yaml-language-support, Property 6: Anchor and Alias Detection
  - `test_property_6_anchor_name_extraction_accuracy(self, anchor_name: str, value: str)` — [`L458`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_anchor_alias_properties.py#L458) — Feature: yaml-language-support, Property 6: Anchor and Alias Detection
  - `test_property_6_multiple_aliases_detection(self, yaml_data: tuple[str, list[str]])` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_anchor_alias_properties.py#L361) — Feature: yaml-language-support, Property 6: Anchor and Alias Detection
  - `test_property_6_multiple_anchors_detection(self, yaml_data: tuple[str, list[str]])` — [`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_anchor_alias_properties.py#L317) — Feature: yaml-language-support, Property 6: Anchor and Alias Detection
  - `test_property_6_nested_anchor_detection(self, yaml_data: tuple[str, str])` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_anchor_alias_properties.py#L397) — Feature: yaml-language-support, Property 6: Anchor and Alias Detection
- uses (calls/refs, reference-scoped): (5 test-only callers)

## Functions
- `_parse_and_extract_yaml(yaml_content: str)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_anchor_alias_properties.py#L99) — Parse YAML with tree-sitter and return extracted elements; skip if unavailable.
- `_yaml_scalar_value_strategy()` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_anchor_alias_properties.py#L83) — Hypothesis strategy for simple YAML scalar values (text or integer string).
- `valid_anchor_name(draw)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_anchor_alias_properties.py#L29) — Generate valid YAML anchor names.
- `yaml_with_anchor_and_alias(draw)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_anchor_alias_properties.py#L54) — Generate YAML content with anchors and aliases.
- `yaml_with_multiple_anchors(draw)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_anchor_alias_properties.py#L115) — Generate YAML content with multiple anchors and aliases.
- `yaml_with_nested_anchor(draw)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_anchor_alias_properties.py#L135) — Generate YAML content with nested structures containing anchors.

## Module values
- `pytestmark` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_anchor_alias_properties.py#L22)

