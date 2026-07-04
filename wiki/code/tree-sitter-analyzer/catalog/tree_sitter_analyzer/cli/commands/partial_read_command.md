---
title: 'Module: tree_sitter_analyzer/cli/commands/partial_read_command.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/partial_read_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.partial_read_command`/
symbols:
  PartialReadCommand.execute: PartialReadCommand#execute().
  PartialReadCommand: PartialReadCommand#
  PartialReadCommand.args: PartialReadCommand#args.
  PartialReadCommand._emit_partial_payload: PartialReadCommand#_emit_partial_payload().
  PartialReadCommand._output_partial_content: PartialReadCommand#_output_partial_content().
  PartialReadCommand.validate_file: PartialReadCommand#validate_file().
  PartialReadCommand._compute_partial_range_flags: PartialReadCommand#_compute_partial_range_flags().
  PartialReadCommand._build_partial_result: PartialReadCommand#_build_partial_result().
  _toon_available: _toon_available.
  PartialReadCommand.execute_async: PartialReadCommand#execute_async().
  PartialReadCommand.__init__: PartialReadCommand#__init__().
---
# Module: [`tree_sitter_analyzer/cli/commands/partial_read_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/partial_read_command.py)

## Classes
### `PartialReadCommand`  ·  implements/extends BaseCommand
- def: [`tree_sitter_analyzer/cli/commands/partial_read_command.py:30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/partial_read_command.py#L30)
- doc: Command for reading partial file content by line range.
- signature: `class PartialReadCommand(BaseCommand):`
- members:
  - `__init__(self, args: Any)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/partial_read_command.py#L33) — Initialize with arguments but skip base class analysis engine setup.
  - `_build_partial_result(self, *, content: str, end_line: int | None, start_column: int | None, end_column: int | None, flags: dict[str, Any])` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/partial_read_command.py#L170) — Build ``result_data`` with K8 flags + r37ag canonical envelope mirror.
  - `_compute_partial_range_flags(self, content: str, end_line: int | None)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/partial_read_command.py#L135) — Compute out-of-range / partial-range / clamped_to flags + line count.
  - `_emit_partial_payload(self, result_data: dict[str, Any], content: str)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/partial_read_command.py#L228) — Emit ``result_data`` via json / toon / text per ``--output-format``.
  - `_output_partial_content(self, content: str)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/partial_read_command.py#L112) — Output the partial content in the specified format.
  - `execute(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/partial_read_command.py#L56) — Execute partial read command.
  - `execute_async(self, language: str)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/partial_read_command.py#L250) — Not used for partial read command.
  - `validate_file(self)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/partial_read_command.py#L38) — Validate input file exists and is accessible.
  - `args` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/partial_read_command.py#L35)
- uses (calls/refs, reference-scoped): [`ToonFormatter`](../../formatters/toon_formatter.md#ToonFormatter), [`read_file_partial`](../../file_handler.md#read_file_partial), [`output_data`](../../output_manager.md#output_data), [`output_error`](../../output_manager.md#output_error), [`BaseCommand`](base_command.md#BaseCommand), [`format`](../../formatters/toon_formatter.md#ToonFormatter.format), [`output_json`](../../output_manager.md#output_json), [`build_agent_summary`](../../mcp/tools/read_partial_helpers.md#build_agent_summary), [`output_section`](../../output_manager.md#output_section), [`_toon_available`](partial_read_command.md#_toon_available), [`count_file_lines`](../../mcp/tools/read_partial_helpers.md#count_file_lines)
- used by: [`BaseCommand`](base_command.md#BaseCommand), [`execute_async`](base_command.md#BaseCommand.execute_async), [`_create_file_command`](../../cli_main.md#_create_file_command), [`validate_file`](base_command.md#BaseCommand.validate_file), [`execute`](base_command.md#BaseCommand.execute)  (26 test-only)

## Module values
- `_toon_available` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/partial_read_command.py#L22)

