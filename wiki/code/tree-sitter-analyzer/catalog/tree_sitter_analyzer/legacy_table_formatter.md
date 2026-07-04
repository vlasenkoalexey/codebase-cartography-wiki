---
title: 'Module: tree_sitter_analyzer/legacy_table_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/legacy_table_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.legacy_table_formatter`/LegacyTableFormatter#
symbols:
  LegacyTableFormatter: ''
  LegacyTableFormatter.format_structure: format_structure().
  LegacyTableFormatter._shorten_type: _shorten_type.
  LegacyTableFormatter._format_class_details: _format_class_details().
  LegacyTableFormatter._abbreviate_type: _abbreviate_type().
  LegacyTableFormatter._format_full_table: _format_full_table().
  LegacyTableFormatter._clean_csv_text: _clean_csv_text.
  LegacyTableFormatter._create_full_signature: _create_full_signature.
  LegacyTableFormatter._extract_doc_summary: _extract_doc_summary.
  LegacyTableFormatter._format_method_row_detailed: _format_method_row_detailed().
  LegacyTableFormatter._get_visibility_symbol: _get_visibility_symbol.
  LegacyTableFormatter._format_compact_table: _format_compact_table().
  LegacyTableFormatter._convert_visibility: _convert_visibility.
  LegacyTableFormatter._get_class_methods: _get_class_methods.
  LegacyTableFormatter._get_class_fields: _get_class_fields.
  LegacyTableFormatter._create_compact_signature: _create_compact_signature().
  LegacyTableFormatter.format_type: format_type.
  LegacyTableFormatter._get_platform_newline: _get_platform_newline.
  LegacyTableFormatter._convert_to_platform_newlines: _convert_to_platform_newlines().
  LegacyTableFormatter._format_compact_method_row: _format_compact_method_row().
  LegacyTableFormatter.include_javadoc: include_javadoc.
  LegacyTableFormatter._format_csv: _format_csv.
  LegacyTableFormatter.language: language.
  LegacyTableFormatter.__init__: __init__().
---
# Module: [`tree_sitter_analyzer/legacy_table_formatter.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py)

## Classes
### `LegacyTableFormatter`
- def: [`tree_sitter_analyzer/legacy_table_formatter.py:82`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L82) — documented in [tree_sitter_analyzer-legacy_table_formatter](../../concepts/tree_sitter_analyzer-legacy_table_formatter.md)
- doc: Legacy table formatter — renamed to DefaultTableFormatter.
- signature: `class LegacyTableFormatter:`
- members:
  - `__init__(self, format_type: str = "full", language: str = "java", include_javadoc: bool = False)` — [`L90`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L90) — Initialize the legacy table formatter.
  - `_abbreviate_type(self, type_str: str)` — [`L295`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L295) — Abbreviate type name for compact display. — documented in [tree_sitter_analyzer-legacy_table_formatter](../../concepts/tree_sitter_analyzer-legacy_table_formatter.md)
  - `_convert_to_platform_newlines(self, text: str)` — [`L120`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L120) — Convert standard \n to platform-specific newline characters — documented in [tree_sitter_analyzer-legacy_table_formatter](../../concepts/tree_sitter_analyzer-legacy_table_formatter.md)
  - `_create_compact_signature(self, method: dict[str, Any])` — [`L279`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L279) — Create compact method signature like (S,S):b
  - `_format_class_details(self, class_info: dict[str, Any], data: dict[str, Any])` — [`L200`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L200) — Format detailed information for a single class. — documented in [tree_sitter_analyzer-legacy_table_formatter](../../concepts/tree_sitter_analyzer-legacy_table_formatter.md)
  - `_format_compact_method_row(self, method: dict[str, Any])` — [`L265`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L265) — Format method row for compact table format.
  - `_format_compact_table(self, data: dict[str, Any])` — [`L336`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L336) — Compact table format - compliant with format specification — documented in [tree_sitter_analyzer-legacy_table_formatter](../../concepts/tree_sitter_analyzer-legacy_table_formatter.md)
  - `_format_full_table(self, data: dict[str, Any])` — [`L158`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L158) — Full table format - compliant with format specification — documented in [tree_sitter_analyzer-legacy_table_formatter](../../concepts/tree_sitter_analyzer-legacy_table_formatter.md)
  - `_format_method_row_detailed(self, method: dict[str, Any])` — [`L248`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L248) — Format method row for detailed class view. — documented in [tree_sitter_analyzer-legacy_table_formatter](../../concepts/tree_sitter_analyzer-legacy_table_formatter.md)
  - `format_structure(self, structure_data: dict[str, Any])` — [`L128`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L128) — Format structure data as table. — documented in [tree_sitter_analyzer-legacy_table_formatter](../../concepts/tree_sitter_analyzer-legacy_table_formatter.md)
  - `format_type` — [`L104`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L104) — documented in [tree_sitter_analyzer-legacy_table_formatter](../../concepts/tree_sitter_analyzer-legacy_table_formatter.md)
  - `include_javadoc` — [`L106`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L106)
  - `language` — [`L105`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L105)
- protocol/private: `_clean_csv_text`[`L117`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L117), `_convert_visibility`[`L115`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L115), `_create_full_signature`[`L113`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L113), `_extract_doc_summary`[`L116`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L116), `_format_csv`[`L111`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L111), `_get_class_fields`[`L110`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L110), `_get_class_methods`[`L109`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L109), `_get_platform_newline`[`L108`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L108), `_get_visibility_symbol`[`L112`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L112), `_shorten_type`[`L114`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/legacy_table_formatter.py#L114)
- uses (calls/refs, reference-scoped): [`format_csv`](_legacy_table_formatter_csv.md#format_csv), [`compact_table_header`](_legacy_table_formatter_compact.md#compact_table_header), [`append_multi_class_full_sections`](_legacy_table_formatter_full.md#append_multi_class_full_sections), [`append_single_class_full_sections`](_legacy_table_formatter_full.md#append_single_class_full_sections), [`append_compact_fields_section`](_legacy_table_formatter_compact.md#append_compact_fields_section), [`append_detail_fields_section`](_legacy_table_formatter_detail.md#append_detail_fields_section), [`get_class_fields`](_legacy_table_formatter_members.md#get_class_fields), [`get_class_methods`](_legacy_table_formatter_members.md#get_class_methods), [`append_detailed_methods_section`](_legacy_table_formatter_detail.md#append_detailed_methods_section), [`convert_visibility`](_legacy_table_formatter_common.md#convert_visibility), [`extract_doc_summary`](_legacy_table_formatter_common.md#extract_doc_summary), [`get_visibility_symbol`](_legacy_table_formatter_common.md#get_visibility_symbol), [`full_table_header`](_legacy_table_formatter_full.md#full_table_header), [`append_compact_info_section`](_legacy_table_formatter_compact.md#append_compact_info_section), [`append_compact_methods_section`](_legacy_table_formatter_compact.md#append_compact_methods_section), [`append_full_class_info_section`](_legacy_table_formatter_full.md#append_full_class_info_section), [`append_full_imports_section`](_legacy_table_formatter_full.md#append_full_imports_section), [`append_full_package_section`](_legacy_table_formatter_full.md#append_full_package_section), [`clean_csv_text`](_legacy_table_formatter_common.md#clean_csv_text), [`create_full_signature`](_legacy_table_formatter_common.md#create_full_signature), [`detail_method_groups`](_legacy_table_formatter_detail.md#detail_method_groups), [`get_platform_newline`](_legacy_table_formatter_common.md#get_platform_newline), [`shorten_type`](_legacy_table_formatter_common.md#shorten_type)
- used by: (279 test-only callers)

