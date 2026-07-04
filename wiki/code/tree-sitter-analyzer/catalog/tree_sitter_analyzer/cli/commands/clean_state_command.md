---
title: 'Module: tree_sitter_analyzer/cli/commands/clean_state_command.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/clean_state_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.clean_state_command`/
symbols:
  run_clean_state: run_clean_state().
  EPHEMERAL_STATE_PATHS.EPHEMERAL_STATE_PATHS: EPHEMERAL_STATE_PATHS.EPHEMERAL_STATE_PATHS.
  _sweep: _sweep().
  OutputErrorFn: OutputErrorFn.
  _build_json_payload: _build_json_payload().
  _remove_single: _remove_single().
---
# Module: [`tree_sitter_analyzer/cli/commands/clean_state_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/clean_state_command.py)

## Functions
- `_build_json_payload(summary: list[str], *, dry_run: bool)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/clean_state_command.py#L91) — Bucket the per-path status lines into a structured JSON envelope.
- `_remove_single(target: Path, rel: str, prefix_remove: str)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/clean_state_command.py#L142) — Best-effort removal of a single path. Returns the status line.
- `_sweep(root: Path, relative_paths: Iterable[str], *, dry_run: bool)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/clean_state_command.py#L120) — Remove each path under ``root``. Returns one status line per path.
- `run_clean_state(args: Any, output_error: OutputErrorFn)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/clean_state_command.py#L57) — Remove ephemeral state files. Returns exit code 0 on success.

## Module values
- `EPHEMERAL_STATE_PATHS` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/clean_state_command.py#L44)
- `OutputErrorFn` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/clean_state_command.py#L54)

