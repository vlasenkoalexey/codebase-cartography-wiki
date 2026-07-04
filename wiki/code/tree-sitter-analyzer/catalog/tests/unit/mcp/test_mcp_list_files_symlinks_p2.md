---
title: 'Module: tests/unit/mcp/test_mcp_list_files_symlinks_p2.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_list_files_symlinks_p2.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_list_files_symlinks_p2`/
symbols:
  test_fd_44_follow_symlinks: test_fd_44_follow_symlinks().
  test_fd_45_file_system_boundaries: test_fd_45_file_system_boundaries().
  test_fd_46_follow_broken_symlink: test_fd_46_follow_broken_symlink().
  test_fd_47_symlink_as_root: test_fd_47_symlink_as_root().
  test_fd_48_symlink_and_absolute_path: test_fd_48_symlink_and_absolute_path().
  test_fd_49_symlink_as_absolute_root: test_fd_49_symlink_as_absolute_root().
  test_fd_44_follow_symlinks.fake_run: test_fd_44_follow_symlinks().fake_run().
  test_fd_45_file_system_boundaries.fake_run: test_fd_45_file_system_boundaries().fake_run().
  test_fd_46_follow_broken_symlink.fake_run: test_fd_46_follow_broken_symlink().fake_run().
  test_fd_47_symlink_as_root.fake_run: test_fd_47_symlink_as_root().fake_run().
  test_fd_48_symlink_and_absolute_path.fake_run: test_fd_48_symlink_and_absolute_path().fake_run().
  test_fd_49_symlink_as_absolute_root.fake_run: test_fd_49_symlink_as_absolute_root().fake_run().
  mock_external_commands: mock_external_commands().
---
# Module: [`tests/unit/mcp/test_mcp_list_files_symlinks_p2.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_symlinks_p2.py)

## Functions
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_symlinks_p2.py#L35)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_symlinks_p2.py#L102)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_symlinks_p2.py#L143)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_symlinks_p2.py#L191)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_symlinks_p2.py#L237)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_symlinks_p2.py#L284)
- `mock_external_commands(monkeypatch)` — [`L7`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_symlinks_p2.py#L7) — Auto-mock external command availability checks for all tests in this module.
- `test_fd_44_follow_symlinks(tmp_path, monkeypatch)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_symlinks_p2.py#L16) — Test following symlinks - corresponds to fd's test_follow.
- `test_fd_45_file_system_boundaries(tmp_path, monkeypatch)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_symlinks_p2.py#L93) — Test file system boundaries - corresponds to fd's test_file_system_boundaries.
- `test_fd_46_follow_broken_symlink(tmp_path, monkeypatch)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_symlinks_p2.py#L127) — Test following broken symlinks - corresponds to fd's test_follow_broken_symlink.
- `test_fd_47_symlink_as_root(tmp_path, monkeypatch)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_symlinks_p2.py#L174) — Test symlink as search root - corresponds to fd's test_symlink_as_root.
- `test_fd_48_symlink_and_absolute_path(tmp_path, monkeypatch)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_symlinks_p2.py#L220) — Test symlinks with absolute paths - corresponds to fd's test_symlink_and_absolute_path.
- `test_fd_49_symlink_as_absolute_root(tmp_path, monkeypatch)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_symlinks_p2.py#L267) — Test symlink as absolute root - corresponds to fd's test_symlink_as_absolute_root.

