---
title: 'Module: _verify_workflow_structure_helpers.py'
type: catalog
provenance: extracted
module: _verify_workflow_structure_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 _verify_workflow_structure_helpers/
symbols:
  reusable_test_errors: reusable_test_errors().
  reusable_quality_errors: reusable_quality_errors().
  _check_test_matrix_job: _check_test_matrix_job().
  composite_action_errors: composite_action_errors().
  load_yaml: load_yaml().
  workflow_path: workflow_path().
  print_result: print_result().
  _check_reusable_test_inputs: _check_reusable_test_inputs().
  _check_action_runs: _check_action_runs().
  _check_input_default_and_type: _check_input_default_and_type().
  _workflow_call: _workflow_call().
  _jobs: _jobs().
  _check_all_extras_step: _check_all_extras_step().
  _check_reusable_test_secrets: _check_reusable_test_secrets().
  _check_test_matrix: _check_test_matrix().
  _check_pr_test_matrix: _check_pr_test_matrix().
  _check_optional_python_version_input: _check_optional_python_version_input().
  _check_quality_jobs: _check_quality_jobs().
  _check_action_inputs: _check_action_inputs().
  _check_os_specific_steps: _check_os_specific_steps().
---
# Module: [`_verify_workflow_structure_helpers.py`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py)

## Functions
- `_check_action_inputs(content: dict[Any, Any], errors: list[str])` — [`L255`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L255)
- `_check_action_runs(content: dict[Any, Any], errors: list[str])` — [`L268`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L268)
- `_check_all_extras_step(test_job: dict[str, Any], errors: list[str])` — [`L213`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L213)
- `_check_input_default_and_type(inputs: dict[str, Any], name: str, expected_default: Any, expected_type: str, errors: list[str])` — [`L114`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L114)
- `_check_optional_python_version_input(workflow_call: dict[str, Any], errors: list[str])` — [`L227`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L227)
- `_check_os_specific_steps(steps: list[dict[str, Any]], errors: list[str])` — [`L285`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L285)
- `_check_pr_test_matrix(test_job: dict[str, Any], errors: list[str])` — [`L186`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L186)
- `_check_quality_jobs(jobs: dict[str, Any], errors: list[str])` — [`L239`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L239)
- `_check_reusable_test_inputs(workflow_call: dict[str, Any], errors: list[str])` — [`L83`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L83)
- `_check_reusable_test_secrets(workflow_call: dict[str, Any], errors: list[str])` — [`L136`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L136)
- `_check_test_matrix(test_job: dict[str, Any], errors: list[str])` — [`L163`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L163)
- `_check_test_matrix_job(jobs: dict[str, Any], errors: list[str])` — [`L147`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L147)
- `_jobs(content: dict[Any, Any], errors: list[str])` — [`L75`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L75)
- `_workflow_call(content: dict[Any, Any], errors: list[str])` — [`L65`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L65)
- `composite_action_errors(content: dict[Any, Any])` — [`L57`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L57) — Return composite setup action structure errors.
- `load_yaml(path: str)` — [`L9`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L9) — Load a YAML file as a mapping.
- `print_result(label: str, success_message: str, errors: list[str])` — [`L16`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L16) — Print validation errors or the success message.
- `reusable_quality_errors(content: dict[Any, Any])` — [`L43`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L43) — Return reusable-quality workflow structure errors.
- `reusable_test_errors(content: dict[Any, Any])` — [`L28`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L28) — Return reusable-test workflow structure errors.
- `workflow_path(*parts: str)` — [`L300`](../../../../raw/code/tree-sitter-analyzer/_verify_workflow_structure_helpers.py#L300) — Return a repository-relative GitHub workflow/action path.

