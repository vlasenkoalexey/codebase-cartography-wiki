---
title: 'Module: tests/unit/formatters/test_java_formatter_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_java_formatter_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_java_formatter_coverage`/TestJavaTableFormatterCoverage#
symbols:
  TestJavaTableFormatterCoverage.test_format_json_error: test_format_json_error().
  TestJavaTableFormatterCoverage.test_format_table_context_manager: test_format_table_context_manager().
  TestJavaTableFormatterCoverage.test_format_full_table_multiple_classes_with_package: test_format_full_table_multiple_classes_with_package().
  TestJavaTableFormatterCoverage.test_format_full_table_multiple_classes_no_package: test_format_full_table_multiple_classes_no_package().
  TestJavaTableFormatterCoverage.test_format_full_table_single_class_no_package: test_format_full_table_single_class_no_package().
  TestJavaTableFormatterCoverage.test_format_enum_details: test_format_enum_details().
  TestJavaTableFormatterCoverage.test_format_advanced_variations: test_format_advanced_variations().
  TestJavaTableFormatterCoverage.test_clean_csv_text: test_clean_csv_text().
  TestJavaTableFormatterCoverage.test_shorten_type_complex: test_shorten_type_complex().
  TestJavaTableFormatterCoverage.test_format_json_error.Unserializable: test_format_json_error().Unserializable#
  TestJavaTableFormatterCoverage: ''
---
# Module: [`tests/unit/formatters/test_java_formatter_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_coverage.py)

## Classes
### `TestJavaTableFormatterCoverage`
- def: [`tests/unit/formatters/test_java_formatter_coverage.py:4`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_coverage.py#L4)
- signature: `class TestJavaTableFormatterCoverage:`
- members:
  - `test_clean_csv_text(self)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_coverage.py#L204) — Test _clean_csv_text inherited method usage in Java formatter context
  - `test_format_advanced_variations(self)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_coverage.py#L172) — Test format_advanced with various outputs
  - `test_format_enum_details(self)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_coverage.py#L75) — Test formatting enum details including fields and methods within enum range
  - `test_format_full_table_multiple_classes_no_package(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_coverage.py#L49) — Test full table formatting with multiple classes without package
  - `test_format_full_table_multiple_classes_with_package(self)` — [`L5`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_coverage.py#L5) — Test full table formatting with multiple classes and package
  - `test_format_full_table_single_class_no_package(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_coverage.py#L64) — Test full table formatting single class no package
  - `test_format_json_error(self)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_coverage.py#L159) — Test JSON serialization error handling
  - `test_format_table_context_manager(self)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_coverage.py#L191) — Test format_table ensures format_type is restored
  - `test_shorten_type_complex(self)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_coverage.py#L121) — Test shortening of complex types
- uses (calls/refs, reference-scoped): [`JavaTableFormatter`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter), [`_format_full_table`](../../../tree_sitter_analyzer/formatters/_java_formatter_full_mixin.md#JavaTableFormatterFullMixin._format_full_table), [`format_type`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter.format_type), [`format_advanced`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter.format_advanced), [`_format_json`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter._format_json), [`_format_method_row`](../../../tree_sitter_analyzer/formatters/_java_formatter_class_mixin.md#JavaTableFormatterClassMixin._format_method_row), [`format_table`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter.format_table)  (1 test-only)

### `Unserializable`
- def: [`tests/unit/formatters/test_java_formatter_coverage.py:164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_coverage.py#L164)
- signature: `class Unserializable:`
- used by: (1 test-only callers)

