---
title: 'Module: tests/unit/cli/_test_cli_main_module_parser_mixin.py'
type: catalog
provenance: extracted
module: tests/unit/cli/_test_cli_main_module_parser_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli._test_cli_main_module_parser_mixin`/TestCreateArgumentParserMixin#
symbols:
  TestCreateArgumentParserMixin: ''
  TestCreateArgumentParserMixin.test_parser_creation: test_parser_creation().
  TestCreateArgumentParserMixin.test_parser_accepts_agent_summary_only_for_change_impact: test_parser_accepts_agent_summary_only_for_change_impact().
  TestCreateArgumentParserMixin.test_parser_accepts_agent_workflow_pack: test_parser_accepts_agent_workflow_pack().
  TestCreateArgumentParserMixin.test_parser_accepts_agent_skills_inventory: test_parser_accepts_agent_skills_inventory().
  TestCreateArgumentParserMixin.test_parser_accepts_list_skills_alias: test_parser_accepts_list_skills_alias().
  TestCreateArgumentParserMixin.test_parser_accepts_change_impact_mode_and_test_toggle: test_parser_accepts_change_impact_mode_and_test_toggle().
  TestCreateArgumentParserMixin.test_parser_accepts_change_impact_resource_profile: test_parser_accepts_change_impact_resource_profile().
  TestCreateArgumentParserMixin.test_parser_has_file_path_argument: test_parser_has_file_path_argument().
  TestCreateArgumentParserMixin.test_parser_has_query_key_argument: test_parser_has_query_key_argument().
  TestCreateArgumentParserMixin.test_parser_has_query_string_argument: test_parser_has_query_string_argument().
  TestCreateArgumentParserMixin.test_parser_has_filter_argument: test_parser_has_filter_argument().
  TestCreateArgumentParserMixin.test_parser_has_list_queries_argument: test_parser_has_list_queries_argument().
  TestCreateArgumentParserMixin.test_parser_has_describe_query_argument: test_parser_has_describe_query_argument().
  TestCreateArgumentParserMixin.test_parser_has_show_supported_languages_argument: test_parser_has_show_supported_languages_argument().
  TestCreateArgumentParserMixin.test_parser_has_show_supported_extensions_argument: test_parser_has_show_supported_extensions_argument().
  TestCreateArgumentParserMixin.test_parser_has_output_format_argument: test_parser_has_output_format_argument().
  TestCreateArgumentParserMixin.test_parser_has_format_argument: test_parser_has_format_argument().
  TestCreateArgumentParserMixin.test_parser_has_table_argument: test_parser_has_table_argument().
  TestCreateArgumentParserMixin.test_parser_has_include_javadoc_argument: test_parser_has_include_javadoc_argument().
  TestCreateArgumentParserMixin.test_parser_has_advanced_argument: test_parser_has_advanced_argument().
  TestCreateArgumentParserMixin.test_parser_has_summary_argument: test_parser_has_summary_argument().
  TestCreateArgumentParserMixin.test_parser_has_structure_argument: test_parser_has_structure_argument().
  TestCreateArgumentParserMixin.test_parser_has_statistics_argument: test_parser_has_statistics_argument().
  TestCreateArgumentParserMixin.test_parser_has_language_argument: test_parser_has_language_argument().
  TestCreateArgumentParserMixin.test_parser_has_project_root_argument: test_parser_has_project_root_argument().
  TestCreateArgumentParserMixin.test_parser_has_quiet_argument: test_parser_has_quiet_argument().
  TestCreateArgumentParserMixin.test_parser_has_partial_read_argument: test_parser_has_partial_read_argument().
  TestCreateArgumentParserMixin.test_parser_has_start_line_argument: test_parser_has_start_line_argument().
  TestCreateArgumentParserMixin.test_parser_has_end_line_argument: test_parser_has_end_line_argument().
  TestCreateArgumentParserMixin.test_parser_has_start_column_argument: test_parser_has_start_column_argument().
  TestCreateArgumentParserMixin.test_parser_has_end_column_argument: test_parser_has_end_column_argument().
  TestCreateArgumentParserMixin.test_parser_default_output_format: test_parser_default_output_format().
  TestCreateArgumentParserMixin.test_parser_file_path_optional: test_parser_file_path_optional().
  TestCreateArgumentParserMixin.test_parser_has_safe_to_edit_edit_type_argument: test_parser_has_safe_to_edit_edit_type_argument().
  TestCreateArgumentParserMixin.test_parser_dependencies_supports_mcp_modes_and_legacy_full: test_parser_dependencies_supports_mcp_modes_and_legacy_full().
  TestCreateArgumentParserMixin.test_agent_command_aliases_normalize_to_existing_flags: test_agent_command_aliases_normalize_to_existing_flags().
  TestCreateArgumentParserMixin.test_agent_file_scoped_alias_without_path_keeps_existing_error_path: test_agent_file_scoped_alias_without_path_keeps_existing_error_path().
  TestCreateArgumentParserMixin.__test__: __test__.
---
# Module: [`tests/unit/cli/_test_cli_main_module_parser_mixin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py)

## Classes
### `TestCreateArgumentParserMixin`
- def: [`tests/unit/cli/_test_cli_main_module_parser_mixin.py:14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L14)
- doc: Tests for create_argument_parser function.
- signature: `class TestCreateArgumentParserMixin:`
- members:
  - `test_agent_command_aliases_normalize_to_existing_flags(self, argv: list[str], expected: list[str])` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L318) — Agent-friendly command aliases reuse the existing flag CLI.
  - `test_agent_file_scoped_alias_without_path_keeps_existing_error_path(self)` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L324) — Missing file paths still flow to MCP command validation.
  - `test_parser_accepts_agent_skills_inventory(self)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L41) — Agent skills inventory can be requested without a target file.
  - `test_parser_accepts_agent_summary_only_for_change_impact(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L25) — Change-impact can request a compact agent-only response.
  - `test_parser_accepts_agent_workflow_pack(self)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L33) — Agent workflow can be requested without a target file.
  - `test_parser_accepts_change_impact_mode_and_test_toggle(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L57) — Change-impact CLI exposes the MCP mode and include_tests controls.
  - `test_parser_accepts_change_impact_resource_profile(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L73) — Change-impact can request resource-aware local verification commands.
  - `test_parser_accepts_list_skills_alias(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L49) — `--list-skills` remains a compatibility alias for `--agent-skills`.
  - `test_parser_creation(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L19) — Test that argument parser is created successfully.
  - `test_parser_default_output_format(self)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L232) — Test that default output format is json.
  - `test_parser_dependencies_supports_mcp_modes_and_legacy_full(self, argv: list[str], expected_mode: str, expected_file_path: str | None)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L261) — Dependency CLI accepts MCP modes and the legacy full alias.
  - `test_parser_file_path_optional(self)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L238) — Test that file_path is optional.
  - `test_parser_has_advanced_argument(self)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L159) — Test that parser has --advanced argument.
  - `test_parser_has_describe_query_argument(self)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L117) — Test that parser has --describe-query argument.
  - `test_parser_has_end_column_argument(self)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L226) — Test that parser has --end-column argument.
  - `test_parser_has_end_line_argument(self)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L214) — Test that parser has --end-line argument.
  - `test_parser_has_file_path_argument(self)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L87) — Test that parser has file_path argument.
  - `test_parser_has_filter_argument(self)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L105) — Test that parser has --filter argument.
  - `test_parser_has_format_argument(self)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L141) — Test that parser has --format argument.
  - `test_parser_has_include_javadoc_argument(self)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L153) — Test that parser has --include-javadoc argument.
  - `test_parser_has_language_argument(self)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L184) — Test that parser has --language argument.
  - `test_parser_has_list_queries_argument(self)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L111) — Test that parser has --list-queries argument.
  - `test_parser_has_output_format_argument(self)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L135) — Test that parser has --output-format argument.
  - `test_parser_has_partial_read_argument(self)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L202) — Test that parser has --partial-read argument.
  - `test_parser_has_project_root_argument(self)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L190) — Test that parser has --project-root argument.
  - `test_parser_has_query_key_argument(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L93) — Test that parser has --query-key argument.
  - `test_parser_has_query_string_argument(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L99) — Test that parser has --query-string argument.
  - `test_parser_has_quiet_argument(self)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L196) — Test that parser has --quiet argument.
  - `test_parser_has_safe_to_edit_edit_type_argument(self)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L244) — Test that --edit-type supports MCP safe_to_edit schema values.
  - `test_parser_has_show_supported_extensions_argument(self)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L129) — Test that parser has --show-supported-extensions argument.
  - `test_parser_has_show_supported_languages_argument(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L123) — Test that parser has --show-supported-languages argument.
  - `test_parser_has_start_column_argument(self)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L220) — Test that parser has --start-column argument.
  - `test_parser_has_start_line_argument(self)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L208) — Test that parser has --start-line argument.
  - `test_parser_has_statistics_argument(self)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L178) — Test that parser has --statistics argument.
  - `test_parser_has_structure_argument(self)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L172) — Test that parser has --structure argument.
  - `test_parser_has_summary_argument(self)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L165) — Test that parser has --summary argument.
  - `test_parser_has_table_argument(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L147) — Test that parser has --table argument.
- protocol/private: `__test__`[`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_parser_mixin.py#L17)
- uses (calls/refs, reference-scoped): [`create_argument_parser`](../../../tree_sitter_analyzer/cli_main.md#create_argument_parser), [`_normalize_agent_command_aliases`](../../../tree_sitter_analyzer/cli_main.md#_normalize_agent_command_aliases)  (1 test-only)
- used by: (1 test-only callers)

