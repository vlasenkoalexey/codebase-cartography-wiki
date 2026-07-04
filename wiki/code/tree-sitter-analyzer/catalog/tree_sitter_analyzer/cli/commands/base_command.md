---
title: 'Module: tree_sitter_analyzer/cli/commands/base_command.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/base_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.base_command`/BaseCommand#
symbols:
  BaseCommand.args: args.
  BaseCommand: ''
  BaseCommand.analyze_file: analyze_file().
  BaseCommand.execute_async: execute_async().
  BaseCommand.detect_language: detect_language().
  BaseCommand.validate_file: validate_file().
  BaseCommand.execute: execute().
  BaseCommand._emit_unsupported_language_envelope: _emit_unsupported_language_envelope().
  BaseCommand.security_validator: security_validator.
  BaseCommand._try_partial_read_precheck: _try_partial_read_precheck().
  BaseCommand.analysis_engine: analysis_engine.
  BaseCommand.project_root: project_root.
  BaseCommand.__init__: __init__().
---
# Module: [`tree_sitter_analyzer/cli/commands/base_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/base_command.py)

## Classes
### `BaseCommand`  ·  implements/extends ABC
- def: [`tree_sitter_analyzer/cli/commands/base_command.py:23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/base_command.py#L23)
- doc: Base class for all CLI commands.
- signature: `class BaseCommand(ABC):`
- members:
  - `__init__(self, args: Namespace)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/base_command.py#L31) — Initialize command with parsed arguments.
  - `_emit_unsupported_language_envelope(self, detected_language: str)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/base_command.py#L103) — Emit a canonical error envelope for an unsupported language.
  - `_try_partial_read_precheck(self)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/base_command.py#L201) — Run the partial-read precheck when ``--partial-read`` was passed.
  - `analyze_file(self, language: str)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/base_command.py#L166) — Perform file analysis using the unified analysis engine. — documented in [tree_sitter_analyzer-models-result](../../../../concepts/tree_sitter_analyzer-models-result.md)
  - `detect_language(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/base_command.py#L68) — Detect or validate the target language. — documented in [tree_sitter_analyzer-security-validator](../../../../concepts/tree_sitter_analyzer-security-validator.md)
  - `execute(self)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/base_command.py#L233) — Execute the command.
  - `execute_async(self, language: str)` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/base_command.py#L257) — Execute the command asynchronously.
  - `validate_file(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/base_command.py#L44) — Validate input file exists and is accessible.
  - `analysis_engine` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/base_command.py#L41)
  - `args` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/base_command.py#L33)
  - `project_root` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/base_command.py#L38)
  - `security_validator` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/base_command.py#L42)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../models/result.md#AnalysisResult), [`AnalysisRequest`](../../core/request.md#AnalysisRequest), [`file_path`](../../core/request.md#AnalysisRequest.file_path), [`SecurityValidator`](../../security/validator.md#SecurityValidator), [`ToonFormatter`](../../formatters/toon_formatter.md#ToonFormatter), [`detect_language_from_file`](../../language_detector.md#detect_language_from_file), [`validate_file_path`](../../security/validator.md#SecurityValidator.validate_file_path), [`language`](../../core/request.md#AnalysisRequest.language), [`get_analysis_engine`](../../core/analysis_engine.md#get_analysis_engine), [`read_file_partial`](../../file_handler.md#read_file_partial), [`output_error`](../../output_manager.md#output_error), [`analyze`](../../core/_analysis_engine_analysis_mixin.md#UnifiedAnalysisEngineAnalysisMixin.analyze), [`include_complexity`](../../core/request.md#AnalysisRequest.include_complexity), [`include_details`](../../core/request.md#AnalysisRequest.include_details), [`format`](../../formatters/toon_formatter.md#ToonFormatter.format), [`output_info`](../../output_manager.md#output_info), [`detect_project_root`](../../project_detector.md#detect_project_root), [`execute`](partial_read_command.md#PartialReadCommand.execute), [`PartialReadCommand`](partial_read_command.md#PartialReadCommand), [`sanitize_input`](../../security/validator.md#SecurityValidator.sanitize_input), [`is_language_supported`](../../language_detector.md#is_language_supported), [`QueryCommand`](query_command.md#QueryCommand), [`SummaryCommand`](summary_command.md#SummaryCommand), [`TableCommand`](table_command.md#TableCommand), [`execute_async`](query_command.md#QueryCommand.execute_async), [`execute_async`](table_command.md#TableCommand.execute_async), [`StructureCommand`](structure_command.md#StructureCommand), [`AdvancedCommand`](advanced_command.md#AdvancedCommand), [`execute_async`](advanced_command.md#AdvancedCommand.execute_async), [`DefaultCommand`](default_command.md#DefaultCommand), [`execute_async`](summary_command.md#SummaryCommand.execute_async), [`validate_file`](partial_read_command.md#PartialReadCommand.validate_file), [`execute_async`](default_command.md#DefaultCommand.execute_async), [`execute_async`](structure_command.md#StructureCommand.execute_async), [`execute_async`](partial_read_command.md#PartialReadCommand.execute_async)  (6 test-only)
- used by: [`_output_statistics`](advanced_command.md#AdvancedCommand._output_statistics), [`_output_full_analysis`](advanced_command.md#AdvancedCommand._output_full_analysis), [`PartialReadCommand`](partial_read_command.md#PartialReadCommand), [`QueryCommand`](query_command.md#QueryCommand), [`_output_summary_analysis`](summary_command.md#SummaryCommand._output_summary_analysis), [`_output_structure_analysis`](structure_command.md#StructureCommand._output_structure_analysis), [`_resolve_query`](query_command.md#QueryCommand._resolve_query), [`execute_query`](query_command.md#QueryCommand.execute_query), [`SummaryCommand`](summary_command.md#SummaryCommand), [`TableCommand`](table_command.md#TableCommand), [`_emit_query_results`](query_command.md#QueryCommand._emit_query_results), [`_emit_summary`](summary_command.md#SummaryCommand._emit_summary), [`_render_table_output`](table_command.md#TableCommand._render_table_output), [`execute_async`](table_command.md#TableCommand.execute_async), [`StructureCommand`](structure_command.md#StructureCommand), [`AdvancedCommand`](advanced_command.md#AdvancedCommand), [`_format_as_toon`](table_command.md#TableCommand._format_as_toon), [`execute_async`](advanced_command.md#AdvancedCommand.execute_async), [`DefaultCommand`](default_command.md#DefaultCommand), [`_convert_function_element`](table_command.md#TableCommand._convert_function_element), [`execute_async`](summary_command.md#SummaryCommand.execute_async), [`_convert_variable_element`](table_command.md#TableCommand._convert_variable_element), [`execute_async`](structure_command.md#StructureCommand.execute_async), [`_build_query_envelope`](query_command.md#QueryCommand._build_query_envelope), [`_requested_summary_types`](summary_command.md#SummaryCommand._requested_summary_types), [`_resolve_table_type`](table_command.md#TableCommand._resolve_table_type), [`__init__`](query_command.md#QueryCommand.__init__), [`__init__`](table_command.md#TableCommand.__init__)  (30 test-only)

