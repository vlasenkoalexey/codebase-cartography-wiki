---
title: 'Module: tree_sitter_analyzer/cli/agent_workflow.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/agent_workflow.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.agent_workflow`/
symbols:
  build_agent_workflow_pack: build_agent_workflow_pack().
  _build_steps: _build_steps().
  _shell_safe_path: _shell_safe_path().
  _build_agent_summary: _build_agent_summary().
  _build_sprint_contract: _build_sprint_contract().
  PHASE_ROUTING.PHASE_ROUTING: PHASE_ROUTING.PHASE_ROUTING.
  _build_evaluator_checks: _build_evaluator_checks().
  _build_next_phase: _build_next_phase().
  _build_transition_signal: _build_transition_signal().
  _build_step_handoffs: _build_step_handoffs().
  _build_phase_routing: _build_phase_routing().
  _trace_step: _trace_step().
  _scoped_change_impact_command: _scoped_change_impact_command().
  PHASE_ORDER: PHASE_ORDER.
  _check_target_path: _check_target_path().
  _current_phase: _current_phase().
  _step_for_phase: _step_for_phase().
  _set_step: _set_step().
  _map_step: _map_step().
  _analyze_step: _analyze_step().
  _retrieve_step: _retrieve_step().
  _build_queue_boundary_commands: _build_queue_boundary_commands().
  _build_toon_content: _build_toon_content().
  _SHELL_SAFE_CHARS._SHELL_SAFE_CHARS: _SHELL_SAFE_CHARS._SHELL_SAFE_CHARS.
---
# Module: [`tree_sitter_analyzer/cli/agent_workflow.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py)

## Functions
- `_analyze_step(target: str)` — [`L255`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L255)
- `_build_agent_summary(target_path: str | None, steps: list[dict[str, Any]], queue_boundary: list[str], current_phase: str, recommended_commands: list[str])` — [`L317`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L317) — Build the compact decision surface for the workflow pack.
- `_build_evaluator_checks(target_path: str | None, queue_boundary: list[str])` — [`L393`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L393) — Build evaluator checks that prevent one-shot and context-regression failures.
- `_build_next_phase(current_phase: str)` — [`L210`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L210) — Return the expected next phase for a queue item.
- `_build_phase_routing(steps: list[dict[str, Any]])` — [`L189`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L189) — Build route metadata in the same order as command pack steps.
- `_build_queue_boundary_commands()` — [`L310`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L310)
- `_build_sprint_contract(target_path: str | None, current_phase: str, current_step: dict[str, Any], steps: list[dict[str, Any]], queue_boundary: list[str])` — [`L363`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L363) — Build a compact evaluator contract for one queue item.
- `_build_step_handoffs(steps: list[dict[str, Any]])` — [`L160`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L160) — Attach handoff condition metadata to each step.
- `_build_steps(target: str)` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L147) — Build all SMART workflow steps.
- `_build_toon_content(result: dict[str, Any])` — [`L454`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L454) — Build a compact text representation for --format toon.
- `_build_transition_signal(current_phase: str)` — [`L218`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L218) — Return a compact reason to move out of the current phase.
- `_check_target_path(project_root: str, target_path: str)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L45) — Return an error message if ``target_path`` is invalid, else ``None``.
- `_current_phase(target_path: str | None)` — [`L176`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L176) — Return the phase an agent should start from for the current request.
- `_map_step()` — [`L241`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L241)
- `_retrieve_step(target: str)` — [`L279`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L279)
- `_scoped_change_impact_command(target: str)` — [`L421`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L421) — Build the scoped trace command that also emits queue_ledger.
- `_set_step()` — [`L226`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L226)
- `_shell_safe_path(path: str | None)` — [`L434`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L434) — Return a shell-safe token for user-provided file paths.
- `_step_for_phase(steps: list[dict[str, Any]], phase: str)` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L181) — Return the workflow step matching the requested phase.
- `_trace_step(target: str)` — [`L294`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L294)
- `build_agent_workflow_pack(project_root: str, target_path: str | None = None)` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L72) — Build a SMART workflow command pack for agents and humans.

## Module values
- `PHASE_ORDER` — [`L8`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L8)
- `PHASE_ROUTING` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L11)
- `_SHELL_SAFE_CHARS` — [`L429`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_workflow.py#L429)

