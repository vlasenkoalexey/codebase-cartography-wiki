---
title: 'Module: tests/unit/cli/test_list_files_cli_comprehensive_parser.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_list_files_cli_comprehensive_parser.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_list_files_cli_comprehensive_parser`/Test
symbols:
  TestBuildParser.test_parser_creation: BuildParser#test_parser_creation().
  TestBuildParser.test_required_arguments: BuildParser#test_required_arguments().
  TestBuildParser.test_minimal_valid_arguments: BuildParser#test_minimal_valid_arguments().
  TestBuildParser.test_multiple_roots: BuildParser#test_multiple_roots().
  TestBuildParser.test_output_format_options: BuildParser#test_output_format_options().
  TestBuildParser.test_quiet_flag: BuildParser#test_quiet_flag().
  TestBuildParser.test_pattern_option: BuildParser#test_pattern_option().
  TestBuildParser.test_glob_flag: BuildParser#test_glob_flag().
  TestBuildParser.test_types_option: BuildParser#test_types_option().
  TestBuildParser.test_extensions_option: BuildParser#test_extensions_option().
  TestBuildParser.test_exclude_option: BuildParser#test_exclude_option().
  TestBuildParser.test_depth_option: BuildParser#test_depth_option().
  TestBuildParser.test_follow_symlinks_flag: BuildParser#test_follow_symlinks_flag().
  TestBuildParser.test_hidden_flag: BuildParser#test_hidden_flag().
  TestBuildParser.test_no_ignore_flag: BuildParser#test_no_ignore_flag().
  TestBuildParser.test_size_option: BuildParser#test_size_option().
  TestBuildParser.test_changed_within_option: BuildParser#test_changed_within_option().
  TestBuildParser.test_changed_before_option: BuildParser#test_changed_before_option().
  TestBuildParser.test_full_path_match_flag: BuildParser#test_full_path_match_flag().
  TestBuildParser.test_limit_option: BuildParser#test_limit_option().
  TestBuildParser.test_count_only_flag: BuildParser#test_count_only_flag().
  TestBuildParser.test_project_root_option: BuildParser#test_project_root_option().
  TestBuildParser.test_all_options_together: BuildParser#test_all_options_together().
  TestParserEdgeCases.test_parser_help: ParserEdgeCases#test_parser_help().
  TestBuildParser: BuildParser#
  TestParserEdgeCases: ParserEdgeCases#
---
# Module: [`tests/unit/cli/test_list_files_cli_comprehensive_parser.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py)

## Classes
### `TestBuildParser`
- def: [`tests/unit/cli/test_list_files_cli_comprehensive_parser.py:13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L13)
- doc: Test argument parser construction.
- signature: `class TestBuildParser:`
- members:
  - `test_all_options_together(self)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L196) — Test all options can be used together.
  - `test_changed_before_option(self)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L158) — Test changed-before option.
  - `test_changed_within_option(self)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L152) — Test changed-within option.
  - `test_count_only_flag(self)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L180) — Test count-only flag.
  - `test_depth_option(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L110) — Test depth option.
  - `test_exclude_option(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L102) — Test exclude option.
  - `test_extensions_option(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L96) — Test extensions option.
  - `test_follow_symlinks_flag(self)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L116) — Test follow-symlinks flag.
  - `test_full_path_match_flag(self)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L164) — Test full-path-match flag.
  - `test_glob_flag(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L80) — Test glob flag.
  - `test_hidden_flag(self)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L126) — Test hidden flag.
  - `test_limit_option(self)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L174) — Test limit option.
  - `test_minimal_valid_arguments(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L32) — Test minimal valid argument set.
  - `test_multiple_roots(self)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L41) — Test multiple search roots.
  - `test_no_ignore_flag(self)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L136) — Test no-ignore flag.
  - `test_output_format_options(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L48) — Test output format choices.
  - `test_parser_creation(self)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L16) — Test parser is created successfully.
  - `test_pattern_option(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L74) — Test pattern option.
  - `test_project_root_option(self)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L190) — Test project root option.
  - `test_quiet_flag(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L64) — Test quiet flag.
  - `test_required_arguments(self)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L24) — Test required arguments are enforced.
  - `test_size_option(self)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L146) — Test size option.
  - `test_types_option(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L90) — Test types option.
- uses (calls/refs, reference-scoped): [`_build_parser`](../../../tree_sitter_analyzer/cli/commands/list_files_cli.md#_build_parser)

### `TestParserEdgeCases`
- def: [`tests/unit/cli/test_list_files_cli_comprehensive_parser.py:257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L257)
- doc: Parser-related edge cases.
- signature: `class TestParserEdgeCases:`
- members:
  - `test_parser_help(self)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_list_files_cli_comprehensive_parser.py#L260) — Test parser help output.
- uses (calls/refs, reference-scoped): [`_build_parser`](../../../tree_sitter_analyzer/cli/commands/list_files_cli.md#_build_parser)

