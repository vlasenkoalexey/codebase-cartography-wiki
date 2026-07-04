---
title: 'Module: tests/test_issue_806_fix.py'
type: catalog
provenance: extracted
module: tests/test_issue_806_fix.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.test_issue_806_fix`/
symbols:
  _SKIP_REASON: _SKIP_REASON.
  run_tests: run_tests().
  TestIssue806Fix.backend: TestIssue806Fix#backend.
  TestIssue806Scenarios: TestIssue806Scenarios#
  TestRegressionAfterFix: TestRegressionAfterFix#
  _get_kuzu_db: _get_kuzu_db().
  _KUZU_CHECK_FUNC: _KUZU_CHECK_FUNC.
  TestIssue806Fix.driver: TestIssue806Fix#driver.
  TestRegressionAfterFix.db: TestRegressionAfterFix#db.
  TestIssue806Fix.db: TestIssue806Fix#db.
  TestIssue806Scenarios.db: TestIssue806Scenarios#db.
  project_root: project_root.
  TestRegressionAfterFix.driver: TestRegressionAfterFix#driver.
  _is_kuzu_available: _is_kuzu_available().
  TestIssue806Fix.setUpClass: TestIssue806Fix#setUpClass().
  TestIssue806Fix.test_01_backend_is_kuzudb: TestIssue806Fix#test_01_backend_is_kuzudb().
  TestIssue806Fix.test_02_fixed_query_importers: TestIssue806Fix#test_02_fixed_query_importers().
  TestIssue806Fix.test_03_fixed_query_coimports: TestIssue806Fix#test_03_fixed_query_coimports().
  TestIssue806Fix.test_04_find_module_dependencies_method: TestIssue806Fix#test_04_find_module_dependencies_method().
  TestIssue806Fix.test_05_multiple_modules: TestIssue806Fix#test_05_multiple_modules().
  TestIssue806Fix.test_06_old_buggy_query_should_fail: TestIssue806Fix#test_06_old_buggy_query_should_fail().
  TestIssue806Scenarios.setUpClass: TestIssue806Scenarios#setUpClass().
  TestIssue806Scenarios.driver: TestIssue806Scenarios#driver.
  TestIssue806Scenarios.test_scenario_empty_module: TestIssue806Scenarios#test_scenario_empty_module().
  TestIssue806Scenarios.test_scenario_special_characters: TestIssue806Scenarios#test_scenario_special_characters().
  TestIssue806Scenarios.test_scenario_concurrent_queries: TestIssue806Scenarios#test_scenario_concurrent_queries().
  TestRegressionAfterFix.setUpClass: TestRegressionAfterFix#setUpClass().
  TestRegressionAfterFix.test_regression_who_imports_module: TestRegressionAfterFix#test_regression_who_imports_module().
  TestRegressionAfterFix.test_regression_find_by_module_name: TestRegressionAfterFix#test_regression_find_by_module_name().
  TestRegressionAfterFix.test_regression_find_imports: TestRegressionAfterFix#test_regression_find_imports().
  TestRegressionAfterFix.test_regression_result_ordering: TestRegressionAfterFix#test_regression_result_ordering().
  TestRegressionAfterFix.test_regression_coexists_with_other_backends: TestRegressionAfterFix#test_regression_coexists_with_other_backends().
  TestKuzuSkipBehavior.test_skip_check_returns_true_when_kuzudb_configured: TestKuzuSkipBehavior#test_skip_check_returns_true_when_kuzudb_configured().
  TestKuzuSkipBehavior.test_skip_reason_is_descriptive: TestKuzuSkipBehavior#test_skip_reason_is_descriptive().
  TestIssue806Fix: TestIssue806Fix#
  TestKuzuSkipBehavior: TestKuzuSkipBehavior#
  TestKuzuSkipBehavior.test_skip_check_returns_false_when_kuzu_not_installed: TestKuzuSkipBehavior#test_skip_check_returns_false_when_kuzu_not_installed().
---
# Module: [`tests/test_issue_806_fix.py`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py)

## Classes
### `TestIssue806Fix`  ·  implements/extends TestCase
- def: [`tests/test_issue_806_fix.py:72`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L72)
- doc: Test cases for Issue #806 fix verification.
- signature: `class TestIssue806Fix(unittest.TestCase):`
- members:
  - `setUpClass(cls)` — [`L79`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L79) — Set up KuzuDB connection for all tests.
  - `test_01_backend_is_kuzudb(self)` — [`L89`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L89) — Verify we're using KuzuDB backend.
  - `test_02_fixed_query_importers(self)` — [`L94`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L94) — Test Query 1: Importers query with fixed ORDER BY.
  - `test_03_fixed_query_coimports(self)` — [`L113`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L113) — Test Query 2: Co-imports query with fixed ORDER BY.
  - `test_04_find_module_dependencies_method(self)` — [`L134`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L134) — Test the actual find_module_dependencies method.
  - `test_05_multiple_modules(self)` — [`L153`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L153) — Test fix works for multiple different modules.
  - `test_06_old_buggy_query_should_fail(self)` — [`L169`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L169) — Verify that the OLD buggy query still fails (regression test).
  - `backend` — [`L86`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L86)
  - `db` — [`L84`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L84)
  - `driver` — [`L85`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L85)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestIssue806Scenarios`  ·  implements/extends TestCase
- def: [`tests/test_issue_806_fix.py:195`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L195)
- doc: Additional test scenarios for Issue #806.
- signature: `class TestIssue806Scenarios(unittest.TestCase):`
- members:
  - `setUpClass(cls)` — [`L202`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L202) — Set up KuzuDB connection.
  - `test_scenario_concurrent_queries(self)` — [`L241`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L241) — Scenario: Multiple queries should work correctly.
  - `test_scenario_empty_module(self)` — [`L210`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L210) — Scenario: Query for non-existent module should return empty results.
  - `test_scenario_special_characters(self)` — [`L222`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L222) — Scenario: Query with special characters in module name.
  - `db` — [`L207`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L207)
  - `driver` — [`L208`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L208)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (1 test-only callers)

### `TestKuzuSkipBehavior`  ·  implements/extends TestCase
- def: [`tests/test_issue_806_fix.py:420`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L420)
- doc: Test that KuzuDB-specific tests skip correctly on non-KuzuDB backends.
- signature: `class TestKuzuSkipBehavior(unittest.TestCase):`
- members:
  - `test_skip_check_returns_false_when_kuzu_not_installed(self)` — [`L449`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L449) — Verify _is_kuzu_available returns False when kuzu module is not available.
  - `test_skip_check_returns_true_when_kuzudb_configured(self)` — [`L423`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L423) — Verify _is_kuzu_available returns True when configured backend is kuzudb.
  - `test_skip_reason_is_descriptive(self)` — [`L443`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L443) — Verify skip reason clearly explains why tests are skipped.
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (1 test-only callers)

### `TestRegressionAfterFix`  ·  implements/extends TestCase
- def: [`tests/test_issue_806_fix.py:260`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L260)
- doc: Regression Tests - Ensure fix doesn't break other CodeFinder methods.
- signature: `class TestRegressionAfterFix(unittest.TestCase):`
- members:
  - `setUpClass(cls)` — [`L271`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L271) — Set up KuzuDB connection.
  - `test_regression_coexists_with_other_backends(self)` — [`L386`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L386) — Regression Test #14: Backend Compatibility
  - `test_regression_find_by_module_name(self)` — [`L310`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L310) — Regression Test #11: find_by_module_name()
  - `test_regression_find_imports(self)` — [`L332`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L332) — Regression Test #12: find_imports()
  - `test_regression_result_ordering(self)` — [`L354`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L354) — Regression Test #13: Result Ordering
  - `test_regression_who_imports_module(self)` — [`L279`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L279) — Regression Test #10: who_imports_module()
  - `db` — [`L276`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L276)
  - `driver` — [`L277`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L277)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (1 test-only callers)

## Functions
- `_get_kuzu_db()` — [`L54`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L54) — Get KuzuDB manager, or return None if not available.
- `_is_kuzu_available()` — [`L27`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L27) — Check if configured backend is KuzuDB.
- `run_tests()` — [`L501`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L501) — Run all test cases with detailed output.

## Module values
- `_KUZU_CHECK_FUNC` — [`L67`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L67)
- `_SKIP_REASON` — [`L68`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L68)
- `project_root` — [`L23`](../../../../../raw/code/codegraphcontext/tests/test_issue_806_fix.py#L23)

