---
title: 'Module: tree_sitter_analyzer/core/_analysis_engine_file_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/core/_analysis_engine_file_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.core._analysis_engine_file_mixin`/UnifiedAnalysisEngineFileMixin#
symbols:
  UnifiedAnalysisEngineFileMixin.analyze_file: analyze_file().
  UnifiedAnalysisEngineFileMixin.analyze_file_async: analyze_file_async().
  UnifiedAnalysisEngineFileMixin: ''
---
# Module: [`tree_sitter_analyzer/core/_analysis_engine_file_mixin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_file_mixin.py)

## Classes
### `UnifiedAnalysisEngineFileMixin`
- def: [`tree_sitter_analyzer/core/_analysis_engine_file_mixin.py:9`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_file_mixin.py#L9)
- doc: Compatibility file-analysis methods.
- signature: `class UnifiedAnalysisEngineFileMixin:`
- members:
  - `analyze_file(self, file_path: str, language: str | None = None, request: AnalysisRequest | None = None, format_type: str | None = None, include_details: bool | None = None, include_complexity: bool | None = None, include_elements: bool | None = None, include_queries: bool | None = None, queries: list[str] | None = None)` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_file_mixin.py#L12) — Compatibility alias for analyze with additional parameters. — documented in [tree_sitter_analyzer-core-request](../../../concepts/tree_sitter_analyzer-core-request.md)
  - `analyze_file_async(self, file_path: str, language: str | None = None, request: AnalysisRequest | None = None)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_file_mixin.py#L49) — Compatibility alias for analyze
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](request.md#AnalysisRequest), [`UnifiedAnalysisEngine`](analysis_engine.md#UnifiedAnalysisEngine), [`build_request_from_params`](request_builder.md#build_request_from_params), [`update_request_from_params`](request_builder.md#update_request_from_params)
- used by: [`UnifiedAnalysisEngine`](analysis_engine.md#UnifiedAnalysisEngine), [`analyze_file`](../plugins/base.md#DefaultLanguagePlugin.analyze_file), [`_analyze`](../../scripts/benchmark_real_projects.md#run_analysis._analyze)  (36 test-only)

