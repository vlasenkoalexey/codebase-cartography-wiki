---
title: 'Module: tests/unit/cli/test_table_command_format_override.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_table_command_format_override.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_table_command_format_override`/
symbols:
  _run: _run().
  FIXTURE: FIXTURE.
  TestTableOutputFormatOverride: TestTableOutputFormatOverride#
  TestTableOutputFormatOverride.test_table_full_default_is_markdown: TestTableOutputFormatOverride#test_table_full_default_is_markdown().
  TestTableOutputFormatOverride.test_table_full_with_output_format_toon_emits_toon: TestTableOutputFormatOverride#test_table_full_with_output_format_toon_emits_toon().
  TestTableOutputFormatOverride.test_table_full_with_output_format_json_emits_json: TestTableOutputFormatOverride#test_table_full_with_output_format_json_emits_json().
  TestTableOutputFormatOverride.test_table_full_with_short_format_alias_toon: TestTableOutputFormatOverride#test_table_full_with_short_format_alias_toon().
  TestTableOutputFormatOverride.test_toon_is_smaller_than_json_for_same_table_data: TestTableOutputFormatOverride#test_toon_is_smaller_than_json_for_same_table_data().
  TestTableOutputFormatOverride.test_explicit_table_toon_still_works: TestTableOutputFormatOverride#test_explicit_table_toon_still_works().
  PROJECT_ROOT: PROJECT_ROOT.
---
# Module: [`tests/unit/cli/test_table_command_format_override.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_format_override.py)

## Classes
### `TestTableOutputFormatOverride`
- def: [`tests/unit/cli/test_table_command_format_override.py:37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_format_override.py#L37)
- signature: `class TestTableOutputFormatOverride:`
- members:
  - `test_explicit_table_toon_still_works(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_format_override.py#L83) — Pre-DOG-3 path: --table=toon alone (no --output-format) still emits TOON.
  - `test_table_full_default_is_markdown(self)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_format_override.py#L38) — No --output-format flag = the documented markdown table layout.
  - `test_table_full_with_output_format_json_emits_json(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_format_override.py#L58)
  - `test_table_full_with_output_format_toon_emits_toon(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_format_override.py#L46) — DOG-3: --output-format=toon must beat --table=full's default.
  - `test_table_full_with_short_format_alias_toon(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_format_override.py#L65) — ``--format`` (alias) also overrides table layout to TOON.
  - `test_toon_is_smaller_than_json_for_same_table_data(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_format_override.py#L71) — The whole point of TOON: significantly fewer bytes than JSON.
- uses (calls/refs, reference-scoped): (2 test-only callers)

## Functions
- `_run(args: list[str])` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_format_override.py#L16) — Run the CLI in-tree and return stdout text.

## Module values
- `FIXTURE` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_format_override.py#L13)
- `PROJECT_ROOT` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_table_command_format_override.py#L12)

