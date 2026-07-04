---
title: 'Module: tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.core._analysis_engine_runtime_mixin`/UnifiedAnalysisEngineRuntimeMixin#
symbols:
  UnifiedAnalysisEngineRuntimeMixin._reset_instance: _reset_instance().
  UnifiedAnalysisEngineRuntimeMixin.analyze_sync: analyze_sync().
  UnifiedAnalysisEngineRuntimeMixin.language_detector: language_detector().
  UnifiedAnalysisEngineRuntimeMixin.parser: parser().
  UnifiedAnalysisEngineRuntimeMixin.cleanup: cleanup().
  UnifiedAnalysisEngineRuntimeMixin.get_supported_languages: get_supported_languages().
  UnifiedAnalysisEngineRuntimeMixin: ''
  UnifiedAnalysisEngineRuntimeMixin.plugin_manager: plugin_manager().
  UnifiedAnalysisEngineRuntimeMixin.measure_operation: measure_operation().
  UnifiedAnalysisEngineRuntimeMixin.get_available_queries: get_available_queries().
  UnifiedAnalysisEngineRuntimeMixin.get_cache_stats: get_cache_stats().
  UnifiedAnalysisEngineRuntimeMixin.query_executor: query_executor().
  UnifiedAnalysisEngineRuntimeMixin.security_validator: security_validator().
  UnifiedAnalysisEngineRuntimeMixin.cache_service: cache_service().
---
# Module: [`tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.py)

## Classes
### `UnifiedAnalysisEngineRuntimeMixin`
- def: [`tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.py:11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.py#L11)
- doc: Sync wrappers, resource cleanup, and compatibility accessors.
- signature: `class UnifiedAnalysisEngineRuntimeMixin:`
- members:
  - `_reset_instance(cls)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.py#L94) — Compatibility method for resetting instances
  - `analyze_sync(self, request: AnalysisRequest)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.py#L24) — Sync version of analyze
  - `cache_service(self)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.py#L65) — Expose cache service
  - `cleanup(self)` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.py#L14) — Resource cleanup
  - `get_available_queries(self, language: str)` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.py#L42) — Get available queries for a language
  - `get_cache_stats(self)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.py#L47) — Get cache statistics (compatibility method)
  - `get_supported_languages(self)` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.py#L37) — Get list of supported languages
  - `language_detector(self)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.py#L53) — Expose language detector
  - `measure_operation(self, operation_name: str)` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.py#L88) — Measure an operation using the performance monitor
  - `parser(self)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.py#L71) — Expose parser
  - `plugin_manager(self)` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.py#L59) — Expose plugin manager
  - `query_executor(self)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.py#L77) — Expose query executor
  - `security_validator(self)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.py#L83) — Expose security validator
- uses (calls/refs, reference-scoped): [`log_debug`](../utils/logging.md#log_debug), [`AnalysisRequest`](request.md#AnalysisRequest), [`UnifiedAnalysisEngine`](analysis_engine.md#UnifiedAnalysisEngine), [`EngineManager`](engine_manager.md#EngineManager), [`reset_instances`](engine_manager.md#EngineManager.reset_instances), [`PerformanceContext`](performance.md#PerformanceContext)
- used by: [`UnifiedAnalysisEngine`](analysis_engine.md#UnifiedAnalysisEngine), [`extract_elements`](../mcp/tools/utils/element_extractor.md#extract_elements), [`_analyze_file_sync`](../api.md#_analyze_file_sync), [`profile_analysis`](../../profile_analysis.md#profile_analysis), [`get_cache_stats`](../../compatibility_test/utils/cache_manager.md#CacheManager.get_cache_stats), [`detect_language`](../api.md#detect_language), [`get_framework_info`](../api.md#get_framework_info), [`get_file_extensions`](../api.md#get_file_extensions), [`get_supported_languages`](../api.md#get_supported_languages), [`get_available_queries`](../api.md#get_available_queries)  (37 test-only)

