---
title: 'Module: tree_sitter_analyzer/cli/commands/mcp_command_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/mcp_command_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.mcp_command_helpers`/
symbols:
  McpCommandSpec: McpCommandSpec#
  McpCommandSpec.flag_name: McpCommandSpec#flag_name.
  McpCommandSpec.build_tool_args: McpCommandSpec#build_tool_args.
  McpCommandSpec.label: McpCommandSpec#label.
  McpCommandSpec.tool_attr: McpCommandSpec#tool_attr.
  validate_mcp_command_args: validate_mcp_command_args().
  find_selected_mcp_command: find_selected_mcp_command().
  McpCommandSpec.required_file_error: McpCommandSpec#required_file_error.
  McpCommandSpec.value_arg_name: McpCommandSpec#value_arg_name.
  build_mcp_tool_args: build_mcp_tool_args().
  McpCommandSpec.required_value_error: McpCommandSpec#required_value_error.
  McpCommandSpec.requires_file: McpCommandSpec#requires_file.
  McpCommandSpec.active_value: McpCommandSpec#active_value.
---
# Module: [`tree_sitter_analyzer/cli/commands/mcp_command_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_command_helpers.py)

## Classes
### `McpCommandSpec`
- def: [`tree_sitter_analyzer/cli/commands/mcp_command_helpers.py:12`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_command_helpers.py#L12)
- doc: Declarative mapping from a CLI flag to an MCP-equivalent tool call.
- signature: `class McpCommandSpec:`
- members:
  - `active_value` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_command_helpers.py#L37)
  - `build_tool_args` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_command_helpers.py#L34)
  - `flag_name` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_command_helpers.py#L31)
  - `label` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_command_helpers.py#L33)
  - `required_file_error` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_command_helpers.py#L35)
  - `required_value_error` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_command_helpers.py#L39)
  - `requires_file` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_command_helpers.py#L36)
  - `tool_attr` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_command_helpers.py#L32)
  - `value_arg_name` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_command_helpers.py#L38)
- used by: [`handle_mcp_commands`](mcp_commands/__init__.md#handle_mcp_commands), [`_EXTENDED_SPECS`](mcp_commands/_specs_extended.md#_EXTENDED_SPECS._EXTENDED_SPECS), [`_CORE_SPECS`](mcp_commands/_specs_core.md#_CORE_SPECS._CORE_SPECS), [`validate_mcp_command_args`](mcp_command_helpers.md#validate_mcp_command_args), [`find_selected_mcp_command`](mcp_command_helpers.md#find_selected_mcp_command), [`MCP_COMMAND_SPECS`](mcp_commands/_specs.md#MCP_COMMAND_SPECS.MCP_COMMAND_SPECS), [`_emit_builder_error`](mcp_commands/__init__.md#_emit_builder_error), [`build_mcp_tool_args`](mcp_command_helpers.md#build_mcp_tool_args)  (9 test-only)

## Functions
- `build_mcp_tool_args(args: Any, spec: McpCommandSpec, output_format: str)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_command_helpers.py#L121) — Build concrete tool arguments for a selected MCP command.
- `find_selected_mcp_command(args: Any, command_specs: tuple[McpCommandSpec, ...])` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_command_helpers.py#L42) — Return the first MCP command selected by parsed CLI args.
- `validate_mcp_command_args(args: Any, spec: McpCommandSpec, output_error_fn: Callable[[str], None])` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_command_helpers.py#L87) — Validate selected MCP command arguments.

