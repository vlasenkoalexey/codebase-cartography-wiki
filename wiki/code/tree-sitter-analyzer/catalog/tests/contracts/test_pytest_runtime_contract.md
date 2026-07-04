---
title: 'Module: tests/contracts/test_pytest_runtime_contract.py'
type: catalog
provenance: extracted
module: tests/contracts/test_pytest_runtime_contract.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.contracts.test_pytest_runtime_contract`/
symbols:
  PROJECT_ROOT: PROJECT_ROOT.
  test_default_pytest_runtime_contract_is_locked: test_default_pytest_runtime_contract_is_locked().
  test_pyproject_does_not_define_pytest_ini_options: test_pyproject_does_not_define_pytest_ini_options().
  test_pytest_runtime_dependencies_are_declared: test_pytest_runtime_dependencies_are_declared().
  test_local_runtime_artifacts_are_gitignored_without_global_results_trap: test_local_runtime_artifacts_are_gitignored_without_global_results_trap().
  test_default_sustained_load_check_stays_fast_and_configurable: test_default_sustained_load_check_stays_fast_and_configurable().
  test_phase7_suite_simulated_work_stays_fast_and_configurable: test_phase7_suite_simulated_work_stays_fast_and_configurable().
  _assert_pytest_runtime_contract: _assert_pytest_runtime_contract().
  SKIPPED_SCAN_DIRS: SKIPPED_SCAN_DIRS.
  test_hypothesis_deadlines_are_disabled_for_parallel_suite_stability: test_hypothesis_deadlines_are_disabled_for_parallel_suite_stability().
---
# Module: [`tests/contracts/test_pytest_runtime_contract.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_pytest_runtime_contract.py)

## Functions
- `_assert_pytest_runtime_contract(addopts: str | list[str], warning_filters: str | list[str])` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_pytest_runtime_contract.py#L52)
- `test_default_pytest_runtime_contract_is_locked()` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_pytest_runtime_contract.py#L35) — The default full suite must stay parallel and bounded under 5 minutes.
- `test_default_sustained_load_check_stays_fast_and_configurable()` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_pytest_runtime_contract.py#L120) — Default performance checks use short configurable waits.
- `test_hypothesis_deadlines_are_disabled_for_parallel_suite_stability()` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_pytest_runtime_contract.py#L115) — xdist load variance is bounded by pytest-timeout, not Hypothesis deadlines.
- `test_local_runtime_artifacts_are_gitignored_without_global_results_trap()` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_pytest_runtime_contract.py#L96) — Dogfood/cache output must stay local without hiding every results dir.
- `test_phase7_suite_simulated_work_stays_fast_and_configurable()` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_pytest_runtime_contract.py#L149) — Summary-style integration checks should not spend seconds sleeping.
- `test_pyproject_does_not_define_pytest_ini_options()` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_pytest_runtime_contract.py#L45) — pytest.ini is the single source of truth for pytest runtime config.
- `test_pytest_runtime_dependencies_are_declared()` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_pytest_runtime_contract.py#L86) — The runtime contract depends on xdist and timeout being installed.

## Module values
- `PROJECT_ROOT` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_pytest_runtime_contract.py#L24)
- `SKIPPED_SCAN_DIRS` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_pytest_runtime_contract.py#L25)

