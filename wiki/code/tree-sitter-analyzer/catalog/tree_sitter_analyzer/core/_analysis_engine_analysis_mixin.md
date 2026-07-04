---
title: 'Module: tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.core._analysis_engine_analysis_mixin`/
symbols:
  UnifiedAnalysisEngineAnalysisMixin.analyze: UnifiedAnalysisEngineAnalysisMixin#analyze().
  UnifiedAnalysisEngineAnalysisMixin._create_empty_result: UnifiedAnalysisEngineAnalysisMixin#_create_empty_result().
  UnifiedAnalysisEngineAnalysisMixin._generate_cache_key: UnifiedAnalysisEngineAnalysisMixin#_generate_cache_key().
  UnifiedAnalysisEngineAnalysisMixin._validate_and_detect_language: UnifiedAnalysisEngineAnalysisMixin#_validate_and_detect_language().
  UnifiedAnalysisEngineAnalysisMixin._run_queries: UnifiedAnalysisEngineAnalysisMixin#_run_queries().
  UnifiedAnalysisEngineAnalysisMixin._execute_requested_queries: UnifiedAnalysisEngineAnalysisMixin#_execute_requested_queries().
  UnifiedAnalysisEngineAnalysisMixin._run_plugin_analysis: UnifiedAnalysisEngineAnalysisMixin#_run_plugin_analysis().
  UnifiedAnalysisEngineAnalysisMixin._detect_language: UnifiedAnalysisEngineAnalysisMixin#_detect_language().
  UnifiedAnalysisEngineAnalysisMixin: UnifiedAnalysisEngineAnalysisMixin#
  UnifiedAnalysisEngineAnalysisMixin._validate_file_path: UnifiedAnalysisEngineAnalysisMixin#_validate_file_path().
  UnifiedAnalysisEngineAnalysisMixin._get_plugin: UnifiedAnalysisEngineAnalysisMixin#_get_plugin().
  UnifiedAnalysisEngineAnalysisMixin._ensure_file_exists: UnifiedAnalysisEngineAnalysisMixin#_ensure_file_exists().
  _query_captures_or_result: _query_captures_or_result().
---
# Module: [`tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.py)

## Classes
### `UnifiedAnalysisEngineAnalysisMixin`
- def: [`tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.py:12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.py#L12)
- doc: Core analyze workflow and internal analysis helpers.
- signature: `class UnifiedAnalysisEngineAnalysisMixin:`
- members:
  - `_create_empty_result(file_path: str, language: str, error: str | None = None)` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.py#L149) — Create empty result on failure
  - `_detect_language(self, file_path: str)` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.py#L140) — Detect language
  - `_generate_cache_key(self, request: AnalysisRequest)` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.py#L124) — Generate cache key
  - `_run_queries(self, request: AnalysisRequest, result: AnalysisResult, plugin: Any, language: Any)` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.py#L80) — Helper to run queries
  - `analyze(self, request: AnalysisRequest)` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.py#L15) — Unified analysis method (Async) — documented in [tree_sitter_analyzer-core-request](../../../concepts/tree_sitter_analyzer-core-request.md)
- protocol/private: `_ensure_file_exists`[`L61`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.py#L61), `_execute_requested_queries`[`L105`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.py#L105), `_get_plugin`[`L65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.py#L65), `_run_plugin_analysis`[`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.py#L71), `_validate_and_detect_language`[`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.py#L45), `_validate_file_path`[`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.py#L52)
- uses (calls/refs, reference-scoped): [`log_debug`](../utils/logging.md#log_debug), [`AnalysisResult`](../models/result.md#AnalysisResult), [`log_error`](../utils/logging.md#log_error), [`AnalysisRequest`](request.md#AnalysisRequest), [`elements`](../models/result.md#AnalysisResult.elements), [`language`](../models/result.md#AnalysisResult.language), [`UnifiedAnalysisEngine`](analysis_engine.md#UnifiedAnalysisEngine), [`file_path`](../models/result.md#AnalysisResult.file_path), [`success`](../models/result.md#AnalysisResult.success), [`file_path`](request.md#AnalysisRequest.file_path), [`error_message`](../models/result.md#AnalysisResult.error_message), [`language`](request.md#AnalysisRequest.language), [`log_info`](../utils/logging.md#log_info), [`include_complexity`](request.md#AnalysisRequest.include_complexity), [`format_type`](request.md#AnalysisRequest.format_type), [`query_results`](../models/result.md#AnalysisResult.query_results), [`include_queries`](request.md#AnalysisRequest.include_queries), [`queries`](request.md#AnalysisRequest.queries), [`UnsupportedLanguageError`](_analysis_engine_errors.md#UnsupportedLanguageError), [`analysis_time`](../models/result.md#AnalysisResult.analysis_time), [`_query_captures_or_result`](_analysis_engine_analysis_mixin.md#_query_captures_or_result)
- used by: [`UnifiedAnalysisEngine`](analysis_engine.md#UnifiedAnalysisEngine), [`analyze_file`](../cli/commands/base_command.md#BaseCommand.analyze_file), [`_run_analysis_and_build_result`](../mcp/tools/analyze_scale_tool_cli_compatible.md#AnalyzeScaleToolCLICompatible._run_analysis_and_build_result), [`_run_outline_analysis`](../mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool._run_outline_analysis), [`profile_analysis`](../../profile_analysis.md#profile_analysis)  (26 test-only)

## Functions
- `_query_captures_or_result(query_result: Any)` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.py#L163)

