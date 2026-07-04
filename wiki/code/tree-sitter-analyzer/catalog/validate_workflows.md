---
title: 'Module: validate_workflows.py'
type: catalog
provenance: extracted
module: validate_workflows.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 validate_workflows/
symbols:
  validate_workflow: validate_workflow().
  main: main().
  _report_workflow: _report_workflow().
  _report_action: _report_action().
  _validate_workflow_jobs: _validate_workflow_jobs().
  _validate_trigger_inputs: _validate_trigger_inputs().
  validate_action: validate_action().
---
# Module: [`validate_workflows.py`](../../../../raw/code/tree-sitter-analyzer/validate_workflows.py)

## Functions
- `_report_action(action_path: Path, label: str)` — [`L131`](../../../../raw/code/tree-sitter-analyzer/validate_workflows.py#L131) — Validate one action file, print status, and return True if valid.
- `_report_workflow(workflow_path: Path, workflow_name: str)` — [`L116`](../../../../raw/code/tree-sitter-analyzer/validate_workflows.py#L116) — Validate one workflow file, print status, and return True if valid.
- `_validate_trigger_inputs(on_config: dict)` — [`L32`](../../../../raw/code/tree-sitter-analyzer/validate_workflows.py#L32)
- `_validate_workflow_jobs(jobs: dict)` — [`L12`](../../../../raw/code/tree-sitter-analyzer/validate_workflows.py#L12)
- `main()` — [`L146`](../../../../raw/code/tree-sitter-analyzer/validate_workflows.py#L146) — Main validation function.
- `validate_action(action_path: Path)` — [`L82`](../../../../raw/code/tree-sitter-analyzer/validate_workflows.py#L82) — Validate a GitHub Actions composite action file.
- `validate_workflow(workflow_path: Path)` — [`L48`](../../../../raw/code/tree-sitter-analyzer/validate_workflows.py#L48) — Validate a GitHub Actions workflow file.

