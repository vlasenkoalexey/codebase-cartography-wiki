---
title: 'Module: tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.find_and_grep_helpers`/
symbols:
  build_count_only_response: build_count_only_response().
  TOOL_SCHEMA.TOOL_SCHEMA: TOOL_SCHEMA.TOOL_SCHEMA.
  build_empty_response: build_empty_response().
  _handle_file_output: _handle_file_output().
  handle_output: handle_output().
  build_search_meta: build_search_meta().
  FindAndGrepCountOnlyContext: FindAndGrepCountOnlyContext#
  FindAndGrepCountOnlyContext.output_format: FindAndGrepCountOnlyContext#output_format.
  FindAndGrepFullMatchContext: FindAndGrepFullMatchContext#
  build_missing_commands_response: build_missing_commands_response().
  _make_minimal: _make_minimal().
  FindAndGrepCountOnlyContext.arguments: FindAndGrepCountOnlyContext#arguments.
  FindAndGrepCountOnlyContext.count_data: FindAndGrepCountOnlyContext#count_data.
  FindAndGrepRgModeContext.files: FindAndGrepRgModeContext#files.
  FindAndGrepCountOnlyContext.searched_file_count: FindAndGrepCountOnlyContext#searched_file_count.
  FindAndGrepCountOnlyContext.truncated: FindAndGrepCountOnlyContext#truncated.
  FindAndGrepCountOnlyContext.fd_elapsed_ms: FindAndGrepCountOnlyContext#fd_elapsed_ms.
  FindAndGrepCountOnlyContext.rg_elapsed_ms: FindAndGrepCountOnlyContext#rg_elapsed_ms.
  FindAndGrepRgModeContext: FindAndGrepRgModeContext#
  FindAndGrepFullMatchContext.fd_elapsed_ms: FindAndGrepFullMatchContext#fd_elapsed_ms.
  FindAndGrepRgModeContext.fd_elapsed_ms: FindAndGrepRgModeContext#fd_elapsed_ms.
  FindAndGrepRgModeContext.truncated_fd: FindAndGrepRgModeContext#truncated_fd.
  FindAndGrepRgModeContext.output_format: FindAndGrepRgModeContext#output_format.
  FindAndGrepFullMatchContext.arguments: FindAndGrepFullMatchContext#arguments.
  FindAndGrepFullMatchContext.rg_out: FindAndGrepFullMatchContext#rg_out.
  FindAndGrepFullMatchContext.rg_elapsed_ms: FindAndGrepFullMatchContext#rg_elapsed_ms.
  FindAndGrepFullMatchContext.searched_file_count: FindAndGrepFullMatchContext#searched_file_count.
  FindAndGrepFullMatchContext.truncated_fd: FindAndGrepFullMatchContext#truncated_fd.
  FindAndGrepFullMatchContext.output_format: FindAndGrepFullMatchContext#output_format.
  FindAndGrepRgModeContext.arguments: FindAndGrepRgModeContext#arguments.
  logger: logger.
---
# Module: [`tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py)

## Classes
### `FindAndGrepCountOnlyContext`
- def: [`tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py:149`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L149)
- doc: State needed to build a count-only find_and_grep response.
- signature: `class FindAndGrepCountOnlyContext:`
- members:
  - `arguments` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L152)
  - `count_data` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L153)
  - `fd_elapsed_ms` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L157)
  - `output_format` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L154)
  - `rg_elapsed_ms` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L158)
  - `searched_file_count` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L155)
  - `truncated` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L156)
- used by: [`build_count_only_response`](find_and_grep_helpers.md#build_count_only_response), [`_build_count_only_context`](find_and_grep_tool.md#_build_count_only_context)  (6 test-only)

### `FindAndGrepFullMatchContext`
- def: [`tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py:136`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L136)
- doc: State needed to build full, summary, or grouped match responses.
- signature: `class FindAndGrepFullMatchContext:`
- members:
  - `arguments` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L139)
  - `fd_elapsed_ms` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L141)
  - `output_format` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L145)
  - `rg_elapsed_ms` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L142)
  - `rg_out` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L140)
  - `searched_file_count` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L143)
  - `truncated_fd` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L144)
- used by: [`_execute_rg_modes`](find_and_grep_tool.md#FindAndGrepTool._execute_rg_modes), [`_execute_full_match_mode`](find_and_grep_tool.md#FindAndGrepTool._execute_full_match_mode)  (4 test-only)

### `FindAndGrepRgModeContext`
- def: [`tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py:162`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L162)
- doc: State needed after fd has produced candidate files.
- signature: `class FindAndGrepRgModeContext:`
- members:
  - `arguments` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L165)
  - `fd_elapsed_ms` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L167)
  - `files` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L166)
  - `output_format` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L169)
  - `truncated_fd` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L168)
- used by: [`execute`](find_and_grep_tool.md#FindAndGrepTool.execute), [`_execute_rg_modes`](find_and_grep_tool.md#FindAndGrepTool._execute_rg_modes), [`_build_count_only_context`](find_and_grep_tool.md#_build_count_only_context)  (2 test-only)

## Functions
- `_handle_file_output(result: dict[str, Any], output_file: str, suppress_output: bool, arguments: dict[str, Any], file_output_manager: Any, matches: list[dict[str, Any]] | None)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L320) — Handle saving results to a file.
- `_make_minimal(result: dict[str, Any], include_summary: bool = False)` — [`L380`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L380) — Create a minimal response for suppress_output mode.
- `build_count_only_response(context: FindAndGrepCountOnlyContext)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L253) — Build a count-only response from parsed ripgrep count output.
- `build_empty_response(arguments: dict[str, Any], *, truncated: bool, fd_elapsed_ms: int)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L215) — Build the response returned when fd finds no candidate files.
- `build_missing_commands_response(missing_commands: list[str])` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L172) — Return an install hint when required fd/rg commands are missing.
- `build_search_meta(*, searched_file_count: int, truncated: bool, fd_elapsed_ms: int, rg_elapsed_ms: int, case: str | None = None)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L186) — Build the shared metadata block for find_and_grep responses.
- `handle_output(result: dict[str, Any], arguments: dict[str, Any], file_output_manager: Any, matches: list[dict[str, Any]] | None = None)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L290) — Handle output_file and suppress_output logic.

## Module values
- `TOOL_SCHEMA` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L20)
- `logger` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.py#L18)

