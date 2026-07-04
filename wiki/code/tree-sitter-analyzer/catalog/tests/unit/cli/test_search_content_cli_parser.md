---
title: 'Module: tests/unit/cli/test_search_content_cli_parser.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_search_content_cli_parser.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_search_content_cli_parser`/TestBuildParser#
symbols:
  TestBuildParser.test_parser_creation: test_parser_creation().
  TestBuildParser.test_required_arguments: test_required_arguments().
  TestBuildParser.test_minimal_valid_arguments_with_roots: test_minimal_valid_arguments_with_roots().
  TestBuildParser.test_minimal_valid_arguments_with_files: test_minimal_valid_arguments_with_files().
  TestBuildParser.test_roots_and_files_mutually_exclusive: test_roots_and_files_mutually_exclusive().
  TestBuildParser.test_multiple_roots: test_multiple_roots().
  TestBuildParser.test_multiple_files: test_multiple_files().
  TestBuildParser.test_output_format_options: test_output_format_options().
  TestBuildParser.test_quiet_flag: test_quiet_flag().
  TestBuildParser.test_case_options: test_case_options().
  TestBuildParser.test_fixed_strings_flag: test_fixed_strings_flag().
  TestBuildParser.test_word_flag: test_word_flag().
  TestBuildParser.test_multiline_flag: test_multiline_flag().
  TestBuildParser.test_include_globs_option: test_include_globs_option().
  TestBuildParser.test_exclude_globs_option: test_exclude_globs_option().
  TestBuildParser.test_follow_symlinks_flag: test_follow_symlinks_flag().
  TestBuildParser.test_hidden_flag: test_hidden_flag().
  TestBuildParser.test_no_ignore_flag: test_no_ignore_flag().
  TestBuildParser.test_max_filesize_option: test_max_filesize_option().
  TestBuildParser.test_context_options: test_context_options().
  TestBuildParser.test_encoding_option: test_encoding_option().
  TestBuildParser.test_max_count_option: test_max_count_option().
  TestBuildParser.test_timeout_ms_option: test_timeout_ms_option().
  TestBuildParser.test_count_only_matches_flag: test_count_only_matches_flag().
  TestBuildParser.test_summary_only_flag: test_summary_only_flag().
  TestBuildParser.test_optimize_paths_flag: test_optimize_paths_flag().
  TestBuildParser.test_group_by_file_flag: test_group_by_file_flag().
  TestBuildParser.test_total_only_flag: test_total_only_flag().
  TestBuildParser.test_project_root_option: test_project_root_option().
  TestBuildParser.test_all_options_together_with_roots: test_all_options_together_with_roots().
  TestBuildParser: ''
---
# Module: [`tests/unit/cli/test_search_content_cli_parser.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py)

## Classes
### `TestBuildParser`
- def: [`tests/unit/cli/test_search_content_cli_parser.py:13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L13)
- doc: Test argument parser construction.
- signature: `class TestBuildParser:`
- members:
  - `test_all_options_together_with_roots(self)` — [`L335`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L335) — Test all options can be used together with roots.
  - `test_case_options(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L120) — Test case sensitivity options.
  - `test_context_options(self)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L218) — Test context before/after options.
  - `test_count_only_matches_flag(self)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L260) — Test count-only-matches flag.
  - `test_encoding_option(self)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L236) — Test encoding option.
  - `test_exclude_globs_option(self)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L170) — Test exclude-globs option.
  - `test_fixed_strings_flag(self)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L130) — Test fixed-strings flag.
  - `test_follow_symlinks_flag(self)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L178) — Test follow-symlinks flag.
  - `test_group_by_file_flag(self)` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L296) — Test group-by-file flag.
  - `test_hidden_flag(self)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L190) — Test hidden flag.
  - `test_include_globs_option(self)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L162) — Test include-globs option.
  - `test_max_count_option(self)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L244) — Test max-count option.
  - `test_max_filesize_option(self)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L210) — Test max-filesize option.
  - `test_minimal_valid_arguments_with_files(self)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L52) — Test minimal valid argument set with files.
  - `test_minimal_valid_arguments_with_roots(self)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L41) — Test minimal valid argument set with roots.
  - `test_multiline_flag(self)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L152) — Test multiline flag.
  - `test_multiple_files(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L81) — Test multiple files.
  - `test_multiple_roots(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L72) — Test multiple search roots.
  - `test_no_ignore_flag(self)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L200) — Test no-ignore flag.
  - `test_optimize_paths_flag(self)` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L284) — Test optimize-paths flag.
  - `test_output_format_options(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L88) — Test output format choices.
  - `test_parser_creation(self)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L16) — Test parser is created successfully.
  - `test_project_root_option(self)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L320) — Test project root option.
  - `test_quiet_flag(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L110) — Test quiet flag.
  - `test_required_arguments(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L25) — Test required arguments are enforced.
  - `test_roots_and_files_mutually_exclusive(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L63) — Test that --roots and --files cannot be used together.
  - `test_summary_only_flag(self)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L272) — Test summary-only flag.
  - `test_timeout_ms_option(self)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L252) — Test timeout-ms option.
  - `test_total_only_flag(self)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L308) — Test total-only flag.
  - `test_word_flag(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_search_content_cli_parser.py#L142) — Test word boundary flag.
- uses (calls/refs, reference-scoped): [`_build_parser`](../../../tree_sitter_analyzer/cli/commands/search_content_cli.md#_build_parser)

