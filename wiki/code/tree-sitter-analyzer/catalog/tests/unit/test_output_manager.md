---
title: 'Module: tests/unit/test_output_manager.py'
type: catalog
provenance: extracted
module: tests/unit/test_output_manager.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_output_manager`/Test
symbols:
  TestOutputManagerInit.test_default_format: OutputManagerInit#test_default_format().
  TestGlobalFunctions.test_set_output_mode_creates_new_manager: GlobalFunctions#test_set_output_mode_creates_new_manager().
  TestOutputManagerInit.test_json_output_forces_format: OutputManagerInit#test_json_output_forces_format().
  TestOutputManagerInit.test_custom_format: OutputManagerInit#test_custom_format().
  TestOutputManagerInit.test_quiet_mode: OutputManagerInit#test_quiet_mode().
  TestOutputManagerInfo.test_info_prints_to_stderr: OutputManagerInfo#test_info_prints_to_stderr().
  TestOutputManagerInfo.test_info_suppressed_in_quiet: OutputManagerInfo#test_info_suppressed_in_quiet().
  TestOutputManagerInfo.test_error_always_prints: OutputManagerInfo#test_error_always_prints().
  TestOutputManagerInfo.test_warning_prints_to_stderr: OutputManagerInfo#test_warning_prints_to_stderr().
  TestOutputManagerInfo.test_warning_suppressed_in_quiet: OutputManagerInfo#test_warning_suppressed_in_quiet().
  TestOutputManagerInfo.test_success_prints_checkmark_to_stderr: OutputManagerInfo#test_success_prints_checkmark_to_stderr().
  TestOutputManagerData.test_json_output: OutputManagerData#test_json_output().
  TestOutputManagerData.test_json_string_passthrough: OutputManagerData#test_json_string_passthrough().
  TestOutputManagerData.test_toon_mcp_response_passthrough: OutputManagerData#test_toon_mcp_response_passthrough().
  TestOutputManagerData.test_toon_response_as_json_when_json_format: OutputManagerData#test_toon_response_as_json_when_json_format().
  TestOutputManagerData.test_json_output_flag_overrides_format: OutputManagerData#test_json_output_flag_overrides_format().
  TestOutputManagerFormatData.test_dict_formatting: OutputManagerFormatData#test_dict_formatting().
  TestOutputManagerFormatData.test_list_formatting: OutputManagerFormatData#test_list_formatting().
  TestOutputManagerFormatData.test_string_formatting: OutputManagerFormatData#test_string_formatting().
  TestOutputManagerResultsHeader.test_results_header: OutputManagerResultsHeader#test_results_header().
  TestOutputManagerResultsHeader.test_results_header_suppressed_quiet: OutputManagerResultsHeader#test_results_header_suppressed_quiet().
  TestOutputManagerQueryResult.test_displays_result: OutputManagerQueryResult#test_displays_result().
  TestOutputManagerQueryResult.test_quiet_suppresses_query_result: OutputManagerQueryResult#test_quiet_suppresses_query_result().
  TestOutputManagerList.test_list_with_title: OutputManagerList#test_list_with_title().
  TestOutputManagerList.test_string_input_becomes_single_item: OutputManagerList#test_string_input_becomes_single_item().
  TestOutputManagerList.test_quiet_suppresses_list: OutputManagerList#test_quiet_suppresses_list().
  TestOutputManagerExtensions.test_shows_extensions: OutputManagerExtensions#test_shows_extensions().
  TestGlobalFunctions.test_output_info_delegates: GlobalFunctions#test_output_info_delegates().
  TestGlobalFunctions.test_output_json_delegates: GlobalFunctions#test_output_json_delegates().
  TestGlobalFunctions.test_output_data_delegates: GlobalFunctions#test_output_data_delegates().
  TestOutputManagerInit: OutputManagerInit#
  TestOutputManagerInfo: OutputManagerInfo#
  TestOutputManagerData: OutputManagerData#
  TestOutputManagerFormatData: OutputManagerFormatData#
  TestOutputManagerResultsHeader: OutputManagerResultsHeader#
  TestOutputManagerQueryResult: OutputManagerQueryResult#
  TestOutputManagerList: OutputManagerList#
  TestOutputManagerExtensions: OutputManagerExtensions#
  TestGlobalFunctions: GlobalFunctions#
---
# Module: [`tests/unit/test_output_manager.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py)

## Classes
### `TestGlobalFunctions`
- def: [`tests/unit/test_output_manager.py:217`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L217)
- doc: Tests for module-level convenience functions.
- signature: `class TestGlobalFunctions:`
- members:
  - `test_output_data_delegates(self, capsys)` — [`L243`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L243)
  - `test_output_info_delegates(self, capsys)` — [`L229`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L229) — Q2 (round-33): convenience wrapper inherits the stderr
  - `test_output_json_delegates(self, capsys)` — [`L238`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L238)
  - `test_set_output_mode_creates_new_manager(self)` — [`L220`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L220)
- uses (calls/refs, reference-scoped): [`output_data`](../../tree_sitter_analyzer/output_manager.md#output_data), [`output_info`](../../tree_sitter_analyzer/output_manager.md#output_info), [`output_json`](../../tree_sitter_analyzer/output_manager.md#output_json), [`set_output_mode`](../../tree_sitter_analyzer/output_manager.md#set_output_mode), [`quiet`](../../tree_sitter_analyzer/output_manager.md#OutputManager.quiet), [`get_output_manager`](../../tree_sitter_analyzer/output_manager.md#get_output_manager)

### `TestOutputManagerData`
- def: [`tests/unit/test_output_manager.py:83`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L83)
- doc: Tests for data() method — format routing.
- signature: `class TestOutputManagerData:`
- members:
  - `test_json_output(self, capsys)` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L86)
  - `test_json_output_flag_overrides_format(self, capsys)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L114)
  - `test_json_string_passthrough(self, capsys)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L93) — ``JsonFormatter`` deliberately passes strings through as-is so
  - `test_toon_mcp_response_passthrough(self, capsys)` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L102)
  - `test_toon_response_as_json_when_json_format(self, capsys)` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L107)
- uses (calls/refs, reference-scoped): [`OutputManager`](../../tree_sitter_analyzer/output_manager.md#OutputManager), [`data`](../../tree_sitter_analyzer/output_manager.md#OutputManager.data)

### `TestOutputManagerExtensions`
- def: [`tests/unit/test_output_manager.py:206`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L206)
- doc: Tests for extension_list method.
- signature: `class TestOutputManagerExtensions:`
- members:
  - `test_shows_extensions(self, capsys)` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L209)
- uses (calls/refs, reference-scoped): [`OutputManager`](../../tree_sitter_analyzer/output_manager.md#OutputManager), [`extension_list`](../../tree_sitter_analyzer/output_manager.md#OutputManager.extension_list)

### `TestOutputManagerFormatData`
- def: [`tests/unit/test_output_manager.py:122`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L122)
- doc: Tests for _format_data fallback.
- signature: `class TestOutputManagerFormatData:`
- members:
  - `test_dict_formatting(self, capsys)` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L125)
  - `test_list_formatting(self, capsys)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L132)
  - `test_string_formatting(self, capsys)` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L139)
- uses (calls/refs, reference-scoped): [`OutputManager`](../../tree_sitter_analyzer/output_manager.md#OutputManager), [`_format_data`](../../tree_sitter_analyzer/output_manager.md#OutputManager._format_data)

### `TestOutputManagerInfo`
- def: [`tests/unit/test_output_manager.py:37`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L37)
- doc: Tests for info/warning/success/error methods.
- signature: `class TestOutputManagerInfo:`
- members:
  - `test_error_always_prints(self, capsys)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L57)
  - `test_info_prints_to_stderr(self, capsys)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L40) — Q2 (round-33): ``info`` is diagnostic, must NOT pollute stdout
  - `test_info_suppressed_in_quiet(self, capsys)` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L50)
  - `test_success_prints_checkmark_to_stderr(self, capsys)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L73) — Q2 (round-33): ``success`` is diagnostic and must go to stderr,
  - `test_warning_prints_to_stderr(self, capsys)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L62)
  - `test_warning_suppressed_in_quiet(self, capsys)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L67)
- uses (calls/refs, reference-scoped): [`OutputManager`](../../tree_sitter_analyzer/output_manager.md#OutputManager), [`warning`](../../tree_sitter_analyzer/output_manager.md#OutputManager.warning), [`info`](../../tree_sitter_analyzer/output_manager.md#OutputManager.info), [`success`](../../tree_sitter_analyzer/output_manager.md#OutputManager.success), [`error`](../../tree_sitter_analyzer/output_manager.md#OutputManager.error)

### `TestOutputManagerInit`
- def: [`tests/unit/test_output_manager.py:15`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L15)
- doc: Tests for OutputManager initialization.
- signature: `class TestOutputManagerInit:`
- members:
  - `test_custom_format(self)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L28)
  - `test_default_format(self)` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L18)
  - `test_json_output_forces_format(self)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L24)
  - `test_quiet_mode(self)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L32)
- uses (calls/refs, reference-scoped): [`OutputManager`](../../tree_sitter_analyzer/output_manager.md#OutputManager), [`quiet`](../../tree_sitter_analyzer/output_manager.md#OutputManager.quiet), [`output_format`](../../tree_sitter_analyzer/output_manager.md#OutputManager.output_format), [`json_output`](../../tree_sitter_analyzer/output_manager.md#OutputManager.json_output)

### `TestOutputManagerList`
- def: [`tests/unit/test_output_manager.py:184`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L184)
- doc: Tests for output_list method.
- signature: `class TestOutputManagerList:`
- members:
  - `test_list_with_title(self, capsys)` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L187)
  - `test_quiet_suppresses_list(self, capsys)` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L200)
  - `test_string_input_becomes_single_item(self, capsys)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L194)
- uses (calls/refs, reference-scoped): [`OutputManager`](../../tree_sitter_analyzer/output_manager.md#OutputManager), [`output_list`](../../tree_sitter_analyzer/output_manager.md#OutputManager.output_list)

### `TestOutputManagerQueryResult`
- def: [`tests/unit/test_output_manager.py:159`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L159)
- doc: Tests for query_result method.
- signature: `class TestOutputManagerQueryResult:`
- members:
  - `test_displays_result(self, capsys)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L162)
  - `test_quiet_suppresses_query_result(self, capsys)` — [`L178`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L178)
- uses (calls/refs, reference-scoped): [`OutputManager`](../../tree_sitter_analyzer/output_manager.md#OutputManager), [`query_result`](../../tree_sitter_analyzer/output_manager.md#OutputManager.query_result)

### `TestOutputManagerResultsHeader`
- def: [`tests/unit/test_output_manager.py:145`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L145)
- doc: Tests for results_header / output_section.
- signature: `class TestOutputManagerResultsHeader:`
- members:
  - `test_results_header(self, capsys)` — [`L148`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L148)
  - `test_results_header_suppressed_quiet(self, capsys)` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_output_manager.py#L153)
- uses (calls/refs, reference-scoped): [`OutputManager`](../../tree_sitter_analyzer/output_manager.md#OutputManager), [`results_header`](../../tree_sitter_analyzer/output_manager.md#OutputManager.results_header)

