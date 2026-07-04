---
title: 'Module: tests/unit/core/test_serialization_roundtrip_properties.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_serialization_roundtrip_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_serialization_roundtrip_properties`/
symbols:
  analysis_result: analysis_result().
  function_element: function_element().
  class_element: class_element().
  variable_element: variable_element().
  import_element: import_element().
  package_element: package_element().
  java_formatter_data: java_formatter_data().
  TestSerializationDataIntegrityProperties.test_property_1_serialization_preserves_metadata: TestSerializationDataIntegrityProperties#test_property_1_serialization_preserves_metadata().
  identifier: identifier.
  TestSerializationDataIntegrityProperties.test_property_1_serialization_preserves_element_counts: TestSerializationDataIntegrityProperties#test_property_1_serialization_preserves_element_counts().
  TestSerializationRoundTripProperties.test_property_1_analysis_result_to_dict_roundtrip: TestSerializationRoundTripProperties#test_property_1_analysis_result_to_dict_roundtrip().
  TestSerializationRoundTripProperties.test_property_1_analysis_result_to_json_roundtrip: TestSerializationRoundTripProperties#test_property_1_analysis_result_to_json_roundtrip().
  TestSerializationRoundTripProperties.test_property_1_analysis_result_to_mcp_format_roundtrip: TestSerializationRoundTripProperties#test_property_1_analysis_result_to_mcp_format_roundtrip().
  TestSerializationRoundTripProperties.test_property_1_analysis_result_summary_dict_roundtrip: TestSerializationRoundTripProperties#test_property_1_analysis_result_summary_dict_roundtrip().
  TestSerializationRoundTripProperties.test_property_1_java_formatter_json_roundtrip: TestSerializationRoundTripProperties#test_property_1_java_formatter_json_roundtrip().
  TestSerializationRoundTripProperties.test_property_1_java_formatter_json_preserves_all_class_names: TestSerializationRoundTripProperties#test_property_1_java_formatter_json_preserves_all_class_names().
  TestSerializationRoundTripProperties.test_property_1_java_formatter_json_preserves_all_method_names: TestSerializationRoundTripProperties#test_property_1_java_formatter_json_preserves_all_method_names().
  TestSerializationRoundTripProperties.test_property_1_java_formatter_json_preserves_all_field_names: TestSerializationRoundTripProperties#test_property_1_java_formatter_json_preserves_all_field_names().
  TestSerializationDataIntegrityProperties.test_property_1_format_table_json_is_valid: TestSerializationDataIntegrityProperties#test_property_1_format_table_json_is_valid().
  TestSerializationDataIntegrityProperties.test_property_1_format_advanced_json_is_valid: TestSerializationDataIntegrityProperties#test_property_1_format_advanced_json_is_valid().
  package_name: package_name.
  java_type: java_type.
  visibility: visibility.
  line_number: line_number.
  TestSerializationRoundTripProperties: TestSerializationRoundTripProperties#
  TestSerializationDataIntegrityProperties: TestSerializationDataIntegrityProperties#
---
# Module: [`tests/unit/core/test_serialization_roundtrip_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py)

## Classes
### `TestSerializationDataIntegrityProperties`
- def: [`tests/unit/core/test_serialization_roundtrip_properties.py:642`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L642)
- doc: Property-based tests for data integrity during serialization.
- signature: `class TestSerializationDataIntegrityProperties:`
- members:
  - `test_property_1_format_advanced_json_is_valid(self, data: dict)` — [`L742`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L742) — **Feature: test-coverage-improvement, Property 1: Serialization Round-Trip Consistency**
  - `test_property_1_format_table_json_is_valid(self, data: dict)` — [`L720`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L720) — **Feature: test-coverage-improvement, Property 1: Serialization Round-Trip Consistency**
  - `test_property_1_serialization_preserves_element_counts(self, result: AnalysisResult)` — [`L652`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L652) — **Feature: test-coverage-improvement, Property 1: Serialization Round-Trip Consistency**
  - `test_property_1_serialization_preserves_metadata(self, result: AnalysisResult)` — [`L692`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L692) — **Feature: test-coverage-improvement, Property 1: Serialization Round-Trip Consistency**
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`JavaTableFormatter`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter), [`to_dict`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.to_dict), [`get_summary`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.get_summary), [`format_advanced`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter.format_advanced), [`analysis_time`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.analysis_time), [`format_table`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter.format_table)  (2 test-only)

### `TestSerializationRoundTripProperties`
- def: [`tests/unit/core/test_serialization_roundtrip_properties.py:393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L393)
- doc: Property-based tests for serialization round-trip consistency.
- signature: `class TestSerializationRoundTripProperties:`
- members:
  - `test_property_1_analysis_result_summary_dict_roundtrip(self, result: AnalysisResult)` — [`L496`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L496) — **Feature: test-coverage-improvement, Property 1: Serialization Round-Trip Consistency**
  - `test_property_1_analysis_result_to_dict_roundtrip(self, result: AnalysisResult)` — [`L403`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L403) — **Feature: test-coverage-improvement, Property 1: Serialization Round-Trip Consistency**
  - `test_property_1_analysis_result_to_json_roundtrip(self, result: AnalysisResult)` — [`L428`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L428) — **Feature: test-coverage-improvement, Property 1: Serialization Round-Trip Consistency**
  - `test_property_1_analysis_result_to_mcp_format_roundtrip(self, result: AnalysisResult)` — [`L461`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L461) — **Feature: test-coverage-improvement, Property 1: Serialization Round-Trip Consistency**
  - `test_property_1_java_formatter_json_preserves_all_class_names(self, data: dict)` — [`L569`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L569) — **Feature: test-coverage-improvement, Property 1: Serialization Round-Trip Consistency**
  - `test_property_1_java_formatter_json_preserves_all_field_names(self, data: dict)` — [`L619`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L619) — **Feature: test-coverage-improvement, Property 1: Serialization Round-Trip Consistency**
  - `test_property_1_java_formatter_json_preserves_all_method_names(self, data: dict)` — [`L593`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L593) — **Feature: test-coverage-improvement, Property 1: Serialization Round-Trip Consistency**
  - `test_property_1_java_formatter_json_roundtrip(self, data: dict)` — [`L529`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L529) — **Feature: test-coverage-improvement, Property 1: Serialization Round-Trip Consistency**
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`JavaTableFormatter`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter), [`to_dict`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.to_dict), [`to_mcp_format`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.to_mcp_format), [`to_summary_dict`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.to_summary_dict), [`_format_json`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter._format_json), [`to_json`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.to_json)  (2 test-only)

## Functions
- `analysis_result(draw)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L247)
- `class_element(draw)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L155)
- `function_element(draw)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L121)
- `import_element(draw)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L213)
- `java_formatter_data(draw)` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L284) — Generate data in the format expected by JavaTableFormatter.
- `package_element(draw)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L234)
- `variable_element(draw)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L185)

## Module values
- `identifier` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L35)
- `java_type` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L89)
- `line_number` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L116)
- `package_name` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L76)
- `visibility` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_serialization_roundtrip_properties.py#L113)

