---
title: 'Module: tests/unit/mcp/test_find_and_grep_tool_execute.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_find_and_grep_tool_execute.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_find_and_grep_tool_execute`/
symbols:
  tool: tool().
  TestExecuteOptionsAndFeatures.test_execute_file_limit_clamping: TestExecuteOptionsAndFeatures#test_execute_file_limit_clamping().
  sample_project_structure: sample_project_structure().
  TestExecuteErrorPaths: TestExecuteErrorPaths#
  TestExecuteErrorPaths.test_execute_missing_commands: TestExecuteErrorPaths#test_execute_missing_commands().
  TestExecuteErrorPaths.test_execute_fd_failure: TestExecuteErrorPaths#test_execute_fd_failure().
  TestExecuteErrorPaths.test_execute_no_files_found: TestExecuteErrorPaths#test_execute_no_files_found().
  TestExecuteErrorPaths.test_execute_rg_failure: TestExecuteErrorPaths#test_execute_rg_failure().
  TestExecuteErrorPaths.test_execute_file_save_error: TestExecuteErrorPaths#test_execute_file_save_error().
  TestExecuteOutputModes: TestExecuteOutputModes#
  TestExecuteOutputModes.test_execute_total_only_mode: TestExecuteOutputModes#test_execute_total_only_mode().
  TestExecuteOutputModes.test_execute_count_only_matches_mode: TestExecuteOutputModes#test_execute_count_only_matches_mode().
  TestExecuteOutputModes.test_execute_group_by_file_mode: TestExecuteOutputModes#test_execute_group_by_file_mode().
  TestExecuteOutputModes.test_execute_summary_only_mode: TestExecuteOutputModes#test_execute_summary_only_mode().
  TestExecuteOutputModes.test_execute_with_toon_format: TestExecuteOutputModes#test_execute_with_toon_format().
  TestExecuteOptionsAndFeatures: TestExecuteOptionsAndFeatures#
  TestExecuteOptionsAndFeatures.test_execute_with_file_output: TestExecuteOptionsAndFeatures#test_execute_with_file_output().
  TestExecuteOptionsAndFeatures.test_execute_with_suppress_output: TestExecuteOptionsAndFeatures#test_execute_with_suppress_output().
  TestExecuteOptionsAndFeatures.test_execute_with_optimize_paths: TestExecuteOptionsAndFeatures#test_execute_with_optimize_paths().
  TestExecuteOptionsAndFeatures.test_execute_with_gitignore_detection: TestExecuteOptionsAndFeatures#test_execute_with_gitignore_detection().
  TestExecuteOptionsAndFeatures.test_execute_with_sort_path: TestExecuteOptionsAndFeatures#test_execute_with_sort_path().
  TestExecuteOptionsAndFeatures.test_execute_with_max_count: TestExecuteOptionsAndFeatures#test_execute_with_max_count().
  TestExecuteOptionsAndFeatures.test_execute_with_timeout: TestExecuteOptionsAndFeatures#test_execute_with_timeout().
---
# Module: [`tests/unit/mcp/test_find_and_grep_tool_execute.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py)

## Classes
### `TestExecuteErrorPaths`
- def: [`tests/unit/mcp/test_find_and_grep_tool_execute.py:38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L38)
- doc: Tests for execute method error and edge-case paths.
- signature: `class TestExecuteErrorPaths:`
- members:
  - `test_execute_fd_failure(self, tool, sample_project_structure)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L55) — Test execute when fd command fails.
  - `test_execute_file_save_error(self, tool, sample_project_structure)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L132) — Test execute when file save fails.
  - `test_execute_missing_commands(self, tool)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L42) — Test execute fails when fd or rg commands are not found.
  - `test_execute_no_files_found(self, tool, sample_project_structure)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L79) — Test execute when no files are found.
  - `test_execute_rg_failure(self, tool, sample_project_structure)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L105) — Test execute when ripgrep command fails.

### `TestExecuteOptionsAndFeatures`
- def: [`tests/unit/mcp/test_find_and_grep_tool_execute.py:361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L361)
- doc: Tests for execute method with various option flags.
- signature: `class TestExecuteOptionsAndFeatures:`
- members:
  - `test_execute_file_limit_clamping(self, tool, sample_project_structure)` — [`L542`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L542) — Test that file_limit is properly clamped.
  - `test_execute_with_file_output(self, tool, sample_project_structure)` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L365) — Test execute with file output.
  - `test_execute_with_gitignore_detection(self, tool, sample_project_structure)` — [`L473`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L473) — Test that .gitignore detection works.
  - `test_execute_with_max_count(self, tool, sample_project_structure)` — [`L576`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L576) — Test execute with max_count parameter.
  - `test_execute_with_optimize_paths(self, tool, sample_project_structure)` — [`L438`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L438) — Test execute with optimize_paths.
  - `test_execute_with_sort_path(self, tool, sample_project_structure)` — [`L516`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L516) — Test execute with sort by path.
  - `test_execute_with_suppress_output(self, tool, sample_project_structure)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L401) — Test execute with suppress_output.
  - `test_execute_with_timeout(self, tool, sample_project_structure)` — [`L614`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L614) — Test execute with timeout parameter.
- uses (calls/refs, reference-scoped): [`MAX_RESULTS_HARD_CAP`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#MAX_RESULTS_HARD_CAP)

### `TestExecuteOutputModes`
- def: [`tests/unit/mcp/test_find_and_grep_tool_execute.py:169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L169)
- doc: Tests for execute method output mode variants.
- signature: `class TestExecuteOutputModes:`
- members:
  - `test_execute_count_only_matches_mode(self, tool, sample_project_structure)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L203) — Test execute in count_only_matches mode.
  - `test_execute_group_by_file_mode(self, tool, sample_project_structure)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L240) — Test execute in group_by_file mode.
  - `test_execute_summary_only_mode(self, tool, sample_project_structure)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L287) — Test execute in summary_only mode.
  - `test_execute_total_only_mode(self, tool, sample_project_structure)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L173) — Test execute in total_only mode.
  - `test_execute_with_toon_format(self, tool, sample_project_structure)` — [`L325`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L325) — Test execute with toon output format.

## Functions
- `sample_project_structure(tmp_path: Path)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L23) — Create a sample project structure for testing.
- `tool()` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_execute.py#L17) — Create a fresh tool instance for each test.

