---
title: 'Module: tests/unit/languages/_test_yaml_element_metadata_properties_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/languages/_test_yaml_element_metadata_properties_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages._test_yaml_element_metadata_properties_helpers`/
symbols:
  parse_yaml_elements_and_lines: parse_yaml_elements_and_lines().
  assert_comment_elements: assert_comment_elements().
  assert_element_line_number_properties: assert_element_line_number_properties().
  assert_mixed_structures_complete_metadata: assert_mixed_structures_complete_metadata().
  assert_mixed_structures_mapping_raw_text: assert_mixed_structures_mapping_raw_text().
  assert_mixed_structures_nesting: assert_mixed_structures_nesting().
  assert_raw_text_fields: assert_raw_text_fields().
  assert_raw_text_matches_source: assert_raw_text_matches_source().
  assert_mapping_raw_text_contains_key: assert_mapping_raw_text_contains_key().
  assert_scalar_raw_text_non_empty: assert_scalar_raw_text_non_empty().
  assert_consistent_mappings: assert_consistent_mappings().
  assert_sequence_metadata: assert_sequence_metadata().
  assert_comment_raw_text: assert_comment_raw_text().
  assert_element_line_metadata: assert_element_line_metadata().
---
# Module: [`tests/unit/languages/_test_yaml_element_metadata_properties_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_yaml_element_metadata_properties_helpers.py)

## Functions
- `assert_comment_elements(elements, source_lines)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_yaml_element_metadata_properties_helpers.py#L205) — Assert comment metadata is complete and source aligned.
- `assert_comment_raw_text(elements, source_lines)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_yaml_element_metadata_properties_helpers.py#L187) — Assert comment elements have raw text and source alignment.
- `assert_consistent_mappings(elements, source_lines, num_keys: int)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_yaml_element_metadata_properties_helpers.py#L237) — Assert mappings are complete and aligned for consistency test.
- `assert_element_line_metadata(elements)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_yaml_element_metadata_properties_helpers.py#L225) — Assert every element has numeric and non-empty metadata.
- `assert_element_line_number_properties(elements, source_lines)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_yaml_element_metadata_properties_helpers.py#L29) — Assert core line-number invariants for extracted YAML elements.
- `assert_mapping_raw_text_contains_key(elements)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_yaml_element_metadata_properties_helpers.py#L168) — Assert mapping raw_text includes declared keys.
- `assert_mixed_structures_complete_metadata(elements)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_yaml_element_metadata_properties_helpers.py#L81) — Assert mixed structure elements have complete metadata fields.
- `assert_mixed_structures_mapping_raw_text(mappings, yaml_content)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_yaml_element_metadata_properties_helpers.py#L98) — Assert mapping raw_text matches the original YAML source lines.
- `assert_mixed_structures_nesting(elements)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_yaml_element_metadata_properties_helpers.py#L111) — Assert same-level elements have no partial overlaps.
- `assert_raw_text_fields(elements)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_yaml_element_metadata_properties_helpers.py#L140) — Assert raw_text presence and string type for extracted elements.
- `assert_raw_text_matches_source(elements, source_lines)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_yaml_element_metadata_properties_helpers.py#L154) — Assert raw_text matches YAML source text for each element range.
- `assert_scalar_raw_text_non_empty(elements)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_yaml_element_metadata_properties_helpers.py#L178) — Assert scalar elements with values have non-empty raw text.
- `assert_sequence_metadata(sequences)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_yaml_element_metadata_properties_helpers.py#L267) — Assert sequence-specific metadata invariants.
- `parse_yaml_elements_and_lines(yaml_content: str)` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_yaml_element_metadata_properties_helpers.py#L10) — Parse YAML content and return elements with their source lines.

