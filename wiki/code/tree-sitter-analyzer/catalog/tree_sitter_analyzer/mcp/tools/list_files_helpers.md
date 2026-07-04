---
title: 'Module: tree_sitter_analyzer/mcp/tools/list_files_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/list_files_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.list_files_helpers`/
symbols:
  _respond_detailed: _respond_detailed().
  _respond_count_only: _respond_count_only().
  _build_agent_summary: _build_agent_summary().
  _save_to_file: _save_to_file().
  _save_count_output: _save_count_output().
  _save_detailed_output: _save_detailed_output().
  CountResponseContext.limit: CountResponseContext#limit.
  _build_fd_command: _build_fd_command().
  DetailedResponseContext.limit: DetailedResponseContext#limit.
  _parse_fd_output: _parse_fd_output().
  _parse_fd_path: _parse_fd_path().
  CountResponseContext: CountResponseContext#
  CountResponseContext.arguments: CountResponseContext#arguments.
  DetailedResponseContext: DetailedResponseContext#
  DetailedResponseContext.arguments: DetailedResponseContext#arguments.
  DetailedResponseContext.no_ignore: DetailedResponseContext#no_ignore.
  _decode_lines: _decode_lines().
  CountResponseContext.lines: CountResponseContext#lines.
  CountResponseContext.elapsed_ms: CountResponseContext#elapsed_ms.
  CountResponseContext.project_root: CountResponseContext#project_root.
  DetailedResponseContext.lines: DetailedResponseContext#lines.
  DetailedResponseContext.elapsed_ms: DetailedResponseContext#elapsed_ms.
  DetailedResponseContext.effective_types: DetailedResponseContext#effective_types.
  DetailedResponseContext.project_root: DetailedResponseContext#project_root.
  build_query_info: build_query_info().
  _missing_fd_response: _missing_fd_response().
  _resolve_effective_types: _resolve_effective_types().
  _attach_total_count_metadata: _attach_total_count_metadata().
  _is_suppressed_file_response: _is_suppressed_file_response().
  _build_list_files_next_steps: _build_list_files_next_steps().
  TOOL_SCHEMA.TOOL_SCHEMA: TOOL_SCHEMA.TOOL_SCHEMA.
  logger: logger.
  _suppressed_count_response: _suppressed_count_response().
  _suppressed_detailed_response: _suppressed_detailed_response().
  _file_metadata: _file_metadata().
  _summary_risk: _summary_risk().
  _summary_next_step: _summary_next_step().
  _summary_suggested_tool: _summary_suggested_tool().
  _summary_stop_condition: _summary_stop_condition().
---
# Module: [`tree_sitter_analyzer/mcp/tools/list_files_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py)

## Classes
### `CountResponseContext`
- def: [`tree_sitter_analyzer/mcp/tools/list_files_helpers.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L20)
- signature: `class CountResponseContext:`
- members:
  - `arguments` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L23)
  - `elapsed_ms` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L22)
  - `limit` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L24)
  - `lines` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L21)
  - `project_root` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L25)
- used by: [`_respond_count_only`](list_files_helpers.md#_respond_count_only), [`_respond_count_only`](list_files_tool.md#ListFilesTool._respond_count_only)

### `DetailedResponseContext`
- def: [`tree_sitter_analyzer/mcp/tools/list_files_helpers.py:29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L29)
- signature: `class DetailedResponseContext:`
- members:
  - `arguments` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L32)
  - `effective_types` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L35)
  - `elapsed_ms` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L31)
  - `limit` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L33)
  - `lines` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L30)
  - `no_ignore` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L34)
  - `project_root` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L36)
- used by: [`execute`](list_files_tool.md#ListFilesTool.execute), [`_respond_detailed`](list_files_helpers.md#_respond_detailed)

## Functions
- `_attach_total_count_metadata(result: dict[str, Any], *, displayed_count: int, real_total: int | None, total_count_known: bool, truncated: bool)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L329) — Attach H3-fix fields so callers can detect truncation honestly.
- `_build_agent_summary(*, count: int, truncated: bool, count_only: bool, limit: int, no_ignore: bool)` — [`L567`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L567) — Summarize list_files output for immediate agent decision-making.
- `_build_fd_command(arguments: dict[str, Any], roots: list[str], limit: int, effective_types: list[str] | None, no_ignore: bool)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L212) — Build the fd command from validated list_files arguments.
- `_build_list_files_next_steps(*, count: int, truncated: bool, count_only: bool, limit: int)` — [`L604`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L604) — Suggest follow-up tools for the list_files response.
- `_decode_lines(output: bytes)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L248) — Decode command output into non-empty stripped lines.
- `_file_metadata(path: str, is_dir: bool)` — [`L556`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L556) — Return size and mtime for files, leaving directories empty.
- `_is_suppressed_file_response(response: dict[str, Any])` — [`L523`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L523)
- `_missing_fd_response()` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L203)
- `_parse_fd_output(lines: list[str], effective_types: list[str] | None)` — [`L527`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L527) — Parse fd output lines into structured results with file metadata.
- `_parse_fd_path(path: str, types_only_files: bool)` — [`L539`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L539) — Parse one fd output path.
- `_resolve_effective_types(arguments: dict[str, Any])` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L257) — Determine effective fd type filter from arguments.
- `_respond_count_only(context: CountResponseContext, *, real_total: int | None = None, total_count_known: bool = True)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L265) — Return count-only response with optional file output.
- `_respond_detailed(context: DetailedResponseContext, *, real_total: int | None = None, total_count_known: bool = True)` — [`L352`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L352) — Return detailed file listing with metadata and optional file output.
- `_save_count_output(project_root: str | None, arguments: dict[str, Any], limit: int, result: dict[str, Any])` — [`L434`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L434) — Save count-only output and return response additions.
- `_save_detailed_output(project_root: str | None, arguments: dict[str, Any], limit: int, no_ignore: bool, result: dict[str, Any])` — [`L459`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L459) — Save detailed output and return response additions.
- `_save_to_file(project_root: str | None, content: dict[str, Any], output_file: str, arguments: dict[str, Any])` — [`L485`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L485) — Save content to output file via FileOutputManager.
- `_summary_next_step(count: int, truncated: bool, count_only: bool, limit: int)` — [`L654`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L654)
- `_summary_risk(count: int, truncated: bool, limit: int)` — [`L644`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L644)
- `_summary_stop_condition(count: int, truncated: bool, limit: int)` — [`L678`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L678)
- `_summary_suggested_tool(count: int, truncated: bool, count_only: bool, limit: int)` — [`L666`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L666)
- `_suppressed_count_response(result: dict[str, Any], saved: str)` — [`L502`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L502)
- `_suppressed_detailed_response(result: dict[str, Any], saved: str)` — [`L513`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L513)
- `build_query_info(arguments: dict[str, Any], limit: int, no_ignore: bool)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L180)

## Module values
- `TOOL_SCHEMA` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L40)
- `logger` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_helpers.py#L16)

