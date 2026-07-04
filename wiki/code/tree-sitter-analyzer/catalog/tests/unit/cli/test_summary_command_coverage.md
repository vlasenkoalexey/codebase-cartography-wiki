---
title: 'Module: tests/unit/cli/test_summary_command_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_summary_command_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_summary_command_coverage`/
symbols:
  TestSummaryCommandCoverage.command: TestSummaryCommandCoverage#command.
  TestSummaryCommandCoverage.test_output_summary_analysis_all_types: TestSummaryCommandCoverage#test_output_summary_analysis_all_types().
  TestSummaryCommandCoverage.test_text_format_with_method_elements: TestSummaryCommandCoverage#test_text_format_with_method_elements().
  TestSummaryCommandCoverage.test_output_summary_analysis_filtered_types: TestSummaryCommandCoverage#test_output_summary_analysis_filtered_types().
  TestSummaryCommandCoverage.test_execute_async_with_result_json: TestSummaryCommandCoverage#test_execute_async_with_result_json().
  TestSummaryCommandCoverage.test_execute_async_no_result: TestSummaryCommandCoverage#test_execute_async_no_result().
  TestSummaryCommandCoverage.test_execute_async_with_result_text: TestSummaryCommandCoverage#test_execute_async_with_result_text().
  TestSummaryCommandCoverage.test_json_output_with_methods: TestSummaryCommandCoverage#test_json_output_with_methods().
  TestSummaryCommandCoverage.test_toon_output_with_elements: TestSummaryCommandCoverage#test_toon_output_with_elements().
  TestSummaryCommandCoverage.test_output_summary_analysis_default_types: TestSummaryCommandCoverage#test_output_summary_analysis_default_types().
  TestSummaryCommandCoverage.mock_args: TestSummaryCommandCoverage#mock_args.
  asyncio_run: asyncio_run().
  TestSummaryCommandCoverage.check_side_effect: TestSummaryCommandCoverage#check_side_effect().
  TestSummaryCommandCoverage: TestSummaryCommandCoverage#
  TestSummaryCommandCoverage.setup_method: TestSummaryCommandCoverage#setup_method().
---
# Module: [`tests/unit/cli/test_summary_command_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_coverage.py)

## Classes
### `TestSummaryCommandCoverage`
- def: [`tests/unit/cli/test_summary_command_coverage.py:12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_coverage.py#L12)
- signature: `class TestSummaryCommandCoverage:`
- members:
  - `check_side_effect(elem, type_const)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_coverage.py#L96)
  - `setup_method(self)` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_coverage.py#L13)
  - `test_execute_async_no_result(self, mock_output_data, mock_output_section)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_coverage.py#L22) — Test execute_async with no analysis result
  - `test_execute_async_with_result_json(self, mock_output_json)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_coverage.py#L48) — Test execute_async with result (json output)
  - `test_execute_async_with_result_text(self, mock_output_data, mock_output_section)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_coverage.py#L30) — Test execute_async with result (text output)
  - `test_json_output_with_methods(self, mock_output_json)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_coverage.py#L229) — Test JSON output path covering lines 130-131
  - `test_output_summary_analysis_all_types(self, mock_output_data)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_coverage.py#L62) — Test _output_summary_analysis with all element types
  - `test_output_summary_analysis_default_types(self, mock_output_section, mock_output_data)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_coverage.py#L150) — Test _output_summary_analysis with default types (classes,methods)
  - `test_output_summary_analysis_filtered_types(self, mock_output_data)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_coverage.py#L115) — Test _output_summary_analysis with specific types requested
  - `test_text_format_with_method_elements(self, mock_output_section, mock_output_data)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_coverage.py#L166) — Test text output with method elements covering lines 95-107, 137-169
  - `test_toon_output_with_elements(self, mock_output_section, mock_toon_cls)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_coverage.py#L267) — Test toon output path covering lines 132-135
  - `command` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_coverage.py#L17)
  - `mock_args` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_coverage.py#L14)
- uses (calls/refs, reference-scoped): [`ELEMENT_TYPE_CLASS`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_CLASS), [`ELEMENT_TYPE_FUNCTION`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_FUNCTION), [`args`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand.args), [`ELEMENT_TYPE_VARIABLE`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_VARIABLE), [`ELEMENT_TYPE_IMPORT`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_IMPORT), [`analyze_file`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand.analyze_file), [`_output_summary_analysis`](../../../tree_sitter_analyzer/cli/commands/summary_command.md#SummaryCommand._output_summary_analysis), [`SummaryCommand`](../../../tree_sitter_analyzer/cli/commands/summary_command.md#SummaryCommand), [`execute_async`](../../../tree_sitter_analyzer/cli/commands/summary_command.md#SummaryCommand.execute_async)  (1 test-only)

## Functions
- `asyncio_run(coro)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_coverage.py#L301)

