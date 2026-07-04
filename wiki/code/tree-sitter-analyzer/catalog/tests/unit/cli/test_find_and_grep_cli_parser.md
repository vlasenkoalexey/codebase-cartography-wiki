---
title: 'Module: tests/unit/cli/test_find_and_grep_cli_parser.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_find_and_grep_cli_parser.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_find_and_grep_cli_parser`/TestBuildParser#
symbols:
  TestBuildParser.test_parser_creation: test_parser_creation().
  TestBuildParser.test_required_arguments: test_required_arguments().
  TestBuildParser.test_minimal_valid_arguments: test_minimal_valid_arguments().
  TestBuildParser.test_multiple_roots: test_multiple_roots().
  TestBuildParser.test_output_format_options: test_output_format_options().
  TestBuildParser.test_quiet_flag: test_quiet_flag().
  TestBuildParser.test_fd_options: test_fd_options().
  TestBuildParser.test_rg_options: test_rg_options().
  TestBuildParser.test_case_options: test_case_options().
  TestBuildParser.test_sort_options: test_sort_options().
  TestBuildParser.test_project_root_option: test_project_root_option().
  TestBuildParser: ''
---
# Module: [`tests/unit/cli/test_find_and_grep_cli_parser.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_parser.py)

## Classes
### `TestBuildParser`
- def: [`tests/unit/cli/test_find_and_grep_cli_parser.py:15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_parser.py#L15)
- doc: Test argument parser construction.
- signature: `class TestBuildParser:`
- members:
  - `test_case_options(self)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_parser.py#L209) — Test case sensitivity options.
  - `test_fd_options(self)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_parser.py#L94) — Test fd-specific options.
  - `test_minimal_valid_arguments(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_parser.py#L43) — Test minimal valid argument set.
  - `test_multiple_roots(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_parser.py#L53) — Test multiple search roots.
  - `test_output_format_options(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_parser.py#L62) — Test output format choices.
  - `test_parser_creation(self)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_parser.py#L18) — Test parser is created successfully.
  - `test_project_root_option(self)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_parser.py#L229) — Test project root option.
  - `test_quiet_flag(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_parser.py#L84) — Test quiet flag.
  - `test_required_arguments(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_parser.py#L27) — Test required arguments are enforced.
  - `test_rg_options(self)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_parser.py#L151) — Test ripgrep-specific options.
  - `test_sort_options(self)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_find_and_grep_cli_parser.py#L219) — Test sort options.
- uses (calls/refs, reference-scoped): [`_build_parser`](../../../tree_sitter_analyzer/cli/commands/find_and_grep_cli.md#_build_parser)

