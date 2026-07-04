---
title: 'Module: tests/unit/languages/test_yaml_multi_document_properties.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_yaml_multi_document_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_yaml_multi_document_properties`/
symbols:
  TestYAMLMultiDocumentProperties.test_property_3_multi_document_separation: TestYAMLMultiDocumentProperties#test_property_3_multi_document_separation().
  TestYAMLMultiDocumentProperties.test_property_3_document_element_association: TestYAMLMultiDocumentProperties#test_property_3_document_element_association().
  TestYAMLMultiDocumentProperties.test_property_3_document_child_count: TestYAMLMultiDocumentProperties#test_property_3_document_child_count().
  _parse_yaml_content: _parse_yaml_content().
  TestYAMLMultiDocumentProperties.test_property_3_explicit_document_markers: TestYAMLMultiDocumentProperties#test_property_3_explicit_document_markers().
  TestYAMLMultiDocumentProperties.test_property_3_single_vs_multi_document: TestYAMLMultiDocumentProperties#test_property_3_single_vs_multi_document().
  pytestmark: pytestmark.
  yaml_multi_document_content: yaml_multi_document_content().
  _find_containing_doc: _find_containing_doc().
  yaml_explicit_multi_document_content: yaml_explicit_multi_document_content().
  _build_multi_doc_yaml: _build_multi_doc_yaml().
  TestYAMLMultiDocumentProperties: TestYAMLMultiDocumentProperties#
---
# Module: [`tests/unit/languages/test_yaml_multi_document_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_multi_document_properties.py)

## Classes
### `TestYAMLMultiDocumentProperties`
- def: [`tests/unit/languages/test_yaml_multi_document_properties.py:125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_multi_document_properties.py#L125)
- doc: Property-based tests for YAML multi-document separation.
- signature: `class TestYAMLMultiDocumentProperties:`
- members:
  - `test_property_3_document_child_count(self, yaml_content: str)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_multi_document_properties.py#L319) — Feature: yaml-language-support, Property 3: Multi-Document Separation
  - `test_property_3_document_element_association(self, num_documents: int, keys_per_doc: int)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_multi_document_properties.py#L247) — Feature: yaml-language-support, Property 3: Multi-Document Separation
  - `test_property_3_explicit_document_markers(self, yaml_content: str)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_multi_document_properties.py#L208) — Feature: yaml-language-support, Property 3: Multi-Document Separation
  - `test_property_3_multi_document_separation(self, yaml_content: str)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_multi_document_properties.py#L130) — Feature: yaml-language-support, Property 3: Multi-Document Separation
  - `test_property_3_single_vs_multi_document(self, num_documents: int)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_multi_document_properties.py#L283) — Feature: yaml-language-support, Property 3: Multi-Document Separation
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`element_type`](../../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`document_index`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.document_index), [`child_count`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.child_count), [`nesting_level`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.nesting_level)  (5 test-only)

## Functions
- `_build_multi_doc_yaml(num_documents: int, keys_per_doc: int)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_multi_document_properties.py#L116) — Build a predictable multi-document YAML string.
- `_find_containing_doc(element, doc_elements)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_multi_document_properties.py#L108) — Return the first document whose line range contains element, or None.
- `_parse_yaml_content(yaml_content: str)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_multi_document_properties.py#L90) — Parse YAML and return (elements, doc_elements). Skips if library unavailable.
- `yaml_explicit_multi_document_content(draw)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_multi_document_properties.py#L75) — Generate YAML content with explicit document markers.
- `yaml_multi_document_content(draw)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_multi_document_properties.py#L29) — Generate YAML content with multiple documents.

## Module values
- `pytestmark` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_multi_document_properties.py#L22)

