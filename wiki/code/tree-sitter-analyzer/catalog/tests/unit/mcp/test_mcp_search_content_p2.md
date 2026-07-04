---
title: 'Module: tests/unit/mcp/test_mcp_search_content_p2.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_search_content_p2.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_search_content_p2`/
symbols:
  test_fd_19_case_sensitive_search: test_fd_19_case_sensitive_search().
  test_fd_20_case_insensitive_search: test_fd_20_case_insensitive_search().
  test_fd_26_regex_overrides_glob: test_fd_26_regex_overrides_glob().
  test_fd_27_full_path_searches: test_fd_27_full_path_searches().
  test_fd_28_fixed_strings_search: test_fd_28_fixed_strings_search().
  test_fd_66_count_only_mode_advanced: test_fd_66_count_only_mode_advanced().
  _rg_json: _rg_json().
  test_fd_20_case_insensitive_search.fake_run: test_fd_20_case_insensitive_search().fake_run().
  test_fd_28_fixed_strings_search.fake_run: test_fd_28_fixed_strings_search().fake_run().
  test_fd_19_case_sensitive_search.fake_run: test_fd_19_case_sensitive_search().fake_run().
  test_fd_26_regex_overrides_glob.fake_run: test_fd_26_regex_overrides_glob().fake_run().
  test_fd_27_full_path_searches.fake_run: test_fd_27_full_path_searches().fake_run().
  test_fd_66_count_only_mode_advanced.fake_run: test_fd_66_count_only_mode_advanced().fake_run().
  mock_external_commands: mock_external_commands().
---
# Module: [`tests/unit/mcp/test_mcp_search_content_p2.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_search_content_p2.py)

## Functions
- `_rg_json(file_paths: list)` — [`L9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_search_content_p2.py#L9) — Build minimal ripgrep --json event stream for a list of file paths.
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_search_content_p2.py#L47)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_search_content_p2.py#L90)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_search_content_p2.py#L133)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_search_content_p2.py#L170)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_search_content_p2.py#L216)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_search_content_p2.py#L253)
- `mock_external_commands(monkeypatch)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_search_content_p2.py#L28) — Auto-mock external command availability checks for all tests in this module.
- `test_fd_19_case_sensitive_search(tmp_path, monkeypatch)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_search_content_p2.py#L38) — Test case sensitive search - corresponds to fd's test_case_sensitive.
- `test_fd_20_case_insensitive_search(tmp_path, monkeypatch)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_search_content_p2.py#L81) — Test case insensitive search - corresponds to fd's test_case_insensitive.
- `test_fd_26_regex_overrides_glob(tmp_path, monkeypatch)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_search_content_p2.py#L125) — Test regex overrides glob - corresponds to fd's test_regex_overrides_glob.
- `test_fd_27_full_path_searches(tmp_path, monkeypatch)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_search_content_p2.py#L159) — Test full path searches - corresponds to fd's test_full_path.
- `test_fd_28_fixed_strings_search(tmp_path, monkeypatch)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_search_content_p2.py#L207) — Test fixed strings search - corresponds to fd's test_fixed_strings.
- `test_fd_66_count_only_mode_advanced(tmp_path, monkeypatch)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_search_content_p2.py#L245) — Test advanced count only mode - corresponds to fd's count functionality.

