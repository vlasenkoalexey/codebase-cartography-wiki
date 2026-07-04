---
title: 'Module: tests/unit/formatters/test_cx_column_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_cx_column_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_cx_column_coverage`/
symbols:
  TestGoFormatterCxColumn.test_functions_header_has_cx_column: TestGoFormatterCxColumn#test_functions_header_has_cx_column().
  TestGoFormatterCxColumn.test_function_row_cx_value_1: TestGoFormatterCxColumn#test_function_row_cx_value_1().
  TestGoFormatterCxColumn.test_function_row_cx_value_5: TestGoFormatterCxColumn#test_function_row_cx_value_5().
  TestGoFormatterCxColumn.test_no_cx_column_absent_from_old_go_output: TestGoFormatterCxColumn#test_no_cx_column_absent_from_old_go_output().
  TestBashFormatterCxColumn.test_functions_header_has_cx_column: TestBashFormatterCxColumn#test_functions_header_has_cx_column().
  TestBashFormatterCxColumn.test_function_row_cx_value_1: TestBashFormatterCxColumn#test_function_row_cx_value_1().
  TestBashFormatterCxColumn.test_function_row_cx_value_4: TestBashFormatterCxColumn#test_function_row_cx_value_4().
  TestBashFormatterCxColumn.test_compact_functions_header_has_cx_column: TestBashFormatterCxColumn#test_compact_functions_header_has_cx_column().
  TestBashFormatterCxColumn.test_compact_function_row_cx_value_2: TestBashFormatterCxColumn#test_compact_function_row_cx_value_2().
  TestBashFormatterCxColumn.test_bash_formatter_registered: TestBashFormatterCxColumn#test_bash_formatter_registered().
  TestBashFormatterCxColumn.test_sh_alias_registered: TestBashFormatterCxColumn#test_sh_alias_registered().
  TestBashFormatterCxColumn.test_bash_section_header_present: TestBashFormatterCxColumn#test_bash_section_header_present().
  TestBashFormatterCxColumn.test_old_legacy_columns_absent: TestBashFormatterCxColumn#test_old_legacy_columns_absent().
  _bash_data_with_func: _bash_data_with_func().
  TestGoFormatterCxColumn.test_methods_header_has_cx_column: TestGoFormatterCxColumn#test_methods_header_has_cx_column().
  TestGoFormatterCxColumn.test_method_row_cx_value_3: TestGoFormatterCxColumn#test_method_row_cx_value_3().
  _go_data_with_func: _go_data_with_func().
  TestGoFormatterCxColumn: TestGoFormatterCxColumn#
  TestBashFormatterCxColumn: TestBashFormatterCxColumn#
---
# Module: [`tests/unit/formatters/test_cx_column_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py)

## Classes
### `TestBashFormatterCxColumn`
- def: [`tests/unit/formatters/test_cx_column_coverage.py:149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py#L149)
- doc: Bash full-table must include Cx column with exact complexity value.
- signature: `class TestBashFormatterCxColumn:`
- members:
  - `test_bash_formatter_registered(self)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py#L181) — BashTableFormatter must be reachable via FormatterRegistry.
  - `test_bash_section_header_present(self)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py#L195) — Full table must include a '## Functions' section.
  - `test_compact_function_row_cx_value_2(self)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py#L175) — Compact Bash row includes exact complexity 2.
  - `test_compact_functions_header_has_cx_column(self)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py#L169) — Compact Bash table also includes Cx column.
  - `test_function_row_cx_value_1(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py#L157) — Simple bash function → complexity_score == 1 → renders '| 1 |'.
  - `test_function_row_cx_value_4(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py#L163) — Bash function with complexity 4 → renders '| 4 |'.
  - `test_functions_header_has_cx_column(self)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py#L152)
  - `test_old_legacy_columns_absent(self)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py#L201) — OLD legacy columns (Name | Return Type | Parameters | Access | Line) must NOT appear.
  - `test_sh_alias_registered(self)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py#L188) — 'sh' language alias must also resolve to BashTableFormatter.
- uses (calls/refs, reference-scoped): [`FormatterRegistry`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry), [`get_formatter_for_language`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry.get_formatter_for_language), [`BashTableFormatter`](../../../tree_sitter_analyzer/formatters/bash_formatter.md#BashTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/formatters/bash_formatter.md#BashTableFormatter.format_structure)  (1 test-only)

### `TestGoFormatterCxColumn`
- def: [`tests/unit/formatters/test_cx_column_coverage.py:64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py#L64)
- doc: Go full-table must include Cx column with exact complexity value.
- signature: `class TestGoFormatterCxColumn:`
- members:
  - `test_function_row_cx_value_1(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py#L72) — Trivial function → complexity_score == 1 → renders '| 1 |' in row.
  - `test_function_row_cx_value_5(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py#L79) — Function with complexity 5 → renders '| 5 |'.
  - `test_functions_header_has_cx_column(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py#L67)
  - `test_method_row_cx_value_3(self)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py#L111) — Go method row includes exact complexity.
  - `test_methods_header_has_cx_column(self)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py#L85) — Go method table (receiver present) must also have Cx column.
  - `test_no_cx_column_absent_from_old_go_output(self)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py#L137) — Negative: the OLD 5-column header should NOT appear anymore.
- uses (calls/refs, reference-scoped): [`GoTableFormatter`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter.format_structure)  (1 test-only)

## Functions
- `_bash_data_with_func(complexity: int)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py#L38) — Minimal Bash structure dict with a single function at known complexity.
- `_go_data_with_func(complexity: int)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cx_column_coverage.py#L16) — Minimal Go structure dict with a single function at known complexity.

