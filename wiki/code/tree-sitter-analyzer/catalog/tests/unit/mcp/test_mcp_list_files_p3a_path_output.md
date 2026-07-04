---
title: 'Module: tests/unit/mcp/test_mcp_list_files_p3a_path_output.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_list_files_p3a_path_output.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_list_files_p3a_path_output`/
symbols:
  test_fd_50_symlink_and_full_path: test_fd_50_symlink_and_full_path().
  test_fd_51_print0_output_simulation: test_fd_51_print0_output_simulation().
  test_fd_52_absolute_path_output: test_fd_52_absolute_path_output().
  test_fd_53_implicit_absolute_path: test_fd_53_implicit_absolute_path().
  test_fd_54_normalized_absolute_path: test_fd_54_normalized_absolute_path().
  test_fd_55_custom_path_separator: test_fd_55_custom_path_separator().
  test_fd_56_base_directory_output: test_fd_56_base_directory_output().
  test_fd_57_strip_cwd_prefix: test_fd_57_strip_cwd_prefix().
  test_fd_58_format_output_structured: test_fd_58_format_output_structured().
  test_fd_65_exec_invalid_utf8_simulation: test_fd_65_exec_invalid_utf8_simulation().
  test_fd_38_gitignore_and_fdignore_advanced: test_fd_38_gitignore_and_fdignore_advanced().
  test_fd_50_symlink_and_full_path.fake_run: test_fd_50_symlink_and_full_path().fake_run().
  test_fd_51_print0_output_simulation.fake_run: test_fd_51_print0_output_simulation().fake_run().
  test_fd_52_absolute_path_output.fake_run: test_fd_52_absolute_path_output().fake_run().
  test_fd_53_implicit_absolute_path.fake_run: test_fd_53_implicit_absolute_path().fake_run().
  test_fd_54_normalized_absolute_path.fake_run: test_fd_54_normalized_absolute_path().fake_run().
  test_fd_55_custom_path_separator.fake_run: test_fd_55_custom_path_separator().fake_run().
  test_fd_56_base_directory_output.fake_run: test_fd_56_base_directory_output().fake_run().
  test_fd_57_strip_cwd_prefix.fake_run: test_fd_57_strip_cwd_prefix().fake_run().
  test_fd_58_format_output_structured.fake_run: test_fd_58_format_output_structured().fake_run().
  test_fd_65_exec_invalid_utf8_simulation.fake_run: test_fd_65_exec_invalid_utf8_simulation().fake_run().
  test_fd_38_gitignore_and_fdignore_advanced.fake_run: test_fd_38_gitignore_and_fdignore_advanced().fake_run().
  mock_external_commands: mock_external_commands().
---
# Module: [`tests/unit/mcp/test_mcp_list_files_p3a_path_output.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py)

## Functions
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L36)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L72)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L110)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L168)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L197)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L232)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L271)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L305)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L337)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L377)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L412)
- `mock_external_commands(monkeypatch)` — [`L9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L9) — Auto-mock external command availability checks for all tests in this module.
- `test_fd_38_gitignore_and_fdignore_advanced(tmp_path, monkeypatch)` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L397) — Test advanced gitignore and fdignore handling - corresponds to fd's test_gitignore_and_fdignore.
- `test_fd_50_symlink_and_full_path(tmp_path, monkeypatch)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L19) — Test symlinks with full path matching - corresponds to fd's test_symlink_and_full_path.
- `test_fd_51_print0_output_simulation(tmp_path, monkeypatch)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L64) — Test print0 output simulation - corresponds to fd's test_print0.
- `test_fd_52_absolute_path_output(tmp_path, monkeypatch)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L101) — Test absolute path output - corresponds to fd's test_absolute_path.
- `test_fd_53_implicit_absolute_path(tmp_path, monkeypatch)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L161) — Test implicit absolute path - corresponds to fd's test_implicit_absolute_path.
- `test_fd_54_normalized_absolute_path(tmp_path, monkeypatch)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L189) — Test normalized absolute path - corresponds to fd's test_normalized_absolute_path.
- `test_fd_55_custom_path_separator(tmp_path, monkeypatch)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L224) — Test custom path separator - corresponds to fd's test_custom_path_separator.
- `test_fd_56_base_directory_output(tmp_path, monkeypatch)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L263) — Test base directory output - corresponds to fd's test_base_directory.
- `test_fd_57_strip_cwd_prefix(tmp_path, monkeypatch)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L298) — Test stripping current working directory prefix - corresponds to fd's test_strip_cwd_prefix.
- `test_fd_58_format_output_structured(tmp_path, monkeypatch)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L329) — Test structured format output - corresponds to fd's format test.
- `test_fd_65_exec_invalid_utf8_simulation(tmp_path, monkeypatch)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p3a_path_output.py#L369) — Test exec invalid UTF-8 simulation - corresponds to fd's test_exec_invalid_utf8.

