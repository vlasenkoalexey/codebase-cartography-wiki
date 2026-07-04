---
title: 'Module: tests/integration/workflows/validate_ci_workflow.py'
type: catalog
provenance: extracted
module: tests/integration/workflows/validate_ci_workflow.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.workflows.validate_ci_workflow`/
symbols:
  CIWorkflowValidator.run_validation: CIWorkflowValidator#run_validation().
  CIWorkflowValidator.errors: CIWorkflowValidator#errors.
  CIWorkflowValidator.validate_uses_composite_setup_action: CIWorkflowValidator#validate_uses_composite_setup_action().
  CIWorkflowValidator.validate_triggers: CIWorkflowValidator#validate_triggers().
  main: main().
  CIWorkflowValidator.warnings: CIWorkflowValidator#warnings.
  CIWorkflowValidator.ci_workflow_path: CIWorkflowValidator#ci_workflow_path.
  CIWorkflowValidator.load_workflow: CIWorkflowValidator#load_workflow().
  CIWorkflowValidator.validate_uses_reusable_test_workflow: CIWorkflowValidator#validate_uses_reusable_test_workflow().
  CIWorkflowValidator.validate_no_deployment_logic: CIWorkflowValidator#validate_no_deployment_logic().
  CIWorkflowValidator.validate_ci_specific_jobs: CIWorkflowValidator#validate_ci_specific_jobs().
  CIWorkflowValidator.validate_all_extras_flag: CIWorkflowValidator#validate_all_extras_flag().
  CIWorkflowValidator: CIWorkflowValidator#
  CIWorkflowValidator.workflow_root: CIWorkflowValidator#workflow_root.
  CIWorkflowValidator.__init__: CIWorkflowValidator#__init__().
---
# Module: [`tests/integration/workflows/validate_ci_workflow.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_ci_workflow.py)

## Classes
### `CIWorkflowValidator`
- def: [`tests/integration/workflows/validate_ci_workflow.py:21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_ci_workflow.py#L21)
- doc: Validator for CI workflow structure and behavior.
- signature: `class CIWorkflowValidator:`
- members:
  - `load_workflow(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_ci_workflow.py#L32) — Load the CI workflow YAML.
  - `run_validation(self)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_ci_workflow.py#L224) — Run all validation checks.
  - `validate_all_extras_flag(self, workflow: dict[str, Any])` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_ci_workflow.py#L200) — Validate that all dependency installations use --all-extras flag.
  - `validate_ci_specific_jobs(self, workflow: dict[str, Any])` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_ci_workflow.py#L143) — Validate that CI workflow maintains CI-specific jobs.
  - `validate_no_deployment_logic(self, workflow: dict[str, Any])` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_ci_workflow.py#L67) — Validate that CI workflow has no deployment logic.
  - `validate_triggers(self, workflow: dict[str, Any])` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_ci_workflow.py#L160) — Validate that CI workflow has appropriate triggers.
  - `validate_uses_composite_setup_action(self, workflow: dict[str, Any])` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_ci_workflow.py#L112) — Validate that CI workflow uses composite setup-system action.
  - `validate_uses_reusable_test_workflow(self, workflow: dict[str, Any])` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_ci_workflow.py#L41) — Validate that CI workflow uses reusable test workflow.
  - `ci_workflow_path` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_ci_workflow.py#L28)
  - `errors` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_ci_workflow.py#L29)
  - `warnings` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_ci_workflow.py#L30)
  - `workflow_root` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_ci_workflow.py#L25)
- protocol/private: `__init__`[`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_ci_workflow.py#L24)
- used by: (1 test-only callers)

## Functions
- `main()` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_ci_workflow.py#L275) — Main entry point.

