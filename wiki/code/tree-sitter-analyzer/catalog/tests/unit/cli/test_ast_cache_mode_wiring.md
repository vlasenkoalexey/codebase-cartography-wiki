---
title: 'Module: tests/unit/cli/test_ast_cache_mode_wiring.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_ast_cache_mode_wiring.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_ast_cache_mode_wiring`/
symbols:
  _run_main: _run_main().
  test_ast_cache_mode_alone_errors_naming_ast_cache: test_ast_cache_mode_alone_errors_naming_ast_cache().
  test_ast_cache_with_mode_still_dispatches: test_ast_cache_with_mode_still_dispatches().
  test_bare_ast_cache_defaults_to_stats: test_bare_ast_cache_defaults_to_stats().
---
# Module: [`tests/unit/cli/test_ast_cache_mode_wiring.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_ast_cache_mode_wiring.py)

## Functions
- `_run_main(argv: list[str])` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_ast_cache_mode_wiring.py#L21) — Run ``main()`` with the given argv, returning the SystemExit info.
- `test_ast_cache_mode_alone_errors_naming_ast_cache(capsys)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_ast_cache_mode_wiring.py#L29) — ``--ast-cache-mode stats`` without ``--ast-cache`` → parser.error (exit 2).
- `test_ast_cache_with_mode_still_dispatches()` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_ast_cache_mode_wiring.py#L44) — ``--ast-cache --ast-cache-mode stats`` → reaches the AST cache dispatch.
- `test_bare_ast_cache_defaults_to_stats()` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_ast_cache_mode_wiring.py#L58) — Bare ``--ast-cache`` (no mode) → still defaults to stats and dispatches.

