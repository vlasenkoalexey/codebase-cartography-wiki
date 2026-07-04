---
title: 'Module: tree_sitter_analyzer/cli/commands/affected_command.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/affected_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.affected_command`/
symbols:
  run_affected: run_affected().
  _is_test_path: _is_test_path().
  _collect_forward_impact: _collect_forward_impact().
  _DEFAULT_TEST_GLOBS._DEFAULT_TEST_GLOBS: _DEFAULT_TEST_GLOBS._DEFAULT_TEST_GLOBS.
  _output_format: _output_format().
  _project_root: _project_root().
---
# Module: [`tree_sitter_analyzer/cli/commands/affected_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/affected_command.py)

## Functions
- `_collect_forward_impact(project_root: str, changed_files: list[str], output_error: Callable[[str], None])` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/affected_command.py#L115) — Run blast_radius once per changed file; return (union, invalid).
- `_is_test_path(rel_path: str, globs: Iterable[str])` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/affected_command.py#L86) — Return True when ``rel_path`` matches any of ``globs``.
- `_output_format(args: Any)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/affected_command.py#L108) — Resolve the output shape — text or JSON envelope.
- `_project_root(args: Any)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/affected_command.py#L104)
- `run_affected(args: Any, output_error: Callable[[str], None])` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/affected_command.py#L160) — Dispatch ``--affected`` → forward-impact union filtered to tests.

## Module values
- `_DEFAULT_TEST_GLOBS` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/affected_command.py#L55)

