---
title: 'Module: tree_sitter_analyzer/formatters/cpp_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/cpp_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.cpp_formatter`/CppTableFormatter#
symbols:
  CppTableFormatter: ''
  CppTableFormatter._format_method_row: _format_method_row().
  CppTableFormatter.format_analysis_result: format_analysis_result().
  CppTableFormatter.format_type: format_type.
  CppTableFormatter.format_advanced: format_advanced().
  CppTableFormatter._create_compact_signature: _create_compact_signature().
  CppTableFormatter._format_full_table: _format_full_table().
  CppTableFormatter._format_compact_table: _format_compact_table().
  CppTableFormatter._shorten_type: _shorten_type().
  CppTableFormatter._format_class_details: _format_class_details().
  CppTableFormatter.format_structure: format_structure().
  CppTableFormatter.format_class_details: format_class_details.
  CppTableFormatter.format_method_row: format_method_row.
  CppTableFormatter.create_compact_signature: create_compact_signature.
  CppTableFormatter.shorten_type: shorten_type.
  CppTableFormatter.format_table: format_table().
  CppTableFormatter.format_summary: format_summary().
  CppTableFormatter._format_json: _format_json().
---
# Module: [`tree_sitter_analyzer/formatters/cpp_formatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/cpp_formatter.py)

## Classes
### `CppTableFormatter`  ·  implements/extends BaseTableFormatter, CppTableFormatterConvertMixin
- def: [`tree_sitter_analyzer/formatters/cpp_formatter.py:20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/cpp_formatter.py#L20)
- doc: Table formatter specialized for C and C++
- signature: `class CppTableFormatter(CppTableFormatterConvertMixin, BaseTableFormatter):`
- members:
  - `_create_compact_signature(self, method: dict[str, Any])` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/cpp_formatter.py#L52) — Create compact method signature
  - `_format_class_details(self, class_info: dict[str, Any], data: dict[str, Any])` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/cpp_formatter.py#L27) — Format details for a single class
  - `_format_compact_table(self, data: dict[str, Any])` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/cpp_formatter.py#L33) — Compact table format for C/C++
  - `_format_full_table(self, data: dict[str, Any])` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/cpp_formatter.py#L23) — Full table format for C/C++
  - `_format_method_row(self, method: dict[str, Any])` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/cpp_formatter.py#L37) — Format a method table row
  - `_shorten_type(self, type_name: Any)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/cpp_formatter.py#L56) — Shorten type name for C/C++ compact display
  - `format_advanced(self, analysis_result: dict[str, Any], output_format: str = "json")` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/cpp_formatter.py#L106) — Format advanced analysis output
  - `format_analysis_result(self, analysis_result: Any, table_type: str)` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/cpp_formatter.py#L84) — Format analysis result directly (C++ specific).
  - `format_structure(self, analysis_result: dict[str, Any])` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/cpp_formatter.py#L102) — Format structure analysis output
  - `format_summary(self, analysis_result: dict[str, Any])` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/cpp_formatter.py#L80) — Format summary output
  - `format_table(self, analysis_result: dict[str, Any], table_type: str = "full")` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/cpp_formatter.py#L66) — Format table output
  - `create_compact_signature` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/cpp_formatter.py#L63)
  - `format_class_details` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/cpp_formatter.py#L61)
  - `format_method_row` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/cpp_formatter.py#L62)
  - `format_type` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/cpp_formatter.py#L71)
  - `shorten_type` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/cpp_formatter.py#L64)
- protocol/private: `_format_json`[`L117`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/cpp_formatter.py#L117)
- uses (calls/refs, reference-scoped): [`format_structure`](base_formatter.md#BaseTableFormatter.format_structure), [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`_format_csv`](base_formatter.md#BaseTableFormatter._format_csv), [`format_cpp_full_table`](_cpp_formatter_helpers.md#format_cpp_full_table), [`_extract_doc_summary`](base_formatter.md#BaseTableFormatter._extract_doc_summary), [`shorten_cpp_type`](_cpp_formatter_helpers.md#shorten_cpp_type), [`_clean_csv_text`](base_formatter.md#BaseTableFormatter._clean_csv_text), [`_create_full_signature`](base_formatter.md#BaseTableFormatter._create_full_signature), [`format_cpp_compact_table`](_cpp_formatter_helpers.md#format_cpp_compact_table), [`_convert_visibility`](base_formatter.md#BaseTableFormatter._convert_visibility), [`format_cpp_class_details`](_cpp_formatter_helpers.md#format_cpp_class_details), [`create_cpp_compact_signature`](_cpp_formatter_helpers.md#create_cpp_compact_signature), [`CppTableFormatterConvertMixin`](_cpp_formatter_convert_mixin.md#CppTableFormatterConvertMixin), [`_convert_analysis_result_to_format`](_cpp_formatter_convert_mixin.md#CppTableFormatterConvertMixin._convert_analysis_result_to_format)
- used by: [`format_structure`](base_formatter.md#BaseTableFormatter.format_structure), [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`_register_language_formatters_safe`](formatter_registry.md#_register_language_formatters_safe), [`_formatters`](language_formatter_factory.md#LanguageFormatterFactory._formatters), [`_format_compact_table`](base_formatter.md#BaseTableFormatter._format_compact_table), [`_format_full_table`](base_formatter.md#BaseTableFormatter._format_full_table), [`format_table`](base_formatter.md#BaseTableFormatter.format_table), [`format_summary`](base_formatter.md#BaseTableFormatter.format_summary), [`format_advanced`](base_formatter.md#BaseTableFormatter.format_advanced), [`CppTableFormatterConvertMixin`](_cpp_formatter_convert_mixin.md#CppTableFormatterConvertMixin)  (3 test-only)

