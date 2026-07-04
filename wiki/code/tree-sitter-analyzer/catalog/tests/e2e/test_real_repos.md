---
title: 'Module: tests/e2e/test_real_repos.py'
type: catalog
provenance: extracted
module: tests/e2e/test_real_repos.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.e2e.test_real_repos`/
symbols:
  TestSafeToEditRealRepos.test_safe_to_edit_no_error_in_stderr: TestSafeToEditRealRepos#test_safe_to_edit_no_error_in_stderr().
  TestCheckProjectHealthRealRepos.test_project_health_returns_result: TestCheckProjectHealthRealRepos#test_project_health_returns_result().
  TestCheckProjectHealthRealRepos.test_project_health_under_30s: TestCheckProjectHealthRealRepos#test_project_health_under_30s().
  TestCheckFileHealthRealRepos.test_file_health_on_discovered_file: TestCheckFileHealthRealRepos#test_file_health_on_discovered_file().
  TestSafeToEditRealRepos.test_safe_to_edit_returns_verdict: TestSafeToEditRealRepos#test_safe_to_edit_returns_verdict().
  TestCheckProjectHealthRealRepos.test_project_health_returns_grade: TestCheckProjectHealthRealRepos#test_project_health_returns_grade().
  TestCrossProjectDiversity.test_project_health_reports_nonzero_file_count: TestCrossProjectDiversity#test_project_health_reports_nonzero_file_count().
  REAL_REPOS: REAL_REPOS.
  _find_python_file: _find_python_file().
  pytestmark: pytestmark.
  TestCheckProjectHealthRealRepos: TestCheckProjectHealthRealRepos#
  TestCheckFileHealthRealRepos: TestCheckFileHealthRealRepos#
  TestSafeToEditRealRepos: TestSafeToEditRealRepos#
  TestCrossProjectDiversity: TestCrossProjectDiversity#
---
# Module: [`tests/e2e/test_real_repos.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_real_repos.py)

## Classes
### `TestCheckFileHealthRealRepos`
- def: [`tests/e2e/test_real_repos.py:143`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_real_repos.py#L143)
- signature: `class TestCheckFileHealthRealRepos:`
- members:
  - `test_file_health_on_discovered_file(self, url: str, name: str, clone_repo_factory: Callable[[str, str], Path], mcp_server_factory: Callable[..., MCPClient])` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_real_repos.py#L145) — check_file_health must return a result for a file in a real repo.
- uses (calls/refs, reference-scoped): (5 test-only callers)

### `TestCheckProjectHealthRealRepos`
- def: [`tests/e2e/test_real_repos.py:72`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_real_repos.py#L72)
- signature: `class TestCheckProjectHealthRealRepos:`
- members:
  - `test_project_health_returns_grade(self, url: str, name: str, clone_repo_factory: Callable[[str, str], Path], mcp_server_factory: Callable[..., MCPClient])` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_real_repos.py#L94) — check_project_health must return a letter grade for real repos.
  - `test_project_health_returns_result(self, url: str, name: str, clone_repo_factory: Callable[[str, str], Path], mcp_server_factory: Callable[..., MCPClient])` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_real_repos.py#L74) — check_project_health must not crash on a real Python project.
  - `test_project_health_under_30s(self, url: str, name: str, clone_repo_factory: Callable[[str, str], Path], mcp_server_factory: Callable[..., MCPClient])` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_real_repos.py#L115) — check_project_health must finish in 30s even on real repos.
- uses (calls/refs, reference-scoped): (5 test-only callers)

### `TestCrossProjectDiversity`
- def: [`tests/e2e/test_real_repos.py:234`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_real_repos.py#L234)
- signature: `class TestCrossProjectDiversity:`
- members:
  - `test_project_health_reports_nonzero_file_count(self, url: str, name: str, clone_repo_factory: Callable[[str, str], Path], mcp_server_factory: Callable[..., MCPClient])` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_real_repos.py#L236) — The analyzed file count must be > 0 for any real repo.
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `TestSafeToEditRealRepos`
- def: [`tests/e2e/test_real_repos.py:172`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_real_repos.py#L172)
- signature: `class TestSafeToEditRealRepos:`
- members:
  - `test_safe_to_edit_no_error_in_stderr(self, url: str, name: str, clone_repo_factory: Callable[[str, str], Path], mcp_server_factory: Callable[..., MCPClient])` — [`L204`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_real_repos.py#L204) — safe_to_edit on a real repo must not produce ERROR-level stderr.
  - `test_safe_to_edit_returns_verdict(self, url: str, name: str, clone_repo_factory: Callable[[str, str], Path], mcp_server_factory: Callable[..., MCPClient])` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_real_repos.py#L174) — safe_to_edit must return a SAFE/UNSAFE verdict for a real-repo file.
- uses (calls/refs, reference-scoped): (6 test-only callers)

## Functions
- `_find_python_file(repo_dir: Path)` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_real_repos.py#L50) — Return a relative path to a small Python file inside ``repo_dir``.

## Module values
- `REAL_REPOS` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_real_repos.py#L39)
- `pytestmark` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_real_repos.py#L33)

