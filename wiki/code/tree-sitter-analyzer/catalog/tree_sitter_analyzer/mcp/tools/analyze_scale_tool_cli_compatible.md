---
title: 'Module: tree_sitter_analyzer/mcp/tools/analyze_scale_tool_cli_compatible.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/analyze_scale_tool_cli_compatible.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.analyze_scale_tool_cli_compatible`/
symbols:
  AnalyzeScaleToolCLICompatible: AnalyzeScaleToolCLICompatible#
  AnalyzeScaleToolCLICompatible.execute: AnalyzeScaleToolCLICompatible#execute().
  AnalyzeScaleToolCLICompatible._run_analysis_and_build_result: AnalyzeScaleToolCLICompatible#_run_analysis_and_build_result().
  AnalyzeScaleToolCLICompatible.analysis_engine: AnalyzeScaleToolCLICompatible#analysis_engine.
  AnalyzeScaleToolCLICompatible.validate_arguments: AnalyzeScaleToolCLICompatible#validate_arguments().
  AnalyzeScaleToolCLICompatible.get_tool_schema: AnalyzeScaleToolCLICompatible#get_tool_schema().
  logger: logger.
  analyze_scale_tool_cli_compatible: analyze_scale_tool_cli_compatible.
  AnalyzeScaleToolCLICompatible.get_tool_definition: AnalyzeScaleToolCLICompatible#get_tool_definition().
  _build_cli_compatible_result: _build_cli_compatible_result().
  _cli_compatible_error_result: _cli_compatible_error_result().
  AnalyzeScaleToolCLICompatible.__init__: AnalyzeScaleToolCLICompatible#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/analyze_scale_tool_cli_compatible.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool_cli_compatible.py)

## Classes
### `AnalyzeScaleToolCLICompatible`
- def: [`tree_sitter_analyzer/mcp/tools/analyze_scale_tool_cli_compatible.py:74`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool_cli_compatible.py#L74)
- doc: MCP Tool for analyzing code scale with CLI-compatible output format.
- signature: `class AnalyzeScaleToolCLICompatible:`
- members:
  - `__init__(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool_cli_compatible.py#L81) — Initialize the CLI-compatible analyze scale tool.
  - `_run_analysis_and_build_result(self, file_path: str, language: str)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool_cli_compatible.py#L146) — Call the analysis engine and produce the CLI-compatible envelope.
  - `execute(self, arguments: dict[str, Any])` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool_cli_compatible.py#L119) — Execute the analyze_code_scale tool with CLI-compatible output.
  - `get_tool_definition(self)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool_cli_compatible.py#L222) — Get the MCP tool definition for analyze_code_scale.
  - `get_tool_schema(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool_cli_compatible.py#L86) — Get the MCP tool schema for analyze_code_scale.
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool_cli_compatible.py#L174) — Validate tool arguments against the schema.
  - `analysis_engine` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool_cli_compatible.py#L83)
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../core/request.md#AnalysisRequest), [`file_path`](../../core/request.md#AnalysisRequest.file_path), [`detect_language_from_file`](../../language_detector.md#detect_language_from_file), [`language`](../../core/request.md#AnalysisRequest.language), [`get_analysis_engine`](../../core/analysis_engine.md#get_analysis_engine), [`analyze`](../../core/_analysis_engine_analysis_mixin.md#UnifiedAnalysisEngineAnalysisMixin.analyze), [`include_complexity`](../../core/request.md#AnalysisRequest.include_complexity), [`include_details`](../../core/request.md#AnalysisRequest.include_details), [`logger`](analyze_scale_tool_cli_compatible.md#logger), [`_build_cli_compatible_result`](analyze_scale_tool_cli_compatible.md#_build_cli_compatible_result), [`_cli_compatible_error_result`](analyze_scale_tool_cli_compatible.md#_cli_compatible_error_result)
- used by: [`analyze_scale_tool_cli_compatible`](analyze_scale_tool_cli_compatible.md#analyze_scale_tool_cli_compatible)  (36 test-only)

## Functions
- `_build_cli_compatible_result(file_path: str, analysis_result: Any, start_time: float)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool_cli_compatible.py#L21) — CLI-compatible element_counts + metadata (matches --advanced --statistics).
- `_cli_compatible_error_result(file_path: str, error_message: str)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool_cli_compatible.py#L56) — Zero-count CLI-compatible envelope returned on analysis failure.

## Module values
- `analyze_scale_tool_cli_compatible` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool_cli_compatible.py#L247)
- `logger` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/analyze_scale_tool_cli_compatible.py#L18)

