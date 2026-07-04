---
title: 'Module: tree_sitter_analyzer/mcp/tools/find_and_grep_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/find_and_grep_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.find_and_grep_tool`/
symbols:
  FindAndGrepTool: FindAndGrepTool#
  FindAndGrepTool.execute: FindAndGrepTool#execute().
  FindAndGrepTool._execute_rg_modes: FindAndGrepTool#_execute_rg_modes().
  FindAndGrepTool._execute_full_match_mode: FindAndGrepTool#_execute_full_match_mode().
  _build_count_only_context: _build_count_only_context().
  FindAndGrepTool._run_fd: FindAndGrepTool#_run_fd().
  FindAndGrepTool.validate_arguments: FindAndGrepTool#validate_arguments().
  FindAndGrepTool._run_rg: FindAndGrepTool#_run_rg().
  FindAndGrepTool._on_project_root_changed: FindAndGrepTool#_on_project_root_changed().
  FindAndGrepTool.file_output_manager: FindAndGrepTool#file_output_manager.
  FindAndGrepTool.get_tool_schema: FindAndGrepTool#get_tool_schema().
  FindAndGrepTool.get_tool_definition: FindAndGrepTool#get_tool_definition().
  FindAndGrepTool._validate_roots: FindAndGrepTool#_validate_roots().
  FindAndGrepTool.__init__: FindAndGrepTool#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/find_and_grep_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_tool.py)

## Classes
### `FindAndGrepTool`  ·  implements/extends BaseMCPTool, FindAndGrepRespondMixin
- def: [`tree_sitter_analyzer/mcp/tools/find_and_grep_tool.py:42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_tool.py#L42) — documented in [tree_sitter_analyzer-mcp-server](../../../../concepts/tree_sitter_analyzer-mcp-server.md)
- doc: MCP tool that composes fd and ripgrep with safety limits and metadata.
- signature: `class FindAndGrepTool(FindAndGrepRespondMixin, BaseMCPTool):`
- members:
  - `__init__(self, project_root: str | None = None)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_tool.py#L49) — Initialize with optional project root for path resolution.
  - `_execute_full_match_mode(self, context: FindAndGrepFullMatchContext, *, files: list[str])` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_tool.py#L216) — Parse rg matches and dispatch the selected response mode.
  - `_execute_rg_modes(self, context: FindAndGrepRgModeContext)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_tool.py#L172) — Run ripgrep and dispatch count or match response modes.
  - `_run_fd(self, arguments: dict[str, Any], roots: list[str])` — [`L273`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_tool.py#L273) — Run fd command. Returns (files, elapsed_ms, truncated) or (error_dict, 0, False).
  - `_run_rg(self, arguments: dict[str, Any], files: list[str])` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_tool.py#L305) — Run ripgrep on found files. Returns (rc, output, elapsed_ms) or error dict.
  - `_validate_roots(self, roots: list[str])` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_tool.py#L97) — Resolve and validate each root directory path.
  - `execute(self, arguments: dict[str, Any])` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_tool.py#L146) — Execute fd+rg pipeline: find files then grep contents. — documented in [tree_sitter_analyzer-mcp-tools-facade_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-facade_tool.md)
  - `get_tool_definition(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_tool.py#L60) — Return the MCP tool name, description, and input schema.
  - `get_tool_schema(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_tool.py#L57)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_tool.py#L108) — Validate roots and query arguments.
  - `file_output_manager` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_tool.py#L51)
- protocol/private: `_on_project_root_changed`[`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_tool.py#L54)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`FileOutputManager`](../utils/file_output_manager.md#FileOutputManager), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`build_count_only_response`](find_and_grep_helpers.md#build_count_only_response), [`handle_mcp_errors`](../utils/error_handler.md#handle_mcp_errors), [`_build_count_only_context`](find_and_grep_tool.md#_build_count_only_context), [`parse_rg_json_lines_to_matches`](fd_rg_result_utils.md#parse_rg_json_lines_to_matches), [`get_managed_instance`](../utils/file_output_manager.md#FileOutputManager.get_managed_instance), [`get_default_detector`](../utils/gitignore_detector.md#get_default_detector), [`_respond_grouped`](find_and_grep_response.md#FindAndGrepRespondMixin._respond_grouped), [`resolve_and_validate_directory_path`](base_tool.md#BaseMCPTool.resolve_and_validate_directory_path), [`_respond_full`](find_and_grep_response.md#FindAndGrepRespondMixin._respond_full), [`run_command_capture`](fd_rg_utils.md#run_command_capture), [`_respond_summary`](find_and_grep_response.md#FindAndGrepRespondMixin._respond_summary), [`TOOL_SCHEMA`](find_and_grep_helpers.md#TOOL_SCHEMA.TOOL_SCHEMA), [`build_empty_response`](find_and_grep_helpers.md#build_empty_response), [`MAX_RESULTS_HARD_CAP`](fd_rg_utils.md#MAX_RESULTS_HARD_CAP), [`optimize_match_paths`](fd_rg_result_utils.md#optimize_match_paths), [`resolve_real_total`](find_and_grep_execution.md#resolve_real_total), [`build_search_meta`](find_and_grep_helpers.md#build_search_meta), [`parse_rg_count_output`](fd_rg_utils.md#parse_rg_count_output), [`clamp_int`](fd_rg_utils.md#clamp_int), [`FindAndGrepFullMatchContext`](find_and_grep_helpers.md#FindAndGrepFullMatchContext), [`build_missing_commands_response`](find_and_grep_helpers.md#build_missing_commands_response), [`files`](find_and_grep_helpers.md#FindAndGrepRgModeContext.files), [`get_missing_commands`](fd_rg_utils.md#get_missing_commands), [`FindAndGrepRgModeContext`](find_and_grep_helpers.md#FindAndGrepRgModeContext), [`build_fd_command_from_arguments`](find_and_grep_execution.md#build_fd_command_from_arguments), [`build_rg_command_from_arguments`](find_and_grep_execution.md#build_rg_command_from_arguments), [`resolve_fd_no_ignore`](find_and_grep_execution.md#resolve_fd_no_ignore), [`fd_elapsed_ms`](find_and_grep_helpers.md#FindAndGrepFullMatchContext.fd_elapsed_ms), [`fd_elapsed_ms`](find_and_grep_helpers.md#FindAndGrepRgModeContext.fd_elapsed_ms), [`output_format`](find_and_grep_helpers.md#FindAndGrepRgModeContext.output_format), [`truncated_fd`](find_and_grep_helpers.md#FindAndGrepRgModeContext.truncated_fd), [`arguments`](find_and_grep_helpers.md#FindAndGrepFullMatchContext.arguments), [`arguments`](find_and_grep_helpers.md#FindAndGrepRgModeContext.arguments), [`output_format`](find_and_grep_helpers.md#FindAndGrepFullMatchContext.output_format), [`rg_elapsed_ms`](find_and_grep_helpers.md#FindAndGrepFullMatchContext.rg_elapsed_ms), [`rg_out`](find_and_grep_helpers.md#FindAndGrepFullMatchContext.rg_out)  (+9 more)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_search_facade`](search_facade.md#build_search_facade), [`_run`](../../cli/commands/find_and_grep_cli.md#_run), [`attach_tool_aliases`](../_server_helpers.md#attach_tool_aliases), [`_load_mcp_tool_class`](../../../compatibility_test/scripts/run_compatibility_test.md#_load_mcp_tool_class), [`FindAndGrepRespondMixin`](find_and_grep_response.md#FindAndGrepRespondMixin)  (77 test-only)

## Functions
- `_build_count_only_context(context: FindAndGrepRgModeContext, count_data: dict[str, int], searched_file_count: int, rg_elapsed_ms: int)` — [`L323`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_tool.py#L323) — Build the count-only response context for the current rg run.

