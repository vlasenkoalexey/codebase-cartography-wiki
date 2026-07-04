---
title: 'Module: tree_sitter_analyzer/cli/commands/summary_command.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/summary_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.summary_command`/
symbols:
  SummaryCommand._output_summary_analysis: SummaryCommand#_output_summary_analysis().
  SummaryCommand: SummaryCommand#
  SummaryCommand._partition_elements: SummaryCommand#_partition_elements().
  SummaryCommand._emit_summary: SummaryCommand#_emit_summary().
  SummaryCommand._build_summary_payload: SummaryCommand#_build_summary_payload().
  SummaryCommand._attach_summary_envelope: SummaryCommand#_attach_summary_envelope().
  SummaryCommand.execute_async: SummaryCommand#execute_async().
  _toon_available: _toon_available.
  SummaryCommand._output_text_format: SummaryCommand#_output_text_format().
  SummaryCommand._count: SummaryCommand#_count().
  SummaryCommand._requested_summary_types: SummaryCommand#_requested_summary_types().
  _format_element_summary_line: _format_element_summary_line().
---
# Module: [`tree_sitter_analyzer/cli/commands/summary_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/summary_command.py)

## Classes
### `SummaryCommand`  ·  implements/extends BaseCommand
- def: [`tree_sitter_analyzer/cli/commands/summary_command.py:58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/summary_command.py#L58)
- doc: Command for summary analysis with specified element types.
- signature: `class SummaryCommand(BaseCommand):`
- members:
  - `_attach_summary_envelope(summary_data: dict[str, Any], analysis_result: AnalysisResult, requested_types: list[str])` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/summary_command.py#L198) — Attach the canonical ``summary_line`` + ``agent_summary`` envelope.
  - `_build_summary_payload(analysis_result: AnalysisResult, *, requested_types: list[str], classes: list[Any], methods: list[Any], fields: list[Any], imports: list[Any])` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/summary_command.py#L131) — Build the ``summary_data`` dict honouring ``requested_types``.
  - `_emit_summary(self, summary_data: dict[str, Any], requested_types: list[str])` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/summary_command.py#L238) — Dispatch to json / toon / text emitter based on ``output_format``.
  - `_output_summary_analysis(self, analysis_result: AnalysisResult)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/summary_command.py#L69) — Output summary analysis results.
  - `_output_text_format(self, summary_data: dict, requested_types: list)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/summary_command.py#L252) — Output summary in human-readable text format.
  - `_partition_elements(analysis_result: AnalysisResult)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/summary_command.py#L104) — Bucket analysis elements into (classes, methods, fields, imports).
  - `_requested_summary_types(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/summary_command.py#L96) — Return the list of summary element types from ``--summary``.
  - `execute_async(self, language: str)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/summary_command.py#L61)
- protocol/private: `_count`[`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/summary_command.py#L213)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../models/result.md#AnalysisResult), [`elements`](../../models/result.md#AnalysisResult.elements), [`language`](../../models/result.md#AnalysisResult.language), [`file_path`](../../models/result.md#AnalysisResult.file_path), [`ToonFormatter`](../../formatters/toon_formatter.md#ToonFormatter), [`ELEMENT_TYPE_CLASS`](../../constants.md#ELEMENT_TYPE_CLASS), [`ELEMENT_TYPE_FUNCTION`](../../constants.md#ELEMENT_TYPE_FUNCTION), [`is_element_of_type`](../../constants.md#is_element_of_type), [`args`](base_command.md#BaseCommand.args), [`ELEMENT_TYPE_VARIABLE`](../../constants.md#ELEMENT_TYPE_VARIABLE), [`output_data`](../../output_manager.md#output_data), [`ELEMENT_TYPE_IMPORT`](../../constants.md#ELEMENT_TYPE_IMPORT), [`BaseCommand`](base_command.md#BaseCommand), [`format`](../../formatters/toon_formatter.md#ToonFormatter.format), [`analyze_file`](base_command.md#BaseCommand.analyze_file), [`output_json`](../../output_manager.md#output_json), [`output_section`](../../output_manager.md#output_section), [`_toon_available`](summary_command.md#_toon_available), [`normalize_parameters`](../../_api_result_helpers.md#normalize_parameters), [`_format_element_summary_line`](summary_command.md#_format_element_summary_line)
- used by: [`BaseCommand`](base_command.md#BaseCommand), [`execute_async`](base_command.md#BaseCommand.execute_async), [`_create_file_command`](../../cli_main.md#_create_file_command)  (20 test-only)

## Functions
- `_format_element_summary_line(element: dict[str, Any])` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/summary_command.py#L33) — Format a single ``element`` dict as the text-summary bullet line.

## Module values
- `_toon_available` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/summary_command.py#L25)

