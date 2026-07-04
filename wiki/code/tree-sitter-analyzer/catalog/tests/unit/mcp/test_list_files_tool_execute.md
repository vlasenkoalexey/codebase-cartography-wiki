---
title: 'Module: tests/unit/mcp/test_list_files_tool_execute.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_list_files_tool_execute.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_list_files_tool_execute`/
symbols:
  tool: tool().
  TestExecute.test_execute_limit_clamping: TestExecute#test_execute_limit_clamping().
  sample_project_structure: sample_project_structure().
  TestExecute: TestExecute#
  TestExecute.test_execute_fd_not_found: TestExecute#test_execute_fd_not_found().
  TestExecute.test_execute_success: TestExecute#test_execute_success().
  TestExecute.test_execute_count_only_mode: TestExecute#test_execute_count_only_mode().
  TestExecute.test_execute_with_file_output: TestExecute#test_execute_with_file_output().
  TestExecute.test_execute_with_suppress_output: TestExecute#test_execute_with_suppress_output().
  TestExecute.test_execute_with_output_format_toon: TestExecute#test_execute_with_output_format_toon().
  TestExecute.test_execute_fd_command_failure: TestExecute#test_execute_fd_command_failure().
  TestExecute.test_execute_with_extensions_auto_types: TestExecute#test_execute_with_extensions_auto_types().
  TestExecute.test_execute_with_gitignore_detection: TestExecute#test_execute_with_gitignore_detection().
  TestExecute.test_execute_truncation_defensive: TestExecute#test_execute_truncation_defensive().
---
# Module: [`tests/unit/mcp/test_list_files_tool_execute.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_list_files_tool_execute.py)

## Classes
### `TestExecute`
- def: [`tests/unit/mcp/test_list_files_tool_execute.py:33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_list_files_tool_execute.py#L33)
- signature: `class TestExecute:`
- members:
  - `test_execute_count_only_mode(self, tool, sample_project_structure)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_list_files_tool_execute.py#L80)
  - `test_execute_fd_command_failure(self, tool, sample_project_structure)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_list_files_tool_execute.py#L225)
  - `test_execute_fd_not_found(self, tool)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_list_files_tool_execute.py#L35)
  - `test_execute_limit_clamping(self, tool, sample_project_structure)` — [`L323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_list_files_tool_execute.py#L323)
  - `test_execute_success(self, tool, sample_project_structure)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_list_files_tool_execute.py#L47)
  - `test_execute_truncation_defensive(self, tool, sample_project_structure)` — [`L359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_list_files_tool_execute.py#L359)
  - `test_execute_with_extensions_auto_types(self, tool, sample_project_structure)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_list_files_tool_execute.py#L255)
  - `test_execute_with_file_output(self, tool, sample_project_structure)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_list_files_tool_execute.py#L113)
  - `test_execute_with_gitignore_detection(self, tool, sample_project_structure)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_list_files_tool_execute.py#L287)
  - `test_execute_with_output_format_toon(self, tool, sample_project_structure)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_list_files_tool_execute.py#L189)
  - `test_execute_with_suppress_output(self, tool, sample_project_structure)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_list_files_tool_execute.py#L150)
- uses (calls/refs, reference-scoped): [`MAX_RESULTS_HARD_CAP`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#MAX_RESULTS_HARD_CAP)

## Functions
- `sample_project_structure(tmp_path: Path)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_list_files_tool_execute.py#L18)
- `tool()` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_list_files_tool_execute.py#L13)

