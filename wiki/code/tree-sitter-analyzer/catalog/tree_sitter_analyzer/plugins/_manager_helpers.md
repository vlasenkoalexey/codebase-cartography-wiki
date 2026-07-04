---
title: 'Module: tree_sitter_analyzer/plugins/_manager_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/plugins/_manager_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.plugins._manager_helpers`/
symbols:
  LogFn: LogFn.
  load_plugins_from_entry_points: load_plugins_from_entry_points().
  load_plugins_from_local_directory: load_plugins_from_local_directory().
  lazy_load_local_plugin: lazy_load_local_plugin().
  validate_plugin_instance: validate_plugin_instance().
  load_plugin_from_entry_point: load_plugin_from_entry_point().
  local_language_module_names_for_loading: local_language_module_names_for_loading().
  lazy_load_entry_point_plugin: lazy_load_entry_point_plugin().
  build_plugin_info: build_plugin_info().
  load_plugins_from_module: load_plugins_from_module().
  discover_entry_points: discover_entry_points().
  PluginLoggers.debug: PluginLoggers#debug.
  PluginLoggers.error: PluginLoggers#error.
  discover_local_plugin_modules: discover_local_plugin_modules().
  PluginLoggers: PluginLoggers#
  plugin_matches_request: plugin_matches_request().
  has_required_plugin_methods: has_required_plugin_methods().
  has_valid_language_name: has_valid_language_name().
  has_valid_extensions: has_valid_extensions().
  PluginLoggers.warning: PluginLoggers#warning.
  ensure_languages_directory: ensure_languages_directory().
  import_languages_package: import_languages_package().
  SubClassCheck: SubClassCheck.
  ClassFinder: ClassFinder.
  default_aliases: default_aliases().
  plugin_module_for_language: plugin_module_for_language().
  find_loaded_plugin_case_insensitive: find_loaded_plugin_case_insensitive().
  find_plugin_classes: find_plugin_classes().
  PLUGIN_ALIASES: PLUGIN_ALIASES.
  entry_points_for_group: entry_points_for_group().
  iter_language_module_names: iter_language_module_names().
  REQUIRED_PLUGIN_METHODS: REQUIRED_PLUGIN_METHODS.
---
# Module: [`tree_sitter_analyzer/plugins/_manager_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py)

## Classes
### `PluginLoggers`
- def: [`tree_sitter_analyzer/plugins/_manager_helpers.py:20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L20)
- doc: Logger callbacks used by plugin manager helpers.
- signature: `class PluginLoggers:`
- members:
  - `debug` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L23) — ---
  - `error` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L25) — ---
  - `warning` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L24) — ---
- uses (calls/refs, reference-scoped): [`log_debug`](../utils/logging.md#log_debug), [`log_error`](../utils/logging.md#log_error), [`log_warning`](../utils/logging.md#log_warning), [`LogFn`](_manager_helpers.md#LogFn)
- used by: [`get_plugin`](manager.md#PluginManager.get_plugin), [`_load_from_local_directory`](manager.md#PluginManager._load_from_local_directory), [`load_plugins_from_local_directory`](_manager_helpers.md#load_plugins_from_local_directory), [`lazy_load_local_plugin`](_manager_helpers.md#lazy_load_local_plugin), [`lazy_load_entry_point_plugin`](_manager_helpers.md#lazy_load_entry_point_plugin)

## Functions
- `build_plugin_info(plugin: LanguagePlugin, *, language: str, error: LogFn = log_error)` — [`L374`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L374) — Build a serializable information dictionary for a plugin.
- `default_aliases()` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L43) — Return default language aliases.
- `discover_entry_points(entry_point_group: str, *, debug: LogFn = log_debug, warning: LogFn = log_warning)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L48) — Discover entry point plugins by name without loading them.
- `discover_local_plugin_modules(languages_dir: Path, languages_package: str, *, warning: LogFn = log_warning)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L85) — Discover local language plugin modules without importing each plugin.
- `ensure_languages_directory(languages_dir: Path, *, debug: LogFn = log_debug)` — [`L307`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L307) — Ensure the local languages directory exists before loading plugins.
- `entry_points_for_group(entry_point_group: str)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L68) — Return entry points for a group across importlib.metadata API versions.
- `find_loaded_plugin_case_insensitive(language: str, loaded_plugins: dict[str, LanguagePlugin])` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L195) — Find an already-loaded plugin by case-insensitive language name.
- `find_plugin_classes(module: Any)` — [`L358`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L358) — Find LanguagePlugin subclasses in a module.
- `has_required_plugin_methods(plugin: LanguagePlugin, *, error: LogFn)` — [`L420`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L420) — Return whether a plugin exposes all required callable methods.
- `has_valid_extensions(plugin: LanguagePlugin, *, error: LogFn)` — [`L444`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L444) — Validate file extensions returned by a plugin.
- `has_valid_language_name(plugin: LanguagePlugin, *, error: LogFn)` — [`L435`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L435) — Validate the language name returned by a plugin.
- `import_languages_package(languages_package: str, *, warning: LogFn = log_warning)` — [`L320`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L320) — Import the local languages package, returning None on ImportError.
- `iter_language_module_names(languages_module: Any)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L109) — Yield module names from the local languages package.
- `lazy_load_entry_point_plugin(language: str, entry_point_map: dict[str, Any] | None, loaded_plugins: dict[str, LanguagePlugin], subclass_check: SubClassCheck, loggers: PluginLoggers | None = None)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L167) — Load one plugin from a previously discovered entry point map.
- `lazy_load_local_plugin(language: str, module_name: str | None, loaded_plugins: dict[str, LanguagePlugin], class_finder: ClassFinder, loggers: PluginLoggers | None = None)` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L117) — Load a local plugin module and return the plugin matching *language*.
- `load_plugin_from_entry_point(entry_point: Any, subclass_check: SubClassCheck, *, debug: LogFn = log_debug, warning: LogFn = log_warning, error: LogFn = log_error)` — [`L233`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L233) — Load and validate a single entry point plugin.
- `load_plugins_from_entry_points(entry_point_group: str, subclass_check: SubClassCheck, *, debug: LogFn = log_debug, warning: LogFn = log_warning, error: LogFn = log_error)` — [`L205`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L205) — Load plugin instances from setuptools entry points.
- `load_plugins_from_local_directory(languages_dir: Path, languages_package: str, class_finder: ClassFinder, loggers: PluginLoggers | None = None)` — [`L256`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L256) — Load plugin instances from the local languages directory.
- `load_plugins_from_module(module_name: str, class_finder: ClassFinder, *, debug: LogFn = log_debug, error: LogFn = log_error)` — [`L333`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L333) — Import one language module and instantiate its plugin classes.
- `local_language_module_names_for_loading(languages_dir: Path, languages_package: str, *, debug: LogFn = log_debug, warning: LogFn = log_warning)` — [`L285`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L285) — Return local language module names that should be imported for loading.
- `plugin_matches_request(plugin: LanguagePlugin, requested_language: str)` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L159) — Return whether a plugin instance satisfies a requested language or alias.
- `plugin_module_for_language(plugin_modules: dict[str, str], language: str)` — [`L143`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L143) — Resolve a direct plugin module name or a default alias target.
- `validate_plugin_instance(plugin: LanguagePlugin, *, error: LogFn = log_error)` — [`L394`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L394) — Validate that a plugin implements the required interface correctly.

## Module values
- `ClassFinder` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L16)
- `LogFn` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L14)
- `PLUGIN_ALIASES` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L28)
- `REQUIRED_PLUGIN_METHODS` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L34)
- `SubClassCheck` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_manager_helpers.py#L15)

