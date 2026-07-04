---
title: 'Module: tree_sitter_analyzer/mcp/tools/list_files_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/list_files_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.list_files_tool`/
symbols:
  ListFilesTool.execute: ListFilesTool#execute().
  ListFilesTool: ListFilesTool#
  ListFilesTool.validate_arguments: ListFilesTool#validate_arguments().
  ListFilesTool._respond_count_only: ListFilesTool#_respond_count_only().
  ListFilesTool._resolve_real_total: ListFilesTool#_resolve_real_total().
  ListFilesTool._resolve_no_ignore: ListFilesTool#_resolve_no_ignore().
  ListFilesTool.get_tool_schema: ListFilesTool#get_tool_schema().
  _check_str_list: _check_str_list().
  ListFilesTool.get_tool_definition: ListFilesTool#get_tool_definition().
  ListFilesTool._validate_single_root: ListFilesTool#_validate_single_root().
  ListFilesTool._validate_roots: ListFilesTool#_validate_roots().
  logger: logger.
  _RECOUNT_BUDGET_MS: _RECOUNT_BUDGET_MS.
  _decode_error: _decode_error().
  _is_string_list: _is_string_list().
  _check_str: _check_str().
  _check_bool: _check_bool().
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/mcp/tools/list_files_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_tool.py)

## Classes
### `ListFilesTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/list_files_tool.py:71`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_tool.py#L71) — documented in [tree_sitter_analyzer-mcp-server](../../../../concepts/tree_sitter_analyzer-mcp-server.md)
- doc: MCP tool that wraps fd to list files with safety limits.
- signature: `class ListFilesTool(BaseMCPTool):`
- members:
  - `_resolve_no_ignore(self, arguments: dict[str, Any])` — [`L306`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_tool.py#L306) — Determine no_ignore flag with smart gitignore detection.
  - `_resolve_real_total(self, lines: list[str], limit: int, arguments: dict[str, Any], roots: list[str], effective_types: list[str] | None, no_ignore: bool)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_tool.py#L250) — Recount without --max-results when fd may have truncated.
  - `_respond_count_only(self, lines: list[str], elapsed_ms: int, arguments: dict[str, Any], limit: int, *, real_total: int | None = None, total_count_known: bool = True)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_tool.py#L326) — Return count-only response through the shared response helper.
  - `_validate_roots(self, roots: list[str])` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_tool.py#L114) — Resolve and validate each root directory path.
  - `_validate_single_root(self, r: str)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_tool.py#L105) — Validate and resolve one root directory path.
  - `execute(self, arguments: dict[str, Any])` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_tool.py#L188) — Execute fd-based file listing with safety limits.
  - `get_tool_definition(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_tool.py#L77) — Return the MCP tool name, description, and input schema.
  - `get_tool_schema(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_tool.py#L74)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_tool.py#L126) — Validate roots and all option types.
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`_respond_detailed`](list_files_helpers.md#_respond_detailed), [`handle_mcp_errors`](../utils/error_handler.md#handle_mcp_errors), [`_respond_count_only`](list_files_helpers.md#_respond_count_only), [`get_default_detector`](../utils/gitignore_detector.md#get_default_detector), [`resolve_and_validate_directory_path`](base_tool.md#BaseMCPTool.resolve_and_validate_directory_path), [`run_command_capture`](fd_rg_utils.md#run_command_capture), [`should_use_no_ignore`](../utils/gitignore_detector.md#GitignoreDetector.should_use_no_ignore), [`MAX_RESULTS_HARD_CAP`](fd_rg_utils.md#MAX_RESULTS_HARD_CAP), [`get_detection_info`](../utils/gitignore_detector.md#GitignoreDetector.get_detection_info), [`clamp_int`](fd_rg_utils.md#clamp_int), [`check_external_command`](fd_rg_utils.md#check_external_command), [`limit`](list_files_helpers.md#CountResponseContext.limit), [`_build_fd_command`](list_files_helpers.md#_build_fd_command), [`limit`](list_files_helpers.md#DetailedResponseContext.limit), [`DEFAULT_RESULTS_LIMIT`](fd_rg_utils.md#DEFAULT_RESULTS_LIMIT), [`_check_str_list`](list_files_tool.md#_check_str_list), [`CountResponseContext`](list_files_helpers.md#CountResponseContext), [`DetailedResponseContext`](list_files_helpers.md#DetailedResponseContext), [`_decode_lines`](list_files_helpers.md#_decode_lines), [`arguments`](list_files_helpers.md#CountResponseContext.arguments), [`arguments`](list_files_helpers.md#DetailedResponseContext.arguments), [`logger`](list_files_tool.md#logger), [`no_ignore`](list_files_helpers.md#DetailedResponseContext.no_ignore), [`TOOL_SCHEMA`](list_files_helpers.md#TOOL_SCHEMA.TOOL_SCHEMA), [`_RECOUNT_BUDGET_MS`](list_files_tool.md#_RECOUNT_BUDGET_MS), [`_missing_fd_response`](list_files_helpers.md#_missing_fd_response), [`_resolve_effective_types`](list_files_helpers.md#_resolve_effective_types), [`effective_types`](list_files_helpers.md#DetailedResponseContext.effective_types), [`elapsed_ms`](list_files_helpers.md#CountResponseContext.elapsed_ms), [`elapsed_ms`](list_files_helpers.md#DetailedResponseContext.elapsed_ms), [`lines`](list_files_helpers.md#CountResponseContext.lines), [`lines`](list_files_helpers.md#DetailedResponseContext.lines), [`project_root`](list_files_helpers.md#CountResponseContext.project_root), [`project_root`](list_files_helpers.md#DetailedResponseContext.project_root), [`_check_bool`](list_files_tool.md#_check_bool), [`_check_str`](list_files_tool.md#_check_str), [`_decode_error`](list_files_tool.md#_decode_error)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_project_facade`](project_facade.md#build_project_facade), [`attach_tool_aliases`](../_server_helpers.md#attach_tool_aliases), [`_run`](../../cli/commands/list_files_cli.md#_run), [`_load_mcp_tool_class`](../../../compatibility_test/scripts/run_compatibility_test.md#_load_mcp_tool_class)  (132 test-only)

## Functions
- `_check_bool(key: str, arguments: dict[str, Any])` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_tool.py#L56) — Raise ValueError if arguments[key] is present but not a bool.
- `_check_str(key: str, arguments: dict[str, Any])` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_tool.py#L50) — Raise ValueError if arguments[key] is present but not a str.
- `_check_str_list(arr: str, arguments: dict[str, Any])` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_tool.py#L62) — Raise ValueError if arguments[arr] is present but not a list of strings.
- `_decode_error(err: bytes)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_tool.py#L40) — Decode fd error bytes to a displayable string.
- `_is_string_list(val: Any)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_tool.py#L45) — Return True iff val is a list of strings.

## Module values
- `_RECOUNT_BUDGET_MS` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_tool.py#L37)
- `__all__` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_tool.py#L68)
- `logger` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/list_files_tool.py#L33)

