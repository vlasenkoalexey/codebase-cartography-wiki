---
title: 'Module: tests/unit/cli/test_shell_safe_path_875.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_shell_safe_path_875.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_shell_safe_path_875`/TestShellSafePathWindowsCompat#
symbols:
  TestShellSafePathWindowsCompat.test_none_returns_empty_string: test_none_returns_empty_string().
  TestShellSafePathWindowsCompat.test_simple_path_no_quoting_needed: test_simple_path_no_quoting_needed().
  TestShellSafePathWindowsCompat.test_path_with_spaces_uses_double_quotes: test_path_with_spaces_uses_double_quotes().
  TestShellSafePathWindowsCompat.test_path_with_spaces_not_single_quoted: test_path_with_spaces_not_single_quoted().
  TestShellSafePathWindowsCompat.test_windows_backslash_path_is_double_quoted: test_windows_backslash_path_is_double_quoted().
  TestShellSafePathWindowsCompat.test_windows_path_with_spaces_double_quoted: test_windows_path_with_spaces_double_quoted().
  TestShellSafePathWindowsCompat.test_dollar_sign_escaped_in_double_quotes: test_dollar_sign_escaped_in_double_quotes().
  TestShellSafePathWindowsCompat.test_backtick_escaped_in_double_quotes: test_backtick_escaped_in_double_quotes().
  TestShellSafePathWindowsCompat.test_empty_path_returns_empty: test_empty_path_returns_empty().
  TestShellSafePathWindowsCompat: ''
---
# Module: [`tests/unit/cli/test_shell_safe_path_875.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_shell_safe_path_875.py)

## Classes
### `TestShellSafePathWindowsCompat`
- def: [`tests/unit/cli/test_shell_safe_path_875.py:10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_shell_safe_path_875.py#L10)
- signature: `class TestShellSafePathWindowsCompat:`
- members:
  - `test_backtick_escaped_in_double_quotes(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_shell_safe_path_875.py#L48)
  - `test_dollar_sign_escaped_in_double_quotes(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_shell_safe_path_875.py#L43)
  - `test_empty_path_returns_empty(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_shell_safe_path_875.py#L53)
  - `test_none_returns_empty_string(self)` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_shell_safe_path_875.py#L11)
  - `test_path_with_spaces_not_single_quoted(self)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_shell_safe_path_875.py#L24)
  - `test_path_with_spaces_uses_double_quotes(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_shell_safe_path_875.py#L19)
  - `test_simple_path_no_quoting_needed(self)` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_shell_safe_path_875.py#L14)
  - `test_windows_backslash_path_is_double_quoted(self)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_shell_safe_path_875.py#L31)
  - `test_windows_path_with_spaces_double_quoted(self)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_shell_safe_path_875.py#L38)
- uses (calls/refs, reference-scoped): [`_shell_safe_path`](../../../tree_sitter_analyzer/cli/agent_workflow.md#_shell_safe_path)

