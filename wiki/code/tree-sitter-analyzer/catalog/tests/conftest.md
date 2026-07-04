---
title: 'Module: tests/conftest.py'
type: catalog
provenance: extracted
module: tests/conftest.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.conftest`/
symbols:
  PROJECT_ROOT: PROJECT_ROOT.
  _cleanup_pytest_git_repos: _cleanup_pytest_git_repos().
  pytest_configure: pytest_configure().
  pytest_sessionfinish: pytest_sessionfinish().
  reset_global_singletons: reset_global_singletons().
  temp_test_file: temp_test_file().
  temp_test_dir: temp_test_dir().
  pytest_runtest_call: pytest_runtest_call().
  _reset_all_singletons: _reset_all_singletons().
  SLOW_TEST_BUDGET_S.SLOW_TEST_BUDGET_S: SLOW_TEST_BUDGET_S.SLOW_TEST_BUDGET_S.
  temp_test_file._create_temp_file: temp_test_file()._create_temp_file().
  temp_test_dir._create_temp_dir: temp_test_dir()._create_temp_dir().
  pytest_xdist_auto_num_workers: pytest_xdist_auto_num_workers().
  pytest_collection_modifyitems: pytest_collection_modifyitems().
  has_external_tools: has_external_tools().
  test_data_dir: test_data_dir().
  temp_project_dir: temp_project_dir().
  pytest_terminal_summary: pytest_terminal_summary().
  cleanup_asyncio_tasks: cleanup_asyncio_tasks().
  cleanup_test_databases: cleanup_test_databases().
  verify_test_isolation: verify_test_isolation().
---
# Module: [`tests/conftest.py`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py)

## Functions
- `_cleanup_pytest_git_repos()` — [`L35`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L35) — Best-effort cleanup for project-local git repos used by subprocess tests.
- `_create_temp_dir(dirname: str)` — [`L455`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L455) — Create a temporary test directory.
- `_create_temp_file(filename: str, content: str = "")` — [`L423`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L423) — Create a temporary test file.
- `_reset_all_singletons()` — [`L301`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L301) — Reset all global singletons. Called before and after each test for isolation.
- `cleanup_asyncio_tasks()` — [`L251`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L251) — Clean up asyncio tasks after each test to prevent 'NoneType' object has no attribute '_PENDING'
- `cleanup_test_databases()` — [`L392`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L392) — Clean up test databases once per session instead of per-test.
- `has_external_tools()` — [`L127`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L127) — Check availability of external tools.
- `pytest_collection_modifyitems(config, items)` — [`L103`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L103) — Modify test collection to skip tests based on missing dependencies.
- `pytest_configure(config)` — [`L49`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L49) — Configure pytest with custom markers and safety checks.
- `pytest_runtest_call(item)` — [`L543`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L543) — Enforce per-test wall-time budget for unit tests.
- `pytest_sessionfinish(session, exitstatus)` — [`L208`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L208) — Force garbage collection at end of session to ensure
- `pytest_terminal_summary(terminalreporter, exitstatus, config)` — [`L221`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L221) — Warn if memory usage is dangerously high at end of session.
- `pytest_xdist_auto_num_workers(config)` — [`L42`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L42) — Cap automatic xdist worker sizing on Windows.
- `reset_global_singletons()` — [`L384`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L384) — Reset all global singletons before and after each test for isolation.
- `temp_project_dir(tmp_path)` — [`L142`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L142) — Create a temporary project directory with sample files.
- `temp_test_dir(tmp_path)` — [`L451`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L451) — Create a temporary test directory with cleanup.
- `temp_test_file(tmp_path)` — [`L419`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L419) — Create a temporary test file with cleanup.
- `test_data_dir()` — [`L136`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L136) — Get test data directory.
- `verify_test_isolation()` — [`L484`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L484) — Verify test isolation by checking for leaked resources.

## Module values
- `PROJECT_ROOT` — [`L13`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L13)
- `SLOW_TEST_BUDGET_S` — [`L539`](../../../../../raw/code/tree-sitter-analyzer/tests/conftest.py#L539)

