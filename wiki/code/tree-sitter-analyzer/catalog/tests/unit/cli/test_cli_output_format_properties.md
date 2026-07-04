---
title: 'Module: tests/unit/cli/test_cli_output_format_properties.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_cli_output_format_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_cli_output_format_properties`/
symbols:
  cli_output_data: cli_output_data.
  PROPERTY_SETTINGS: PROPERTY_SETTINGS.
  TestCLIOutputFormatProperties.test_property_12_json_format_produces_valid_json: TestCLIOutputFormatProperties#test_property_12_json_format_produces_valid_json().
  TestCLIOutputFormatProperties.test_property_12_json_format_roundtrip_preserves_data: TestCLIOutputFormatProperties#test_property_12_json_format_roundtrip_preserves_data().
  TestCLIOutputFormatProperties.test_property_12_text_format_produces_readable_output: TestCLIOutputFormatProperties#test_property_12_text_format_produces_readable_output().
  TestCLIOutputFormatProperties.test_property_12_search_result_json_contains_required_fields: TestCLIOutputFormatProperties#test_property_12_search_result_json_contains_required_fields().
  TestCLIOutputFormatProperties.test_property_12_list_files_result_json_contains_required_fields: TestCLIOutputFormatProperties#test_property_12_list_files_result_json_contains_required_fields().
  TestCLIOutputFormatProperties.test_property_12_analysis_result_json_contains_required_fields: TestCLIOutputFormatProperties#test_property_12_analysis_result_json_contains_required_fields().
  TestCLIOutputFormatEdgeCases.test_property_12_arbitrary_dict_json_format: TestCLIOutputFormatEdgeCases#test_property_12_arbitrary_dict_json_format().
  TestCLIOutputFormatEdgeCases.test_property_12_arbitrary_list_json_format: TestCLIOutputFormatEdgeCases#test_property_12_arbitrary_list_json_format().
  TestGlobalOutputFunctions.test_property_12_global_output_data_json: TestGlobalOutputFunctions#test_property_12_global_output_data_json().
  TestGlobalOutputFunctions.test_property_12_global_output_json_function: TestGlobalOutputFunctions#test_property_12_global_output_json_function().
  TestCLIOutputFormatProperties.test_property_12_output_mode_configuration: TestCLIOutputFormatProperties#test_property_12_output_mode_configuration().
  TestCLIOutputFormatProperties.test_property_12_output_list_contains_all_items: TestCLIOutputFormatProperties#test_property_12_output_list_contains_all_items().
  TestCLIOutputFormatEdgeCases.test_property_12_integer_count_json_format: TestCLIOutputFormatEdgeCases#test_property_12_integer_count_json_format().
  TestCLIOutputFormatEdgeCases.test_property_12_error_output_contains_message: TestCLIOutputFormatEdgeCases#test_property_12_error_output_contains_message().
  file_path: file_path.
  TestCLIOutputFormatEdgeCases.test_property_12_empty_data_json_format: TestCLIOutputFormatEdgeCases#test_property_12_empty_data_json_format().
  TestCLIOutputFormatEdgeCases.test_property_12_none_data_json_format: TestCLIOutputFormatEdgeCases#test_property_12_none_data_json_format().
  search_result: search_result().
  list_files_result: list_files_result().
  analysis_result_data: analysis_result_data().
  file_list: file_list.
  match_result: match_result().
  error_result: error_result().
  simple_value: simple_value.
  TestCLIOutputFormatProperties: TestCLIOutputFormatProperties#
  TestCLIOutputFormatEdgeCases: TestCLIOutputFormatEdgeCases#
  TestGlobalOutputFunctions: TestGlobalOutputFunctions#
---
# Module: [`tests/unit/cli/test_cli_output_format_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py)

## Classes
### `TestCLIOutputFormatEdgeCases`
- def: [`tests/unit/cli/test_cli_output_format_properties.py:468`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L468)
- doc: Property-based tests for CLI output format edge cases.
- signature: `class TestCLIOutputFormatEdgeCases:`
- members:
  - `test_property_12_arbitrary_dict_json_format(self, data: dict, capsys)` — [`L491`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L491) — **Feature: test-coverage-improvement, Property 12: CLI Output Format Consistency**
  - `test_property_12_arbitrary_list_json_format(self, data: list, capsys)` — [`L515`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L515) — **Feature: test-coverage-improvement, Property 12: CLI Output Format Consistency**
  - `test_property_12_empty_data_json_format(self, capsys)` — [`L592`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L592) — **Feature: test-coverage-improvement, Property 12: CLI Output Format Consistency**
  - `test_property_12_error_output_contains_message(self, error_msg: str, capsys)` — [`L571`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L571) — **Feature: test-coverage-improvement, Property 12: CLI Output Format Consistency**
  - `test_property_12_integer_count_json_format(self, count: int, capsys)` — [`L540`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L540) — **Feature: test-coverage-improvement, Property 12: CLI Output Format Consistency**
  - `test_property_12_none_data_json_format(self, capsys)` — [`L612`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L612) — **Feature: test-coverage-improvement, Property 12: CLI Output Format Consistency**
- uses (calls/refs, reference-scoped): [`OutputManager`](../../../tree_sitter_analyzer/output_manager.md#OutputManager), [`data`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.data), [`error`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.error)  (2 test-only)

### `TestCLIOutputFormatProperties`
- def: [`tests/unit/cli/test_cli_output_format_properties.py:217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L217)
- doc: Property-based tests for CLI output format consistency.
- signature: `class TestCLIOutputFormatProperties:`
- members:
  - `test_property_12_analysis_result_json_contains_required_fields(self, data: dict, capsys)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L377) — **Feature: test-coverage-improvement, Property 12: CLI Output Format Consistency**
  - `test_property_12_json_format_produces_valid_json(self, data: Any, capsys)` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L227) — **Feature: test-coverage-improvement, Property 12: CLI Output Format Consistency**
  - `test_property_12_json_format_roundtrip_preserves_data(self, data: Any, capsys)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L260) — **Feature: test-coverage-improvement, Property 12: CLI Output Format Consistency**
  - `test_property_12_list_files_result_json_contains_required_fields(self, data: dict, capsys)` — [`L349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L349) — **Feature: test-coverage-improvement, Property 12: CLI Output Format Consistency**
  - `test_property_12_output_list_contains_all_items(self, items: list, capsys)` — [`L450`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L450) — **Feature: test-coverage-improvement, Property 12: CLI Output Format Consistency**
  - `test_property_12_output_mode_configuration(self, quiet: bool, json_output: bool, capsys)` — [`L400`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L400) — **Feature: test-coverage-improvement, Property 12: CLI Output Format Consistency**
  - `test_property_12_search_result_json_contains_required_fields(self, data: dict, capsys)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L319) — **Feature: test-coverage-improvement, Property 12: CLI Output Format Consistency**
  - `test_property_12_text_format_produces_readable_output(self, data: Any, capsys)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L294) — **Feature: test-coverage-improvement, Property 12: CLI Output Format Consistency**
- uses (calls/refs, reference-scoped): [`OutputManager`](../../../tree_sitter_analyzer/output_manager.md#OutputManager), [`data`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.data), [`info`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.info), [`output_list`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.output_list)  (5 test-only)

### `TestGlobalOutputFunctions`
- def: [`tests/unit/cli/test_cli_output_format_properties.py:629`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L629)
- doc: Property-based tests for global output functions.
- signature: `class TestGlobalOutputFunctions:`
- members:
  - `test_property_12_global_output_data_json(self, data: Any, capsys)` — [`L639`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L639) — **Feature: test-coverage-improvement, Property 12: CLI Output Format Consistency**
  - `test_property_12_global_output_json_function(self, data: Any, capsys)` — [`L664`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L664) — **Feature: test-coverage-improvement, Property 12: CLI Output Format Consistency**
- uses (calls/refs, reference-scoped): [`output_data`](../../../tree_sitter_analyzer/output_manager.md#output_data), [`output_json`](../../../tree_sitter_analyzer/output_manager.md#output_json), [`set_output_mode`](../../../tree_sitter_analyzer/output_manager.md#set_output_mode)  (2 test-only)

## Functions
- `analysis_result_data(draw)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L140) — Generate an analysis result data structure.
- `error_result(draw)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L182) — Generate an error result.
- `list_files_result(draw)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L127) — Generate a list files result.
- `match_result(draw)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L74) — Generate a search match result.
- `search_result(draw)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L105) — Generate a complete search result.

## Module values
- `PROPERTY_SETTINGS` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L28)
- `cli_output_data` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L202)
- `file_list` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L69)
- `file_path` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L55)
- `simple_value` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_output_format_properties.py#L39)

