---
title: 'Module: tests/unit/formatters/test_java_formatter_advanced.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_java_formatter_advanced.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_java_formatter_advanced`/
symbols:
  _FMT: _FMT.
  _data: _data().
  TestFormatStructure.test_format_structure: TestFormatStructure#test_format_structure().
  TestFormatAdvanced.test_format_advanced_csv: TestFormatAdvanced#test_format_advanced_csv().
  TestFormatAdvanced.test_format_advanced_default: TestFormatAdvanced#test_format_advanced_default().
  TestJavaDocHandling.test_format_with_javadoc: TestJavaDocHandling#test_format_with_javadoc().
  TestPrivateMethods.test_format_private_methods: TestPrivateMethods#test_format_private_methods().
  TestPrivateMethods.test_format_mixed_visibility_methods: TestPrivateMethods#test_format_mixed_visibility_methods().
  TestCompactTableMultipleClasses.test_format_compact_multiple_classes_with_package: TestCompactTableMultipleClasses#test_format_compact_multiple_classes_with_package().
  TestCompactTableMultipleClasses.test_format_compact_multiple_classes_no_package: TestCompactTableMultipleClasses#test_format_compact_multiple_classes_no_package().
  TestCompactTableMultipleClasses.test_format_compact_single_class_no_package: TestCompactTableMultipleClasses#test_format_compact_single_class_no_package().
  TestEdgeCases.test_format_empty_data: TestEdgeCases#test_format_empty_data().
  TestEdgeCases.test_format_missing_package: TestEdgeCases#test_format_missing_package().
  TestEdgeCases.test_format_missing_statistics: TestEdgeCases#test_format_missing_statistics().
  TestEdgeCases.test_format_none_values: TestEdgeCases#test_format_none_values().
  _BASE_DATA._BASE_DATA: _BASE_DATA._BASE_DATA.
  _BASE_CLASS: _BASE_CLASS.
  TestFormatStructure: TestFormatStructure#
  TestFormatAdvanced: TestFormatAdvanced#
  TestJavaDocHandling: TestJavaDocHandling#
  TestPrivateMethods: TestPrivateMethods#
  TestCompactTableMultipleClasses: TestCompactTableMultipleClasses#
  TestEdgeCases: TestEdgeCases#
---
# Module: [`tests/unit/formatters/test_java_formatter_advanced.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py)

## Classes
### `TestCompactTableMultipleClasses`
- def: [`tests/unit/formatters/test_java_formatter_advanced.py:169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L169)
- doc: Test compact table formatting with multiple classes
- signature: `class TestCompactTableMultipleClasses:`
- members:
  - `test_format_compact_multiple_classes_no_package(self)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L195) — Test compact format with multiple classes without package
  - `test_format_compact_multiple_classes_with_package(self)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L172) — Test compact format with multiple classes and package
  - `test_format_compact_single_class_no_package(self)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L219) — Test compact format with single class without package
- uses (calls/refs, reference-scoped): [`_format_compact_table`](../../../tree_sitter_analyzer/formatters/_java_formatter_compact_mixin.md#JavaTableFormatterCompactMixin._format_compact_table)  (2 test-only)

### `TestEdgeCases`
- def: [`tests/unit/formatters/test_java_formatter_advanced.py:237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L237)
- doc: Test edge cases and error handling
- signature: `class TestEdgeCases:`
- members:
  - `test_format_empty_data(self)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L240) — Test formatting empty data
  - `test_format_missing_package(self)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L245) — Test formatting with missing package
  - `test_format_missing_statistics(self)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L251) — Test formatting with missing statistics
  - `test_format_none_values(self)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L258) — Test formatting with None values
- uses (calls/refs, reference-scoped): [`_format_full_table`](../../../tree_sitter_analyzer/formatters/_java_formatter_full_mixin.md#JavaTableFormatterFullMixin._format_full_table)  (2 test-only)

### `TestFormatAdvanced`
- def: [`tests/unit/formatters/test_java_formatter_advanced.py:46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L46)
- doc: Test format_advanced method
- signature: `class TestFormatAdvanced:`
- members:
  - `test_format_advanced_csv(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L49) — Test advanced formatting with CSV
  - `test_format_advanced_default(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L54) — Test advanced formatting with default format
- uses (calls/refs, reference-scoped): [`format_advanced`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter.format_advanced)  (2 test-only)

### `TestFormatStructure`
- def: [`tests/unit/formatters/test_java_formatter_advanced.py:36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L36)
- doc: Test format_structure method
- signature: `class TestFormatStructure:`
- members:
  - `test_format_structure(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L39) — Test structure formatting
- uses (calls/refs, reference-scoped): [`format_structure`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_structure)  (2 test-only)

### `TestJavaDocHandling`
- def: [`tests/unit/formatters/test_java_formatter_advanced.py:61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L61)
- doc: Test JavaDoc comment handling
- signature: `class TestJavaDocHandling:`
- members:
  - `test_format_with_javadoc(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L64) — Test formatting with JavaDoc comments
- uses (calls/refs, reference-scoped): [`_format_full_table`](../../../tree_sitter_analyzer/formatters/_java_formatter_full_mixin.md#JavaTableFormatterFullMixin._format_full_table)  (2 test-only)

### `TestPrivateMethods`
- def: [`tests/unit/formatters/test_java_formatter_advanced.py:95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L95)
- doc: Test private method formatting
- signature: `class TestPrivateMethods:`
- members:
  - `test_format_mixed_visibility_methods(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L127) — Test formatting class with both public and private methods
  - `test_format_private_methods(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L98) — Test formatting class with private methods
- uses (calls/refs, reference-scoped): [`_format_full_table`](../../../tree_sitter_analyzer/formatters/_java_formatter_full_mixin.md#JavaTableFormatterFullMixin._format_full_table)  (2 test-only)

## Functions
- `_data(**overrides: Any)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L31) — Return a copy of _BASE_DATA with top-level keys overridden.

## Module values
- `_BASE_CLASS` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L15)
- `_BASE_DATA` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L21)
- `_FMT` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_advanced.py#L13)

