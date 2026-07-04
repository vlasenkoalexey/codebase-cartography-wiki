---
title: 'Module: tests/unit/cli/test_default_command.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_default_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_default_command`/
symbols:
  TestDefaultCommandInit.test_init_with_args: TestDefaultCommandInit#test_init_with_args().
  command: command().
  TestDefaultCommandInit.test_init: TestDefaultCommandInit#test_init().
  mock_args: mock_args().
  TestDefaultCommandInit: TestDefaultCommandInit#
  TestDefaultCommandExecuteAsync: TestDefaultCommandExecuteAsync#
  TestDefaultCommandExecuteAsync.test_execute_async_returns_1: TestDefaultCommandExecuteAsync#test_execute_async_returns_1().
  TestDefaultCommandExecuteAsync.test_execute_async_with_language: TestDefaultCommandExecuteAsync#test_execute_async_with_language().
  TestDefaultCommandExecuteAsync.test_execute_async_with_none_language: TestDefaultCommandExecuteAsync#test_execute_async_with_none_language().
  TestDefaultCommandOutput: TestDefaultCommandOutput#
  TestDefaultCommandOutput.test_execute_async_outputs_error_message: TestDefaultCommandOutput#test_execute_async_outputs_error_message().
  TestDefaultCommandOutput.test_execute_async_outputs_usage_examples: TestDefaultCommandOutput#test_execute_async_outputs_usage_examples().
  TestDefaultCommandOutput.test_execute_async_outputs_examples: TestDefaultCommandOutput#test_execute_async_outputs_examples().
  TestDefaultCommandBehavior: TestDefaultCommandBehavior#
  TestDefaultCommandBehavior.test_execute_async_does_not_call_analyze_file: TestDefaultCommandBehavior#test_execute_async_does_not_call_analyze_file().
  TestDefaultCommandBehavior.test_execute_async_always_returns_error: TestDefaultCommandBehavior#test_execute_async_always_returns_error().
---
# Module: [`tests/unit/cli/test_default_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_default_command.py)

## Classes
### `TestDefaultCommandBehavior`
- def: [`tests/unit/cli/test_default_command.py:131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_default_command.py#L131)
- doc: Tests for DefaultCommand behavior.
- signature: `class TestDefaultCommandBehavior:`
- members:
  - `test_execute_async_always_returns_error(self, command)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_default_command.py#L144) — Test execute_async always returns error regardless of language.
  - `test_execute_async_does_not_call_analyze_file(self, command)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_default_command.py#L135) — Test execute_async does not call analyze_file.

### `TestDefaultCommandExecuteAsync`
- def: [`tests/unit/cli/test_default_command.py:67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_default_command.py#L67)
- doc: Tests for DefaultCommand.execute_async method.
- signature: `class TestDefaultCommandExecuteAsync:`
- members:
  - `test_execute_async_returns_1(self, command)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_default_command.py#L71) — Test execute_async returns error code 1.
  - `test_execute_async_with_language(self, command)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_default_command.py#L77) — Test execute_async with language parameter.
  - `test_execute_async_with_none_language(self, command)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_default_command.py#L83) — Test execute_async with None language.

### `TestDefaultCommandInit`
- def: [`tests/unit/cli/test_default_command.py:52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_default_command.py#L52)
- doc: Tests for DefaultCommand initialization.
- signature: `class TestDefaultCommandInit:`
- members:
  - `test_init(self, command)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_default_command.py#L55) — Test DefaultCommand initialization.
  - `test_init_with_args(self, mock_args)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_default_command.py#L61) — Test DefaultCommand initialization with args.
- uses (calls/refs, reference-scoped): [`args`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand.args), [`DefaultCommand`](../../../tree_sitter_analyzer/cli/commands/default_command.md#DefaultCommand)

### `TestDefaultCommandOutput`
- def: [`tests/unit/cli/test_default_command.py:89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_default_command.py#L89)
- doc: Tests for DefaultCommand output.
- signature: `class TestDefaultCommandOutput:`
- members:
  - `test_execute_async_outputs_error_message(self, command)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_default_command.py#L93) — Test execute_async outputs error message.
  - `test_execute_async_outputs_examples(self, command)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_default_command.py#L119) — Test execute_async outputs example commands.
  - `test_execute_async_outputs_usage_examples(self, command)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_default_command.py#L104) — Test execute_async outputs usage examples.

## Functions
- `command(mock_args)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_default_command.py#L47) — Create DefaultCommand instance for testing.
- `mock_args()` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_default_command.py#L15) — Create mock args for BaseCommand initialization.

