---
title: 'Module: tree_sitter_analyzer/cli/commands/constraint_check_command.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/constraint_check_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.constraint_check_command`/
symbols:
  _run_and_persist: _run_and_persist().
  _evaluate_with_explicit_file: _evaluate_with_explicit_file().
  run_check_constraints: run_check_constraints().
  _exit_code_for: _exit_code_for().
  _filter_violations: _filter_violations().
  _compute_verdict: _compute_verdict().
  _failure_envelope: _failure_envelope().
  _run_tool: _run_tool().
  _load_explicit: _load_explicit().
  _format_response: _format_response().
  _violations_ddl: _violations_ddl().
  _resolve_output_format: _resolve_output_format().
  _print_result: _print_result().
  get_default_project_root: get_default_project_root().
  _EXIT_UNSAFE: _EXIT_UNSAFE.
  _SEVERITY_ORDER._SEVERITY_ORDER: _SEVERITY_ORDER._SEVERITY_ORDER.
  _EXIT_CAUTION: _EXIT_CAUTION.
  _EXIT_SAFE: _EXIT_SAFE.
  _BLOCKING_SEVERITIES._BLOCKING_SEVERITIES: _BLOCKING_SEVERITIES._BLOCKING_SEVERITIES.
  _WARNING_SEVERITIES._WARNING_SEVERITIES: _WARNING_SEVERITIES._WARNING_SEVERITIES.
---
# Module: [`tree_sitter_analyzer/cli/commands/constraint_check_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py)

## Functions
- `_compute_verdict(rows: list[dict[str, Any]])` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L277) — Map (filtered) violations to the canonical verdict.
- `_evaluate_with_explicit_file(*, project_root: str, constraint_file: str, severity_min: str, path_filter: str, output_format: str)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L105) — Evaluate against an explicit constraint file (CLI-only override).
- `_exit_code_for(result: dict[str, Any])` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L345) — Map verdict to shell exit code.
- `_failure_envelope(message: str, output_format: str)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L312) — Build a CAUTION-verdict failure response that obeys the envelope.
- `_filter_violations(violations: list[Any], *, path_filter: str, min_severity_rank: int)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L247) — Apply severity floor + path-glob filters; return dict rows.
- `_format_response(payload: dict[str, Any], output_format: str)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L305) — Apply TOON formatting when requested, identical to MCP tool helper.
- `_load_explicit(config_path: Path)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L172) — Load constraints from an explicit file by reusing ``load_constraints``.
- `_print_result(result: dict[str, Any], output_format: str)` — [`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L337) — Write the response to stdout in the requested format.
- `_resolve_output_format(args: Any)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L326) — Return ``json`` or ``toon`` based on argparse-visible format flags.
- `_run_and_persist(db_path: Path, constraints: list[Any])` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L195) — Run evaluator + persist violations (mirrors the MCP tool's path).
- `_run_tool(project_root: str, severity_min: str, path_filter: str, output_format: str)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L88) — Await the MCP ConstraintCheckTool with CLI-supplied arguments.
- `_violations_ddl()` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L288) — Self-healing DDL — mirrors constraint_check_tool._violations_ddl.
- `get_default_project_root(args: Any)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L357) — Return ``--project-root`` if set, else CWD.
- `run_check_constraints(args: Any, project_root: str)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L41) — Run the constraint check and print the verdict to stdout.

## Module values
- `_BLOCKING_SEVERITIES` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L29)
- `_EXIT_CAUTION` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L37)
- `_EXIT_SAFE` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L38)
- `_EXIT_UNSAFE` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L36)
- `_SEVERITY_ORDER` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L28)
- `_WARNING_SEVERITIES` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/constraint_check_command.py#L30)

