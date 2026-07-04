---
title: 'Module: tests/unit/mcp/test_mcp_list_files_p2.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_list_files_p2.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_list_files_p2`/
symbols:
  test_fd_33_type_empty: test_fd_33_type_empty().
  test_fd_34_extension_filtering: test_fd_34_extension_filtering().
  test_fd_35_no_extension: test_fd_35_no_extension().
  test_fd_36_size_filtering: test_fd_36_size_filtering().
  test_fd_37_no_ignore_basic: test_fd_37_no_ignore_basic().
  test_fd_39_max_depth_filtering: test_fd_39_max_depth_filtering().
  test_fd_40_min_depth_filtering: test_fd_40_min_depth_filtering().
  test_fd_41_exact_depth_filtering: test_fd_41_exact_depth_filtering().
  test_fd_42_prune_functionality: test_fd_42_prune_functionality().
  test_fd_43_excludes_pattern: test_fd_43_excludes_pattern().
  test_fd_33_type_empty.fake_run: test_fd_33_type_empty().fake_run().
  test_fd_34_extension_filtering.fake_run: test_fd_34_extension_filtering().fake_run().
  test_fd_35_no_extension.fake_run: test_fd_35_no_extension().fake_run().
  test_fd_36_size_filtering.fake_run: test_fd_36_size_filtering().fake_run().
  test_fd_37_no_ignore_basic.fake_run: test_fd_37_no_ignore_basic().fake_run().
  test_fd_39_max_depth_filtering.fake_run: test_fd_39_max_depth_filtering().fake_run().
  test_fd_40_min_depth_filtering.fake_run: test_fd_40_min_depth_filtering().fake_run().
  test_fd_41_exact_depth_filtering.fake_run: test_fd_41_exact_depth_filtering().fake_run().
  test_fd_42_prune_functionality.fake_run: test_fd_42_prune_functionality().fake_run().
  test_fd_43_excludes_pattern.fake_run: test_fd_43_excludes_pattern().fake_run().
  mock_external_commands: mock_external_commands().
---
# Module: [`tests/unit/mcp/test_mcp_list_files_p2.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py)

## Functions
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L26)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L63)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L116)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L147)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L203)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L258)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L330)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L365)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L415`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L415)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L460`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L460)
- `mock_external_commands(monkeypatch)` — [`L7`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L7) — Auto-mock external command availability checks for all tests in this module.
- `test_fd_33_type_empty(tmp_path, monkeypatch)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L17) — Test empty file type - corresponds to fd's test_type_empty.
- `test_fd_34_extension_filtering(tmp_path, monkeypatch)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L53) — Test file extension filtering - corresponds to fd's test_extension.
- `test_fd_35_no_extension(tmp_path, monkeypatch)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L106) — Test files without extension - corresponds to fd's test_no_extension.
- `test_fd_36_size_filtering(tmp_path, monkeypatch)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L138) — Test file size filtering - corresponds to fd's test_size.
- `test_fd_37_no_ignore_basic(tmp_path, monkeypatch)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L192) — Test basic no ignore functionality - corresponds to fd's test_no_ignore.
- `test_fd_39_max_depth_filtering(tmp_path, monkeypatch)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L244) — Test maximum depth filtering - corresponds to fd's test_max_depth.
- `test_fd_40_min_depth_filtering(tmp_path, monkeypatch)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L319) — Test minimum depth filtering - corresponds to fd's test_min_depth.
- `test_fd_41_exact_depth_filtering(tmp_path, monkeypatch)` — [`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L355) — Test exact depth filtering - corresponds to fd's test_exact_depth.
- `test_fd_42_prune_functionality(tmp_path, monkeypatch)` — [`L404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L404) — Test prune functionality - corresponds to fd's test_prune.
- `test_fd_43_excludes_pattern(tmp_path, monkeypatch)` — [`L450`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p2.py#L450) — Test exclude patterns - corresponds to fd's test_excludes.

