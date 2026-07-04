---
title: 'Module: tree_sitter_analyzer/cli/commands/default_command.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/default_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.default_command`/DefaultCommand#
symbols:
  DefaultCommand: ''
  DefaultCommand.execute_async: execute_async().
---
# Module: [`tree_sitter_analyzer/cli/commands/default_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/default_command.py)

## Classes
### `DefaultCommand`  ·  implements/extends BaseCommand
- def: [`tree_sitter_analyzer/cli/commands/default_command.py:12`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/default_command.py#L12)
- doc: Default command that shows error when no specific command is given.
- signature: `class DefaultCommand(BaseCommand):`
- members:
  - `execute_async(self, language: str)` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/default_command.py#L15) — Execute default command - show error for missing options.
- uses (calls/refs, reference-scoped): [`output_error`](../../output_manager.md#output_error), [`BaseCommand`](base_command.md#BaseCommand), [`output_info`](../../output_manager.md#output_info)
- used by: [`BaseCommand`](base_command.md#BaseCommand), [`execute_async`](base_command.md#BaseCommand.execute_async), [`_create_file_command`](../../cli_main.md#_create_file_command)  (3 test-only)

