---
title: 'Module: tests/unit/formatters/test_typescript_formatter_core.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_typescript_formatter_core.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_typescript_formatter_core`/TestTypeScript
symbols:
  TestTypeScriptTableFormatter.test_format_compact_table: TableFormatter#test_format_compact_table().
  TestTypeScriptTableFormatter.test_format_csv: TableFormatter#test_format_csv().
  TestTypeScriptTableFormatter.formatter: TableFormatter#formatter().
  TestTypeScriptFormatterModifiers.formatter: FormatterModifiers#formatter().
  TestTypeScriptFormatterFullTableMethods.formatter: FormatterFullTableMethods#formatter().
  TestTypeScriptTableFormatter: TableFormatter#
  TestTypeScriptTableFormatter.sample_data: TableFormatter#sample_data().
  TestTypeScriptTableFormatter.test_format_full_table: TableFormatter#test_format_full_table().
  TestTypeScriptTableFormatter.test_format_full_table_tsx_file: TableFormatter#test_format_full_table_tsx_file().
  TestTypeScriptTableFormatter.test_format_full_table_declaration_file: TableFormatter#test_format_full_table_declaration_file().
  TestTypeScriptTableFormatter.test_format_interfaces_section: TableFormatter#test_format_interfaces_section().
  TestTypeScriptTableFormatter.test_format_type_aliases_section: TableFormatter#test_format_type_aliases_section().
  TestTypeScriptTableFormatter.test_format_enums_section: TableFormatter#test_format_enums_section().
  TestTypeScriptTableFormatter.test_format_classes_section: TableFormatter#test_format_classes_section().
  TestTypeScriptTableFormatter.test_format_functions_section: TableFormatter#test_format_functions_section().
  TestTypeScriptTableFormatter.test_format_variables_section: TableFormatter#test_format_variables_section().
  TestTypeScriptTableFormatter.test_get_element_type_name: TableFormatter#test_get_element_type_name().
  TestTypeScriptTableFormatter.test_format_element_details: TableFormatter#test_format_element_details().
  TestTypeScriptTableFormatter.test_format_element_details_minimal: TableFormatter#test_format_element_details_minimal().
  TestTypeScriptTableFormatter.test_format_empty_data: TableFormatter#test_format_empty_data().
  TestTypeScriptTableFormatter.test_format_with_imports: TableFormatter#test_format_with_imports().
  TestTypeScriptTableFormatter.test_format_with_exports: TableFormatter#test_format_with_exports().
  TestTypeScriptTableFormatter.test_format_module_info_statistics: TableFormatter#test_format_module_info_statistics().
  TestTypeScriptTableFormatter.test_format_different_file_types: TableFormatter#test_format_different_file_types().
  TestTypeScriptFormatterModifiers: FormatterModifiers#
  TestTypeScriptFormatterModifiers.test_format_modifiers_static: FormatterModifiers#test_format_modifiers_static().
  TestTypeScriptFormatterModifiers.test_format_modifiers_readonly: FormatterModifiers#test_format_modifiers_readonly().
  TestTypeScriptFormatterModifiers.test_format_modifiers_abstract: FormatterModifiers#test_format_modifiers_abstract().
  TestTypeScriptFormatterModifiers.test_format_modifiers_combined: FormatterModifiers#test_format_modifiers_combined().
  TestTypeScriptFormatterModifiers.test_format_modifiers_none: FormatterModifiers#test_format_modifiers_none().
  TestTypeScriptFormatterFullTableMethods: FormatterFullTableMethods#
  TestTypeScriptFormatterFullTableMethods.test_full_table_with_constructor: FormatterFullTableMethods#test_full_table_with_constructor().
  TestTypeScriptFormatterFullTableMethods.test_full_table_with_protected_method: FormatterFullTableMethods#test_full_table_with_protected_method().
  TestTypeScriptFormatterFullTableMethods.test_full_table_with_private_method: FormatterFullTableMethods#test_full_table_with_private_method().
---
# Module: [`tests/unit/formatters/test_typescript_formatter_core.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py)

## Classes
### `TestTypeScriptFormatterFullTableMethods`
- def: [`tests/unit/formatters/test_typescript_formatter_core.py:394`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L394)
- doc: Test constructor/protected/private method sections
- signature: `class TestTypeScriptFormatterFullTableMethods:`
- members:
  - `formatter(self)` — [`L398`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L398)
  - `test_full_table_with_constructor(self, formatter)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L401)
  - `test_full_table_with_private_method(self, formatter)` — [`L452`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L452)
  - `test_full_table_with_protected_method(self, formatter)` — [`L427`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L427)
- uses (calls/refs, reference-scoped): [`TypeScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/typescript_formatter.md#TypeScriptTableFormatter)

### `TestTypeScriptFormatterModifiers`
- def: [`tests/unit/formatters/test_typescript_formatter_core.py:362`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L362)
- doc: Test _format_modifiers method
- signature: `class TestTypeScriptFormatterModifiers:`
- members:
  - `formatter(self)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L366)
  - `test_format_modifiers_abstract(self, formatter)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L377)
  - `test_format_modifiers_combined(self, formatter)` — [`L381`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L381)
  - `test_format_modifiers_none(self, formatter)` — [`L389`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L389)
  - `test_format_modifiers_readonly(self, formatter)` — [`L373`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L373)
  - `test_format_modifiers_static(self, formatter)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L369)
- uses (calls/refs, reference-scoped): [`TypeScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/typescript_formatter.md#TypeScriptTableFormatter)

### `TestTypeScriptTableFormatter`
- def: [`tests/unit/formatters/test_typescript_formatter_core.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L16)
- doc: Test cases for TypeScriptTableFormatter class
- signature: `class TestTypeScriptTableFormatter:`
- members:
  - `formatter(self)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L20) — Create a TypeScriptTableFormatter instance for testing
  - `sample_data(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L25) — Sample TypeScript analysis data for testing
  - `test_format_classes_section(self, formatter, sample_data)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L232) — Test classes section formatting
  - `test_format_compact_table(self, sample_data)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L256) — Test compact table formatting
  - `test_format_csv(self, sample_data)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L268) — Test CSV formatting
  - `test_format_different_file_types(self, formatter)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L338) — Test formatting for different TypeScript file types
  - `test_format_element_details(self, formatter)` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L288) — Test element details formatting - method may not exist in new implementation
  - `test_format_element_details_minimal(self, formatter)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L293) — Test element details formatting with minimal data - method may not exist
  - `test_format_empty_data(self, formatter)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L298) — Test formatting with empty data
  - `test_format_enums_section(self, formatter, sample_data)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L224) — Test enums section formatting
  - `test_format_full_table(self, formatter, sample_data)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L166) — Test full table formatting
  - `test_format_full_table_declaration_file(self, formatter)` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L194) — Test full table formatting for declaration files
  - `test_format_full_table_tsx_file(self, formatter)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L179) — Test full table formatting for TSX files
  - `test_format_functions_section(self, formatter, sample_data)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L242) — Test functions section formatting
  - `test_format_interfaces_section(self, formatter, sample_data)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L209) — Test interfaces section formatting
  - `test_format_module_info_statistics(self, formatter, sample_data)` — [`L328`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L328) — Test output contains element information
  - `test_format_type_aliases_section(self, formatter, sample_data)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L216) — Test type aliases section formatting
  - `test_format_variables_section(self, formatter, sample_data)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L249) — Test variables section formatting
  - `test_format_with_exports(self, formatter, sample_data)` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L321) — Test formatting includes class content
  - `test_format_with_imports(self, formatter, sample_data)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L314) — Test formatting includes expected content
  - `test_get_element_type_name(self, formatter)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_typescript_formatter_core.py#L283) — Test element type name generation - method may not exist in new implementation
- uses (calls/refs, reference-scoped): [`TypeScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/typescript_formatter.md#TypeScriptTableFormatter), [`format`](../../../tree_sitter_analyzer/formatters/typescript_formatter.md#TypeScriptTableFormatter.format)

