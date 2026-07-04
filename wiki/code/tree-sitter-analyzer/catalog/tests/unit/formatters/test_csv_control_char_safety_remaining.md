---
title: 'Module: tests/unit/formatters/test_csv_control_char_safety_remaining.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_csv_control_char_safety_remaining.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_csv_control_char_safety_remaining`/
symbols:
  _base_csv: _base_csv().
  _legacy_csv: _legacy_csv().
  test_base_formatter_handles_control_chars: test_base_formatter_handles_control_chars().
  test_base_formatter_output_is_readable_with_cr: test_base_formatter_output_is_readable_with_cr().
  test_legacy_csv_handles_control_chars: test_legacy_csv_handles_control_chars().
  test_legacy_csv_output_is_readable_with_cr: test_legacy_csv_output_is_readable_with_cr().
  test_base_formatter_preserves_backslashes: test_base_formatter_preserves_backslashes().
  test_base_formatter_preserves_regex_backslashes: test_base_formatter_preserves_regex_backslashes().
  test_legacy_csv_preserves_backslashes: test_legacy_csv_preserves_backslashes().
  test_legacy_csv_preserves_regex_backslashes: test_legacy_csv_preserves_regex_backslashes().
  CONTROL_NAMES: CONTROL_NAMES.
  CR_NAMES: CR_NAMES.
---
# Module: [`tests/unit/formatters/test_csv_control_char_safety_remaining.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety_remaining.py)

## Functions
- `_base_csv(name: str)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety_remaining.py#L37) — Run ``name`` through the base_formatter CSV path (method + field).
- `_legacy_csv(name: str)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety_remaining.py#L62) — Run ``name`` through the legacy ``--table csv`` path (class/method/field).
- `test_base_formatter_handles_control_chars(name: str)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety_remaining.py#L99) — base_formatter CSV must serialize a control-char name without raising.
- `test_base_formatter_output_is_readable_with_cr(name: str)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety_remaining.py#L107) — base_formatter CSV must round-trip through csv.reader for CR-laden names.
- `test_base_formatter_preserves_backslashes()` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety_remaining.py#L115) — Literal backslashes must NOT be doubled (the escapechar regression).
- `test_base_formatter_preserves_regex_backslashes()` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety_remaining.py#L122) — A regex-like name keeps its backslashes intact.
- `test_legacy_csv_handles_control_chars(name: str)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety_remaining.py#L133) — legacy CSV must serialize a control-char name without raising.
- `test_legacy_csv_output_is_readable_with_cr(name: str)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety_remaining.py#L141) — legacy CSV must round-trip through csv.reader for CR-laden names.
- `test_legacy_csv_preserves_backslashes()` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety_remaining.py#L149) — Literal backslashes must NOT be doubled in the legacy path.
- `test_legacy_csv_preserves_regex_backslashes()` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety_remaining.py#L156) — A regex-like name keeps its backslashes intact in the legacy path.

## Module values
- `CONTROL_NAMES` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety_remaining.py#L32)
- `CR_NAMES` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_csv_control_char_safety_remaining.py#L34)

