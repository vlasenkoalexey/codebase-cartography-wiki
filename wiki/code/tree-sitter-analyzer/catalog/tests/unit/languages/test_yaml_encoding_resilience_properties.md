---
title: 'Module: tests/unit/languages/test_yaml_encoding_resilience_properties.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_yaml_encoding_resilience_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_yaml_encoding_resilience_properties`/
symbols:
  TestYAMLEncodingResilienceProperties.test_property_13_utf8_encoding_handling: TestYAMLEncodingResilienceProperties#test_property_13_utf8_encoding_handling().
  TestYAMLEncodingResilienceProperties.test_property_13_latin1_encoding_handling: TestYAMLEncodingResilienceProperties#test_property_13_latin1_encoding_handling().
  TestYAMLEncodingResilienceProperties.test_property_13_encoding_consistency: TestYAMLEncodingResilienceProperties#test_property_13_encoding_consistency().
  MockRequest: MockRequest#
  pytestmark: pytestmark.
  MockRequest.__init__: MockRequest#__init__().
  MockRequest.output_format: MockRequest#output_format.
  MockRequest.detail_level: MockRequest#detail_level.
  TestYAMLEncodingResilienceProperties: TestYAMLEncodingResilienceProperties#
---
# Module: [`tests/unit/languages/test_yaml_encoding_resilience_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_encoding_resilience_properties.py)

## Classes
### `MockRequest`
- def: [`tests/unit/languages/test_yaml_encoding_resilience_properties.py:31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_encoding_resilience_properties.py#L31)
- doc: Mock request for testing.
- signature: `class MockRequest:`
- members:
  - `detail_level` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_encoding_resilience_properties.py#L36)
  - `output_format` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_encoding_resilience_properties.py#L35)
- protocol/private: `__init__`[`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_encoding_resilience_properties.py#L34)
- used by: (3 test-only callers)

### `TestYAMLEncodingResilienceProperties`
- def: [`tests/unit/languages/test_yaml_encoding_resilience_properties.py:39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_encoding_resilience_properties.py#L39)
- doc: Property-based tests for YAML encoding resilience.
- signature: `class TestYAMLEncodingResilienceProperties:`
- members:
  - `test_property_13_encoding_consistency(self, num_keys: int)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_encoding_resilience_properties.py#L150) — Feature: yaml-language-support, Property 13: Encoding Resilience
  - `test_property_13_latin1_encoding_handling(self, key_name: str, value: int)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_encoding_resilience_properties.py#L112) — Feature: yaml-language-support, Property 13: Encoding Resilience
  - `test_property_13_utf8_encoding_handling(self, key_name: str, value: str)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_encoding_resilience_properties.py#L65) — Feature: yaml-language-support, Property 13: Encoding Resilience
- uses (calls/refs, reference-scoped): [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`YAMLPlugin`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin), [`analyze_file`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin.analyze_file)  (1 test-only)

## Module values
- `pytestmark` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_encoding_resilience_properties.py#L26)

