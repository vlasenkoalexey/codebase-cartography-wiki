---
title: 'Module: tree_sitter_analyzer/cli/commands/_case_resolution.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/_case_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands._case_resolution`/
symbols:
  warn_on_duplicate_case: warn_on_duplicate_case().
  collect_case_args: collect_case_args().
  case_to_sensitive_bool: case_to_sensitive_bool().
  _CASE_FLAG: _CASE_FLAG.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/cli/commands/_case_resolution.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/_case_resolution.py)

## Functions
- `case_to_sensitive_bool(case: str | None)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/_case_resolution.py#L50) — Map the textual ``--case`` value to the canonical bool echo.
- `collect_case_args(argv: Iterable[str] | None = None)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/_case_resolution.py#L29) — Return every ``--case`` value seen on the command line, in order.
- `warn_on_duplicate_case(resolved: str | None, *, argv: Iterable[str] | None = None, stream: IO[str] | None = None)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/_case_resolution.py#L60) — Emit a stderr warning when ``--case`` is passed more than once.

## Module values
- `_CASE_FLAG` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/_case_resolution.py#L26)
- `__all__` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/_case_resolution.py#L83)

