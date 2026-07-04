---
title: 'Module: tests/integration/workflows/validate_release_workflow.py'
type: catalog
provenance: extracted
module: tests/integration/workflows/validate_release_workflow.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.workflows.validate_release_workflow`/
symbols:
  ReleaseWorkflowValidator.validate: ReleaseWorkflowValidator#validate().
  ReleaseWorkflowValidator.errors: ReleaseWorkflowValidator#errors.
  ReleaseWorkflowValidator.validate_reusable_workflow_usage: ReleaseWorkflowValidator#validate_reusable_workflow_usage().
  ReleaseWorkflowValidator.successes: ReleaseWorkflowValidator#successes.
  ReleaseWorkflowValidator.validate_deployment_dependency: ReleaseWorkflowValidator#validate_deployment_dependency().
  ReleaseWorkflowValidator.validate_pypi_deployment: ReleaseWorkflowValidator#validate_pypi_deployment().
  ReleaseWorkflowValidator.validate_pr_creation: ReleaseWorkflowValidator#validate_pr_creation().
  ReleaseWorkflowValidator.validate_branch_triggers: ReleaseWorkflowValidator#validate_branch_triggers().
  main: main().
  ReleaseWorkflowValidator.load_workflow: ReleaseWorkflowValidator#load_workflow().
  ReleaseWorkflowValidator.warnings: ReleaseWorkflowValidator#warnings.
  ReleaseWorkflowValidator: ReleaseWorkflowValidator#
  ReleaseWorkflowValidator.workflow_root: ReleaseWorkflowValidator#workflow_root.
  ReleaseWorkflowValidator.__init__: ReleaseWorkflowValidator#__init__().
---
# Module: [`tests/integration/workflows/validate_release_workflow.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_release_workflow.py)

## Classes
### `ReleaseWorkflowValidator`
- def: [`tests/integration/workflows/validate_release_workflow.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_release_workflow.py#L17)
- doc: Validator for release workflow configuration.
- signature: `class ReleaseWorkflowValidator:`
- members:
  - `load_workflow(self, filename: str)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_release_workflow.py#L28) — Load a workflow YAML file.
  - `validate(self)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_release_workflow.py#L174) — Run all validations.
  - `validate_branch_triggers(self, workflow: dict[str, Any])` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_release_workflow.py#L159) — Validate workflow triggers on release branches.
  - `validate_deployment_dependency(self, workflow: dict[str, Any])` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_release_workflow.py#L61) — Validate that deployment depends on tests.
  - `validate_pr_creation(self, workflow: dict[str, Any])` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_release_workflow.py#L112) — Validate PR creation to main.
  - `validate_pypi_deployment(self, workflow: dict[str, Any])` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_release_workflow.py#L91) — Validate PyPI deployment configuration.
  - `validate_reusable_workflow_usage(self, workflow: dict[str, Any])` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_release_workflow.py#L38) — Validate that workflow uses reusable components.
  - `errors` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_release_workflow.py#L24)
  - `successes` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_release_workflow.py#L26)
  - `warnings` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_release_workflow.py#L25)
  - `workflow_root` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_release_workflow.py#L21)
- protocol/private: `__init__`[`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_release_workflow.py#L20)
- used by: (1 test-only callers)

## Functions
- `main()` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_release_workflow.py#L244) — Main entry point.

