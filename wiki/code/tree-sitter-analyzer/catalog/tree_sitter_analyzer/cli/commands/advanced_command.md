---
title: 'Module: tree_sitter_analyzer/cli/commands/advanced_command.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/advanced_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.advanced_command`/
symbols:
  AdvancedCommand._output_statistics: AdvancedCommand#_output_statistics().
  AdvancedCommand._output_full_analysis: AdvancedCommand#_output_full_analysis().
  AdvancedCommand._output_text_analysis: AdvancedCommand#_output_text_analysis().
  _full_analysis_dict: _full_analysis_dict().
  _per_element_counts: _per_element_counts().
  AdvancedCommand: AdvancedCommand#
  _build_elements_payload: _build_elements_payload().
  AdvancedCommand.execute_async: AdvancedCommand#execute_async().
  _toon_available: _toon_available.
  _collect_complexity_metrics: _collect_complexity_metrics().
  AdvancedCommand._calculate_file_metrics: AdvancedCommand#_calculate_file_metrics().
  _build_advanced_summary_line: _build_advanced_summary_line().
---
# Module: [`tree_sitter_analyzer/cli/commands/advanced_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command.py)

## Classes
### `AdvancedCommand`  ·  implements/extends BaseCommand
- def: [`tree_sitter_analyzer/cli/commands/advanced_command.py:188`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command.py#L188)
- doc: Command for advanced analysis.
- signature: `class AdvancedCommand(BaseCommand):`
- members:
  - `_calculate_file_metrics(self, file_path: str, language: str)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command.py#L203) — Calculate accurate file metrics including line counts.
  - `_output_full_analysis(self, analysis_result: AnalysisResult)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command.py#L274) — Output full analysis results. — documented in [tree_sitter_analyzer-models-result](../../../../concepts/tree_sitter_analyzer-models-result.md)
  - `_output_statistics(self, analysis_result: AnalysisResult)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command.py#L216) — Output statistics only. — documented in [tree_sitter_analyzer-models-result](../../../../concepts/tree_sitter_analyzer-models-result.md)
  - `_output_text_analysis(self, analysis_result: AnalysisResult)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command.py#L304) — Output analysis in text format.
  - `execute_async(self, language: str)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command.py#L191)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../models/result.md#AnalysisResult), [`elements`](../../models/result.md#AnalysisResult.elements), [`language`](../../models/result.md#AnalysisResult.language), [`file_path`](../../models/result.md#AnalysisResult.file_path), [`ToonFormatter`](../../formatters/toon_formatter.md#ToonFormatter), [`ELEMENT_TYPE_CLASS`](../../constants.md#ELEMENT_TYPE_CLASS), [`line_count`](../../models/result.md#AnalysisResult.line_count), [`ELEMENT_TYPE_FUNCTION`](../../constants.md#ELEMENT_TYPE_FUNCTION), [`args`](base_command.md#BaseCommand.args), [`ELEMENT_TYPE_VARIABLE`](../../constants.md#ELEMENT_TYPE_VARIABLE), [`output_data`](../../output_manager.md#output_data), [`node_count`](../../models/result.md#AnalysisResult.node_count), [`ELEMENT_TYPE_IMPORT`](../../constants.md#ELEMENT_TYPE_IMPORT), [`BaseCommand`](base_command.md#BaseCommand), [`format`](../../formatters/toon_formatter.md#ToonFormatter.format), [`analyze_file`](base_command.md#BaseCommand.analyze_file), [`output_json`](../../output_manager.md#output_json), [`get_element_type`](../../constants.md#get_element_type), [`_full_analysis_dict`](advanced_command.md#_full_analysis_dict), [`output_section`](../../output_manager.md#output_section), [`_per_element_counts`](advanced_command.md#_per_element_counts), [`_build_elements_payload`](advanced_command.md#_build_elements_payload), [`calculate_file_metrics`](advanced_command_helpers.md#calculate_file_metrics), [`_toon_available`](advanced_command.md#_toon_available), [`_collect_complexity_metrics`](advanced_command.md#_collect_complexity_metrics), [`_build_advanced_summary_line`](advanced_command.md#_build_advanced_summary_line)
- used by: [`BaseCommand`](base_command.md#BaseCommand), [`execute_async`](base_command.md#BaseCommand.execute_async), [`_create_file_command`](../../cli_main.md#_create_file_command)  (3 test-only)

## Functions
- `_build_advanced_summary_line(file_path: str, language: str, line_count: int, counts: dict[str, int], element_count: int, *, mode: str)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command.py#L36) — Compose the canonical headline for CLI ``--advanced`` responses.
- `_build_elements_payload(elements: Sequence[object], result_language: str | None = None)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command.py#L109) — Convert AST elements to JSON-payload dicts via ``element_to_dict``.
- `_collect_complexity_metrics(elements: Sequence[object])` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command.py#L89) — Aggregate function-level complexity stats from ``elements``.
- `_full_analysis_dict(analysis_result: AnalysisResult, elements_payload: list[dict[str, object]], counts: dict[str, int], complexity: dict[str, float])` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command.py#L140) — Assemble the canonical full-analysis envelope.
- `_per_element_counts(elements: Sequence[object])` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command.py#L61) — Compute per-kind element aggregations for parity with MCP analyze_scale.

## Module values
- `_toon_available` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command.py#L28)

