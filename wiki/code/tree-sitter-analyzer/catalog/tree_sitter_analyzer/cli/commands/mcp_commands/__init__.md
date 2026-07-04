---
title: 'Module: tree_sitter_analyzer/cli/commands/mcp_commands/__init__.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/mcp_commands/__init__.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.mcp_commands`/
symbols:
  handle_mcp_commands: handle_mcp_commands().
  _emit_builder_error: _emit_builder_error().
  _TOOL_CLASS_NAMES._TOOL_CLASS_NAMES: _TOOL_CLASS_NAMES._TOOL_CLASS_NAMES.
  _get_tool_class: _get_tool_class().
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/cli/commands/mcp_commands/__init__.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/__init__.py)

## Functions
- `_emit_builder_error(spec: McpCommandSpec, exc: Exception, output_format: str, output_json_fn: Callable[[dict[str, Any]], None], output_error_fn: Callable[[str], None])` — [`L319`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/__init__.py#L319) — Emit a structured error envelope for a build_tool_args failure (#1003).
- `_get_tool_class(tool_attr: str)` — [`L261`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/__init__.py#L261) — Resolve a tool class by its command spec attribute name.
- `handle_mcp_commands(args: Any, output_json_fn: Callable[[dict[str, Any]], None], output_error_fn: Callable[[str], None], output_format_fn: Callable[[], str])` — [`L279`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/__init__.py#L279) — Handle MCP-equivalent CLI commands. Returns exit code or None if not handled.

## Module values
- `_TOOL_CLASS_NAMES` — [`L198`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/__init__.py#L198)
- `__all__` — [`L341`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/__init__.py#L341)

