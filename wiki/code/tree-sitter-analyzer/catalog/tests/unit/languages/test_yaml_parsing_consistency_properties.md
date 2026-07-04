---
title: 'Module: tests/unit/languages/test_yaml_parsing_consistency_properties.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_yaml_parsing_consistency_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_yaml_parsing_consistency_properties`/
symbols:
  TestYAMLParsingConsistencyProperties.test_property_1_parsing_round_trip_consistency_simple: TestYAMLParsingConsistencyProperties#test_property_1_parsing_round_trip_consistency_simple().
  TestYAMLParsingConsistencyProperties.test_property_1_parsing_round_trip_consistency_comments: TestYAMLParsingConsistencyProperties#test_property_1_parsing_round_trip_consistency_comments().
  TestYAMLParsingConsistencyProperties.test_property_1_parsing_round_trip_consistency_sequences: TestYAMLParsingConsistencyProperties#test_property_1_parsing_round_trip_consistency_sequences().
  TestYAMLParsingConsistencyProperties.test_property_1_parsing_round_trip_consistency_nested: TestYAMLParsingConsistencyProperties#test_property_1_parsing_round_trip_consistency_nested().
  TestYAMLParsingConsistencyProperties.test_property_1_parsing_round_trip_consistency_deterministic: TestYAMLParsingConsistencyProperties#test_property_1_parsing_round_trip_consistency_deterministic().
  TestYAMLParsingConsistencyProperties.test_property_1_parsing_round_trip_consistency_multi_document: TestYAMLParsingConsistencyProperties#test_property_1_parsing_round_trip_consistency_multi_document().
  TestYAMLParsingConsistencyProperties.test_property_1_parsing_round_trip_consistency_stability: TestYAMLParsingConsistencyProperties#test_property_1_parsing_round_trip_consistency_stability().
  simple_yaml_content: simple_yaml_content().
  pytestmark: pytestmark.
  yaml_with_sequences: yaml_with_sequences().
  yaml_with_nested_structures: yaml_with_nested_structures().
  yaml_with_comments: yaml_with_comments().
  yaml_with_multi_documents: yaml_with_multi_documents().
  TestYAMLParsingConsistencyProperties: TestYAMLParsingConsistencyProperties#
---
# Module: [`tests/unit/languages/test_yaml_parsing_consistency_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_parsing_consistency_properties.py)

## Classes
### `TestYAMLParsingConsistencyProperties`
- def: [`tests/unit/languages/test_yaml_parsing_consistency_properties.py:211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_parsing_consistency_properties.py#L211)
- doc: Property-based tests for YAML parsing consistency.
- signature: `class TestYAMLParsingConsistencyProperties:`
- members:
  - `test_property_1_parsing_round_trip_consistency_comments(self, yaml_content: str)` — [`L420`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_parsing_consistency_properties.py#L420) — Feature: yaml-language-support, Property 1: Parsing Round-Trip Consistency
  - `test_property_1_parsing_round_trip_consistency_deterministic(self, yaml_content: str)` — [`L532`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_parsing_consistency_properties.py#L532) — Feature: yaml-language-support, Property 1: Parsing Round-Trip Consistency
  - `test_property_1_parsing_round_trip_consistency_multi_document(self, yaml_content: str)` — [`L471`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_parsing_consistency_properties.py#L471) — Feature: yaml-language-support, Property 1: Parsing Round-Trip Consistency
  - `test_property_1_parsing_round_trip_consistency_nested(self, yaml_content: str)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_parsing_consistency_properties.py#L366) — Feature: yaml-language-support, Property 1: Parsing Round-Trip Consistency
  - `test_property_1_parsing_round_trip_consistency_sequences(self, yaml_content: str)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_parsing_consistency_properties.py#L314) — Feature: yaml-language-support, Property 1: Parsing Round-Trip Consistency
  - `test_property_1_parsing_round_trip_consistency_simple(self, yaml_content: str)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_parsing_consistency_properties.py#L224) — Feature: yaml-language-support, Property 1: Parsing Round-Trip Consistency
  - `test_property_1_parsing_round_trip_consistency_stability(self, yaml_content: str, num_parses: int)` — [`L600`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_parsing_consistency_properties.py#L600) — Feature: yaml-language-support, Property 1: Parsing Round-Trip Consistency
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`element_type`](../../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`YAMLPlugin`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin), [`analyze_file`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin.analyze_file)  (5 test-only)

## Functions
- `simple_yaml_content(draw)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_parsing_consistency_properties.py#L30) — Generate simple valid YAML content.
- `yaml_with_comments(draw)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_parsing_consistency_properties.py#L136) — Generate YAML content with comments.
- `yaml_with_multi_documents(draw)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_parsing_consistency_properties.py#L171) — Generate YAML content with multiple documents.
- `yaml_with_nested_structures(draw)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_parsing_consistency_properties.py#L87) — Generate YAML content with nested structures.
- `yaml_with_sequences(draw)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_parsing_consistency_properties.py#L66) — Generate YAML content with sequences.

## Module values
- `pytestmark` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_parsing_consistency_properties.py#L23)

