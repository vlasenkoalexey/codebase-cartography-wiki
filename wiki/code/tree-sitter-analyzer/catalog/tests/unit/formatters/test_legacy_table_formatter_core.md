---
title: 'Module: tests/unit/formatters/test_legacy_table_formatter_core.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_legacy_table_formatter_core.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_legacy_table_formatter_core`/Test
symbols:
  TestLegacyTableFormatterBasic.test_default_initialization: LegacyTableFormatterBasic#test_default_initialization().
  TestLegacyTableFormatterBasic.test_custom_initialization: LegacyTableFormatterBasic#test_custom_initialization().
  TestLegacyTableFormatterBasic.test_invalid_format_type_raises_error: LegacyTableFormatterBasic#test_invalid_format_type_raises_error().
  TestFullTableFormat.test_format_empty_structure: FullTableFormat#test_format_empty_structure().
  TestFullTableFormat.test_format_single_class: FullTableFormat#test_format_single_class().
  TestFullTableFormat.test_format_class_with_extends: FullTableFormat#test_format_class_with_extends().
  TestFullTableFormat.test_format_class_with_implements: FullTableFormat#test_format_class_with_implements().
  TestFullTableFormat.test_format_with_imports: FullTableFormat#test_format_with_imports().
  TestFullTableFormat.test_format_with_methods: FullTableFormat#test_format_with_methods().
  TestFullTableFormat.test_format_with_constructor: FullTableFormat#test_format_with_constructor().
  TestFullTableFormat.test_format_with_fields: FullTableFormat#test_format_with_fields().
  TestFullTableFormat.test_format_static_final_fields: FullTableFormat#test_format_static_final_fields().
  TestMultipleClassesFormat.test_format_multiple_classes: MultipleClassesFormat#test_format_multiple_classes().
  TestMultipleClassesFormat.test_format_nested_classes: MultipleClassesFormat#test_format_nested_classes().
  TestCompactTableFormat.test_compact_format_empty: CompactTableFormat#test_compact_format_empty().
  TestCompactTableFormat.test_compact_format_basic: CompactTableFormat#test_compact_format_basic().
  TestCompactTableFormat.test_compact_format_methods_table: CompactTableFormat#test_compact_format_methods_table().
  TestCompactTableFormat.test_compact_format_fields_table: CompactTableFormat#test_compact_format_fields_table().
  TestCSVFormat.test_csv_format_header: CSVFormat#test_csv_format_header().
  TestCSVFormat.test_csv_format_class_row: CSVFormat#test_csv_format_class_row().
  TestCSVFormat.test_csv_format_method_row: CSVFormat#test_csv_format_method_row().
  TestCSVFormat.test_csv_format_constructor_row: CSVFormat#test_csv_format_constructor_row().
  TestCSVFormat.test_csv_format_parameters: CSVFormat#test_csv_format_parameters().
  TestCSVFormat.test_csv_format_string_parameters: CSVFormat#test_csv_format_string_parameters().
  TestCSVFormat.test_csv_format_static_final: CSVFormat#test_csv_format_static_final().
  TestFullTableFormat.formatter: FullTableFormat#formatter().
  TestMultipleClassesFormat.formatter: MultipleClassesFormat#formatter().
  TestCompactTableFormat.formatter: CompactTableFormat#formatter().
  TestCSVFormat.formatter: CSVFormat#formatter().
  TestLegacyTableFormatterBasic: LegacyTableFormatterBasic#
  TestFullTableFormat: FullTableFormat#
  TestMultipleClassesFormat: MultipleClassesFormat#
  TestCompactTableFormat: CompactTableFormat#
  TestCSVFormat: CSVFormat#
---
# Module: [`tests/unit/formatters/test_legacy_table_formatter_core.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py)

## Classes
### `TestCSVFormat`
- def: [`tests/unit/formatters/test_legacy_table_formatter_core.py:401`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L401)
- signature: `class TestCSVFormat:`
- members:
  - `formatter(self)` — [`L403`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L403)
  - `test_csv_format_class_row(self, formatter: LegacyTableFormatter)` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L418)
  - `test_csv_format_constructor_row(self, formatter: LegacyTableFormatter)` — [`L463`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L463)
  - `test_csv_format_header(self, formatter: LegacyTableFormatter)` — [`L406`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L406)
  - `test_csv_format_method_row(self, formatter: LegacyTableFormatter)` — [`L439`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L439)
  - `test_csv_format_parameters(self, formatter: LegacyTableFormatter)` — [`L484`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L484)
  - `test_csv_format_static_final(self, formatter: LegacyTableFormatter)` — [`L525`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L525)
  - `test_csv_format_string_parameters(self, formatter: LegacyTableFormatter)` — [`L505`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L505)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

### `TestCompactTableFormat`
- def: [`tests/unit/formatters/test_legacy_table_formatter_core.py:314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L314)
- signature: `class TestCompactTableFormat:`
- members:
  - `formatter(self)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L316)
  - `test_compact_format_basic(self, formatter: LegacyTableFormatter)` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L327)
  - `test_compact_format_empty(self, formatter: LegacyTableFormatter)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L319)
  - `test_compact_format_fields_table(self, formatter: LegacyTableFormatter)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L383)
  - `test_compact_format_methods_table(self, formatter: LegacyTableFormatter)` — [`L364`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L364)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

### `TestFullTableFormat`
- def: [`tests/unit/formatters/test_legacy_table_formatter_core.py:45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L45)
- signature: `class TestFullTableFormat:`
- members:
  - `formatter(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L47)
  - `test_format_class_with_extends(self, formatter: LegacyTableFormatter)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L75)
  - `test_format_class_with_implements(self, formatter: LegacyTableFormatter)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L91)
  - `test_format_empty_structure(self, formatter: LegacyTableFormatter)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L50)
  - `test_format_single_class(self, formatter: LegacyTableFormatter)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L56)
  - `test_format_static_final_fields(self, formatter: LegacyTableFormatter)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L196)
  - `test_format_with_constructor(self, formatter: LegacyTableFormatter)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L152)
  - `test_format_with_fields(self, formatter: LegacyTableFormatter)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L170)
  - `test_format_with_imports(self, formatter: LegacyTableFormatter)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L109)
  - `test_format_with_methods(self, formatter: LegacyTableFormatter)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L124)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

### `TestLegacyTableFormatterBasic`
- def: [`tests/unit/formatters/test_legacy_table_formatter_core.py:24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L24)
- signature: `class TestLegacyTableFormatterBasic:`
- members:
  - `test_custom_initialization(self)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L31)
  - `test_default_initialization(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L25)
  - `test_invalid_format_type_raises_error(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L39)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure), [`format_type`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_type), [`include_javadoc`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.include_javadoc), [`language`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.language)

### `TestMultipleClassesFormat`
- def: [`tests/unit/formatters/test_legacy_table_formatter_core.py:221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L221)
- signature: `class TestMultipleClassesFormat:`
- members:
  - `formatter(self)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L223)
  - `test_format_multiple_classes(self, formatter: LegacyTableFormatter)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L226)
  - `test_format_nested_classes(self, formatter: LegacyTableFormatter)` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_core.py#L277)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

