---
title: 'Module: tree_sitter_analyzer/default_table_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/default_table_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.default_table_formatter`/DefaultTableFormatter#
symbols:
  DefaultTableFormatter._format_full_table: _format_full_table().
  DefaultTableFormatter._format_class_details: _format_class_details().
  DefaultTableFormatter.format_structure: format_structure().
  DefaultTableFormatter._format_compact_table: _format_compact_table().
  DefaultTableFormatter._format_method_row_detailed: _format_method_row_detailed().
  DefaultTableFormatter._format_signatures_table: _format_signatures_table().
  DefaultTableFormatter.format_type: format_type.
  DefaultTableFormatter: ''
  DefaultTableFormatter._abbreviate_type: _abbreviate_type().
  DefaultTableFormatter._format_compact_method_row: _format_compact_method_row().
  DefaultTableFormatter._get_class_methods: _get_class_methods.
  DefaultTableFormatter._get_class_fields: _get_class_fields.
  DefaultTableFormatter._get_platform_newline: _get_platform_newline.
  DefaultTableFormatter._format_csv: _format_csv.
  DefaultTableFormatter._get_visibility_symbol: _get_visibility_symbol.
  DefaultTableFormatter._create_full_signature: _create_full_signature.
  DefaultTableFormatter._convert_visibility: _convert_visibility.
  DefaultTableFormatter._extract_doc_summary: _extract_doc_summary.
  DefaultTableFormatter._convert_to_platform_newlines: _convert_to_platform_newlines().
  DefaultTableFormatter._create_compact_signature: _create_compact_signature().
  DefaultTableFormatter._shorten_type: _shorten_type.
  DefaultTableFormatter._clean_csv_text: _clean_csv_text.
  DefaultTableFormatter.include_javadoc: include_javadoc.
  DefaultTableFormatter.language: language.
  DefaultTableFormatter.__init__: __init__().
---
# Module: [`tree_sitter_analyzer/default_table_formatter.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py)

## Classes
### `DefaultTableFormatter`
- def: [`tree_sitter_analyzer/default_table_formatter.py:82`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L82)
- doc: Default table formatter for code analysis results.
- signature: `class DefaultTableFormatter:`
- members:
  - `__init__(self, format_type: str = "full", language: str = "java", include_javadoc: bool = False)` — [`L90`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L90) — Initialize the legacy table formatter.
  - `_abbreviate_type(self, type_str: str)` — [`L297`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L297) — Abbreviate type name for compact display.
  - `_convert_to_platform_newlines(self, text: str)` — [`L120`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L120) — Convert standard \n to platform-specific newline characters
  - `_create_compact_signature(self, method: dict[str, Any])` — [`L281`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L281) — Create compact method signature like (S,S):b
  - `_format_class_details(self, class_info: dict[str, Any], data: dict[str, Any])` — [`L202`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L202) — Format detailed information for a single class.
  - `_format_compact_method_row(self, method: dict[str, Any])` — [`L267`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L267) — Format method row for compact table format.
  - `_format_compact_table(self, data: dict[str, Any])` — [`L385`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L385) — Compact table format - compliant with format specification
  - `_format_full_table(self, data: dict[str, Any])` — [`L160`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L160) — Full table format - compliant with format specification
  - `_format_method_row_detailed(self, method: dict[str, Any])` — [`L250`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L250) — Format method row for detailed class view.
  - `_format_signatures_table(self, data: dict[str, Any])` — [`L338`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L338) — Lightweight method-directory format.
  - `format_structure(self, structure_data: dict[str, Any])` — [`L128`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L128) — Format structure data as table.
  - `format_type` — [`L104`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L104)
  - `include_javadoc` — [`L106`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L106)
  - `language` — [`L105`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L105)
- protocol/private: `_clean_csv_text`[`L117`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L117), `_convert_visibility`[`L115`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L115), `_create_full_signature`[`L113`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L113), `_extract_doc_summary`[`L116`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L116), `_format_csv`[`L111`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L111), `_get_class_fields`[`L110`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L110), `_get_class_methods`[`L109`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L109), `_get_platform_newline`[`L108`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L108), `_get_visibility_symbol`[`L112`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L112), `_shorten_type`[`L114`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/default_table_formatter.py#L114)
- uses (calls/refs, reference-scoped): [`format_csv`](_legacy_table_formatter_csv.md#format_csv), [`compact_table_header`](_legacy_table_formatter_compact.md#compact_table_header), [`_append_class_block`](formatters/_java_formatter_signatures_mixin.md#_append_class_block), [`append_multi_class_full_sections`](_legacy_table_formatter_full.md#append_multi_class_full_sections), [`append_single_class_full_sections`](_legacy_table_formatter_full.md#append_single_class_full_sections), [`append_compact_fields_section`](_legacy_table_formatter_compact.md#append_compact_fields_section), [`append_detail_fields_section`](_legacy_table_formatter_detail.md#append_detail_fields_section), [`get_class_fields`](_legacy_table_formatter_members.md#get_class_fields), [`get_class_methods`](_legacy_table_formatter_members.md#get_class_methods), [`append_detailed_methods_section`](_legacy_table_formatter_detail.md#append_detailed_methods_section), [`convert_visibility`](_legacy_table_formatter_common.md#convert_visibility), [`extract_doc_summary`](_legacy_table_formatter_common.md#extract_doc_summary), [`get_visibility_symbol`](_legacy_table_formatter_common.md#get_visibility_symbol), [`_append_method_lines`](formatters/_java_formatter_signatures_mixin.md#_append_method_lines), [`full_table_header`](_legacy_table_formatter_full.md#full_table_header), [`append_compact_info_section`](_legacy_table_formatter_compact.md#append_compact_info_section), [`append_compact_methods_section`](_legacy_table_formatter_compact.md#append_compact_methods_section), [`append_full_class_info_section`](_legacy_table_formatter_full.md#append_full_class_info_section), [`append_full_imports_section`](_legacy_table_formatter_full.md#append_full_imports_section), [`append_full_package_section`](_legacy_table_formatter_full.md#append_full_package_section), [`clean_csv_text`](_legacy_table_formatter_common.md#clean_csv_text), [`create_full_signature`](_legacy_table_formatter_common.md#create_full_signature), [`detail_method_groups`](_legacy_table_formatter_detail.md#detail_method_groups), [`get_platform_newline`](_legacy_table_formatter_common.md#get_platform_newline), [`shorten_type`](_legacy_table_formatter_common.md#shorten_type)
- used by: [`_register_language_formatters_safe`](formatters/formatter_registry.md#_register_language_formatters_safe)  (3 test-only)

