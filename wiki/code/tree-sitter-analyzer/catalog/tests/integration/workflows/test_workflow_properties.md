---
title: 'Module: tests/integration/workflows/test_workflow_properties.py'
type: catalog
provenance: extracted
module: tests/integration/workflows/test_workflow_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.workflows.test_workflow_properties`/TestWorkflowProperties#
symbols:
  TestWorkflowProperties.test_property_1_test_matrix_standard: test_property_1_test_matrix_standard().
  TestWorkflowProperties.test_property_2_uv_usage: test_property_2_uv_usage().
  TestWorkflowProperties.test_property_3_quality_check_presence: test_property_3_quality_check_presence().
  TestWorkflowProperties.extract_quality_tools: extract_quality_tools().
  TestWorkflowProperties.extract_test_matrix: extract_test_matrix().
  TestWorkflowProperties.extract_install_commands: extract_install_commands().
  TestWorkflowProperties: ''
  TestWorkflowProperties.workflow_root: workflow_root().
  TestWorkflowProperties.all_workflows: all_workflows().
  TestWorkflowProperties.reusable_test_workflow: reusable_test_workflow().
  TestWorkflowProperties.reusable_quality_workflow: reusable_quality_workflow().
  TestWorkflowProperties.test_coverage_workflow: test_coverage_workflow().
  TestWorkflowProperties.test_property_4_python_version_standard: test_property_4_python_version_standard().
  TestWorkflowProperties.test_property_7_system_dependencies: test_property_7_system_dependencies().
  TestWorkflowProperties.test_property_11_reusable_workflow_structure: test_property_11_reusable_workflow_structure().
  TestWorkflowProperties.test_property_12_ci_xdist_worker_override: test_property_12_ci_xdist_worker_override().
  TestWorkflowProperties.test_property_13_ci_does_not_duplicate_feature_pr_runs: test_property_13_ci_does_not_duplicate_feature_pr_runs().
---
# Module: [`tests/integration/workflows/test_workflow_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/test_workflow_properties.py)

## Classes
### `TestWorkflowProperties`
- def: [`tests/integration/workflows/test_workflow_properties.py:32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/test_workflow_properties.py#L32)
- doc: Comprehensive property-based tests for workflow consistency.
- signature: `class TestWorkflowProperties:`
- members:
  - `all_workflows(self, workflow_root: Path)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/test_workflow_properties.py#L41) — Load all branch workflows.
  - `extract_install_commands(self, workflow: dict[str, Any])` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/test_workflow_properties.py#L113) — Extract dependency installation commands from workflow.
  - `extract_quality_tools(self, workflow: dict[str, Any])` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/test_workflow_properties.py#L132) — Extract quality check tools from workflow.
  - `extract_test_matrix(self, workflow: dict[str, Any])` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/test_workflow_properties.py#L83) — Extract test matrix configuration from workflow.
  - `reusable_quality_workflow(self, workflow_root: Path)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/test_workflow_properties.py#L70) — Load the reusable quality workflow.
  - `reusable_test_workflow(self, workflow_root: Path)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/test_workflow_properties.py#L63) — Load the reusable test workflow.
  - `test_coverage_workflow(self, workflow_root: Path)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/test_workflow_properties.py#L77) — Load the standalone coverage workflow.
  - `test_property_11_reusable_workflow_structure(self, reusable_test_workflow: dict[str, Any], reusable_quality_workflow: dict[str, Any])` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/test_workflow_properties.py#L189) — Property 11: Reusable workflows must have a clear job structure.
  - `test_property_12_ci_xdist_worker_override(self, reusable_test_workflow: dict[str, Any], test_coverage_workflow: dict[str, Any])` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/test_workflow_properties.py#L198) — Property 12: CI should not leave xdist auto at the 2-core runner floor.
  - `test_property_13_ci_does_not_duplicate_feature_pr_runs(self, all_workflows: dict[str, dict[str, Any]])` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/test_workflow_properties.py#L215) — Property 13: Feature PRs should use pull_request CI, not duplicate push CI.
  - `test_property_1_test_matrix_standard(self, reusable_test_workflow: dict[str, Any])` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/test_workflow_properties.py#L149) — Property 1: Test Matrix configuration must follow standards.
  - `test_property_2_uv_usage(self, reusable_test_workflow: dict[str, Any])` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/test_workflow_properties.py#L157) — Property 2: uv must be used for dependency management.
  - `test_property_3_quality_check_presence(self, reusable_test_workflow: dict[str, Any], reusable_quality_workflow: dict[str, Any])` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/test_workflow_properties.py#L162) — Property 3: Ruff, MyPy, and Bandit must be present.
  - `test_property_4_python_version_standard(self, reusable_quality_workflow: dict[str, Any])` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/test_workflow_properties.py#L174) — Property 4: Quality checks should use Python 3.11.
  - `test_property_7_system_dependencies(self, reusable_test_workflow: dict[str, Any])` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/test_workflow_properties.py#L182) — Property 7: System dependencies (fd, ripgrep) must be handled.
  - `workflow_root(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/workflows/test_workflow_properties.py#L36) — Get the workflow directory root.

