---
title: 'Module: tests/unit/languages/test_plugins_fixed.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_plugins_fixed.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_plugins_fixed`/
symbols:
  test_extract_method_with_body: test_extract_method_with_body().
  test_extract_class_with_superclass: test_extract_class_with_superclass().
  test_extract_class_with_interfaces: test_extract_class_with_interfaces().
  test_extract_method_optimized_with_valid_node: test_extract_method_optimized_with_valid_node().
  java_extractor: java_extractor().
  test_parse_method_signature_parameters: test_parse_method_signature_parameters().
  test_parse_method_signature_throws: test_parse_method_signature_throws().
  test_extract_method_optimized_with_valid_node.mock_get_text: test_extract_method_optimized_with_valid_node().mock_get_text().
  test_parse_method_signature_parameters.mock_get_text: test_parse_method_signature_parameters().mock_get_text().
  test_parse_method_signature_throws.mock_get_text: test_parse_method_signature_throws().mock_get_text().
  test_extract_method_with_body.mock_get_text: test_extract_method_with_body().mock_get_text().
  test_extract_class_with_superclass.mock_get_text: test_extract_class_with_superclass().mock_get_text().
  test_extract_class_with_interfaces.mock_get_text: test_extract_class_with_interfaces().mock_get_text().
  test_extract_class_name_with_identifier: test_extract_class_name_with_identifier().
---
# Module: [`tests/unit/languages/test_plugins_fixed.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_fixed.py)

## Functions
- `java_extractor()` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_fixed.py#L22) — Fixture to provide JavaElementExtractor instance
- `mock_get_text(node)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_fixed.py#L71)
- `mock_get_text(node)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_fixed.py#L129)
- `mock_get_text(node)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_fixed.py#L162)
- `mock_get_text(node)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_fixed.py#L203)
- `mock_get_text(node)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_fixed.py#L251)
- `mock_get_text(node)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_fixed.py#L303)
- `test_extract_class_name_with_identifier(mocker, java_extractor)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_fixed.py#L91) — Test class name extraction from node with identifier using current implementation
- `test_extract_class_with_interfaces(mocker, java_extractor)` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_fixed.py#L270) — Test class extraction with interfaces using current implementation
- `test_extract_class_with_superclass(mocker, java_extractor)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_fixed.py#L221) — Test class extraction with superclass using current implementation
- `test_extract_method_optimized_with_valid_node(mocker, java_extractor)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_fixed.py#L27) — Test method extraction with valid node using current implementation
- `test_extract_method_with_body(mocker, java_extractor)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_fixed.py#L183) — Test method extraction includes body information using current implementation
- `test_parse_method_signature_parameters(mocker, java_extractor)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_fixed.py#L111) — Test parameter extraction from method signature using current implementation
- `test_parse_method_signature_throws(mocker, java_extractor)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_fixed.py#L149) — Test throws clause extraction from method signature using current implementation

