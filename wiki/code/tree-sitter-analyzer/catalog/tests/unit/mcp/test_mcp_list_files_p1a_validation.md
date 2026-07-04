---
title: 'Module: tests/unit/mcp/test_mcp_list_files_p1a_validation.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_list_files_p1a_validation.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_list_files_p1a_validation`/
symbols:
  test_list_files_exec_happy_path: test_list_files_exec_happy_path().
  test_list_files_exclude: test_list_files_exclude().
  test_list_files_count_only: test_list_files_count_only().
  test_list_files_error_handling: test_list_files_error_handling().
  test_list_files_with_pattern_and_no_pattern: test_list_files_with_pattern_and_no_pattern().
  test_list_files_with_size_filters: test_list_files_with_size_filters().
  test_list_files_with_time_filters: test_list_files_with_time_filters().
  test_list_files_with_types_and_extensions: test_list_files_with_types_and_extensions().
  test_list_files_with_depth_and_symlinks: test_list_files_with_depth_and_symlinks().
  test_list_files_with_full_path_match: test_list_files_with_full_path_match().
  test_list_files_metadata_fields: test_list_files_metadata_fields().
  test_list_files_validation_requires_roots: test_list_files_validation_requires_roots().
  test_list_files_validation_invalid_types: test_list_files_validation_invalid_types().
  test_list_files_validation_comprehensive: test_list_files_validation_comprehensive().
  test_list_files_exec_happy_path.fake_run: test_list_files_exec_happy_path().fake_run().
  test_list_files_exclude.fake_run: test_list_files_exclude().fake_run().
  test_list_files_count_only.fake_run: test_list_files_count_only().fake_run().
  test_list_files_error_handling.fake_run: test_list_files_error_handling().fake_run().
  test_list_files_with_pattern_and_no_pattern.fake_run: test_list_files_with_pattern_and_no_pattern().fake_run().
  test_list_files_with_size_filters.fake_run: test_list_files_with_size_filters().fake_run().
  test_list_files_with_time_filters.fake_run: test_list_files_with_time_filters().fake_run().
  test_list_files_with_types_and_extensions.fake_run: test_list_files_with_types_and_extensions().fake_run().
  test_list_files_with_depth_and_symlinks.fake_run: test_list_files_with_depth_and_symlinks().fake_run().
  test_list_files_with_full_path_match.fake_run: test_list_files_with_full_path_match().fake_run().
  test_list_files_metadata_fields.fake_run: test_list_files_metadata_fields().fake_run().
  mock_external_commands: mock_external_commands().
---
# Module: [`tests/unit/mcp/test_mcp_list_files_p1a_validation.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py)

## Functions
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L43)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L73)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L111)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L138)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L182)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L231)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L255)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L280)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L304)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L329)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L355)
- `mock_external_commands(monkeypatch)` — [`L7`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L7) — Auto-mock external command availability checks for all tests in this module.
- `test_list_files_count_only(monkeypatch, tmp_path)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L99) — Test list_files tool with count_only option.
- `test_list_files_error_handling(monkeypatch, tmp_path)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L134) — Test ListFilesTool error handling when fd command fails.
- `test_list_files_exclude(monkeypatch, tmp_path)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L62) — Test ListFilesTool with exclude patterns to filter out specific directories.
- `test_list_files_exec_happy_path(monkeypatch, tmp_path)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L35) — Test successful execution of ListFilesTool with file extension filtering.
- `test_list_files_metadata_fields(monkeypatch, tmp_path)` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L347) — Test ListFilesTool returns correct metadata fields.
- `test_list_files_validation_comprehensive(tmp_path)` — [`L380`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L380) — Test comprehensive parameter validation for ListFilesTool.
- `test_list_files_validation_invalid_types(tmp_path)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L153) — Test ListFilesTool validation with invalid parameter types.
- `test_list_files_validation_requires_roots(tmp_path)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L16) — ``roots`` is required when no project_root is configured.
- `test_list_files_with_depth_and_symlinks(monkeypatch, tmp_path)` — [`L300`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L300) — Test ListFilesTool with depth limit and symlink following.
- `test_list_files_with_full_path_match(monkeypatch, tmp_path)` — [`L325`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L325) — Test ListFilesTool with full path matching.
- `test_list_files_with_pattern_and_no_pattern(monkeypatch, tmp_path)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L176) — Test ListFilesTool with and without pattern to verify fd command building.
- `test_list_files_with_size_filters(monkeypatch, tmp_path)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L221) — Test ListFilesTool with size filter parameters.
- `test_list_files_with_time_filters(monkeypatch, tmp_path)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L251) — Test ListFilesTool with time-based filters.
- `test_list_files_with_types_and_extensions(monkeypatch, tmp_path)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_list_files_p1a_validation.py#L276) — Test ListFilesTool with file type and extension filters.

