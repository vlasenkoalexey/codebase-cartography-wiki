---
title: 'Module: tests/unit/formatters/test_java_formatter_properties.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_java_formatter_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_java_formatter_properties`/
symbols:
  java_analysis_result: java_analysis_result().
  java_field: java_field().
  java_method: java_method().
  java_type: java_type.
  java_identifier: java_identifier.
  TestFormatterOutputCompletenessProperties.test_property_2_full_table_contains_all_field_names: TestFormatterOutputCompletenessProperties#test_property_2_full_table_contains_all_field_names().
  TestFormatterOutputCompletenessProperties.test_property_2_full_table_contains_all_method_names: TestFormatterOutputCompletenessProperties#test_property_2_full_table_contains_all_method_names().
  TestFormatterOutputCompletenessProperties.test_property_2_full_table_contains_field_types: TestFormatterOutputCompletenessProperties#test_property_2_full_table_contains_field_types().
  TestFormatterAnnotationHandlingProperties.test_property_2_class_visibility_in_output: TestFormatterAnnotationHandlingProperties#test_property_2_class_visibility_in_output().
  TestFormatterGenericTypeHandlingProperties.test_property_2_method_signature_completeness: TestFormatterGenericTypeHandlingProperties#test_property_2_method_signature_completeness().
  java_class: java_class().
  TestFormatterOutputCompletenessProperties.test_property_2_full_table_contains_all_class_names: TestFormatterOutputCompletenessProperties#test_property_2_full_table_contains_all_class_names().
  TestFormatterOutputCompletenessProperties.test_property_2_compact_table_contains_all_method_names: TestFormatterOutputCompletenessProperties#test_property_2_compact_table_contains_all_method_names().
  TestFormatterOutputCompletenessProperties.test_property_2_imports_appear_in_output: TestFormatterOutputCompletenessProperties#test_property_2_imports_appear_in_output().
  TestFormatterOutputCompletenessProperties.test_property_2_package_name_appears_in_output: TestFormatterOutputCompletenessProperties#test_property_2_package_name_appears_in_output().
  TestFormatterOutputCompletenessProperties.test_property_2_csv_format_contains_all_elements: TestFormatterOutputCompletenessProperties#test_property_2_csv_format_contains_all_elements().
  TestFormatterOutputCompletenessProperties.test_property_2_json_format_preserves_all_data: TestFormatterOutputCompletenessProperties#test_property_2_json_format_preserves_all_data().
  TestFormatterEdgeCaseProperties.test_property_2_enum_constants_in_output: TestFormatterEdgeCaseProperties#test_property_2_enum_constants_in_output().
  parameter: parameter.
  java_import: java_import().
  TestFormatterEdgeCaseProperties.test_property_2_output_scales_with_elements: TestFormatterEdgeCaseProperties#test_property_2_output_scales_with_elements().
  parameters: parameters.
  visibility: visibility.
  line_range: line_range.
  TestFormatterOutputCompletenessProperties.is_in_class_range: TestFormatterOutputCompletenessProperties#is_in_class_range().
  TestFormatterGenericTypeHandlingProperties.test_property_2_generic_type_shortening_consistency: TestFormatterGenericTypeHandlingProperties#test_property_2_generic_type_shortening_consistency().
  package_name: package_name.
  java_primitive_types: java_primitive_types.
  java_common_types: java_common_types.
  method_visibility: method_visibility.
  modifiers: modifiers.
  TestFormatterOutputCompletenessProperties: TestFormatterOutputCompletenessProperties#
  TestFormatterAnnotationHandlingProperties: TestFormatterAnnotationHandlingProperties#
  TestFormatterGenericTypeHandlingProperties: TestFormatterGenericTypeHandlingProperties#
  TestFormatterEdgeCaseProperties: TestFormatterEdgeCaseProperties#
---
# Module: [`tests/unit/formatters/test_java_formatter_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py)

## Classes
### `TestFormatterAnnotationHandlingProperties`
- def: [`tests/unit/formatters/test_java_formatter_properties.py:478`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L478)
- doc: Property-based tests for annotation handling in formatter output.
- signature: `class TestFormatterAnnotationHandlingProperties:`
- members:
  - `test_property_2_class_visibility_in_output(self, class_name: str, visibility_val: str, class_type: str)` — [`L494`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L494) — **Feature: test-coverage-improvement, Property 2: Formatter Output Completeness**
- uses (calls/refs, reference-scoped): [`JavaTableFormatter`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter), [`_format_full_table`](../../../tree_sitter_analyzer/formatters/_java_formatter_full_mixin.md#JavaTableFormatterFullMixin._format_full_table)  (2 test-only)

### `TestFormatterEdgeCaseProperties`
- def: [`tests/unit/formatters/test_java_formatter_properties.py:649`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L649)
- doc: Property-based tests for edge cases in formatter output.
- signature: `class TestFormatterEdgeCaseProperties:`
- members:
  - `test_property_2_enum_constants_in_output(self, enum_name: str, constants: list[str])` — [`L750`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L750) — **Feature: test-coverage-improvement, Property 2: Formatter Output Completeness**
  - `test_property_2_output_scales_with_elements(self, num_classes: int, num_methods: int, num_fields: int)` — [`L665`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L665) — **Feature: test-coverage-improvement, Property 2: Formatter Output Completeness**
- uses (calls/refs, reference-scoped): [`JavaTableFormatter`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter), [`_format_full_table`](../../../tree_sitter_analyzer/formatters/_java_formatter_full_mixin.md#JavaTableFormatterFullMixin._format_full_table)  (1 test-only)

### `TestFormatterGenericTypeHandlingProperties`
- def: [`tests/unit/formatters/test_java_formatter_properties.py:543`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L543)
- doc: Property-based tests for generic type handling in formatter output.
- signature: `class TestFormatterGenericTypeHandlingProperties:`
- members:
  - `test_property_2_generic_type_shortening_consistency(self, type_name: str)` — [`L622`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L622) — **Feature: test-coverage-improvement, Property 2: Formatter Output Completeness**
  - `test_property_2_method_signature_completeness(self, method_name: str, return_type: str, param_types: list[str])` — [`L559`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L559) — **Feature: test-coverage-improvement, Property 2: Formatter Output Completeness**
- uses (calls/refs, reference-scoped): [`JavaTableFormatter`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter), [`_format_full_table`](../../../tree_sitter_analyzer/formatters/_java_formatter_full_mixin.md#JavaTableFormatterFullMixin._format_full_table)  (2 test-only)

### `TestFormatterOutputCompletenessProperties`
- def: [`tests/unit/formatters/test_java_formatter_properties.py:200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L200)
- doc: Property-based tests for formatter output completeness.
- signature: `class TestFormatterOutputCompletenessProperties:`
- members:
  - `is_in_class_range(field)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L248)
  - `test_property_2_compact_table_contains_all_method_names(self, data: dict)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L338) — **Feature: test-coverage-improvement, Property 2: Formatter Output Completeness**
  - `test_property_2_csv_format_contains_all_elements(self, data: dict)` — [`L409`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L409) — **Feature: test-coverage-improvement, Property 2: Formatter Output Completeness**
  - `test_property_2_full_table_contains_all_class_names(self, data: dict)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L212) — **Feature: test-coverage-improvement, Property 2: Formatter Output Completeness**
  - `test_property_2_full_table_contains_all_field_names(self, data: dict)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L235) — **Feature: test-coverage-improvement, Property 2: Formatter Output Completeness**
  - `test_property_2_full_table_contains_all_method_names(self, data: dict)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L269) — **Feature: test-coverage-improvement, Property 2: Formatter Output Completeness**
  - `test_property_2_full_table_contains_field_types(self, data: dict)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L303) — **Feature: test-coverage-improvement, Property 2: Formatter Output Completeness**
  - `test_property_2_imports_appear_in_output(self, data: dict)` — [`L362`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L362) — **Feature: test-coverage-improvement, Property 2: Formatter Output Completeness**
  - `test_property_2_json_format_preserves_all_data(self, data: dict)` — [`L441`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L441) — **Feature: test-coverage-improvement, Property 2: Formatter Output Completeness**
  - `test_property_2_package_name_appears_in_output(self, data: dict)` — [`L386`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L386) — **Feature: test-coverage-improvement, Property 2: Formatter Output Completeness**
- uses (calls/refs, reference-scoped): [`JavaTableFormatter`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter), [`_format_full_table`](../../../tree_sitter_analyzer/formatters/_java_formatter_full_mixin.md#JavaTableFormatterFullMixin._format_full_table), [`_format_csv`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter._format_csv), [`_format_compact_table`](../../../tree_sitter_analyzer/formatters/_java_formatter_compact_mixin.md#JavaTableFormatterCompactMixin._format_compact_table), [`_format_json`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter._format_json)  (1 test-only)

## Functions
- `java_analysis_result(draw)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L180)
- `java_class(draw)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L157)
- `java_field(draw)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L122)
- `java_import(draw)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L172)
- `java_method(draw, is_constructor=None)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L135)

## Module values
- `java_common_types` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L73)
- `java_identifier` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L19)
- `java_primitive_types` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L69)
- `java_type` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L87)
- `line_range` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L96)
- `method_visibility` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L93)
- `modifiers` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L103)
- `package_name` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L56)
- `parameter` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L111)
- `parameters` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L117)
- `visibility` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_properties.py#L90)

