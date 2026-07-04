---
title: 'Module: tree_sitter_analyzer/mcp/server_utils/tool_registration.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/server_utils/tool_registration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.server_utils.tool_registration`/
symbols:
  register_tools.handle_call_tool: register_tools().handle_call_tool().
  _dispatch_tool: _dispatch_tool().
  logger: logger.
  register_tools.handle_list_tools: register_tools().handle_list_tools().
  _safe_log_error: _safe_log_error().
  _SET_PROJECT_PATH_TOOL: _SET_PROJECT_PATH_TOOL.
  register_tools: register_tools().
  _json_dumps: _json_dumps().
---
# Module: [`tree_sitter_analyzer/mcp/server_utils/tool_registration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/tool_registration.py)

## Functions
- `_dispatch_tool(server_instance: Any, name: str, arguments: dict[str, Any])` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/tool_registration.py#L114) — Route a tool call to the appropriate handler.
- `_json_dumps(obj: Any)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/tool_registration.py#L145)
- `_safe_log_error(msg: str)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/tool_registration.py#L151)
- `handle_call_tool(name: str, arguments: dict[str, Any])` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/tool_registration.py#L59)
- `handle_list_tools()` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/tool_registration.py#L48) — List all available tools.
- `register_tools(server: Any, server_instance: Any)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/tool_registration.py#L39) — Register tool list and call handlers on the MCP server.

## Module values
- `_SET_PROJECT_PATH_TOOL` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/tool_registration.py#L22)
- `logger` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/tool_registration.py#L20)

