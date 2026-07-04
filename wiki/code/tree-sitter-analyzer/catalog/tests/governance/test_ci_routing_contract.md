---
title: 'Module: tests/governance/test_ci_routing_contract.py'
type: catalog
provenance: extracted
module: tests/governance/test_ci_routing_contract.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.governance.test_ci_routing_contract`/
symbols:
  PROJECT_ROOT: PROJECT_ROOT.
  test_reusable_test_workflow_has_job_timeout: test_reusable_test_workflow_has_job_timeout().
  test_pr_ci_uses_fast_matrix_while_release_keeps_full_matrix: test_pr_ci_uses_fast_matrix_while_release_keeps_full_matrix().
  test_ci_full_language_suite_runs_once_per_reusable_test_matrix: test_ci_full_language_suite_runs_once_per_reusable_test_matrix().
  test_standalone_coverage_workflow_is_manual_only: test_standalone_coverage_workflow_is_manual_only().
  test_all_language_golden_tests_are_tier_marked: test_all_language_golden_tests_are_tier_marked().
  test_agent_docs_lock_ci_test_tier_contract: test_agent_docs_lock_ci_test_tier_contract().
  test_ci_route_job_controls_expensive_optional_jobs: test_ci_route_job_controls_expensive_optional_jobs().
  test_expensive_workflows_are_not_direct_pr_push_duplicates: test_expensive_workflows_are_not_direct_pr_push_duplicates().
  test_benchmarks_are_path_filtered_for_pr_and_push: test_benchmarks_are_path_filtered_for_pr_and_push().
  test_bandit_security_scan_is_blocking_and_configured: test_bandit_security_scan_is_blocking_and_configured().
  SKIPPED_SCAN_DIRS: SKIPPED_SCAN_DIRS.
---
# Module: [`tests/governance/test_ci_routing_contract.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_ci_routing_contract.py)

## Functions
- `test_agent_docs_lock_ci_test_tier_contract()` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_ci_routing_contract.py#L131) — Agents should preserve the CI split between focused and exhaustive gates.
- `test_all_language_golden_tests_are_tier_marked()` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_ci_routing_contract.py#L119) — All-language suites need an explicit marker so CI can tier them.
- `test_bandit_security_scan_is_blocking_and_configured()` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_ci_routing_contract.py#L184) — The reusable quality workflow must not paper over Bandit failures.
- `test_benchmarks_are_path_filtered_for_pr_and_push()` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_ci_routing_contract.py#L173) — Benchmarks should not run for unrelated PRs.
- `test_ci_full_language_suite_runs_once_per_reusable_test_matrix()` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_ci_routing_contract.py#L91) — Exhaustive language golden tests must not run on every OS/Python axis.
- `test_ci_route_job_controls_expensive_optional_jobs()` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_ci_routing_contract.py#L144) — Main CI should route slow optional jobs instead of always running them.
- `test_expensive_workflows_are_not_direct_pr_push_duplicates()` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_ci_routing_contract.py#L158) — Regression and SQL compatibility run through CI routing, not twice.
- `test_pr_ci_uses_fast_matrix_while_release_keeps_full_matrix()` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_ci_routing_contract.py#L52) — PRs should get fast feedback; release/hotfix keep exhaustive validation.
- `test_reusable_test_workflow_has_job_timeout()` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_ci_routing_contract.py#L34) — The CI matrix must fail fast instead of hanging forever on runner stalls.
- `test_standalone_coverage_workflow_is_manual_only()` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_ci_routing_contract.py#L105) — Avoid duplicate full coverage runs; reusable-test owns PR/push coverage.

## Module values
- `PROJECT_ROOT` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_ci_routing_contract.py#L23)
- `SKIPPED_SCAN_DIRS` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/governance/test_ci_routing_contract.py#L24)

