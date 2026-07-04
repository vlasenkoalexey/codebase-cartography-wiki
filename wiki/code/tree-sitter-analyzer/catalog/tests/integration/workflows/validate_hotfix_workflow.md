---
title: 'Module: tests/integration/workflows/validate_hotfix_workflow.py'
type: catalog
provenance: extracted
module: tests/integration/workflows/validate_hotfix_workflow.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.workflows.validate_hotfix_workflow`/
symbols:
  main: main().
  load_workflow: load_workflow().
  validate_test_job: validate_test_job().
  validate_deployment_job: validate_deployment_job().
  validate_pr_creation_job: validate_pr_creation_job().
  validate_workflow_triggers: validate_workflow_triggers().
  validate_consistency_with_release: validate_consistency_with_release().
---
# Module: [`tests/integration/workflows/validate_hotfix_workflow.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_hotfix_workflow.py)

## Functions
- `load_workflow(workflow_name: str)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_hotfix_workflow.py#L17) — Load a workflow YAML file.
- `main()` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_hotfix_workflow.py#L205) — Main validation function.
- `validate_consistency_with_release(hotfix_workflow: dict[str, Any], release_workflow: dict[str, Any])` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_hotfix_workflow.py#L169) — Validate that hotfix workflow matches release workflow structure.
- `validate_deployment_job(workflow: dict[str, Any])` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_hotfix_workflow.py#L59) — Validate that deployment job depends on test job.
- `validate_pr_creation_job(workflow: dict[str, Any])` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_hotfix_workflow.py#L103) — Validate that PR creation job depends on test and deploy.
- `validate_test_job(workflow: dict[str, Any])` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_hotfix_workflow.py#L33) — Validate that test job uses reusable workflow.
- `validate_workflow_triggers(workflow: dict[str, Any])` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/validate_hotfix_workflow.py#L144) — Validate that workflow triggers on hotfix branches.

