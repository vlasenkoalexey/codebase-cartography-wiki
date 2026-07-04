---
title: 'Module: tree_sitter_analyzer/cli/argument_validator.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/argument_validator.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.argument_validator`/CLIArgumentValidator#
symbols:
  CLIArgumentValidator.validate_arguments: validate_arguments().
  CLIArgumentValidator: ''
  CLIArgumentValidator.validate_table_query_exclusivity: validate_table_query_exclusivity().
  CLIArgumentValidator.get_usage_examples: get_usage_examples().
  CLIArgumentValidator.__init__: __init__().
---
# Module: [`tree_sitter_analyzer/cli/argument_validator.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/argument_validator.py)

## Classes
### `CLIArgumentValidator`
- def: [`tree_sitter_analyzer/cli/argument_validator.py:11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/argument_validator.py#L11)
- doc: Validator for CLI argument combinations.
- signature: `class CLIArgumentValidator:`
- members:
  - `__init__(self)` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/argument_validator.py#L14) — Initialize the validator.
  - `get_usage_examples(self)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/argument_validator.py#L68) — Get usage examples for correct argument combinations.
  - `validate_arguments(self, args: Any)` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/argument_validator.py#L18) — Validate CLI argument combinations.
  - `validate_table_query_exclusivity(self, args: Any)` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/argument_validator.py#L44) — Validate that --table and --query-key are mutually exclusive.
- used by: [`_validate_command_arguments`](../cli_main.md#_validate_command_arguments)  (17 test-only)

