---
title: 'Module: tests/unit/formatters/test_legacy_table_formatter_edge.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_legacy_table_formatter_edge.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_legacy_table_formatter_edge`/Test
symbols:
  TestFullTableMultiClassParamTypes.test_string_param_in_multi_class: FullTableMultiClassParamTypes#test_string_param_in_multi_class().
  TestFullTableMultiClassParamTypes.test_fallback_param_in_multi_class: FullTableMultiClassParamTypes#test_fallback_param_in_multi_class().
  TestEdgeCases.test_none_classes: EdgeCases#test_none_classes().
  TestEdgeCases.test_none_methods: EdgeCases#test_none_methods().
  TestEdgeCases.test_none_fields: EdgeCases#test_none_fields().
  TestEdgeCases.test_empty_package_name: EdgeCases#test_empty_package_name().
  TestEdgeCases.test_unknown_package: EdgeCases#test_unknown_package().
  TestEdgeCases.test_file_path_handling: EdgeCases#test_file_path_handling().
  TestEdgeCases.test_file_path_with_various_extensions: EdgeCases#test_file_path_with_various_extensions().
  TestEdgeCases.test_method_with_no_parameters: EdgeCases#test_method_with_no_parameters().
  TestEdgeCases.test_parameter_as_plain_string: EdgeCases#test_parameter_as_plain_string().
  TestEdgeCases.test_parameter_as_other_type: EdgeCases#test_parameter_as_other_type().
  TestEdgeCases.test_missing_line_range: EdgeCases#test_missing_line_range().
  TestDetailedFormatting.test_get_class_methods_basic: DetailedFormatting#test_get_class_methods_basic().
  TestDetailedFormatting.test_get_class_fields_basic: DetailedFormatting#test_get_class_fields_basic().
  TestDetailedFormatting.test_get_class_methods_excludes_nested: DetailedFormatting#test_get_class_methods_excludes_nested().
  TestDetailedFormatting.test_get_class_fields_excludes_nested: DetailedFormatting#test_get_class_fields_excludes_nested().
  TestLanguageSpecificFormatting.test_python_language_formatting: LanguageSpecificFormatting#test_python_language_formatting().
  TestLanguageSpecificFormatting.test_java_language_formatting: LanguageSpecificFormatting#test_java_language_formatting().
  TestLanguageSpecificFormatting.test_javascript_language_formatting: LanguageSpecificFormatting#test_javascript_language_formatting().
  TestCSVFieldAndParamCoverage.test_csv_with_field_rows: CSVFieldAndParamCoverage#test_csv_with_field_rows().
  TestCSVFieldAndParamCoverage.test_csv_method_with_string_params: CSVFieldAndParamCoverage#test_csv_method_with_string_params().
  TestCSVFieldAndParamCoverage.test_csv_method_with_fallback_params: CSVFieldAndParamCoverage#test_csv_method_with_fallback_params().
  TestCSVFieldAndParamCoverage.test_csv_method_is_static: CSVFieldAndParamCoverage#test_csv_method_is_static().
  TestCSVFieldAndParamCoverage.test_csv_method_is_final: CSVFieldAndParamCoverage#test_csv_method_is_final().
  TestCSVFieldAndParamCoverage.test_csv_constructor: CSVFieldAndParamCoverage#test_csv_constructor().
  TestCSVFieldAndParamCoverage.test_csv_class_with_final_modifier: CSVFieldAndParamCoverage#test_csv_class_with_final_modifier().
  TestCSVFieldAndParamCoverage.test_csv_field_with_is_static_flag: CSVFieldAndParamCoverage#test_csv_field_with_is_static_flag().
  TestDetailedFormatting.formatter_with_javadoc: DetailedFormatting#formatter_with_javadoc().
  TestFullTableMultiClassParamTypes._multi_class_data: FullTableMultiClassParamTypes#_multi_class_data().
  TestEdgeCases: EdgeCases#
  TestDetailedFormatting: DetailedFormatting#
  TestLanguageSpecificFormatting: LanguageSpecificFormatting#
  TestFullTableMultiClassParamTypes: FullTableMultiClassParamTypes#
  TestCSVFieldAndParamCoverage: CSVFieldAndParamCoverage#
---
# Module: [`tests/unit/formatters/test_legacy_table_formatter_edge.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py)

## Classes
### `TestCSVFieldAndParamCoverage`
- def: [`tests/unit/formatters/test_legacy_table_formatter_edge.py:325`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L325)
- doc: Cover _format_csv field rows and method param type branches.
- signature: `class TestCSVFieldAndParamCoverage:`
- members:
  - `test_csv_class_with_final_modifier(self)` — [`L429`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L429)
  - `test_csv_constructor(self)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L412)
  - `test_csv_field_with_is_static_flag(self)` — [`L446`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L446)
  - `test_csv_method_is_final(self)` — [`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L395)
  - `test_csv_method_is_static(self)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L378)
  - `test_csv_method_with_fallback_params(self)` — [`L362`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L362)
  - `test_csv_method_with_string_params(self)` — [`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L346)
  - `test_csv_with_field_rows(self)` — [`L328`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L328)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

### `TestDetailedFormatting`
- def: [`tests/unit/formatters/test_legacy_table_formatter_edge.py:145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L145)
- doc: Tests for detailed formatting methods.
- signature: `class TestDetailedFormatting:`
- members:
  - `formatter_with_javadoc(self)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L149) — Create formatter with javadoc enabled.
  - `test_get_class_fields_basic(self)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L168) — Test _get_class_fields method.
  - `test_get_class_fields_excludes_nested(self)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L204) — Test that nested class fields are excluded.
  - `test_get_class_methods_basic(self)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L153) — Test _get_class_methods method.
  - `test_get_class_methods_excludes_nested(self)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L183) — Test that nested class methods are excluded.
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_get_class_fields`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._get_class_fields), [`_get_class_methods`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._get_class_methods)

### `TestEdgeCases`
- def: [`tests/unit/formatters/test_legacy_table_formatter_edge.py:13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L13)
- doc: Tests for edge cases and error handling.
- signature: `class TestEdgeCases:`
- members:
  - `test_empty_package_name(self)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L37) — Test handling of empty package name.
  - `test_file_path_handling(self)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L52) — Test file path extraction for header.
  - `test_file_path_with_various_extensions(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L59) — Test file path handling with different extensions.
  - `test_method_with_no_parameters(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L73) — Test method with empty parameters list.
  - `test_missing_line_range(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L127) — Test handling of missing line range.
  - `test_none_classes(self)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L16) — Test handling of None classes list.
  - `test_none_fields(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L30) — Test handling of None fields list.
  - `test_none_methods(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L23) — Test handling of None methods list.
  - `test_parameter_as_other_type(self)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L109) — Test parameter handling when it's an unexpected type.
  - `test_parameter_as_plain_string(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L91) — Test parameter handling when it's just a string.
  - `test_unknown_package(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L44) — Test handling of unknown package.
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

### `TestFullTableMultiClassParamTypes`
- def: [`tests/unit/formatters/test_legacy_table_formatter_edge.py:265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L265)
- doc: Cover string and fallback param branches in _format_full_table multi-class path.
- signature: `class TestFullTableMultiClassParamTypes:`
- members:
  - `test_fallback_param_in_multi_class(self)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L303)
  - `test_string_param_in_multi_class(self)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L287)
- protocol/private: `_multi_class_data`[`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L268)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

### `TestLanguageSpecificFormatting`
- def: [`tests/unit/formatters/test_legacy_table_formatter_edge.py:226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L226)
- doc: Tests for language-specific formatting.
- signature: `class TestLanguageSpecificFormatting:`
- members:
  - `test_java_language_formatting(self)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L239) — Test Java language code block formatting.
  - `test_javascript_language_formatting(self)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L249) — Test JavaScript language code block formatting.
  - `test_python_language_formatting(self)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_edge.py#L229) — Test Python language code block formatting.
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

