---
title: 'Module: tests/unit/formatters/test_js_formatter_table_output.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_js_formatter_table_output.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_js_formatter_table_output`/
symbols:
  TestJavaScriptSectionAbsence._empty_data: TestJavaScriptSectionAbsence#_empty_data().
  TestJavaScriptFullTableFormatting.formatter: TestJavaScriptFullTableFormatting#formatter().
  TestJavaScriptFullTableFormatting.sample_js_data: TestJavaScriptFullTableFormatting#sample_js_data().
  TestJavaScriptSectionAbsence.formatter: TestJavaScriptSectionAbsence#formatter().
  TestJavaScriptSectionAbsence.test_format_full_table_no_imports: TestJavaScriptSectionAbsence#test_format_full_table_no_imports().
  TestJavaScriptSectionAbsence.test_format_full_table_no_classes: TestJavaScriptSectionAbsence#test_format_full_table_no_classes().
  TestJavaScriptSectionAbsence.test_format_full_table_no_variables: TestJavaScriptSectionAbsence#test_format_full_table_no_variables().
  TestJavaScriptSectionAbsence.test_format_full_table_no_functions: TestJavaScriptSectionAbsence#test_format_full_table_no_functions().
  TestJavaScriptSectionAbsence.test_format_full_table_no_exports: TestJavaScriptSectionAbsence#test_format_full_table_no_exports().
  TestJavaScriptSectionAbsence.test_format_full_table_trailing_blank_lines_removal: TestJavaScriptSectionAbsence#test_format_full_table_trailing_blank_lines_removal().
  TestJavaScriptCompactTableFormatting.formatter: TestJavaScriptCompactTableFormatting#formatter().
  TestJavaScriptCompactTableFormatting.sample_js_data: TestJavaScriptCompactTableFormatting#sample_js_data().
  TestJavaScriptCompactSignatureMixin.formatter: TestJavaScriptCompactSignatureMixin#formatter().
  _sample_js_data: _sample_js_data().
  TestJavaScriptFullTableFormatting: TestJavaScriptFullTableFormatting#
  TestJavaScriptFullTableFormatting.test_format_full_table_complete: TestJavaScriptFullTableFormatting#test_format_full_table_complete().
  TestJavaScriptFullTableFormatting.test_format_full_table_script_type: TestJavaScriptFullTableFormatting#test_format_full_table_script_type().
  TestJavaScriptFullTableFormatting.test_format_full_table_with_import_construction: TestJavaScriptFullTableFormatting#test_format_full_table_with_import_construction().
  TestJavaScriptFullTableFormatting.test_format_full_table_class_methods_and_properties_counting: TestJavaScriptFullTableFormatting#test_format_full_table_class_methods_and_properties_counting().
  TestJavaScriptFullTableFormatting.test_format_function_row: TestJavaScriptFullTableFormatting#test_format_function_row().
  TestJavaScriptFullTableFormatting.test_format_method_row: TestJavaScriptFullTableFormatting#test_format_method_row().
  TestJavaScriptSectionAbsence: TestJavaScriptSectionAbsence#
  TestJavaScriptSectionAbsence.test_format_compact_table_trailing_blank_lines_removal: TestJavaScriptSectionAbsence#test_format_compact_table_trailing_blank_lines_removal().
  TestJavaScriptCompactTableFormatting: TestJavaScriptCompactTableFormatting#
  TestJavaScriptCompactTableFormatting.test_format_compact_table: TestJavaScriptCompactTableFormatting#test_format_compact_table().
  TestJavaScriptCompactTableFormatting.test_format_compact_table_with_methods: TestJavaScriptCompactTableFormatting#test_format_compact_table_with_methods().
  TestJavaScriptCompactTableFormatting.test_format_compact_table_no_methods: TestJavaScriptCompactTableFormatting#test_format_compact_table_no_methods().
  TestJavaScriptCompactTableFormatting.test_format_compact_table_method_row_content: TestJavaScriptCompactTableFormatting#test_format_compact_table_method_row_content().
  TestJavaScriptCompactTableFormatting.test_format_compact_info_section_method_count: TestJavaScriptCompactTableFormatting#test_format_compact_info_section_method_count().
  TestJavaScriptCompactTableFormatting.test_format_compact_method_missing_line_range: TestJavaScriptCompactTableFormatting#test_format_compact_method_missing_line_range().
  TestJavaScriptCompactSignatureMixin: TestJavaScriptCompactSignatureMixin#
  TestJavaScriptCompactSignatureMixin.test_create_compact_signature_dict_params: TestJavaScriptCompactSignatureMixin#test_create_compact_signature_dict_params().
  TestJavaScriptCompactSignatureMixin.test_create_compact_signature_non_dict_params: TestJavaScriptCompactSignatureMixin#test_create_compact_signature_non_dict_params().
  TestJavaScriptCompactSignatureMixin.test_create_compact_signature_empty_params: TestJavaScriptCompactSignatureMixin#test_create_compact_signature_empty_params().
  TestJavaScriptCompactSignatureMixin.test_create_compact_signature_string_params: TestJavaScriptCompactSignatureMixin#test_create_compact_signature_string_params().
  TestJavaScriptCompactSignatureMixin.test_create_compact_signature_no_params_key: TestJavaScriptCompactSignatureMixin#test_create_compact_signature_no_params_key().
  TestJavaScriptCompactSignatureMixin.test_create_compact_signature_dict_without_type: TestJavaScriptCompactSignatureMixin#test_create_compact_signature_dict_without_type().
  TestJavaScriptCompactSignatureMixin.test_create_compact_signature_default_return_type: TestJavaScriptCompactSignatureMixin#test_create_compact_signature_default_return_type().
---
# Module: [`tests/unit/formatters/test_js_formatter_table_output.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py)

## Classes
### `TestJavaScriptCompactSignatureMixin`
- def: [`tests/unit/formatters/test_js_formatter_table_output.py:535`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L535)
- doc: Cover uncovered branches in _javascript_formatter_compact_mixin.py.
- signature: `class TestJavaScriptCompactSignatureMixin:`
- members:
  - `formatter(self)` — [`L539`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L539)
  - `test_create_compact_signature_default_return_type(self, formatter)` — [`L584`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L584)
  - `test_create_compact_signature_dict_params(self, formatter)` — [`L542`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L542)
  - `test_create_compact_signature_dict_without_type(self, formatter)` — [`L576`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L576)
  - `test_create_compact_signature_empty_params(self, formatter)` — [`L561`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L561)
  - `test_create_compact_signature_no_params_key(self, formatter)` — [`L571`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L571)
  - `test_create_compact_signature_non_dict_params(self, formatter)` — [`L553`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L553)
  - `test_create_compact_signature_string_params(self, formatter)` — [`L566`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L566)
- uses (calls/refs, reference-scoped): [`JavaScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/javascript_formatter.md#JavaScriptTableFormatter)

### `TestJavaScriptCompactTableFormatting`
- def: [`tests/unit/formatters/test_js_formatter_table_output.py:419`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L419)
- doc: Tests for compact table formatting output.
- signature: `class TestJavaScriptCompactTableFormatting:`
- members:
  - `formatter(self)` — [`L423`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L423)
  - `sample_js_data(self)` — [`L427`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L427)
  - `test_format_compact_info_section_method_count(self, formatter)` — [`L503`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L503)
  - `test_format_compact_method_missing_line_range(self, formatter)` — [`L519`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L519)
  - `test_format_compact_table(self, formatter, sample_js_data)` — [`L430`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L430)
  - `test_format_compact_table_method_row_content(self, formatter)` — [`L483`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L483)
  - `test_format_compact_table_no_methods(self, formatter)` — [`L470`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L470)
  - `test_format_compact_table_with_methods(self, formatter)` — [`L437`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L437)
- uses (calls/refs, reference-scoped): [`JavaScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/javascript_formatter.md#JavaScriptTableFormatter)  (1 test-only)

### `TestJavaScriptFullTableFormatting`
- def: [`tests/unit/formatters/test_js_formatter_table_output.py:223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L223)
- doc: Tests for full table formatting output.
- signature: `class TestJavaScriptFullTableFormatting:`
- members:
  - `formatter(self)` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L227)
  - `sample_js_data(self)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L231)
  - `test_format_full_table_class_methods_and_properties_counting(self, formatter)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L274)
  - `test_format_full_table_complete(self, formatter, sample_js_data)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L234)
  - `test_format_full_table_script_type(self, formatter)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L242)
  - `test_format_full_table_with_import_construction(self, formatter)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L255)
  - `test_format_function_row(self, formatter)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L320)
  - `test_format_method_row(self, formatter)` — [`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L340)
- uses (calls/refs, reference-scoped): [`JavaScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/javascript_formatter.md#JavaScriptTableFormatter)  (1 test-only)

### `TestJavaScriptSectionAbsence`
- def: [`tests/unit/formatters/test_js_formatter_table_output.py:363`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L363)
- doc: Tests verifying sections are omitted when data is empty.
- signature: `class TestJavaScriptSectionAbsence:`
- members:
  - `formatter(self)` — [`L367`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L367)
  - `test_format_compact_table_trailing_blank_lines_removal(self, formatter)` — [`L407`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L407)
  - `test_format_full_table_no_classes(self, formatter)` — [`L385`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L385)
  - `test_format_full_table_no_exports(self, formatter)` — [`L399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L399)
  - `test_format_full_table_no_functions(self, formatter)` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L393)
  - `test_format_full_table_no_imports(self, formatter)` — [`L381`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L381)
  - `test_format_full_table_no_variables(self, formatter)` — [`L389`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L389)
  - `test_format_full_table_trailing_blank_lines_removal(self, formatter)` — [`L403`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L403)
- protocol/private: `_empty_data`[`L370`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L370)
- uses (calls/refs, reference-scoped): [`JavaScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/javascript_formatter.md#JavaScriptTableFormatter)

## Functions
- `_sample_js_data()` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_table_output.py#L12)

