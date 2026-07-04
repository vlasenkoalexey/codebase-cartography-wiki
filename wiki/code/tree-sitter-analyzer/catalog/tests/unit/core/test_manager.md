---
title: 'Module: tests/unit/core/test_manager.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_manager.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_manager`/
symbols:
  MockLanguagePlugin: MockLanguagePlugin#
  MockLanguagePlugin.analyze_file: MockLanguagePlugin#analyze_file().
  TestPluginManagerIntegration.test_full_plugin_lifecycle: TestPluginManagerIntegration#test_full_plugin_lifecycle().
  TestPluginManager.plugin_manager: TestPluginManager#plugin_manager().
  TestPluginManagerErrorHandling.plugin_manager: TestPluginManagerErrorHandling#plugin_manager().
  TestPluginManagerIntegration.plugin_manager: TestPluginManagerIntegration#plugin_manager().
  TestPluginManagerIntegration.test_plugin_discovery_and_loading: TestPluginManagerIntegration#test_plugin_discovery_and_loading().
  TestPluginManager.test_get_plugin_existing: TestPluginManager#test_get_plugin_existing().
  TestPluginManager.test_unregister_plugin_existing: TestPluginManager#test_unregister_plugin_existing().
  TestPluginManagerIntegration.test_plugin_reload_preserves_manual_registrations: TestPluginManagerIntegration#test_plugin_reload_preserves_manual_registrations().
  TestPluginManager.test_load_plugins_success: TestPluginManager#test_load_plugins_success().
  TestPluginManager.test_find_plugin_classes: TestPluginManager#test_find_plugin_classes().
  TestPluginManager.test_get_all_plugins: TestPluginManager#test_get_all_plugins().
  TestPluginManager.test_get_supported_languages: TestPluginManager#test_get_supported_languages().
  TestPluginManager.test_register_plugin_success: TestPluginManager#test_register_plugin_success().
  TestPluginManager.test_get_plugin_info_existing: TestPluginManager#test_get_plugin_info_existing().
  TestPluginManagerIntegration.test_plugin_validation_during_registration: TestPluginManagerIntegration#test_plugin_validation_during_registration().
  TestPluginManagerIntegration.test_plugin_manager_with_multiple_extensions: TestPluginManagerIntegration#test_plugin_manager_with_multiple_extensions().
  TestPluginManager.test_load_from_entry_points_success: TestPluginManager#test_load_from_entry_points_success().
  TestPluginManager.test_load_from_local_directory_success: TestPluginManager#test_load_from_local_directory_success().
  TestPluginManager.test_reload_plugins: TestPluginManager#test_reload_plugins().
  TestPluginManager.test_register_plugin_duplicate: TestPluginManager#test_register_plugin_duplicate().
  TestPluginManager.test_validate_plugin_valid: TestPluginManager#test_validate_plugin_valid().
  TestPluginManagerErrorHandling.test_get_plugin_info_with_exception: TestPluginManagerErrorHandling#test_get_plugin_info_with_exception().
  TestPluginManager.test_find_plugin_classes.TestPlugin: TestPluginManager#test_find_plugin_classes().TestPlugin#
  TestPluginManager.test_load_from_entry_points_with_exception: TestPluginManager#test_load_from_entry_points_with_exception().
  TestPluginManager.test_load_from_local_directory_with_exception: TestPluginManager#test_load_from_local_directory_with_exception().
  TestPluginManager.test_get_plugin_nonexistent: TestPluginManager#test_get_plugin_nonexistent().
  TestPluginManager.test_register_plugin_with_exception: TestPluginManager#test_register_plugin_with_exception().
  TestPluginManager.test_unregister_plugin_nonexistent: TestPluginManager#test_unregister_plugin_nonexistent().
  TestPluginManager.test_get_plugin_info_nonexistent: TestPluginManager#test_get_plugin_info_nonexistent().
  TestPluginManager.test_validate_plugin_invalid: TestPluginManager#test_validate_plugin_invalid().
  TestPluginManager.test_validate_plugin_missing_methods: TestPluginManager#test_validate_plugin_missing_methods().
  TestPluginManagerErrorHandling.test_load_plugins_with_import_error: TestPluginManagerErrorHandling#test_load_plugins_with_import_error().
  TestPluginManagerErrorHandling.test_load_plugins_with_corrupted_entry_point: TestPluginManagerErrorHandling#test_load_plugins_with_corrupted_entry_point().
  TestPluginManagerErrorHandling.test_register_plugin_none: TestPluginManagerErrorHandling#test_register_plugin_none().
  TestPluginManagerErrorHandling.test_validate_plugin_with_none: TestPluginManagerErrorHandling#test_validate_plugin_with_none().
  MockLanguagePlugin.get_language_name: MockLanguagePlugin#get_language_name().
  MockLanguagePlugin.get_file_extensions: MockLanguagePlugin#get_file_extensions().
  MockLanguagePlugin.is_applicable: MockLanguagePlugin#is_applicable().
  TestPluginManager.mock_java_plugin: TestPluginManager#mock_java_plugin().
  TestPluginManager.mock_python_plugin: TestPluginManager#mock_python_plugin().
  TestPluginManager.mock_javascript_plugin: TestPluginManager#mock_javascript_plugin().
  TestPluginManager.mock_typescript_plugin: TestPluginManager#mock_typescript_plugin().
  TestPluginManager.test_plugin_manager_initialization: TestPluginManager#test_plugin_manager_initialization().
  TestPluginManager.test_find_plugin_classes.TestPlugin.__init__: TestPluginManager#test_find_plugin_classes().TestPlugin#__init__().
  MockLanguagePlugin._language: MockLanguagePlugin#_language.
  MockLanguagePlugin._extensions: MockLanguagePlugin#_extensions.
  TestPluginManager.test_find_plugin_classes.OtherClass: TestPluginManager#test_find_plugin_classes().OtherClass#
  MockLanguagePlugin.__init__: MockLanguagePlugin#__init__().
  MockLanguagePlugin.create_extractor: MockLanguagePlugin#create_extractor().
  TestPluginManager: TestPluginManager#
  TestPluginManagerErrorHandling: TestPluginManagerErrorHandling#
  TestPluginManagerIntegration: TestPluginManagerIntegration#
---
# Module: [`tests/unit/core/test_manager.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py)

## Classes
### `MockLanguagePlugin`  ·  implements/extends LanguagePlugin
- def: [`tests/unit/core/test_manager.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L17)
- doc: Mock language plugin for testing
- signature: `class MockLanguagePlugin(LanguagePlugin):`
- members:
  - `analyze_file(self, file_path: str, request)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L36) — Mock implementation of analyze_file
  - `create_extractor(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L30)
  - `get_file_extensions(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L27)
  - `get_language_name(self)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L24)
  - `is_applicable(self, file_path: str)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L33)
- protocol/private: `__init__`[`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L20), `_extensions`[`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L22), `_language`[`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L21)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`LanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`source_code`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.source_code), [`node_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.node_count), [`query_results`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.query_results)  (1 test-only)
- used by: [`LanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin), [`get_language_name`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.create_extractor), [`is_applicable`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.is_applicable)  (23 test-only)

### `OtherClass`
- def: [`tests/unit/core/test_manager.py:199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L199)
- signature: `class OtherClass:`
- used by: (1 test-only callers)

### `TestPlugin`  ·  implements/extends MockLanguagePlugin
- def: [`tests/unit/core/test_manager.py:194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L194)
- signature: `class TestPlugin(MockLanguagePlugin):`
- protocol/private: `__init__`[`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L195)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (2 test-only callers)

### `TestPluginManager`
- def: [`tests/unit/core/test_manager.py:53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L53)
- doc: Test cases for PluginManager class
- signature: `class TestPluginManager:`
- members:
  - `mock_java_plugin(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L73) — Create a mock Java plugin
  - `mock_javascript_plugin(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L83) — Create a mock JavaScript plugin
  - `mock_python_plugin(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L78) — Create a mock Python plugin
  - `mock_typescript_plugin(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L88) — Create a mock TypeScript plugin
  - `plugin_manager(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L57) — Create an isolated PluginManager instance for testing
  - `test_find_plugin_classes(self, plugin_manager: PluginManager)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L188) — Test finding plugin classes in a module
  - `test_get_all_plugins(self, plugin_manager: PluginManager, mock_java_plugin: MockLanguagePlugin, mock_python_plugin: MockLanguagePlugin, mock_javascript_plugin: MockLanguagePlugin, mock_typescript_plugin: MockLanguagePlugin)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L237) — Test getting all registered plugins
  - `test_get_plugin_existing(self, plugin_manager: PluginManager, mock_java_plugin: MockLanguagePlugin)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L220) — Test getting an existing plugin
  - `test_get_plugin_info_existing(self, plugin_manager: PluginManager, mock_java_plugin: MockLanguagePlugin)` — [`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L343) — Test getting plugin info for existing plugin
  - `test_get_plugin_info_nonexistent(self, plugin_manager: PluginManager)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L356) — Test getting plugin info for non-existent plugin
  - `test_get_plugin_nonexistent(self, plugin_manager: PluginManager)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L231) — Test getting a non-existent plugin
  - `test_get_supported_languages(self, plugin_manager: PluginManager, mock_java_plugin: MockLanguagePlugin, mock_python_plugin: MockLanguagePlugin, mock_javascript_plugin: MockLanguagePlugin, mock_typescript_plugin: MockLanguagePlugin)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L260) — Test getting list of supported languages
  - `test_load_from_entry_points_success(self, plugin_manager: PluginManager)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L113) — Test loading plugins from entry points
  - `test_load_from_entry_points_with_exception(self, plugin_manager: PluginManager)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L129) — Test loading plugins from entry points with exception
  - `test_load_from_local_directory_success(self, plugin_manager: PluginManager)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L146) — Test loading plugins from local directory
  - `test_load_from_local_directory_with_exception(self, plugin_manager: PluginManager)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L175) — Test loading plugins from local directory with exception
  - `test_load_plugins_success(self, plugin_manager: PluginManager)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L99) — Test successful plugin loading with manually registered plugins
  - `test_plugin_manager_initialization(self, plugin_manager: PluginManager)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L92) — Test PluginManager initialization
  - `test_register_plugin_duplicate(self, plugin_manager: PluginManager, mock_java_plugin: MockLanguagePlugin)` — [`L302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L302) — Test registering duplicate plugin
  - `test_register_plugin_success(self, plugin_manager: PluginManager, mock_java_plugin: MockLanguagePlugin)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L293) — Test successful plugin registration
  - `test_register_plugin_with_exception(self, plugin_manager: PluginManager)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L315) — Test plugin registration with exception
  - `test_reload_plugins(self, plugin_manager: PluginManager)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L283) — Test reloading plugins
  - `test_unregister_plugin_existing(self, plugin_manager: PluginManager, mock_java_plugin: MockLanguagePlugin)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L326) — Test unregistering an existing plugin
  - `test_unregister_plugin_nonexistent(self, plugin_manager: PluginManager)` — [`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L337) — Test unregistering a non-existent plugin
  - `test_validate_plugin_invalid(self, plugin_manager: PluginManager)` — [`L370`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L370) — Test validating an invalid plugin
  - `test_validate_plugin_missing_methods(self, plugin_manager: PluginManager)` — [`L380`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L380) — Test validating a plugin with missing methods
  - `test_validate_plugin_valid(self, plugin_manager: PluginManager, mock_java_plugin: MockLanguagePlugin)` — [`L362`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L362) — Test validating a valid plugin
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`get_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_plugin), [`get_language_name`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_language_name), [`register_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.register_plugin), [`load_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.load_plugins), [`_load_from_local_directory`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._load_from_local_directory), [`_load_from_entry_points`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._load_from_entry_points), [`get_supported_languages`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_supported_languages), [`get_all_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_all_plugins), [`validate_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.validate_plugin), [`reload_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.reload_plugins), [`get_plugin_info`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_plugin_info), [`_discover_from_local_directory`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._discover_from_local_directory), [`unregister_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.unregister_plugin), [`_find_plugin_classes`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._find_plugin_classes), [`_get_default_aliases`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._get_default_aliases), [`_discover_from_entry_points`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._discover_from_entry_points)  (3 test-only)

### `TestPluginManagerErrorHandling`
- def: [`tests/unit/core/test_manager.py:393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L393)
- doc: Test error handling in PluginManager
- signature: `class TestPluginManagerErrorHandling:`
- members:
  - `plugin_manager(self)` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L397) — Create an isolated PluginManager instance for testing
  - `test_get_plugin_info_with_exception(self, plugin_manager: PluginManager)` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L447) — Test getting plugin info when plugin raises exception
  - `test_load_plugins_with_corrupted_entry_point(self, plugin_manager: PluginManager)` — [`L424`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L424) — Test loading plugins with corrupted entry point
  - `test_load_plugins_with_import_error(self, plugin_manager: PluginManager)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L412) — Test plugin loading with import errors
  - `test_register_plugin_none(self, plugin_manager: PluginManager)` — [`L441`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L441) — Test registering None as plugin
  - `test_validate_plugin_with_none(self, plugin_manager: PluginManager)` — [`L462`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L462) — Test validating None plugin
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`register_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.register_plugin), [`load_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.load_plugins), [`_load_from_local_directory`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._load_from_local_directory), [`_load_from_entry_points`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._load_from_entry_points), [`validate_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.validate_plugin), [`get_plugin_info`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_plugin_info), [`_discover_from_local_directory`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._discover_from_local_directory), [`_get_default_aliases`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._get_default_aliases), [`_discover_from_entry_points`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._discover_from_entry_points)

### `TestPluginManagerIntegration`
- def: [`tests/unit/core/test_manager.py:469`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L469)
- doc: Integration tests for PluginManager
- signature: `class TestPluginManagerIntegration:`
- members:
  - `plugin_manager(self)` — [`L473`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L473) — Create an isolated PluginManager instance for testing
  - `test_full_plugin_lifecycle(self, plugin_manager: PluginManager)` — [`L488`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L488) — Test complete plugin lifecycle
  - `test_plugin_discovery_and_loading(self, plugin_manager: PluginManager)` — [`L513`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L513) — Test plugin discovery and loading process
  - `test_plugin_manager_with_multiple_extensions(self, plugin_manager: PluginManager)` — [`L553`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L553) — Test plugin manager with plugins supporting multiple extensions
  - `test_plugin_reload_preserves_manual_registrations(self, plugin_manager: PluginManager)` — [`L573`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L573) — Test that plugin reload preserves manually registered plugins
  - `test_plugin_validation_during_registration(self, plugin_manager: PluginManager)` — [`L536`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager.py#L536) — Test plugin validation during registration process
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`get_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_plugin), [`get_language_name`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_language_name), [`register_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.register_plugin), [`load_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.load_plugins), [`_load_from_local_directory`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._load_from_local_directory), [`_load_from_entry_points`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._load_from_entry_points), [`get_supported_languages`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_supported_languages), [`reload_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.reload_plugins), [`get_plugin_info`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_plugin_info), [`_discover_from_local_directory`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._discover_from_local_directory), [`unregister_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.unregister_plugin), [`_get_default_aliases`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._get_default_aliases), [`_discover_from_entry_points`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._discover_from_entry_points)  (1 test-only)

