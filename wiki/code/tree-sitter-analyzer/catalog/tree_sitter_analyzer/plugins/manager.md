---
title: 'Module: tree_sitter_analyzer/plugins/manager.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/plugins/manager.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.plugins.manager`/
symbols:
  PluginManager: PluginManager#
  PluginManager.get_plugin: PluginManager#get_plugin().
  PluginManager.register_plugin: PluginManager#register_plugin().
  PluginManager.load_plugins: PluginManager#load_plugins().
  PluginManager._loaded_plugins: PluginManager#_loaded_plugins.
  PluginManager._load_from_local_directory: PluginManager#_load_from_local_directory().
  PluginManager._load_from_entry_points: PluginManager#_load_from_entry_points().
  PluginManager.get_supported_languages: PluginManager#get_supported_languages().
  PluginManager.get_all_plugins: PluginManager#get_all_plugins().
  PluginManager.validate_plugin: PluginManager#validate_plugin().
  PluginManager.reload_plugins: PluginManager#reload_plugins().
  PluginManager.get_plugin_info: PluginManager#get_plugin_info().
  PluginManager._entry_point_map: PluginManager#_entry_point_map.
  PluginManager._discover_from_local_directory: PluginManager#_discover_from_local_directory().
  PluginManager._plugin_modules: PluginManager#_plugin_modules.
  PluginManager._discovered: PluginManager#_discovered.
  PluginManager.unregister_plugin: PluginManager#unregister_plugin().
  PluginManager._find_plugin_classes: PluginManager#_find_plugin_classes().
  PluginManager._get_default_aliases: PluginManager#_get_default_aliases().
  PluginManager._discover_from_entry_points: PluginManager#_discover_from_entry_points().
  _should_load_entry_points: _should_load_entry_points().
  _prewarm_local_language_modules_for_tests: _prewarm_local_language_modules_for_tests().
  _is_source_checkout: _is_source_checkout().
  _is_running_under_pytest: _is_running_under_pytest().
  _prewarm_local_language_modules_for_tests._safe_import: _prewarm_local_language_modules_for_tests()._safe_import().
  PluginManager._entry_point_group: PluginManager#_entry_point_group.
  logger: logger.
  PluginManager.__init__: PluginManager#__init__().
---
# Module: [`tree_sitter_analyzer/plugins/manager.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py)

## Classes
### `PluginManager`
- def: [`tree_sitter_analyzer/plugins/manager.py:98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L98) — documented in [tree_sitter_analyzer-mcp-tools-base_tool](../../../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)
- doc: Manages dynamic discovery and loading of language plugins.
- signature: `class PluginManager:`
- members:
  - `__init__(self)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L109) — Initialize the plugin manager.
  - `_discover_from_entry_points(self)` — [`L136`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L136) — Discover plugins from setuptools entry points without loading classes.
  - `_discover_from_local_directory(self)` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L144) — Discover plugins from the local languages directory without importing.
  - `_find_plugin_classes(self, module: Any)` — [`L220`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L220) — Find LanguagePlugin classes in a module.
  - `_get_default_aliases(self)` — [`L249`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L249) — Get default language aliases.
  - `_load_from_entry_points(self)` — [`L190`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L190) — Load plugins from setuptools entry points.
  - `_load_from_local_directory(self)` — [`L205`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L205) — Load plugins from the local languages directory.
  - `get_all_plugins(self)` — [`L232`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L232) — Get all plugins, loading them if not already done.
  - `get_plugin(self, language: str)` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L155) — Get a plugin for a specific language, loading it if necessary. — documented in [tree_sitter_analyzer-plugins-base](../../../concepts/tree_sitter_analyzer-plugins-base.md)
  - `get_plugin_info(self, language: str)` — [`L333`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L333) — Get information about a specific plugin.
  - `get_supported_languages(self)` — [`L258`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L258) — Get list of all supported languages (discovered or loaded).
  - `load_plugins(self)` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L116) — Discover available plugins without fully loading them for performance. — documented in [tree_sitter_analyzer-plugins-manager](../../../concepts/tree_sitter_analyzer-plugins-manager.md)
  - `register_plugin(self, plugin: LanguagePlugin)` — [`L293`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L293) — Manually register a plugin instance. — documented in [tree_sitter_analyzer-plugins-manager](../../../concepts/tree_sitter_analyzer-plugins-manager.md)
  - `reload_plugins(self)` — [`L276`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L276) — Reload all plugins (useful for development).
  - `unregister_plugin(self, language: str)` — [`L316`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L316) — Unregister a plugin for a specific language.
  - `validate_plugin(self, plugin: LanguagePlugin)` — [`L349`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L349) — Validate that a plugin implements the required interface correctly.
- protocol/private: `_discovered`[`L114`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L114), `_entry_point_group`[`L113`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L113), `_entry_point_map`[`L138`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L138), `_loaded_plugins`[`L111`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L111), `_plugin_modules`[`L112`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L112)
- uses (calls/refs, reference-scoped): [`log_debug`](../utils/logging.md#log_debug), [`log_error`](../utils/logging.md#log_error), [`LanguagePlugin`](base.md#LanguagePlugin), [`log_warning`](../utils/logging.md#log_warning), [`get_language_name`](base.md#LanguagePlugin.get_language_name), [`log_info`](../utils/logging.md#log_info), [`load_plugins_from_entry_points`](_manager_helpers.md#load_plugins_from_entry_points), [`load_plugins_from_local_directory`](_manager_helpers.md#load_plugins_from_local_directory), [`lazy_load_local_plugin`](_manager_helpers.md#lazy_load_local_plugin), [`validate_plugin_instance`](_manager_helpers.md#validate_plugin_instance), [`build_plugin_info`](_manager_helpers.md#build_plugin_info), [`lazy_load_entry_point_plugin`](_manager_helpers.md#lazy_load_entry_point_plugin), [`discover_entry_points`](_manager_helpers.md#discover_entry_points), [`debug`](_manager_helpers.md#PluginLoggers.debug), [`error`](_manager_helpers.md#PluginLoggers.error), [`discover_local_plugin_modules`](_manager_helpers.md#discover_local_plugin_modules), [`PluginLoggers`](_manager_helpers.md#PluginLoggers), [`warning`](_manager_helpers.md#PluginLoggers.warning), [`_should_load_entry_points`](manager.md#_should_load_entry_points), [`default_aliases`](_manager_helpers.md#default_aliases), [`find_loaded_plugin_case_insensitive`](_manager_helpers.md#find_loaded_plugin_case_insensitive), [`find_plugin_classes`](_manager_helpers.md#find_plugin_classes), [`plugin_module_for_language`](_manager_helpers.md#plugin_module_for_language)
- used by: [`_get_covered_node_types_from_plugin`](../grammar_coverage/validator.md#_get_covered_node_types_from_plugin), [`_ensure_initialized`](../core/analysis_engine.md#UnifiedAnalysisEngine._ensure_initialized), [`_extract_functions_via_plugin`](../complexity_heatmap.md#_extract_functions_via_plugin), [`is_language_supported`](../language_detector.md#is_language_supported), [`_execute_plugin_query`](../core/query_service.md#QueryService._execute_plugin_query), [`is_supported`](../language_detector.md#LanguageDetector.is_supported), [`plugin_manager`](../core/query_service.md#QueryService.plugin_manager), [`_extractor_complexity_by_line`](../complexity_heatmap.md#_extractor_complexity_by_line), [`_annotate_canonical_complexity`](../_ast_extraction.md#_annotate_canonical_complexity), [`_ensure_plugin_manager`](../core/analysis_engine.md#_ensure_plugin_manager)  (103 test-only)

## Functions
- `_is_running_under_pytest()` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L56) — Best-effort detection for pytest to allow test-only pre-warming.
- `_is_source_checkout()` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L39) — Heuristic to detect running from a source checkout (tests/dev).
- `_prewarm_local_language_modules_for_tests()` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L61) — Import local language plugin modules during test collection.
- `_safe_import(module_name: str)` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L69) — Best-effort import helper (never raises).
- `_should_load_entry_points()` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L48) — Decide whether to scan setuptools entry points for plugins.

## Module values
- `logger` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/manager.py#L36)

