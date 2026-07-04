---
title: 'Module: tests/integration/cli/test_cli_argument_validation.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_cli_argument_validation.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_cli_argument_validation`/TestCLIArgumentValidation#
symbols:
  TestCLIArgumentValidation.validator: validator.
  TestCLIArgumentValidation.create_args: create_args().
  TestCLIArgumentValidation.test_validator_initialization: test_validator_initialization().
  TestCLIArgumentValidation.test_valid_table_only: test_valid_table_only().
  TestCLIArgumentValidation.test_valid_query_key_only: test_valid_query_key_only().
  TestCLIArgumentValidation.test_valid_query_key_with_filter: test_valid_query_key_with_filter().
  TestCLIArgumentValidation.test_valid_no_table_no_query_key: test_valid_no_table_no_query_key().
  TestCLIArgumentValidation.test_invalid_table_and_query_key_combination: test_invalid_table_and_query_key_combination().
  TestCLIArgumentValidation.test_invalid_table_and_query_key_with_filter: test_invalid_table_and_query_key_with_filter().
  TestCLIArgumentValidation.test_table_query_exclusivity_validator: test_table_query_exclusivity_validator().
  TestCLIArgumentValidation.test_different_table_formats_with_query_key: test_different_table_formats_with_query_key().
  TestCLIArgumentValidation.test_empty_string_values: test_empty_string_values().
  TestCLIArgumentValidation.test_none_values_explicitly: test_none_values_explicitly().
  TestCLIArgumentValidation.test_usage_examples_content: test_usage_examples_content().
  TestCLIArgumentValidation.test_missing_attributes_handling: test_missing_attributes_handling().
  TestCLIArgumentValidation: ''
  TestCLIArgumentValidation.setup_method: setup_method().
---
# Module: [`tests/integration/cli/test_cli_argument_validation.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_argument_validation.py)

## Classes
### `TestCLIArgumentValidation`
- def: [`tests/integration/cli/test_cli_argument_validation.py:15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_argument_validation.py#L15)
- doc: Tests for CLI argument validation.
- signature: `class TestCLIArgumentValidation:`
- members:
  - `create_args(self, **kwargs)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_argument_validation.py#L22) — Helper to create argparse.Namespace with specified attributes.
  - `setup_method(self)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_argument_validation.py#L18) — Set up test fixtures.
  - `test_different_table_formats_with_query_key(self)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_argument_validation.py#L94) — Test that all table formats are invalid with query-key.
  - `test_empty_string_values(self)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_argument_validation.py#L125) — Test handling of empty string values.
  - `test_invalid_table_and_query_key_combination(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_argument_validation.py#L53) — Test that --table and --query-key together is invalid.
  - `test_invalid_table_and_query_key_with_filter(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_argument_validation.py#L61) — Test that --table and --query-key with --filter is invalid.
  - `test_missing_attributes_handling(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_argument_validation.py#L106) — Test handling of missing attributes in args.
  - `test_none_values_explicitly(self)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_argument_validation.py#L141) — Test explicit None values.
  - `test_table_query_exclusivity_validator(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_argument_validation.py#L68) — Test the specific table-query exclusivity validator.
  - `test_usage_examples_content(self)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_argument_validation.py#L85) — Test that usage examples contain expected content.
  - `test_valid_no_table_no_query_key(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_argument_validation.py#L47) — Test that neither --table nor --query-key is valid.
  - `test_valid_query_key_only(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_argument_validation.py#L35) — Test that --query-key only is valid.
  - `test_valid_query_key_with_filter(self)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_argument_validation.py#L41) — Test that --query-key with --filter is valid.
  - `test_valid_table_only(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_argument_validation.py#L29) — Test that --table only is valid.
  - `test_validator_initialization(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_argument_validation.py#L147) — Test validator can be initialized properly.
  - `validator` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_argument_validation.py#L20)
- uses (calls/refs, reference-scoped): [`validate_arguments`](../../../tree_sitter_analyzer/cli/argument_validator.md#CLIArgumentValidator.validate_arguments), [`CLIArgumentValidator`](../../../tree_sitter_analyzer/cli/argument_validator.md#CLIArgumentValidator), [`validate_table_query_exclusivity`](../../../tree_sitter_analyzer/cli/argument_validator.md#CLIArgumentValidator.validate_table_query_exclusivity), [`get_usage_examples`](../../../tree_sitter_analyzer/cli/argument_validator.md#CLIArgumentValidator.get_usage_examples)

