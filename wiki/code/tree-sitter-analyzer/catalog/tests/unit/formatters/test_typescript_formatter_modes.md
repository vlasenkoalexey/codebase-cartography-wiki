---
title: 'Module: tests/unit/formatters/test_typescript_formatter_modes.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_typescript_formatter_modes.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_typescript_formatter_modes`/TestTypeScriptFormatter
symbols:
  TestTypeScriptFormatterCompactTable.formatter: CompactTable#formatter().
  TestTypeScriptFormatterSignatureHelpers.formatter: SignatureHelpers#formatter().
  TestTypeScriptFormatterFormatTable.formatter: FormatTable#formatter().
  TestTypeScriptFormatterFormatSummary.formatter: FormatSummary#formatter().
  TestTypeScriptFormatterFormatAdvanced.formatter: FormatAdvanced#formatter().
  TestTypeScriptFormatterFormatJson.formatter: FormatJson#formatter().
  TestTypeScriptFormatterCompactTable: CompactTable#
  TestTypeScriptFormatterCompactTable.test_compact_table_with_classes: CompactTable#test_compact_table_with_classes().
  TestTypeScriptFormatterCompactTable.test_compact_table_no_classes: CompactTable#test_compact_table_no_classes().
  TestTypeScriptFormatterCompactTable.test_compact_table_with_methods: CompactTable#test_compact_table_with_methods().
  TestTypeScriptFormatterCompactTable.test_compact_table_with_fields: CompactTable#test_compact_table_with_fields().
  TestTypeScriptFormatterCompactTable.test_compact_table_with_package_none: CompactTable#test_compact_table_with_package_none().
  TestTypeScriptFormatterCompactTable.test_compact_table_no_methods: CompactTable#test_compact_table_no_methods().
  TestTypeScriptFormatterSignatureHelpers: SignatureHelpers#
  TestTypeScriptFormatterSignatureHelpers.test_create_full_signature_with_modifiers: SignatureHelpers#test_create_full_signature_with_modifiers().
  TestTypeScriptFormatterSignatureHelpers.test_create_csv_signature_with_modifiers: SignatureHelpers#test_create_csv_signature_with_modifiers().
  TestTypeScriptFormatterSignatureHelpers.test_create_compact_signature_dict_params: SignatureHelpers#test_create_compact_signature_dict_params().
  TestTypeScriptFormatterSignatureHelpers.test_create_compact_signature_non_dict_params: SignatureHelpers#test_create_compact_signature_non_dict_params().
  TestTypeScriptFormatterFormatTable: FormatTable#
  TestTypeScriptFormatterFormatTable.test_format_table_changes_type_temporarily: FormatTable#test_format_table_changes_type_temporarily().
  TestTypeScriptFormatterFormatTable.test_format_table_default_type: FormatTable#test_format_table_default_type().
  TestTypeScriptFormatterFormatSummary: FormatSummary#
  TestTypeScriptFormatterFormatSummary.test_format_summary_delegates_to_compact: FormatSummary#test_format_summary_delegates_to_compact().
  TestTypeScriptFormatterFormatAdvanced: FormatAdvanced#
  TestTypeScriptFormatterFormatAdvanced.test_format_advanced_json: FormatAdvanced#test_format_advanced_json().
  TestTypeScriptFormatterFormatAdvanced.test_format_advanced_csv: FormatAdvanced#test_format_advanced_csv().
  TestTypeScriptFormatterFormatAdvanced.test_format_advanced_default_falls_back_to_full: FormatAdvanced#test_format_advanced_default_falls_back_to_full().
  TestTypeScriptFormatterFormatJson: FormatJson#
  TestTypeScriptFormatterFormatJson.test_format_json_success: FormatJson#test_format_json_success().
  TestTypeScriptFormatterFormatJson.test_format_json_error: FormatJson#test_format_json_error().
---
# Module: [`tests/unit/formatters/test_typescript_formatter_modes.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py)

## Classes
### `TestTypeScriptFormatterCompactTable`
- def: [`tests/unit/formatters/test_typescript_formatter_modes.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L16)
- doc: Test _format_compact_table method
- signature: `class TestTypeScriptFormatterCompactTable:`
- members:
  - `formatter(self)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L20)
  - `test_compact_table_no_classes(self, formatter)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L44)
  - `test_compact_table_no_methods(self, formatter)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L125)
  - `test_compact_table_with_classes(self, formatter)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L23)
  - `test_compact_table_with_fields(self, formatter)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L92)
  - `test_compact_table_with_methods(self, formatter)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L56)
  - `test_compact_table_with_package_none(self, formatter)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L108)
- uses (calls/refs, reference-scoped): [`TypeScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/typescript_formatter.md#TypeScriptTableFormatter)

### `TestTypeScriptFormatterFormatAdvanced`
- def: [`tests/unit/formatters/test_typescript_formatter_modes.py:255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L255)
- doc: Test format_advanced method
- signature: `class TestTypeScriptFormatterFormatAdvanced:`
- members:
  - `formatter(self)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L259)
  - `test_format_advanced_csv(self, formatter)` — [`L273`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L273)
  - `test_format_advanced_default_falls_back_to_full(self, formatter)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L283)
  - `test_format_advanced_json(self, formatter)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L262)
- uses (calls/refs, reference-scoped): [`TypeScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/typescript_formatter.md#TypeScriptTableFormatter)

### `TestTypeScriptFormatterFormatJson`
- def: [`tests/unit/formatters/test_typescript_formatter_modes.py:300`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L300)
- doc: Test _format_json method
- signature: `class TestTypeScriptFormatterFormatJson:`
- members:
  - `formatter(self)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L304)
  - `test_format_json_error(self, formatter)` — [`L313`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L313)
  - `test_format_json_success(self, formatter)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L307)
- uses (calls/refs, reference-scoped): [`TypeScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/typescript_formatter.md#TypeScriptTableFormatter)

### `TestTypeScriptFormatterFormatSummary`
- def: [`tests/unit/formatters/test_typescript_formatter_modes.py:231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L231)
- doc: Test format_summary method
- signature: `class TestTypeScriptFormatterFormatSummary:`
- members:
  - `formatter(self)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L235)
  - `test_format_summary_delegates_to_compact(self, formatter)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L238)
- uses (calls/refs, reference-scoped): [`TypeScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/typescript_formatter.md#TypeScriptTableFormatter)

### `TestTypeScriptFormatterFormatTable`
- def: [`tests/unit/formatters/test_typescript_formatter_modes.py:194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L194)
- doc: Test format_table method
- signature: `class TestTypeScriptFormatterFormatTable:`
- members:
  - `formatter(self)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L198)
  - `test_format_table_changes_type_temporarily(self, formatter)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L201)
  - `test_format_table_default_type(self, formatter)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L214)
- uses (calls/refs, reference-scoped): [`TypeScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/typescript_formatter.md#TypeScriptTableFormatter)

### `TestTypeScriptFormatterSignatureHelpers`
- def: [`tests/unit/formatters/test_typescript_formatter_modes.py:142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L142)
- doc: Test _create_signature / _create_compact_signature / _create_csv_signature
- signature: `class TestTypeScriptFormatterSignatureHelpers:`
- members:
  - `formatter(self)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L146)
  - `test_create_compact_signature_dict_params(self, formatter)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L175)
  - `test_create_compact_signature_non_dict_params(self, formatter)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L184)
  - `test_create_csv_signature_with_modifiers(self, formatter)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L163)
  - `test_create_full_signature_with_modifiers(self, formatter)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_modes.py#L149)
- uses (calls/refs, reference-scoped): [`TypeScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/typescript_formatter.md#TypeScriptTableFormatter)

