---
title: 'Module: tests/unit/cli/test_base_command_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_base_command_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_base_command_coverage`/
symbols:
  _ConcreteCommand: _ConcreteCommand#
  TestBaseCommandInit.test_init_sets_project_root: TestBaseCommandInit#test_init_sets_project_root().
  TestValidateFile.test_no_file_path_returns_false: TestValidateFile#test_no_file_path_returns_false().
  TestValidateFile.test_none_file_path_returns_false: TestValidateFile#test_none_file_path_returns_false().
  cmd: cmd().
  _ConcreteCommand.execute_async: _ConcreteCommand#execute_async().
  args: args().
  TestBaseCommandInit: TestBaseCommandInit#
  TestValidateFile: TestValidateFile#
  TestDetectLanguage: TestDetectLanguage#
  TestDetectLanguage.test_unknown_language_returns_none: TestDetectLanguage#test_unknown_language_returns_none().
  TestDetectLanguage.test_unsupported_language_returns_none_and_emits_envelope: TestDetectLanguage#test_unsupported_language_returns_none_and_emits_envelope().
  TestExecute: TestExecute#
  TestExecute.test_execute_async_exception_returns_1: TestExecute#test_execute_async_exception_returns_1().
---
# Module: [`tests/unit/cli/test_base_command_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_base_command_coverage.py)

## Classes
### `TestBaseCommandInit`
- def: [`tests/unit/cli/test_base_command_coverage.py:29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_base_command_coverage.py#L29)
- doc: Tests for BaseCommand.__init__
- signature: `class TestBaseCommandInit:`
- members:
  - `test_init_sets_project_root(self, args)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_base_command_coverage.py#L32) — __init__ should detect and set project_root (lines 46-47)
- uses (calls/refs, reference-scoped): [`project_root`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand.project_root)  (1 test-only)

### `TestDetectLanguage`
- def: [`tests/unit/cli/test_base_command_coverage.py:60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_base_command_coverage.py#L60)
- doc: Tests for BaseCommand.detect_language
- signature: `class TestDetectLanguage:`
- members:
  - `test_unknown_language_returns_none(self, cmd)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_base_command_coverage.py#L63) — Returns None when language detection fails (lines 109-110)
  - `test_unsupported_language_returns_none_and_emits_envelope(self, cmd, capsys)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_base_command_coverage.py#L76) — Q2 (round-33): non-java unsupported language no longer silently

### `TestExecute`
- def: [`tests/unit/cli/test_base_command_coverage.py:103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_base_command_coverage.py#L103)
- doc: Tests for BaseCommand.execute
- signature: `class TestExecute:`
- members:
  - `test_execute_async_exception_returns_1(self, cmd)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_base_command_coverage.py#L106) — Exception in execute_async returns exit code 1 (lines 166-168)

### `TestValidateFile`
- def: [`tests/unit/cli/test_base_command_coverage.py:42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_base_command_coverage.py#L42)
- doc: Tests for BaseCommand.validate_file
- signature: `class TestValidateFile:`
- members:
  - `test_no_file_path_returns_false(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_base_command_coverage.py#L45) — Returns False when args has no file_path (lines 60-61)
  - `test_none_file_path_returns_false(self)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_base_command_coverage.py#L52) — Returns False when file_path is None
- uses (calls/refs, reference-scoped): [`validate_file`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand.validate_file)  (1 test-only)

### `_ConcreteCommand`  ·  implements/extends BaseCommand
- def: [`tests/unit/cli/test_base_command_coverage.py:12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_base_command_coverage.py#L12)
- doc: Minimal concrete subclass for testing BaseCommand
- signature: `class _ConcreteCommand(BaseCommand):`
- members:
  - `execute_async(self, language: str)` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_base_command_coverage.py#L15)
- uses (calls/refs, reference-scoped): [`BaseCommand`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand)
- used by: [`BaseCommand`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand), [`execute_async`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand.execute_async)  (4 test-only)

## Functions
- `args()` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_base_command_coverage.py#L20)
- `cmd(args)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_base_command_coverage.py#L25)

