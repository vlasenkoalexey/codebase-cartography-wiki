---
title: 'Module: tests/unit/mcp/test_mcp_list_files_p3b_filters.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_list_files_p3b_filters.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_list_files_p3b_filters`/
symbols:
  test_fd_75_modified_relative_time: test_fd_75_modified_relative_time().
  test_fd_76_modified_absolute_time: test_fd_76_modified_absolute_time().
  test_fd_77_size_filtering_advanced: test_fd_77_size_filtering_advanced().
  test_fd_78_no_extension_filter: test_fd_78_no_extension_filter().
  test_fd_79_owner_ignore_all: test_fd_79_owner_ignore_all().
  test_fd_80_owner_current_user: test_fd_80_owner_current_user().
  test_fd_81_owner_current_group: test_fd_81_owner_current_group().
  test_fd_82_owner_root: test_fd_82_owner_root().
  test_fd_83_quiet_mode_simulation: test_fd_83_quiet_mode_simulation().
  test_fd_84_max_results_advanced: test_fd_84_max_results_advanced().
  test_fd_86_list_details_advanced: test_fd_86_list_details_advanced().
  test_fd_75_modified_relative_time.fake_run: test_fd_75_modified_relative_time().fake_run().
  test_fd_76_modified_absolute_time.fake_run: test_fd_76_modified_absolute_time().fake_run().
  test_fd_77_size_filtering_advanced.fake_run: test_fd_77_size_filtering_advanced().fake_run().
  test_fd_78_no_extension_filter.fake_run: test_fd_78_no_extension_filter().fake_run().
  test_fd_79_owner_ignore_all.fake_run: test_fd_79_owner_ignore_all().fake_run().
  test_fd_80_owner_current_user.fake_run: test_fd_80_owner_current_user().fake_run().
  test_fd_81_owner_current_group.fake_run: test_fd_81_owner_current_group().fake_run().
  test_fd_82_owner_root.fake_run: test_fd_82_owner_root().fake_run().
  test_fd_83_quiet_mode_simulation.fake_run: test_fd_83_quiet_mode_simulation().fake_run().
  test_fd_84_max_results_advanced.fake_run: test_fd_84_max_results_advanced().fake_run().
  test_fd_86_list_details_advanced.fake_run: test_fd_86_list_details_advanced().fake_run().
  mock_external_commands: mock_external_commands().
---
# Module: [`tests/unit/mcp/test_mcp_list_files_p3b_filters.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py)

## Functions
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L24)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L58)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L97)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L143)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L176)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L205)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L233)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L261)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L289)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L318)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L363)
- `mock_external_commands(monkeypatch)` — [`L7`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L7) — Auto-mock external command availability checks for all tests in this module.
- `test_fd_75_modified_relative_time(tmp_path, monkeypatch)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L16) — Test relative modification time filtering - corresponds to fd's test_modified_relative.
- `test_fd_76_modified_absolute_time(tmp_path, monkeypatch)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L50) — Test absolute modification time filtering - corresponds to fd's test_modified_absolute.
- `test_fd_77_size_filtering_advanced(tmp_path, monkeypatch)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L89) — Test advanced size filtering - corresponds to fd's test_size.
- `test_fd_78_no_extension_filter(tmp_path, monkeypatch)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L134) — Test no extension filter - corresponds to fd's test_no_extension.
- `test_fd_79_owner_ignore_all(tmp_path, monkeypatch)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L168) — Test owner filtering - ignore all - corresponds to fd's test_owner_ignore_all.
- `test_fd_80_owner_current_user(tmp_path, monkeypatch)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L197) — Test current user owner filtering - corresponds to fd's test_owner_current_user.
- `test_fd_81_owner_current_group(tmp_path, monkeypatch)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L226) — Test current group owner filtering - corresponds to fd's test_owner_current_group.
- `test_fd_82_owner_root(tmp_path, monkeypatch)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L254) — Test root owner filtering - corresponds to fd's test_owner_root.
- `test_fd_83_quiet_mode_simulation(tmp_path, monkeypatch)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L282) — Test quiet mode simulation - corresponds to fd's test_quiet.
- `test_fd_84_max_results_advanced(tmp_path, monkeypatch)` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L310) — Test advanced max results limiting - corresponds to fd's test_max_results.
- `test_fd_86_list_details_advanced(tmp_path, monkeypatch)` — [`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3b_filters.py#L355) — Test advanced list details - corresponds to fd's test_list_details.

