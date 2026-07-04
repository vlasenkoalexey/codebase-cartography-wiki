---
title: 'Module: tree_sitter_analyzer/cli/commands/find_and_grep_cli_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/find_and_grep_cli_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.find_and_grep_cli_helpers`/
symbols:
  build_find_and_grep_payload: build_find_and_grep_payload().
  add_output_options: add_output_options().
  add_fd_options: add_fd_options().
  add_rg_options: add_rg_options().
  _add_fd_payload_options: _add_fd_payload_options().
  _add_rg_payload_options: _add_rg_payload_options().
---
# Module: [`tree_sitter_analyzer/cli/commands/find_and_grep_cli_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/find_and_grep_cli_helpers.py)

## Functions
- `_add_fd_payload_options(payload: dict[str, Any], args: argparse.Namespace)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/find_and_grep_cli_helpers.py#L85) — Add fd-stage payload options when present.
- `_add_rg_payload_options(payload: dict[str, Any], args: argparse.Namespace)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/find_and_grep_cli_helpers.py#L118) — Add ripgrep-stage payload options when present.
- `add_fd_options(parser: argparse.ArgumentParser)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/find_and_grep_cli_helpers.py#L31) — Register fd-stage filtering flags.
- `add_output_options(parser: argparse.ArgumentParser)` — [`L9`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/find_and_grep_cli_helpers.py#L9) — Register shared output flags.
- `add_rg_options(parser: argparse.ArgumentParser)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/find_and_grep_cli_helpers.py#L50) — Register ripgrep-stage content matching flags.
- `build_find_and_grep_payload(args: argparse.Namespace)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/find_and_grep_cli_helpers.py#L73) — Map CLI arguments to FindAndGrepTool arguments.

