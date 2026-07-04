---
title: 'Module: tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_find_and_grep_fd_simulation_p1`/
symbols:
  test_fd_02_multi_file_search: test_fd_02_multi_file_search().
  test_fd_03_multi_file_with_missing: test_fd_03_multi_file_with_missing().
  test_fd_04_explicit_root_path: test_fd_04_explicit_root_path().
  test_fd_05_and_basic_simulation: test_fd_05_and_basic_simulation().
  test_fd_06_and_empty_pattern_simulation: test_fd_06_and_empty_pattern_simulation().
  test_fd_07_and_bad_pattern_simulation: test_fd_07_and_bad_pattern_simulation().
  test_fd_08_and_pattern_starts_with_dash: test_fd_08_and_pattern_starts_with_dash().
  test_fd_09_and_plus_extension: test_fd_09_and_plus_extension().
  test_fd_10_and_plus_type: test_fd_10_and_plus_type().
  test_fd_10_and_plus_type.fake_run: test_fd_10_and_plus_type().fake_run().
  _fd_type_filter_files: _fd_type_filter_files().
  test_fd_02_multi_file_search.fake_run: test_fd_02_multi_file_search().fake_run().
  test_fd_03_multi_file_with_missing.fake_run: test_fd_03_multi_file_with_missing().fake_run().
  test_fd_04_explicit_root_path.fake_run: test_fd_04_explicit_root_path().fake_run().
  test_fd_05_and_basic_simulation.fake_run: test_fd_05_and_basic_simulation().fake_run().
  test_fd_06_and_empty_pattern_simulation.fake_run: test_fd_06_and_empty_pattern_simulation().fake_run().
  test_fd_07_and_bad_pattern_simulation.fake_run: test_fd_07_and_bad_pattern_simulation().fake_run().
  test_fd_08_and_pattern_starts_with_dash.fake_run: test_fd_08_and_pattern_starts_with_dash().fake_run().
  test_fd_09_and_plus_extension.fake_run: test_fd_09_and_plus_extension().fake_run().
  mock_external_commands: mock_external_commands().
---
# Module: [`tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py)

## Functions
- `_fd_type_filter_files(tmp_path, cmd)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L18) — Return simulated fd output for the files-only type filter.
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L45)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L95)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L132)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L171)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L206)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L229)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L261)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L292)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L341)
- `mock_external_commands(monkeypatch)` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L10) — Auto-mock external command availability checks for all tests in this module.
- `test_fd_02_multi_file_search(tmp_path, monkeypatch)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L33) — Test multi-directory search - corresponds to fd's test_multi_file.
- `test_fd_03_multi_file_with_missing(tmp_path, monkeypatch)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L86) — Test search with missing directories - corresponds to fd's test_multi_file_with_missing.
- `test_fd_04_explicit_root_path(tmp_path, monkeypatch)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L122) — Test explicit root path - corresponds to fd's test_explicit_root_path.
- `test_fd_05_and_basic_simulation(tmp_path, monkeypatch)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L162) — Test AND search basic functionality - simulates fd's test_and_basic.
- `test_fd_06_and_empty_pattern_simulation(tmp_path, monkeypatch)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L198) — Test AND search with empty pattern - simulates fd's test_and_empty_pattern.
- `test_fd_07_and_bad_pattern_simulation(tmp_path, monkeypatch)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L225) — Test AND search with bad pattern - simulates fd's test_and_bad_pattern.
- `test_fd_08_and_pattern_starts_with_dash(tmp_path, monkeypatch)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L253) — Test AND search with dash-prefixed pattern - simulates fd's test_and_pattern_starts_with_dash.
- `test_fd_09_and_plus_extension(tmp_path, monkeypatch)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L283) — Test AND search with extension filter - simulates fd's test_and_plus_extension.
- `test_fd_10_and_plus_type(tmp_path, monkeypatch)` — [`L332`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_fd_simulation_p1.py#L332) — Test AND search with type filter - simulates fd's test_and_plus_type.

