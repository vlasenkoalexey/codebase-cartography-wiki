---
title: 'Module: tree_sitter_analyzer/cli_main.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli_main.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli_main`/
symbols:
  main: main().
  create_argument_parser: create_argument_parser().
  handle_special_commands: handle_special_commands().
  _create_file_command: _create_file_command().
  CLICommandFactory.create_command: CLICommandFactory#create_command().
  msg: msg.
  _print_filter_help: _print_filter_help().
  _create_info_command: _create_info_command().
  _validate_command_arguments: _validate_command_arguments().
  _normalize_agent_command_aliases: _normalize_agent_command_aliases().
  CLICommandFactory: CLICommandFactory#
  _execute_selected_command: _execute_selected_command().
  _MODE_FLAG_WIRING._MODE_FLAG_WIRING: _MODE_FLAG_WIRING._MODE_FLAG_WIRING.
  _normalize_file_scoped_alias: _normalize_file_scoped_alias().
  _validate_mode_flag_wiring: _validate_mode_flag_wiring().
  _NO_COMMAND_MATCH: _NO_COMMAND_MATCH.
  _FILE_SCOPED_AGENT_COMMANDS: _FILE_SCOPED_AGENT_COMMANDS.
  _PROJECT_SCOPED_AGENT_COMMANDS: _PROJECT_SCOPED_AGENT_COMMANDS.
  _argument_is_selected: _argument_is_selected().
  _set_cli_log_environment: _set_cli_log_environment().
  _apply_format_alias: _apply_format_alias().
  _configure_logging: _configure_logging().
  e: e.
---
# Module: [`tree_sitter_analyzer/cli_main.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py)

## Classes
### `CLICommandFactory`
- def: [`tree_sitter_analyzer/cli_main.py:51`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L51)
- doc: Factory for creating CLI commands based on arguments.
- signature: `class CLICommandFactory:`
- members:
  - `create_command(args: argparse.Namespace)` — [`L55`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L55) — Create appropriate command based on arguments.
- uses (calls/refs, reference-scoped): [`_create_file_command`](cli_main.md#_create_file_command), [`_create_info_command`](cli_main.md#_create_info_command), [`_validate_command_arguments`](cli_main.md#_validate_command_arguments), [`_NO_COMMAND_MATCH`](cli_main.md#_NO_COMMAND_MATCH)
- used by: [`_execute_selected_command`](cli_main.md#_execute_selected_command)  (8 test-only)

## Functions
- `_apply_format_alias(args: argparse.Namespace)` — [`L230`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L230) — Mirror --format into --output-format after parsing.
- `_argument_is_selected(args: argparse.Namespace, attr_name: str)` — [`L153`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L153) — Return True when an argparse field selects a command.
- `_configure_logging(args: argparse.Namespace)` — [`L303`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L303) — Configure noisy loggers before command execution.
- `_create_file_command(args: argparse.Namespace)` — [`L136`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L136) — Create the highest-priority file-analysis command for parsed arguments.
- `_create_info_command(args: argparse.Namespace)` — [`L81`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L81) — Create commands that do not require a file path.
- `_execute_selected_command(args: argparse.Namespace, parser: argparse.ArgumentParser)` — [`L315`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L315) — Create the selected command and exit with the correct status.
- `_normalize_agent_command_aliases(argv: list[str])` — [`L210`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L210) — Rewrite agent-friendly subcommands to the existing flag-based CLI.
- `_normalize_file_scoped_alias(command: str, rest: list[str])` — [`L223`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L223)
- `_print_filter_help(args: argparse.Namespace | None = None)` — [`L97`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L97) — Print query filter help (text) or emit a JSON envelope.
- `_set_cli_log_environment()` — [`L205`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L205) — Force CLI logging to stderr-only error noise regardless of quiet mode.
- `_validate_command_arguments(args: argparse.Namespace)` — [`L70`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L70) — Validate CLI argument combinations before selecting a command.
- `_validate_mode_flag_wiring(args: argparse.Namespace, parser: argparse.ArgumentParser)` — [`L275`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L275) — Fail fast when a ``--X-mode`` selector is used without its trigger (#1000).
- `create_argument_parser()` — [`L159`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L159) — Create and configure the argument parser.
- `handle_special_commands(args: argparse.Namespace)` — [`L166`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L166) — Handle special commands that don't fit the normal pattern.
- `main()` — [`L189`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L189) — Main entry point for the CLI.

## Module values
- `_FILE_SCOPED_AGENT_COMMANDS` — [`L33`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L33)
- `_MODE_FLAG_WIRING` — [`L249`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L249)
- `_NO_COMMAND_MATCH` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L32)
- `_PROJECT_SCOPED_AGENT_COMMANDS` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L39)
- `e` — [`L343`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L343)
- `msg` — [`L344`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli_main.py#L344)

