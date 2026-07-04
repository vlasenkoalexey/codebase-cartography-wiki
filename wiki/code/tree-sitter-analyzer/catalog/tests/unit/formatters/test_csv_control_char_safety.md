---
title: 'Module: tests/unit/formatters/test_csv_control_char_safety.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_csv_control_char_safety.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_csv_control_char_safety`/
symbols:
  test_csv_formatter_is_idempotent_on_control_chars: test_csv_formatter_is_idempotent_on_control_chars().
  test_csv_formatter_handles_control_chars: test_csv_formatter_handles_control_chars().
  test_csv_formatter_preserves_backslashes: test_csv_formatter_preserves_backslashes().
  test_csv_formatter_output_is_readable_with_cr: test_csv_formatter_output_is_readable_with_cr().
  test_html_csv_helper_handles_control_chars: test_html_csv_helper_handles_control_chars().
  CONTROL_NAMES: CONTROL_NAMES.
  test_markdown_csv_output_handles_control_chars: test_markdown_csv_output_handles_control_chars().
  test_csv_safe_cell_strips_controls_keeps_tab_newline: test_csv_safe_cell_strips_controls_keeps_tab_newline().
  test_csv_safe_row_only_touches_string_cells: test_csv_safe_row_only_touches_string_cells().
---
# Module: [`tests/unit/formatters/test_csv_control_char_safety.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety.py)

## Functions
- `test_csv_formatter_handles_control_chars(name: str)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety.py#L37) — CsvFormatter must serialize a control-char name without raising.
- `test_csv_formatter_is_idempotent_on_control_chars(name: str)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety.py#L52) — Idempotency must hold for control-char input (the property that flaked).
- `test_csv_formatter_output_is_readable_with_cr(name: str)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety.py#L130) — CSV output must round-trip through csv.reader even for CR-laden names.
- `test_csv_formatter_preserves_backslashes()` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety.py#L96) — Literal backslashes (Windows paths, regex) must NOT be doubled.
- `test_csv_safe_cell_strips_controls_keeps_tab_newline()` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety.py#L114) — The sanitizer removes C0/DEL controls + bare CR, keeps tab and LF.
- `test_csv_safe_row_only_touches_string_cells()` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety.py#L153) — Numeric cells keep their type so csv.writer formats them normally.
- `test_html_csv_helper_handles_control_chars()` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety.py#L65) — format_html_csv must not raise on a control-char element name.
- `test_markdown_csv_output_handles_control_chars()` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety.py#L79) — format_csv_output must not raise on a control-char text field.

## Module values
- `CONTROL_NAMES` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety.py#L33)

