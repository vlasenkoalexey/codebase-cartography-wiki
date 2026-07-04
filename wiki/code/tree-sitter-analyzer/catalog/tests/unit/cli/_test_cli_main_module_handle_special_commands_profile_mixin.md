---
title: 'Module: tests/unit/cli/_test_cli_main_module_handle_special_commands_profile_mixin.py'
type: catalog
provenance: extracted
module: tests/unit/cli/_test_cli_main_module_handle_special_commands_profile_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli._test_cli_main_module_handle_special_commands_profile_mixin`/TestHandleSpecialCommandsProfileMixin#
symbols:
  TestHandleSpecialCommandsProfileMixin: ''
  TestHandleSpecialCommandsProfileMixin.test_effective_output_format_default: test_effective_output_format_default().
  TestHandleSpecialCommandsProfileMixin.test_effective_output_format_toon: test_effective_output_format_toon().
  TestHandleSpecialCommandsProfileMixin.test_show_common_queries_with_results: test_show_common_queries_with_results().
  TestHandleSpecialCommandsProfileMixin.test_show_common_queries_empty: test_show_common_queries_empty().
  TestHandleSpecialCommandsProfileMixin.test_sql_platform_info_with_profile: test_sql_platform_info_with_profile().
  TestHandleSpecialCommandsProfileMixin.test_sql_platform_info_no_profile: test_sql_platform_info_no_profile().
  TestHandleSpecialCommandsProfileMixin.test_record_sql_profile_success: test_record_sql_profile_success().
  TestHandleSpecialCommandsProfileMixin.test_record_sql_profile_failure: test_record_sql_profile_failure().
  TestHandleSpecialCommandsProfileMixin.test_compare_sql_profiles_missing_first: test_compare_sql_profiles_missing_first().
  TestHandleSpecialCommandsProfileMixin.test_compare_sql_profiles_missing_second: test_compare_sql_profiles_missing_second().
  TestHandleSpecialCommandsProfileMixin.test_compare_sql_profiles_success: test_compare_sql_profiles_success().
  TestHandleSpecialCommandsProfileMixin.test_compare_sql_profiles_error: test_compare_sql_profiles_error().
  TestHandleSpecialCommandsProfileMixin.__test__: __test__.
---
# Module: [`tests/unit/cli/_test_cli_main_module_handle_special_commands_profile_mixin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_profile_mixin.py)

## Classes
### `TestHandleSpecialCommandsProfileMixin`
- def: [`tests/unit/cli/_test_cli_main_module_handle_special_commands_profile_mixin.py:14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_profile_mixin.py#L14)
- doc: Tests for handle_special_commands() covering all branches.
- signature: `class TestHandleSpecialCommandsProfileMixin:`
- members:
  - `test_compare_sql_profiles_error(self, mock_output_error, mock_path_cls)` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_profile_mixin.py#L348) — compare_sql_profiles when comparison raises.
  - `test_compare_sql_profiles_missing_first(self, mock_output_error, mock_path_cls)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_profile_mixin.py#L237) — compare_sql_profiles when first profile doesn't exist.
  - `test_compare_sql_profiles_missing_second(self, mock_output_error, mock_path_cls)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_profile_mixin.py#L262) — compare_sql_profiles when second profile doesn't exist.
  - `test_compare_sql_profiles_success(self, mock_print, mock_generate_diff, mock_compare, mock_path_cls)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_profile_mixin.py#L291) — compare_sql_profiles success path.
  - `test_effective_output_format_default(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_profile_mixin.py#L21) — _effective_output_format returns 'json' by default.
  - `test_effective_output_format_toon(self)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_profile_mixin.py#L37) — _effective_output_format respects --format=toon.
  - `test_record_sql_profile_failure(self, mock_output_info, mock_output_error, mock_recorder_cls)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_profile_mixin.py#L212) — record_sql_profile failure path.
  - `test_record_sql_profile_success(self, mock_path_cls, mock_output_info, mock_recorder_cls)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_profile_mixin.py#L180) — record_sql_profile success path.
  - `test_show_common_queries_empty(self, mock_output_info, mock_get_common)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_profile_mixin.py#L80) — show_common_queries shows info when no common queries.
  - `test_show_common_queries_with_results(self, mock_output_list, mock_get_common)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_profile_mixin.py#L58) — show_common_queries lists common queries when available.
  - `test_sql_platform_info_no_profile(self, mock_output_list, mock_profile_cls, mock_detector)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_profile_mixin.py#L141) — sql_platform_info when no profile found.
  - `test_sql_platform_info_with_profile(self, mock_output_list, mock_profile_cls, mock_detector)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_profile_mixin.py#L104) — sql_platform_info when profile exists.
- protocol/private: `__test__`[`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/_test_cli_main_module_handle_special_commands_profile_mixin.py#L17)
- uses (calls/refs, reference-scoped): [`handle_special_commands`](../../../tree_sitter_analyzer/cli_main.md#handle_special_commands)  (1 test-only)
- used by: (1 test-only callers)

