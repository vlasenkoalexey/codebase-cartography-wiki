---
title: 'Module: tree_sitter_analyzer/core/analysis_engine.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/core/analysis_engine.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.core.analysis_engine`/
symbols:
  UnifiedAnalysisEngine: UnifiedAnalysisEngine#
  get_analysis_engine: get_analysis_engine().
  UnifiedAnalysisEngine._ensure_initialized: UnifiedAnalysisEngine#_ensure_initialized().
  MockLanguagePlugin.analyze_file: MockLanguagePlugin#analyze_file().
  UnifiedAnalysisEngine._load_plugins: UnifiedAnalysisEngine#_load_plugins().
  UnifiedAnalysisEngine._project_root: UnifiedAnalysisEngine#_project_root.
  UnifiedAnalysisEngine._instances: UnifiedAnalysisEngine#_instances.
  UnifiedAnalysisEngine.__new__: UnifiedAnalysisEngine#__new__().
  UnifiedAnalysisEngine._get_or_create: UnifiedAnalysisEngine#_get_or_create().
  UnifiedAnalysisEngine.clear_cache: UnifiedAnalysisEngine#clear_cache().
  MockLanguagePlugin: MockLanguagePlugin#
  UnifiedAnalysisEngine.register_plugin: UnifiedAnalysisEngine#register_plugin().
  UnifiedAnalysisEngine._cache_service: UnifiedAnalysisEngine#_cache_service.
  UnifiedAnalysisEngine._plugin_manager: UnifiedAnalysisEngine#_plugin_manager.
  UnifiedAnalysisEngine._parser: UnifiedAnalysisEngine#_parser.
  MockLanguagePlugin.language: MockLanguagePlugin#language.
  _ensure_plugin_manager: _ensure_plugin_manager().
  _run_plugin_discovery: _run_plugin_discovery().
  MockLanguagePlugin.get_language_name: MockLanguagePlugin#get_language_name().
  MockLanguagePlugin.get_file_extensions: MockLanguagePlugin#get_file_extensions().
  LanguagePlugin.analyze_file: LanguagePlugin#analyze_file().
  UnifiedAnalysisEngine._language_detector: UnifiedAnalysisEngine#_language_detector.
  UnifiedAnalysisEngine._performance_monitor: UnifiedAnalysisEngine#_performance_monitor.
  UnifiedAnalysisEngine._lock: UnifiedAnalysisEngine#_lock.
  UnifiedAnalysisEngine._initialized: UnifiedAnalysisEngine#_initialized.
  UnifiedAnalysisEngine._security_validator: UnifiedAnalysisEngine#_security_validator.
  UnifiedAnalysisEngine._query_executor: UnifiedAnalysisEngine#_query_executor.
  MockLanguagePlugin.create_extractor: MockLanguagePlugin#create_extractor().
  __all__: __all__.
  LanguagePlugin: LanguagePlugin#
  UnifiedAnalysisEngine.__init__: UnifiedAnalysisEngine#__init__().
  MockLanguagePlugin.__init__: MockLanguagePlugin#__init__().
---
# Module: [`tree_sitter_analyzer/core/analysis_engine.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py)

## Classes
### `LanguagePlugin`  ·  implements/extends Protocol
- def: [`tree_sitter_analyzer/core/analysis_engine.py:47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L47)
- doc: Language plugin protocol
- signature: `class LanguagePlugin(Protocol):`
- members:
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L50) — File analysis
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](request.md#AnalysisRequest)

### `MockLanguagePlugin`
- def: [`tree_sitter_analyzer/core/analysis_engine.py:157`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L157)
- doc: Mock plugin for testing
- signature: `class MockLanguagePlugin:`
- members:
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L174) — documented in [tree_sitter_analyzer-core-request](../../../concepts/tree_sitter_analyzer-core-request.md)
  - `create_extractor()` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L170)
  - `get_file_extensions(self)` — [`L166`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L166)
  - `get_language_name(self)` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L163)
  - `language` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L161)
- protocol/private: `__init__`[`L160`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L160)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../models/result.md#AnalysisResult), [`AnalysisRequest`](request.md#AnalysisRequest), [`elements`](../models/result.md#AnalysisResult.elements), [`language`](../models/result.md#AnalysisResult.language), [`file_path`](../models/result.md#AnalysisResult.file_path), [`success`](../models/result.md#AnalysisResult.success), [`line_count`](../models/result.md#AnalysisResult.line_count), [`error_message`](../models/result.md#AnalysisResult.error_message), [`source_code`](../models/result.md#AnalysisResult.source_code), [`node_count`](../models/result.md#AnalysisResult.node_count), [`query_results`](../models/result.md#AnalysisResult.query_results), [`package`](../models/result.md#AnalysisResult.package), [`analysis_time`](../models/result.md#AnalysisResult.analysis_time)
- used by: (6 test-only callers)

### `UnifiedAnalysisEngine`  ·  implements/extends UnifiedAnalysisEngineAnalysisMixin, UnifiedAnalysisEngineCodeMixin, UnifiedAnalysisEngineFileMixin, UnifiedAnalysisEngineRuntimeMixin
- def: [`tree_sitter_analyzer/core/analysis_engine.py:55`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L55) — documented in [tree_sitter_analyzer-mcp-server](../../../concepts/tree_sitter_analyzer-mcp-server.md)
- doc: Unified analysis engine
- signature: `class UnifiedAnalysisEngine(UnifiedAnalysisEngineAnalysisMixin, UnifiedAnalysisEngineFileMixin, UnifiedAnalysisEngineCodeMixin, UnifiedAnalysisEngineRuntimeMixin):`
- members:
  - `__init__(self, project_root: str | None = None)` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L92) — Initialize the engine
  - `__new__(cls, project_root: str | None = None)` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L82) — Singleton instance management (backward compatible)
  - `_ensure_initialized(self)` — [`L111`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L111) — Ensure all components are lazily initialized only when needed
  - `_get_or_create(cls, instance_key: str)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L71) — Singleton factory: get or create an instance for the given key.
  - `_load_plugins(self)` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L147) — Discover available plugins (fast metadata scan)
  - `clear_cache(self)` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L139) — Clear the analysis cache (compatibility method)
  - `register_plugin(self, language: str, plugin: Any)` — [`L133`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L133) — Register a plugin (compatibility method)
- protocol/private: `_cache_service`[`L98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L98), `_initialized`[`L109`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L109), `_instances`[`L67`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L67), `_language_detector`[`L101`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L101), `_lock`[`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L68), `_parser`[`L103`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L103), `_performance_monitor`[`L100`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L100), `_plugin_manager`[`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L99), `_project_root`[`L105`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L105), `_query_executor`[`L104`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L104), `_security_validator`[`L102`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L102)
- uses (calls/refs, reference-scoped): [`log_debug`](../utils/logging.md#log_debug), [`SecurityValidator`](../security/validator.md#SecurityValidator), [`Parser`](parser.md#Parser), [`PluginManager`](../plugins/manager.md#PluginManager), [`QueryExecutor`](query.md#QueryExecutor), [`CacheService`](cache_service.md#CacheService), [`PerformanceMonitor`](performance.md#PerformanceMonitor), [`LanguageDetector`](../language_detector.md#LanguageDetector), [`UnifiedAnalysisEngineAnalysisMixin`](_analysis_engine_analysis_mixin.md#UnifiedAnalysisEngineAnalysisMixin), [`UnifiedAnalysisEngineCodeMixin`](_analysis_engine_code_mixin.md#UnifiedAnalysisEngineCodeMixin), [`UnifiedAnalysisEngineFileMixin`](_analysis_engine_file_mixin.md#UnifiedAnalysisEngineFileMixin), [`UnifiedAnalysisEngineRuntimeMixin`](_analysis_engine_runtime_mixin.md#UnifiedAnalysisEngineRuntimeMixin), [`_ensure_plugin_manager`](analysis_engine.md#_ensure_plugin_manager), [`_run_plugin_discovery`](analysis_engine.md#_run_plugin_discovery)
- used by: [`get_analysis_engine`](analysis_engine.md#get_analysis_engine), [`get_instance`](engine_manager.md#EngineManager.get_instance), [`analyze_file`](../plugins/base.md#DefaultLanguagePlugin.analyze_file), [`get_engine`](../api.md#get_engine), [`profile_analysis`](../../profile_analysis.md#profile_analysis), [`_clear_analysis_engine_cache`](../../compatibility_test/utils/cache_manager.md#CacheManager._clear_analysis_engine_cache), [`_instances`](engine_manager.md#EngineManager._instances), [`_engine`](../api.md#_engine._engine), [`_analyze`](../../scripts/benchmark_real_projects.md#run_analysis._analyze), [`UnifiedAnalysisEngineAnalysisMixin`](_analysis_engine_analysis_mixin.md#UnifiedAnalysisEngineAnalysisMixin), [`UnifiedAnalysisEngineCodeMixin`](_analysis_engine_code_mixin.md#UnifiedAnalysisEngineCodeMixin), [`UnifiedAnalysisEngineFileMixin`](_analysis_engine_file_mixin.md#UnifiedAnalysisEngineFileMixin), [`UnifiedAnalysisEngineRuntimeMixin`](_analysis_engine_runtime_mixin.md#UnifiedAnalysisEngineRuntimeMixin)  (108 test-only)

## Functions
- `_ensure_plugin_manager(plugin_manager: Any)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L28) — Return existing manager or lazily construct a new PluginManager.
- `_run_plugin_discovery(plugin_manager: Any)` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L37) — Call load_plugins() and log any exception via %s (avoids f-string depth).
- `get_analysis_engine(project_root: str | None = None)` — [`L190`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L190) — Get unified analysis engine instance — documented in [tree_sitter_analyzer-mcp-server](../../../concepts/tree_sitter_analyzer-mcp-server.md)

## Module values
- `__all__` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_engine.py#L20)

