---
title: 'Module: tree_sitter_analyzer/mcp/tools/batch_search_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/batch_search_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.batch_search_tool`/
symbols:
  BatchSearchTool.execute: BatchSearchTool#execute().
  BatchSearchTool: BatchSearchTool#
  BatchSearchTool._build_command_for_query: BatchSearchTool#_build_command_for_query().
  BatchSearchTool.get_tool_definition: BatchSearchTool#get_tool_definition().
  BatchSearchTool.validate_arguments: BatchSearchTool#validate_arguments().
  _BATCH_MAX_MATCHES_PER_QUERY: _BATCH_MAX_MATCHES_PER_QUERY.
  BatchSearchTool.get_tool_schema: BatchSearchTool#get_tool_schema().
  BatchSearchTool._resolve_single_root: BatchSearchTool#_resolve_single_root().
  _case_mode: _case_mode().
  _QUERY_ITEM_SCHEMA._QUERY_ITEM_SCHEMA: _QUERY_ITEM_SCHEMA._QUERY_ITEM_SCHEMA.
---
# Module: [`tree_sitter_analyzer/mcp/tools/batch_search_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_search_tool.py)

## Classes
### `BatchSearchTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/batch_search_tool.py:58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_search_tool.py#L58)
- doc: MCP tool that runs multiple ripgrep searches concurrently.
- signature: `class BatchSearchTool(BaseMCPTool):`
- members:
  - `_build_command_for_query(self, query: dict[str, Any])` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_search_tool.py#L144) — Build a ripgrep command for a single query dict.
  - `_resolve_single_root(self, r: str)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_search_tool.py#L137) — Resolve and validate a single root path; fall back to raw value on error.
  - `execute(self, arguments: dict[str, Any])` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_search_tool.py#L181) — Execute all queries in parallel and aggregate results.
  - `get_tool_definition(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_search_tool.py#L77)
  - `get_tool_schema(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_search_tool.py#L61)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_search_tool.py#L107)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`build_rg_command`](fd_rg_utils.md#build_rg_command), [`mirror_summary_line`](base_tool.md#mirror_summary_line), [`handle_mcp_errors`](../utils/error_handler.md#handle_mcp_errors), [`parse_rg_json_lines_to_matches`](fd_rg_result_utils.md#parse_rg_json_lines_to_matches), [`resolve_and_validate_directory_path`](base_tool.md#BaseMCPTool.resolve_and_validate_directory_path), [`run_parallel_rg_searches`](fd_rg_utils.md#run_parallel_rg_searches), [`_BATCH_MAX_MATCHES_PER_QUERY`](batch_search_tool.md#_BATCH_MAX_MATCHES_PER_QUERY), [`DEFAULT_RG_TIMEOUT_MS`](fd_rg_utils.md#DEFAULT_RG_TIMEOUT_MS), [`_QUERY_ITEM_SCHEMA`](batch_search_tool.md#_QUERY_ITEM_SCHEMA._QUERY_ITEM_SCHEMA), [`_case_mode`](batch_search_tool.md#_case_mode)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_search_facade`](search_facade.md#build_search_facade)  (18 test-only)

## Functions
- `_case_mode(case_sensitive: bool | None)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_search_tool.py#L49) — Map the case_sensitive flag to a ripgrep case mode string.

## Module values
- `_BATCH_MAX_MATCHES_PER_QUERY` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_search_tool.py#L16)
- `_QUERY_ITEM_SCHEMA` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_search_tool.py#L20)

