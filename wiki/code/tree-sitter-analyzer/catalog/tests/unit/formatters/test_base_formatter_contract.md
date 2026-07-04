---
title: 'Module: tests/unit/formatters/test_base_formatter_contract.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_base_formatter_contract.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_base_formatter_contract`/
symbols:
  _FORMATTER_CLASSES._FORMATTER_CLASSES: _FORMATTER_CLASSES._FORMATTER_CLASSES.
  TestBaseFormatterContract.test_format_structure_returns_string: TestBaseFormatterContract#test_format_structure_returns_string().
  TestBaseFormatterContract.test_format_summary_returns_string: TestBaseFormatterContract#test_format_summary_returns_string().
  _make_formatter: _make_formatter().
  TestBaseFormatterContract: TestBaseFormatterContract#
  TestBaseFormatterContract.test_instantiates_with_full_format: TestBaseFormatterContract#test_instantiates_with_full_format().
  _IDS: _IDS.
  _CLASSES: _CLASSES.
  TestBaseFormatterContract.test_is_subclass_of_base_table_formatter: TestBaseFormatterContract#test_is_subclass_of_base_table_formatter().
  TestBaseFormatterContract.test_has_format_structure_method: TestBaseFormatterContract#test_has_format_structure_method().
  TestBaseFormatterContract.test_has_format_summary_method: TestBaseFormatterContract#test_has_format_summary_method().
  TestBaseFormatterContract.test_has_format_table_method: TestBaseFormatterContract#test_has_format_table_method().
  TestBaseFormatterContract.test_class_name_matches_module: TestBaseFormatterContract#test_class_name_matches_module().
  _MINIMAL_STRUCTURE_DATA: _MINIMAL_STRUCTURE_DATA.
  _MINIMAL_SUMMARY_DATA: _MINIMAL_SUMMARY_DATA.
---
# Module: [`tests/unit/formatters/test_base_formatter_contract.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_base_formatter_contract.py)

## Classes
### `TestBaseFormatterContract`
- def: [`tests/unit/formatters/test_base_formatter_contract.py:85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_base_formatter_contract.py#L85)
- doc: Every concrete BaseTableFormatter must satisfy these 8 invariants.
- signature: `class TestBaseFormatterContract:`
- members:
  - `test_class_name_matches_module(self, formatter_cls: type[BaseTableFormatter])` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_base_formatter_contract.py#L128)
  - `test_format_structure_returns_string(self, formatter_cls: type[BaseTableFormatter])` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_base_formatter_contract.py#L114)
  - `test_format_summary_returns_string(self, formatter_cls: type[BaseTableFormatter])` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_base_formatter_contract.py#L121)
  - `test_has_format_structure_method(self, formatter_cls: type[BaseTableFormatter])` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_base_formatter_contract.py#L99)
  - `test_has_format_summary_method(self, formatter_cls: type[BaseTableFormatter])` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_base_formatter_contract.py#L104)
  - `test_has_format_table_method(self, formatter_cls: type[BaseTableFormatter])` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_base_formatter_contract.py#L109)
  - `test_instantiates_with_full_format(self, formatter_cls: type[BaseTableFormatter])` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_base_formatter_contract.py#L88)
  - `test_is_subclass_of_base_table_formatter(self, formatter_cls: type[BaseTableFormatter])` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_base_formatter_contract.py#L94)
- uses (calls/refs, reference-scoped): [`format_structure`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_structure), [`BaseTableFormatter`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter), [`format_summary`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_summary)  (5 test-only)

## Functions
- `_make_formatter(cls: type[BaseTableFormatter])` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_base_formatter_contract.py#L77)

## Module values
- `_CLASSES` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_base_formatter_contract.py#L74)
- `_FORMATTER_CLASSES` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_base_formatter_contract.py#L54)
- `_IDS` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_base_formatter_contract.py#L73)
- `_MINIMAL_STRUCTURE_DATA` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_base_formatter_contract.py#L38)
- `_MINIMAL_SUMMARY_DATA` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_base_formatter_contract.py#L48)

