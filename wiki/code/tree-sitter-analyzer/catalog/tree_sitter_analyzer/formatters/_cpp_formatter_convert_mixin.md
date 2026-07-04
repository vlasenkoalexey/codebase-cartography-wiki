---
title: 'Module: tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._cpp_formatter_convert_mixin`/
symbols:
  _append_converted_cpp_element: _append_converted_cpp_element().
  CppTableFormatterConvertMixin._convert_one_cpp_element: CppTableFormatterConvertMixin#_convert_one_cpp_element().
  CppTableFormatterConvertMixin: CppTableFormatterConvertMixin#
  _valid_namespace_name: _valid_namespace_name().
  CppTableFormatterConvertMixin._convert_analysis_result_to_format: CppTableFormatterConvertMixin#_convert_analysis_result_to_format().
  _namespace_entry: _namespace_entry().
  _parse_cpp_parameter: _parse_cpp_parameter().
  CppTableFormatterConvertMixin._convert_function_element: CppTableFormatterConvertMixin#_convert_function_element().
  CppTableFormatterConvertMixin.convert_class_element: CppTableFormatterConvertMixin#convert_class_element.
  CppTableFormatterConvertMixin.convert_function_element: CppTableFormatterConvertMixin#convert_function_element.
  CppTableFormatterConvertMixin.convert_variable_element: CppTableFormatterConvertMixin#convert_variable_element.
  COMMON_NON_NAMESPACE_NAMES: COMMON_NON_NAMESPACE_NAMES.
  _parse_cpp_parameter_string: _parse_cpp_parameter_string().
  _build_cpp_format_result: _build_cpp_format_result().
  CppTableFormatterConvertMixin._convert_class_element: CppTableFormatterConvertMixin#_convert_class_element().
  CppTableFormatterConvertMixin._convert_variable_element: CppTableFormatterConvertMixin#_convert_variable_element().
  CppTableFormatterConvertMixin._convert_import_element: CppTableFormatterConvertMixin#_convert_import_element().
  CppTableFormatterConvertMixin.convert_import_element: CppTableFormatterConvertMixin#convert_import_element.
---
# Module: [`tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py)

## Classes
### `CppTableFormatterConvertMixin`
- def: [`tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py:127`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py#L127)
- doc: Convert analyzer models into the dict shape used by C/C++ formatters.
- signature: `class CppTableFormatterConvertMixin:`
- members:
  - `_convert_class_element(self, element: Any, index: int)` — [`L204`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py#L204) — Convert class element to table format.
  - `_convert_function_element(self, element: Any)` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py#L221) — Convert function element to table format.
  - `_convert_import_element(self, element: Any)` — [`L261`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py#L261) — Convert import element to table format.
  - `_convert_one_cpp_element(self, element: Any, index: int, classes: list[dict[str, Any]], methods: list[dict[str, Any]], fields: list[dict[str, Any]], imports: list[dict[str, Any]], packages: list[dict[str, Any]])` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py#L164) — Convert a single C++ element and route it to the right bucket.
  - `_convert_variable_element(self, element: Any)` — [`L244`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py#L244) — Convert variable element to table format.
  - `convert_class_element` — [`L278`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py#L278)
  - `convert_function_element` — [`L279`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py#L279)
  - `convert_import_element` — [`L281`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py#L281)
  - `convert_variable_element` — [`L280`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py#L280)
- protocol/private: `_convert_analysis_result_to_format`[`L130`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py#L130)
- uses (calls/refs, reference-scoped): [`Package`](../models/base.md#Package), [`CppTableFormatter`](cpp_formatter.md#CppTableFormatter), [`_append_converted_cpp_element`](_cpp_formatter_convert_mixin.md#_append_converted_cpp_element), [`_valid_namespace_name`](_cpp_formatter_convert_mixin.md#_valid_namespace_name), [`_namespace_entry`](_cpp_formatter_convert_mixin.md#_namespace_entry), [`_parse_cpp_parameter`](_cpp_formatter_convert_mixin.md#_parse_cpp_parameter), [`_build_cpp_format_result`](_cpp_formatter_convert_mixin.md#_build_cpp_format_result)
- used by: [`CppTableFormatter`](cpp_formatter.md#CppTableFormatter), [`format_analysis_result`](cpp_formatter.md#CppTableFormatter.format_analysis_result)

## Functions
- `_append_converted_cpp_element(formatter: Any, element: Any, index: int, classes: list[dict[str, Any]], methods: list[dict[str, Any]], fields: list[dict[str, Any]], imports: list[dict[str, Any]])` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py#L54)
- `_build_cpp_format_result(analysis_result: Any, package_name: str, packages: list[dict[str, Any]], classes: list[dict[str, Any]], methods: list[dict[str, Any]], fields: list[dict[str, Any]], imports: list[dict[str, Any]])` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py#L99)
- `_namespace_entry(namespace_name: str, element: Package)` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py#L44)
- `_parse_cpp_parameter(param: Any)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py#L74)
- `_parse_cpp_parameter_string(param: str)` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py#L82)
- `_valid_namespace_name(element: Package)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py#L24)

## Module values
- `COMMON_NON_NAMESPACE_NAMES` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_cpp_formatter_convert_mixin.py#L14)

