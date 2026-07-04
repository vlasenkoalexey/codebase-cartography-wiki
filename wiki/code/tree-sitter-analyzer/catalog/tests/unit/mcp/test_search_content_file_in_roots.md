---
title: 'Module: tests/unit/mcp/test_search_content_file_in_roots.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_search_content_file_in_roots.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_search_content_file_in_roots`/
symbols:
  test_file_in_roots_returns_canonical_envelope: test_file_in_roots_returns_canonical_envelope().
  test_normal_directory_root_still_succeeds: test_normal_directory_root_still_succeeds().
  test_files_parameter_still_succeeds: test_files_parameter_still_succeeds().
  test_mixed_dir_and_file_in_roots_still_envelope: test_mixed_dir_and_file_in_roots_still_envelope().
  test_nonexistent_root_keeps_existing_error_behavior: test_nonexistent_root_keeps_existing_error_behavior().
  tool: tool().
  project_with_files: project_with_files().
---
# Module: [`tests/unit/mcp/test_search_content_file_in_roots.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_file_in_roots.py)

## Functions
- `project_with_files(tmp_path: Path)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_file_in_roots.py#L31) — Build a small project that contains both directories and real files.
- `test_file_in_roots_returns_canonical_envelope(tool: SearchContentTool, project_with_files: Path)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_file_in_roots.py#L47)
- `test_files_parameter_still_succeeds(tool: SearchContentTool, project_with_files: Path)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_file_in_roots.py#L97)
- `test_mixed_dir_and_file_in_roots_still_envelope(tool: SearchContentTool, project_with_files: Path)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_file_in_roots.py#L114)
- `test_nonexistent_root_keeps_existing_error_behavior(tool: SearchContentTool)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_file_in_roots.py#L134)
- `test_normal_directory_root_still_succeeds(tool: SearchContentTool, project_with_files: Path)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_file_in_roots.py#L79)
- `tool(project_with_files: Path)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_file_in_roots.py#L42)

