---
title: 'Module: tests/unit/core/test_manager_internal_branches.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_manager_internal_branches.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_manager_internal_branches`/Test
symbols:
  TestGetPluginEntryPoint.test_get_plugin_from_entry_point_map: GetPluginEntryPoint#test_get_plugin_from_entry_point_map().
  TestGetPluginEntryPoint.test_get_plugin_entry_point_fails_gracefully: GetPluginEntryPoint#test_get_plugin_entry_point_fails_gracefully().
  TestDiscoverFromEntryPoints.test_entry_point_map_init: DiscoverFromEntryPoints#test_entry_point_map_init().
  TestDiscoverFromLocalDirectory.test_discovers_plugin_modules: DiscoverFromLocalDirectory#test_discovers_plugin_modules().
  TestLoadFromLocalDirectory.test_plugin_instantiation_exception: LoadFromLocalDirectory#test_plugin_instantiation_exception().
  TestPrewarmPluginImports.test_prewarm_called_during_init: PrewarmPluginImports#test_prewarm_called_during_init().
  TestPrewarmPluginImports.test_prewarm_non_import_error: PrewarmPluginImports#test_prewarm_non_import_error().
  TestLoadFromEntryPoints.test_old_api_get_no_select: LoadFromEntryPoints#test_old_api_get_no_select().
  TestLoadFromEntryPoints.test_load_exception_in_loop: LoadFromEntryPoints#test_load_exception_in_loop().
  TestLoadFromEntryPoints.test_entry_points_type_error_outer: LoadFromEntryPoints#test_entry_points_type_error_outer().
  TestLoadFromLocalDirectory.test_languages_package_import_error: LoadFromLocalDirectory#test_languages_package_import_error().
  TestValidatePluginCallable.test_method_not_callable: ValidatePluginCallable#test_method_not_callable().
  TestLoadFromLocalDirectory.test_plugin_instantiation_exception.BadPlugin: LoadFromLocalDirectory#test_plugin_instantiation_exception().BadPlugin#
  TestPrewarmPluginImports: PrewarmPluginImports#
  TestDiscoverFromEntryPoints: DiscoverFromEntryPoints#
  TestDiscoverFromLocalDirectory: DiscoverFromLocalDirectory#
  TestGetPluginEntryPoint: GetPluginEntryPoint#
  TestLoadFromEntryPoints: LoadFromEntryPoints#
  TestLoadFromLocalDirectory: LoadFromLocalDirectory#
  TestLoadFromLocalDirectory.test_plugin_instantiation_exception.BadPlugin.__init__: LoadFromLocalDirectory#test_plugin_instantiation_exception().BadPlugin#__init__().
  TestValidatePluginCallable: ValidatePluginCallable#
---
# Module: [`tests/unit/core/test_manager_internal_branches.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py)

## Classes
### `BadPlugin`
- def: [`tests/unit/core/test_manager_internal_branches.py:162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L162)
- signature: `class BadPlugin:`
- protocol/private: `__init__`[`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L163)
- used by: (1 test-only callers)

### `TestDiscoverFromEntryPoints`
- def: [`tests/unit/core/test_manager_internal_branches.py:43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L43)
- signature: `class TestDiscoverFromEntryPoints:`
- members:
  - `test_entry_point_map_init(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L44)
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`_entry_point_map`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._entry_point_map), [`_discover_from_entry_points`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._discover_from_entry_points)

### `TestDiscoverFromLocalDirectory`
- def: [`tests/unit/core/test_manager_internal_branches.py:58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L58)
- signature: `class TestDiscoverFromLocalDirectory:`
- members:
  - `test_discovers_plugin_modules(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L59) — hits lines 156-168: iter_modules + _plugin suffix matching
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`_discover_from_local_directory`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._discover_from_local_directory), [`_plugin_modules`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._plugin_modules)

### `TestGetPluginEntryPoint`
- def: [`tests/unit/core/test_manager_internal_branches.py:72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L72)
- signature: `class TestGetPluginEntryPoint:`
- members:
  - `test_get_plugin_entry_point_fails_gracefully(self)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L92)
  - `test_get_plugin_from_entry_point_map(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L73)
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`get_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_plugin), [`_loaded_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._loaded_plugins), [`_entry_point_map`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._entry_point_map), [`_plugin_modules`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._plugin_modules), [`_discovered`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._discovered)

### `TestLoadFromEntryPoints`
- def: [`tests/unit/core/test_manager_internal_branches.py:113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L113)
- signature: `class TestLoadFromEntryPoints:`
- members:
  - `test_entry_points_type_error_outer(self)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L132)
  - `test_load_exception_in_loop(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L123)
  - `test_old_api_get_no_select(self)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L114)
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`_load_from_entry_points`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._load_from_entry_points)

### `TestLoadFromLocalDirectory`
- def: [`tests/unit/core/test_manager_internal_branches.py:144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L144)
- signature: `class TestLoadFromLocalDirectory:`
- members:
  - `test_languages_package_import_error(self)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L145)
  - `test_plugin_instantiation_exception(self)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L152)
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`_load_from_local_directory`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._load_from_local_directory)  (1 test-only)

### `TestPrewarmPluginImports`
- def: [`tests/unit/core/test_manager_internal_branches.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L18)
- signature: `class TestPrewarmPluginImports:`
- members:
  - `test_prewarm_called_during_init(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L19) — __init__ calls _prewarm_plugin_imports unconditionally
  - `test_prewarm_non_import_error(self)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L28) — languages import_module raises RuntimeError → log_debug path
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`_plugin_modules`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager._plugin_modules)

### `TestValidatePluginCallable`
- def: [`tests/unit/core/test_manager_internal_branches.py:176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L176)
- signature: `class TestValidatePluginCallable:`
- members:
  - `test_method_not_callable(self)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_manager_internal_branches.py#L177)
- uses (calls/refs, reference-scoped): [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`validate_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.validate_plugin)

