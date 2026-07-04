---
title: 'Module: tests/unit/core/test_plugins_manager.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_plugins_manager.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_plugins_manager`/
symbols:
  MockPlugin: MockPlugin#
  TestPluginManagerIntegration.test_full_lifecycle: TestPluginManagerIntegration#test_full_lifecycle().
  TestPluginManagerReloadPlugins.test_reload_plugins: TestPluginManagerReloadPlugins#test_reload_plugins().
  TestPluginManagerIntegration.test_multiple_plugins: TestPluginManagerIntegration#test_multiple_plugins().
  TestPluginManagerInitialization.test_initialization: TestPluginManagerInitialization#test_initialization().
  TestPluginManagerGetPlugin.test_get_plugin_lazy_load: TestPluginManagerGetPlugin#test_get_plugin_lazy_load().
  TestPluginManagerGetAllPlugins.test_get_all_plugins_with_loaded: TestPluginManagerGetAllPlugins#test_get_all_plugins_with_loaded().
  TestPluginManagerGetSupportedLanguages.test_get_supported_languages_with_plugins: TestPluginManagerGetSupportedLanguages#test_get_supported_languages_with_plugins().
  TestPluginManagerIntegration.test_plugin_replacement: TestPluginManagerIntegration#test_plugin_replacement().
  TestPluginManagerLoadPlugins.test_load_plugins_with_manual_registration: TestPluginManagerLoadPlugins#test_load_plugins_with_manual_registration().
  TestPluginManagerGetPlugin.test_get_plugin_already_loaded: TestPluginManagerGetPlugin#test_get_plugin_already_loaded().
  TestPluginManagerGetPlugin.test_get_plugin_case_insensitive: TestPluginManagerGetPlugin#test_get_plugin_case_insensitive().
  TestPluginManagerFindPluginClasses.test_find_plugin_classes: TestPluginManagerFindPluginClasses#test_find_plugin_classes().
  TestPluginManagerRegisterPlugin.test_register_plugin_success: TestPluginManagerRegisterPlugin#test_register_plugin_success().
  TestPluginManagerRegisterPlugin.test_register_plugin_duplicate: TestPluginManagerRegisterPlugin#test_register_plugin_duplicate().
  TestPluginManagerUnregisterPlugin.test_unregister_plugin_success: TestPluginManagerUnregisterPlugin#test_unregister_plugin_success().
  TestPluginManagerGetPluginInfo.test_get_plugin_info_success: TestPluginManagerGetPluginInfo#test_get_plugin_info_success().
  MockPlugin2: MockPlugin2#
  TestPluginManagerLoadPlugins.test_load_plugins_first_call: TestPluginManagerLoadPlugins#test_load_plugins_first_call().
  TestPluginManagerDiscoverFromEntryPoints.test_discover_with_select_api: TestPluginManagerDiscoverFromEntryPoints#test_discover_with_select_api().
  TestPluginManagerDiscoverFromLocalDirectory.test_discover_no_languages_dir: TestPluginManagerDiscoverFromLocalDirectory#test_discover_no_languages_dir().
  TestPluginManagerLoadFromEntryPoints.test_load_from_entry_points_success: TestPluginManagerLoadFromEntryPoints#test_load_from_entry_points_success().
  TestPluginManagerFindPluginClasses.test_find_plugin_classes_excludes_base: TestPluginManagerFindPluginClasses#test_find_plugin_classes_excludes_base().
  TestPluginManagerValidatePlugin.test_validate_plugin_success: TestPluginManagerValidatePlugin#test_validate_plugin_success().
  TestPluginManagerLoadPlugins.test_load_plugins_cached: TestPluginManagerLoadPlugins#test_load_plugins_cached().
  TestPluginManagerDiscoverFromEntryPoints.test_discover_exception_handling: TestPluginManagerDiscoverFromEntryPoints#test_discover_exception_handling().
  TestPluginManagerDiscoverFromLocalDirectory.test_discover_local_plugins: TestPluginManagerDiscoverFromLocalDirectory#test_discover_local_plugins().
  TestPluginManagerGetPlugin.test_get_plugin_not_found: TestPluginManagerGetPlugin#test_get_plugin_not_found().
  TestPluginManagerLoadFromEntryPoints.test_load_invalid_plugin: TestPluginManagerLoadFromEntryPoints#test_load_invalid_plugin().
  TestPluginManagerLoadFromLocalDirectory.test_load_local_plugins: TestPluginManagerLoadFromLocalDirectory#test_load_local_plugins().
  TestPluginManagerLoadFromLocalDirectory.test_load_creates_languages_dir: TestPluginManagerLoadFromLocalDirectory#test_load_creates_languages_dir().
  TestPluginManagerGetAllPlugins.test_get_all_plugins_empty: TestPluginManagerGetAllPlugins#test_get_all_plugins_empty().
  TestPluginManagerGetDefaultAliases.test_get_default_aliases: TestPluginManagerGetDefaultAliases#test_get_default_aliases().
  TestPluginManagerGetSupportedLanguages.test_get_supported_languages_empty: TestPluginManagerGetSupportedLanguages#test_get_supported_languages_empty().
  TestPluginManagerRegisterPlugin.test_register_plugin_exception: TestPluginManagerRegisterPlugin#test_register_plugin_exception().
  TestPluginManagerUnregisterPlugin.test_unregister_plugin_not_found: TestPluginManagerUnregisterPlugin#test_unregister_plugin_not_found().
  TestPluginManagerGetPluginInfo.test_get_plugin_info_not_found: TestPluginManagerGetPluginInfo#test_get_plugin_info_not_found().
  TestPluginManagerValidatePlugin.test_validate_plugin_missing_method: TestPluginManagerValidatePlugin#test_validate_plugin_missing_method().
  TestPluginManagerValidatePlugin.test_validate_plugin_invalid_language_name: TestPluginManagerValidatePlugin#test_validate_plugin_invalid_language_name().
  TestPluginManagerValidatePlugin.test_validate_plugin_invalid_extensions: TestPluginManagerValidatePlugin#test_validate_plugin_invalid_extensions().
  TestPluginManagerValidatePlugin.test_validate_plugin_no_extractor: TestPluginManagerValidatePlugin#test_validate_plugin_no_extractor().
  TestIsSourceCheckout.test_is_source_checkout_with_git: TestIsSourceCheckout#test_is_source_checkout_with_git().
  TestIsSourceCheckout.test_is_source_checkout_without_git: TestIsSourceCheckout#test_is_source_checkout_without_git().
  TestIsSourceCheckout.test_is_source_checkout_exception: TestIsSourceCheckout#test_is_source_checkout_exception().
  TestShouldLoadEntryPoints.test_skip_entry_points_env_set: TestShouldLoadEntryPoints#test_skip_entry_points_env_set().
  TestShouldLoadEntryPoints.test_load_entry_points_env_set_to_zero: TestShouldLoadEntryPoints#test_load_entry_points_env_set_to_zero().
  TestShouldLoadEntryPoints.test_load_entry_points_default: TestShouldLoadEntryPoints#test_load_entry_points_default().
  TestShouldLoadEntryPoints.test_skip_entry_points_with_whitespace: TestShouldLoadEntryPoints#test_skip_entry_points_with_whitespace().
  TestIsRunningUnderPytest.test_running_under_pytest: TestIsRunningUnderPytest#test_running_under_pytest().
  TestIsRunningUnderPytest.test_not_running_under_pytest: TestIsRunningUnderPytest#test_not_running_under_pytest().
  MockPlugin.get_language_name: MockPlugin#get_language_name().
  MockPlugin.get_file_extensions: MockPlugin#get_file_extensions().
  MockPlugin.create_extractor: MockPlugin#create_extractor().
  MockPlugin.analyze_file: MockPlugin#analyze_file().
  MockPlugin2.get_language_name: MockPlugin2#get_language_name().
  MockPlugin2.get_file_extensions: MockPlugin2#get_file_extensions().
  MockPlugin2.create_extractor: MockPlugin2#create_extractor().
  MockPlugin2.analyze_file: MockPlugin2#analyze_file().
  TestIsSourceCheckout: TestIsSourceCheckout#
  TestShouldLoadEntryPoints: TestShouldLoadEntryPoints#
  TestIsRunningUnderPytest: TestIsRunningUnderPytest#
  TestPluginManagerInitialization: TestPluginManagerInitialization#
  TestPluginManagerLoadPlugins: TestPluginManagerLoadPlugins#
  TestPluginManagerDiscoverFromEntryPoints: TestPluginManagerDiscoverFromEntryPoints#
  TestPluginManagerDiscoverFromLocalDirectory: TestPluginManagerDiscoverFromLocalDirectory#
  TestPluginManagerGetPlugin: TestPluginManagerGetPlugin#
  TestPluginManagerLoadFromEntryPoints: TestPluginManagerLoadFromEntryPoints#
  TestPluginManagerLoadFromLocalDirectory: TestPluginManagerLoadFromLocalDirectory#
  TestPluginManagerFindPluginClasses: TestPluginManagerFindPluginClasses#
  TestPluginManagerGetAllPlugins: TestPluginManagerGetAllPlugins#
  TestPluginManagerGetDefaultAliases: TestPluginManagerGetDefaultAliases#
  TestPluginManagerGetSupportedLanguages: TestPluginManagerGetSupportedLanguages#
  TestPluginManagerReloadPlugins: TestPluginManagerReloadPlugins#
  TestPluginManagerRegisterPlugin: TestPluginManagerRegisterPlugin#
  TestPluginManagerUnregisterPlugin: TestPluginManagerUnregisterPlugin#
  TestPluginManagerGetPluginInfo: TestPluginManagerGetPluginInfo#
  TestPluginManagerValidatePlugin: TestPluginManagerValidatePlugin#
  TestPluginManagerIntegration: TestPluginManagerIntegration#
---
# Module: [`tests/unit/core/test_plugins_manager.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py)

## Classes
### `MockPlugin`  ·  implements/extends LanguagePlugin
- def: [`tests/unit/core/test_plugins_manager.py:22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L22)
- doc: Mock plugin for testing
- signature: `class MockPlugin(LanguagePlugin):`
- members:
  - `analyze_file(self, file_path: Path, options: dict[str, Any] | None = None)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L34)
  - `create_extractor(self)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L31)
  - `get_file_extensions(self)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L28)
  - `get_language_name(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L25)
- uses (calls/refs, reference-scoped): [`LanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin)
- used by: [`LanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin), [`get_language_name`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.create_extractor)  (17 test-only)

### `MockPlugin2`  ·  implements/extends LanguagePlugin
- def: [`tests/unit/core/test_plugins_manager.py:40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L40)
- doc: Another mock plugin for testing
- signature: `class MockPlugin2(LanguagePlugin):`
- members:
  - `analyze_file(self, file_path: Path, options: dict[str, Any] | None = None)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L52)
  - `create_extractor(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L49)
  - `get_file_extensions(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L46)
  - `get_language_name(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L43)
- uses (calls/refs, reference-scoped): [`LanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin)
- used by: [`LanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin), [`get_language_name`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.create_extractor)  (5 test-only)

### `TestIsRunningUnderPytest`
- def: [`tests/unit/core/test_plugins_manager.py:124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L124)
- doc: Tests for _is_running_under_pytest function
- signature: `class TestIsRunningUnderPytest:`
- members:
  - `test_not_running_under_pytest(self)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L134) — Test detection when pytest is not in sys.modules
  - `test_running_under_pytest(self)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L128) — Test detection when pytest is in sys.modules
- uses (calls/refs, reference-scoped): [`_is_running_under_pytest`](../../../tree_sitter_analyzer/plugins/manager.md#_is_running_under_pytest)

### `TestIsSourceCheckout`
- def: [`tests/unit/core/test_plugins_manager.py:58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L58)
- doc: Tests for _is_source_checkout function
- signature: `class TestIsSourceCheckout:`
- members:
  - `test_is_source_checkout_exception(self, mock_path: MagicMock)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L88) — Test exception handling
  - `test_is_source_checkout_with_git(self, mock_path: MagicMock)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L62) — Test detection when .git directory exists
  - `test_is_source_checkout_without_git(self, mock_path: MagicMock)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L74) — Test detection when no .git directory exists
- uses (calls/refs, reference-scoped): [`_is_source_checkout`](../../../tree_sitter_analyzer/plugins/manager.md#_is_source_checkout)

### `TestPluginManagerDiscoverFromEntryPoints`
- def: [`tests/unit/core/test_plugins_manager.py:187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L187)
- doc: Tests for _discover_from_entry_points method
- signature: `class TestPluginManagerDiscoverFromEntryPoints:`
- members:
  - `test_discover_exception_handling(self, mock_log_warning: MagicMock, mock_entry_points: MagicMock)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L209) — Test exception handling during discovery
  - `test_discover_with_select_api(self, mock_log_debug: MagicMock, mock_entry_points: MagicMock)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L192) — Test discovery with select API (Python 3.10+)
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`_entry_point_map`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._entry_point_map), [`_discover_from_entry_points`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._discover_from_entry_points)

### `TestPluginManagerDiscoverFromLocalDirectory`
- def: [`tests/unit/core/test_plugins_manager.py:221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L221)
- doc: Tests for _discover_from_local_directory method
- signature: `class TestPluginManagerDiscoverFromLocalDirectory:`
- members:
  - `test_discover_local_plugins(self, mock_path: MagicMock)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L225) — Test discovering local plugins
  - `test_discover_no_languages_dir(self, mock_path: MagicMock)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L245) — Test when languages directory doesn't exist
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`_discover_from_local_directory`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._discover_from_local_directory), [`_plugin_modules`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._plugin_modules)

### `TestPluginManagerFindPluginClasses`
- def: [`tests/unit/core/test_plugins_manager.py:393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L393)
- doc: Tests for _find_plugin_classes method
- signature: `class TestPluginManagerFindPluginClasses:`
- members:
  - `test_find_plugin_classes(self)` — [`L396`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L396) — Test finding plugin classes in a module
  - `test_find_plugin_classes_excludes_base(self)` — [`L413`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L413) — Test that LanguagePlugin base class is excluded
- uses (calls/refs, reference-scoped): [`LanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin), [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`_find_plugin_classes`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._find_plugin_classes)  (2 test-only)

### `TestPluginManagerGetAllPlugins`
- def: [`tests/unit/core/test_plugins_manager.py:425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L425)
- doc: Tests for get_all_plugins method
- signature: `class TestPluginManagerGetAllPlugins:`
- members:
  - `test_get_all_plugins_empty(self)` — [`L428`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L428) — Test getting all plugins when none are loaded
  - `test_get_all_plugins_with_loaded(self)` — [`L436`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L436) — Test getting all loaded plugins
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`_loaded_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._loaded_plugins), [`get_all_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_all_plugins)  (2 test-only)

### `TestPluginManagerGetDefaultAliases`
- def: [`tests/unit/core/test_plugins_manager.py:453`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L453)
- doc: Tests for _get_default_aliases method
- signature: `class TestPluginManagerGetDefaultAliases:`
- members:
  - `test_get_default_aliases(self)` — [`L456`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L456) — Test getting default aliases
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`_get_default_aliases`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._get_default_aliases)

### `TestPluginManagerGetPlugin`
- def: [`tests/unit/core/test_plugins_manager.py:260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L260)
- doc: Tests for get_plugin method
- signature: `class TestPluginManagerGetPlugin:`
- members:
  - `test_get_plugin_already_loaded(self)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L263) — Test getting already loaded plugin
  - `test_get_plugin_case_insensitive(self)` — [`L281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L281) — Test case-insensitive plugin lookup
  - `test_get_plugin_lazy_load(self, mock_import: MagicMock)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L292) — Test lazy loading of plugin
  - `test_get_plugin_not_found(self)` — [`L273`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L273) — Test getting non-existent plugin
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`get_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_plugin), [`_loaded_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._loaded_plugins), [`_plugin_modules`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._plugin_modules)  (1 test-only)

### `TestPluginManagerGetPluginInfo`
- def: [`tests/unit/core/test_plugins_manager.py:581`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L581)
- doc: Tests for get_plugin_info method
- signature: `class TestPluginManagerGetPluginInfo:`
- members:
  - `test_get_plugin_info_not_found(self)` — [`L598`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L598) — Test getting info for non-existent plugin
  - `test_get_plugin_info_success(self)` — [`L584`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L584) — Test getting plugin info
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`_loaded_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._loaded_plugins), [`get_plugin_info`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_plugin_info)  (1 test-only)

### `TestPluginManagerGetSupportedLanguages`
- def: [`tests/unit/core/test_plugins_manager.py:468`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L468)
- doc: Tests for get_supported_languages method
- signature: `class TestPluginManagerGetSupportedLanguages:`
- members:
  - `test_get_supported_languages_empty(self)` — [`L471`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L471) — Test getting supported languages when none are loaded
  - `test_get_supported_languages_with_plugins(self)` — [`L479`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L479) — Test getting supported languages with loaded plugins
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`_loaded_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._loaded_plugins), [`get_supported_languages`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_supported_languages)  (2 test-only)

### `TestPluginManagerInitialization`
- def: [`tests/unit/core/test_plugins_manager.py:140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L140)
- doc: Tests for PluginManager initialization
- signature: `class TestPluginManagerInitialization:`
- members:
  - `test_initialization(self)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L143) — Test default initialization of PluginManager
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`_loaded_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._loaded_plugins), [`_plugin_modules`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._plugin_modules), [`_discovered`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._discovered), [`_entry_point_group`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._entry_point_group)

### `TestPluginManagerIntegration`
- def: [`tests/unit/core/test_plugins_manager.py:683`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L683)
- doc: Integration tests for PluginManager
- signature: `class TestPluginManagerIntegration:`
- members:
  - `test_full_lifecycle(self)` — [`L686`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L686) — Test full plugin lifecycle
  - `test_multiple_plugins(self)` — [`L709`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L709) — Test managing multiple plugins
  - `test_plugin_replacement(self)` — [`L728`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L728) — Test replacing an existing plugin
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`get_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_plugin), [`register_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.register_plugin), [`_loaded_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._loaded_plugins), [`get_supported_languages`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_supported_languages), [`get_all_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_all_plugins), [`validate_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.validate_plugin), [`get_plugin_info`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_plugin_info), [`unregister_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.unregister_plugin)  (2 test-only)

### `TestPluginManagerLoadFromEntryPoints`
- def: [`tests/unit/core/test_plugins_manager.py:309`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L309)
- doc: Tests for _load_from_entry_points method
- signature: `class TestPluginManagerLoadFromEntryPoints:`
- members:
  - `test_load_from_entry_points_success(self, mock_log_debug: MagicMock, mock_entry_points: MagicMock)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L314) — Test successful loading from entry points
  - `test_load_invalid_plugin(self, mock_log_warning: MagicMock, mock_entry_points: MagicMock)` — [`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L333) — Test loading invalid plugin (not a LanguagePlugin subclass)
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`_load_from_entry_points`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._load_from_entry_points)  (1 test-only)

### `TestPluginManagerLoadFromLocalDirectory`
- def: [`tests/unit/core/test_plugins_manager.py:351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L351)
- doc: Tests for _load_from_local_directory method
- signature: `class TestPluginManagerLoadFromLocalDirectory:`
- members:
  - `test_load_creates_languages_dir(self, mock_log_debug: MagicMock, mock_path: MagicMock)` — [`L375`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L375) — Test that languages directory is created if it doesn't exist
  - `test_load_local_plugins(self, mock_path: MagicMock)` — [`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L355) — Test loading local plugins
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`_load_from_local_directory`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._load_from_local_directory)

### `TestPluginManagerLoadPlugins`
- def: [`tests/unit/core/test_plugins_manager.py:152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L152)
- doc: Tests for load_plugins method
- signature: `class TestPluginManagerLoadPlugins:`
- members:
  - `test_load_plugins_cached(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L163) — Test that subsequent calls return cached results
  - `test_load_plugins_first_call(self)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L155) — Test first call to load_plugins
  - `test_load_plugins_with_manual_registration(self)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L175) — Test load_plugins returns manually registered plugins
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`register_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.register_plugin), [`load_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.load_plugins), [`_discovered`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._discovered)  (1 test-only)

### `TestPluginManagerRegisterPlugin`
- def: [`tests/unit/core/test_plugins_manager.py:514`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L514)
- doc: Tests for register_plugin method
- signature: `class TestPluginManagerRegisterPlugin:`
- members:
  - `test_register_plugin_duplicate(self, mock_log_warning: MagicMock)` — [`L530`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L530) — Test registering duplicate plugin
  - `test_register_plugin_exception(self, mock_log_error: MagicMock)` — [`L544`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L544) — Test exception handling during registration
  - `test_register_plugin_success(self, mock_log_debug: MagicMock)` — [`L518`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L518) — Test successful plugin registration
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`register_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.register_plugin), [`_loaded_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._loaded_plugins)  (1 test-only)

### `TestPluginManagerReloadPlugins`
- def: [`tests/unit/core/test_plugins_manager.py:494`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L494)
- doc: Tests for reload_plugins method
- signature: `class TestPluginManagerReloadPlugins:`
- members:
  - `test_reload_plugins(self, mock_log_info: MagicMock)` — [`L498`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L498) — Test reloading plugins
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`_loaded_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._loaded_plugins), [`reload_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.reload_plugins), [`_plugin_modules`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._plugin_modules), [`_discovered`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._discovered)  (1 test-only)

### `TestPluginManagerUnregisterPlugin`
- def: [`tests/unit/core/test_plugins_manager.py:556`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L556)
- doc: Tests for unregister_plugin method
- signature: `class TestPluginManagerUnregisterPlugin:`
- members:
  - `test_unregister_plugin_not_found(self)` — [`L572`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L572) — Test unregistering non-existent plugin
  - `test_unregister_plugin_success(self, mock_log_debug: MagicMock)` — [`L560`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L560) — Test successful plugin unregistration
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`_loaded_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._loaded_plugins), [`unregister_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.unregister_plugin)  (1 test-only)

### `TestPluginManagerValidatePlugin`
- def: [`tests/unit/core/test_plugins_manager.py:607`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L607)
- doc: Tests for validate_plugin method
- signature: `class TestPluginManagerValidatePlugin:`
- members:
  - `test_validate_plugin_invalid_extensions(self, mock_log_error: MagicMock)` — [`L653`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L653) — Test validating plugin with invalid extensions
  - `test_validate_plugin_invalid_language_name(self, mock_log_error: MagicMock)` — [`L637`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L637) — Test validating plugin with invalid language name
  - `test_validate_plugin_missing_method(self, mock_log_error: MagicMock)` — [`L622`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L622) — Test validating plugin with missing method
  - `test_validate_plugin_no_extractor(self, mock_log_error: MagicMock)` — [`L669`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L669) — Test validating plugin that returns no extractor
  - `test_validate_plugin_success(self, mock_log_error: MagicMock)` — [`L611`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L611) — Test validating a valid plugin
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`validate_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.validate_plugin)  (1 test-only)

### `TestShouldLoadEntryPoints`
- def: [`tests/unit/core/test_plugins_manager.py:96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L96)
- doc: Tests for _should_load_entry_points function
- signature: `class TestShouldLoadEntryPoints:`
- members:
  - `test_load_entry_points_default(self)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L112) — Test default behavior (load entry points)
  - `test_load_entry_points_env_set_to_zero(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L106) — Test loading when environment variable is set to 0
  - `test_skip_entry_points_env_set(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L100) — Test skipping when environment variable is set to 1
  - `test_skip_entry_points_with_whitespace(self)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_plugins_manager.py#L118) — Test skipping with whitespace in environment variable
- uses (calls/refs, reference-scoped): [`_should_load_entry_points`](../../../tree_sitter_analyzer/plugins/manager.md#_should_load_entry_points)

