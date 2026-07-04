---
title: 'Module: tests/unit/cli/test_subcommand_format_alias.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_subcommand_format_alias.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_subcommand_format_alias`/
symbols:
  _strip_volatile: _strip_volatile().
  TestSearchContentSubprocessAlias.test_format_and_output_format_match: TestSearchContentSubprocessAlias#test_format_and_output_format_match().
  TestFindAndGrepSubprocessAlias.test_format_and_output_format_match: TestFindAndGrepSubprocessAlias#test_format_and_output_format_match().
  TestListFilesSubprocessAlias.test_format_and_output_format_match: TestListFilesSubprocessAlias#test_format_and_output_format_match().
  _run_cli: _run_cli().
  _parse_first_json: _parse_first_json().
  TestSearchContentSubprocessAlias.test_format_alias_yields_valid_json: TestSearchContentSubprocessAlias#test_format_alias_yields_valid_json().
  TestFindAndGrepSubprocessAlias.test_format_alias_yields_valid_json: TestFindAndGrepSubprocessAlias#test_format_alias_yields_valid_json().
  TestListFilesSubprocessAlias.test_format_alias_yields_valid_json: TestListFilesSubprocessAlias#test_format_alias_yields_valid_json().
  _module_for: _module_for().
  _is_volatile: _is_volatile().
  TestSearchContentFormatAlias.test_output_format_long: TestSearchContentFormatAlias#test_output_format_long().
  TestSearchContentFormatAlias.test_format_alias: TestSearchContentFormatAlias#test_format_alias().
  TestSearchContentFormatAlias.test_format_alias_all_choices: TestSearchContentFormatAlias#test_format_alias_all_choices().
  TestFindAndGrepFormatAlias.test_output_format_long: TestFindAndGrepFormatAlias#test_output_format_long().
  TestFindAndGrepFormatAlias.test_format_alias: TestFindAndGrepFormatAlias#test_format_alias().
  TestFindAndGrepFormatAlias.test_format_alias_all_choices: TestFindAndGrepFormatAlias#test_format_alias_all_choices().
  TestListFilesFormatAlias.test_output_format_long: TestListFilesFormatAlias#test_output_format_long().
  TestListFilesFormatAlias.test_format_alias: TestListFilesFormatAlias#test_format_alias().
  TestListFilesFormatAlias.test_format_alias_all_choices: TestListFilesFormatAlias#test_format_alias_all_choices().
  _VOLATILE_KEY_SUFFIXES: _VOLATILE_KEY_SUFFIXES.
  _VOLATILE_KEYS: _VOLATILE_KEYS.
  TestSearchContentFormatAlias: TestSearchContentFormatAlias#
  TestFindAndGrepFormatAlias: TestFindAndGrepFormatAlias#
  TestListFilesFormatAlias: TestListFilesFormatAlias#
  fixture_root: fixture_root().
  TestSearchContentSubprocessAlias: TestSearchContentSubprocessAlias#
  TestFindAndGrepSubprocessAlias: TestFindAndGrepSubprocessAlias#
  TestListFilesSubprocessAlias: TestListFilesSubprocessAlias#
---
# Module: [`tests/unit/cli/test_subcommand_format_alias.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py)

## Classes
### `TestFindAndGrepFormatAlias`
- def: [`tests/unit/cli/test_subcommand_format_alias.py:71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L71)
- doc: `find-and-grep` accepts both `--format` and `--output-format`.
- signature: `class TestFindAndGrepFormatAlias:`
- members:
  - `test_format_alias(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L81)
  - `test_format_alias_all_choices(self, fmt: str)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L89)
  - `test_output_format_long(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L74)
- uses (calls/refs, reference-scoped): [`_build_parser`](../../../tree_sitter_analyzer/cli/commands/find_and_grep_cli.md#_build_parser)

### `TestFindAndGrepSubprocessAlias`
- def: [`tests/unit/cli/test_subcommand_format_alias.py:244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L244)
- doc: End-to-end: both flag forms produce equivalent JSON for find-and-grep.
- signature: `class TestFindAndGrepSubprocessAlias:`
- members:
  - `test_format_alias_yields_valid_json(self, fixture_root: Path)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L247)
  - `test_format_and_output_format_match(self, fixture_root: Path)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L267)
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `TestListFilesFormatAlias`
- def: [`tests/unit/cli/test_subcommand_format_alias.py:95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L95)
- doc: `list-files` accepts both `--format` and `--output-format`.
- signature: `class TestListFilesFormatAlias:`
- members:
  - `test_format_alias(self)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L103)
  - `test_format_alias_all_choices(self, fmt: str)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L109)
  - `test_output_format_long(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L98)
- uses (calls/refs, reference-scoped): [`_build_parser`](../../../tree_sitter_analyzer/cli/commands/list_files_cli.md#_build_parser)

### `TestListFilesSubprocessAlias`
- def: [`tests/unit/cli/test_subcommand_format_alias.py:292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L292)
- doc: End-to-end: both flag forms produce equivalent JSON for list-files.
- signature: `class TestListFilesSubprocessAlias:`
- members:
  - `test_format_alias_yields_valid_json(self, fixture_root: Path)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L295)
  - `test_format_and_output_format_match(self, fixture_root: Path)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L312)
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `TestSearchContentFormatAlias`
- def: [`tests/unit/cli/test_subcommand_format_alias.py:47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L47)
- doc: `search-content` accepts both `--format` and `--output-format`.
- signature: `class TestSearchContentFormatAlias:`
- members:
  - `test_format_alias(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L57)
  - `test_format_alias_all_choices(self, fmt: str)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L65)
  - `test_output_format_long(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L50)
- uses (calls/refs, reference-scoped): [`_build_parser`](../../../tree_sitter_analyzer/cli/commands/search_content_cli.md#_build_parser)

### `TestSearchContentSubprocessAlias`
- def: [`tests/unit/cli/test_subcommand_format_alias.py:196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L196)
- doc: End-to-end: both flag forms produce equivalent JSON for search-content.
- signature: `class TestSearchContentSubprocessAlias:`
- members:
  - `test_format_alias_yields_valid_json(self, fixture_root: Path)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L199)
  - `test_format_and_output_format_match(self, fixture_root: Path)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L219)
- uses (calls/refs, reference-scoped): (4 test-only callers)

## Functions
- `_is_volatile(key: str)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L174)
- `_module_for(subcommand: str)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L152)
- `_parse_first_json(stdout: str)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L160) — Parse the stdout payload as JSON; fail loudly with the actual stream.
- `_run_cli(args: list[str], cwd: Path)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L138) — Run a subcommand via ``python -m`` to avoid PATH/console-script flakiness.
- `_strip_volatile(value)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L180)
- `fixture_root(tmp_path: Path)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L121) — Tiny tree with one file containing a known token.

## Module values
- `_VOLATILE_KEYS` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L171)
- `_VOLATILE_KEY_SUFFIXES` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_subcommand_format_alias.py#L170)

