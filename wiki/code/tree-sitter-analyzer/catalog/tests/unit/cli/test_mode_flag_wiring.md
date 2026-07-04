---
title: 'Module: tests/unit/cli/test_mode_flag_wiring.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_mode_flag_wiring.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_mode_flag_wiring`/
symbols:
  test_mode_flag_alone_errors_naming_trigger: test_mode_flag_alone_errors_naming_trigger().
  test_every_mode_flag_token_exists_in_parser: test_every_mode_flag_token_exists_in_parser().
  _run_main: _run_main().
  _PAIR_IDS: _PAIR_IDS.
  _PAIRS: _PAIRS.
  _valid_mode_value: _valid_mode_value().
  _trigger_flag: _trigger_flag().
  test_table_has_expected_pair_count: test_table_has_expected_pair_count().
  test_watch_exempts_ast_cache_mode: test_watch_exempts_ast_cache_mode().
  test_ast_cache_with_mode_still_dispatches: test_ast_cache_with_mode_still_dispatches().
  test_class_hierarchy_with_mode_does_not_false_error: test_class_hierarchy_with_mode_does_not_false_error().
---
# Module: [`tests/unit/cli/test_mode_flag_wiring.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mode_flag_wiring.py)

## Functions
- `_run_main(argv: list[str])` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mode_flag_wiring.py#L29) — Run ``main()`` with the given argv, returning the SystemExit info.
- `_trigger_flag(trigger_dest: str)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mode_flag_wiring.py#L48) — Map a trigger dest (``ast_cache``) to its flag token (``--ast-cache``).
- `_valid_mode_value(mode_flag: str)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mode_flag_wiring.py#L37) — Return a valid value for ``mode_flag`` taken from its argparse choices.
- `test_ast_cache_with_mode_still_dispatches()` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mode_flag_wiring.py#L119) — ``--ast-cache --ast-cache-mode stats`` → reaches dispatch, exits 0.
- `test_class_hierarchy_with_mode_does_not_false_error(capsys)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mode_flag_wiring.py#L126) — ``--class-hierarchy --class-hierarchy-mode summary`` → no wiring error.
- `test_every_mode_flag_token_exists_in_parser()` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mode_flag_wiring.py#L85) — Every table entry's mode flag + derived trigger flag are real options.
- `test_mode_flag_alone_errors_naming_trigger(mode_flag: str, trigger_dest: str, _exempt: tuple[str, ...], capsys)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mode_flag_wiring.py#L59) — ``--X-mode <val>`` without ``--X`` → parser.error (exit 2) naming ``--X``.
- `test_table_has_expected_pair_count()` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mode_flag_wiring.py#L80) — The wiring table covers exactly the 22 discovered ``--X-mode`` pairs.
- `test_watch_exempts_ast_cache_mode()` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mode_flag_wiring.py#L104) — ``--watch --ast-cache-mode <val>`` (no ``--ast-cache``) must NOT error.

## Module values
- `_PAIRS` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mode_flag_wiring.py#L54)
- `_PAIR_IDS` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mode_flag_wiring.py#L55)

