---
title: 'Module: tree_sitter_analyzer/cli/commands/structure_command.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/structure_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.structure_command`/
symbols:
  StructureCommand._convert_to_legacy_format: StructureCommand#_convert_to_legacy_format().
  StructureCommand._output_structure_analysis: StructureCommand#_output_structure_analysis().
  StructureCommand._partition_structure_elements: StructureCommand#_partition_structure_elements().
  StructureCommand: StructureCommand#
  StructureCommand._attach_structure_envelope: StructureCommand#_attach_structure_envelope().
  StructureCommand._legacy_metadata_block: StructureCommand#_legacy_metadata_block().
  _toon_available: _toon_available.
  StructureCommand._legacy_statistics_block: StructureCommand#_legacy_statistics_block().
  StructureCommand.execute_async: StructureCommand#execute_async().
  StructureCommand._output_text_format: StructureCommand#_output_text_format().
  StructureCommand._legacy_method_row: StructureCommand#_legacy_method_row().
  StructureCommand._legacy_class_row: StructureCommand#_legacy_class_row().
  StructureCommand._legacy_field_row: StructureCommand#_legacy_field_row().
  StructureCommand._legacy_import_row: StructureCommand#_legacy_import_row().
  StructureCommand._legacy_package_block: StructureCommand#_legacy_package_block().
---
# Module: [`tree_sitter_analyzer/cli/commands/structure_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/structure_command.py)

## Classes
### `StructureCommand`  ·  implements/extends BaseCommand
- def: [`tree_sitter_analyzer/cli/commands/structure_command.py:33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/structure_command.py#L33)
- doc: Command for structure analysis with Japanese output.
- signature: `class StructureCommand(BaseCommand):`
- members:
  - `_attach_structure_envelope(legacy_dict: dict[str, Any], analysis_result: AnalysisResult, *, classes: list[Any], methods: list[Any], fields: list[Any], imports: list[Any])` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/structure_command.py#L235) — Attach the r37aa canonical envelope (success / summary_line /
  - `_convert_to_legacy_format(self, analysis_result: AnalysisResult)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/structure_command.py#L61) — Convert AnalysisResult to legacy structure format expected by tests.
  - `_legacy_class_row(c: Any)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/structure_command.py#L100) — Return the legacy ``classes[]`` dict row for one class element.
  - `_legacy_field_row(f: Any)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/structure_command.py#L131) — Return the legacy ``fields[]`` dict row for one field element.
  - `_legacy_import_row(i: Any)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/structure_command.py#L143) — Return the legacy ``imports[]`` dict row for one import element.
  - `_legacy_metadata_block(analysis_result: AnalysisResult)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/structure_command.py#L220) — Return the legacy ``analysis_metadata`` dict (incl. timestamp).
  - `_legacy_method_row(m: Any)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/structure_command.py#L112) — Return the legacy ``methods[]`` dict row for one method element.
  - `_legacy_package_block(packages: list[Any])` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/structure_command.py#L189) — Return the package dict (name + line_range tuple) or ``None``.
  - `_legacy_statistics_block(analysis_result: AnalysisResult, classes: list[Any], methods: list[Any], fields: list[Any], imports: list[Any])` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/structure_command.py#L202) — Return the legacy ``statistics`` dict.
  - `_output_structure_analysis(self, analysis_result: AnalysisResult)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/structure_command.py#L44) — Output structure analysis results with appropriate header.
  - `_output_text_format(self, structure_dict: dict)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/structure_command.py#L268) — Output structure analysis in human-readable text format.
  - `_partition_structure_elements(analysis_result: AnalysisResult)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/structure_command.py#L157) — Bucket elements into (classes, methods, fields, imports, packages).
  - `execute_async(self, language: str)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/structure_command.py#L36)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../models/result.md#AnalysisResult), [`elements`](../../models/result.md#AnalysisResult.elements), [`language`](../../models/result.md#AnalysisResult.language), [`file_path`](../../models/result.md#AnalysisResult.file_path), [`ToonFormatter`](../../formatters/toon_formatter.md#ToonFormatter), [`ELEMENT_TYPE_CLASS`](../../constants.md#ELEMENT_TYPE_CLASS), [`line_count`](../../models/result.md#AnalysisResult.line_count), [`ELEMENT_TYPE_FUNCTION`](../../constants.md#ELEMENT_TYPE_FUNCTION), [`is_element_of_type`](../../constants.md#is_element_of_type), [`args`](base_command.md#BaseCommand.args), [`ELEMENT_TYPE_VARIABLE`](../../constants.md#ELEMENT_TYPE_VARIABLE), [`output_data`](../../output_manager.md#output_data), [`ELEMENT_TYPE_IMPORT`](../../constants.md#ELEMENT_TYPE_IMPORT), [`BaseCommand`](base_command.md#BaseCommand), [`format`](../../formatters/toon_formatter.md#ToonFormatter.format), [`analyze_file`](base_command.md#BaseCommand.analyze_file), [`output_json`](../../output_manager.md#output_json), [`ELEMENT_TYPE_PACKAGE`](../../constants.md#ELEMENT_TYPE_PACKAGE), [`output_section`](../../output_manager.md#output_section), [`_toon_available`](structure_command.md#_toon_available)
- used by: [`BaseCommand`](base_command.md#BaseCommand), [`execute_async`](base_command.md#BaseCommand.execute_async), [`_create_file_command`](../../cli_main.md#_create_file_command)  (5 test-only)

## Module values
- `_toon_available` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/structure_command.py#L25)

