---
title: 'Module: tests/unit/synapse_resolver/test_context.py'
type: catalog
provenance: extracted
module: tests/unit/synapse_resolver/test_context.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.synapse_resolver.test_context`/
symbols:
  TestResolverContextConstruction.test_no_cache_empty_maps: TestResolverContextConstruction#test_no_cache_empty_maps().
  TestResolverContextProperties.test_imports_by_file_property: TestResolverContextProperties#test_imports_by_file_property().
  _prebuilt_ctx: _prebuilt_ctx().
  TestEnsureLoaded.test_with_cache_calls_build: TestEnsureLoaded#test_with_cache_calls_build().
  TestEnsureLoaded.test_second_property_access_does_not_rebuild: TestEnsureLoaded#test_second_property_access_does_not_rebuild().
  TestBuildResolverContextCache.test_lru_cache_miss_different_identity: TestBuildResolverContextCache#test_lru_cache_miss_different_identity().
  TestBuildResolverContextCache.test_clear_cache_forces_rebuild: TestBuildResolverContextCache#test_clear_cache_forces_rebuild().
  TestEnsureLoaded.test_no_cache_marks_loaded_without_build: TestEnsureLoaded#test_no_cache_marks_loaded_without_build().
  TestFileClassMethodsLazy.test_lazy_load_from_cache: TestFileClassMethodsLazy#test_lazy_load_from_cache().
  TestBuildResolverContextCache.test_lru_cache_hit: TestBuildResolverContextCache#test_lru_cache_hit().
  _make_cache: _make_cache().
  TestResolverContextConstruction.test_cache_stored: TestResolverContextConstruction#test_cache_stored().
  TestFileClassMethodsLazy.test_no_double_load: TestFileClassMethodsLazy#test_no_double_load().
  TestResolverContextConstruction.test_no_cache_loaded_flag_false: TestResolverContextConstruction#test_no_cache_loaded_flag_false().
  TestResolverContextConstruction.test_prebuilt_maps_loaded_flag_true: TestResolverContextConstruction#test_prebuilt_maps_loaded_flag_true().
  TestResolverContextConstruction.test_project_root_stored: TestResolverContextConstruction#test_project_root_stored().
  TestResolverContextConstruction.test_single_prebuilt_map_sets_loaded: TestResolverContextConstruction#test_single_prebuilt_map_sets_loaded().
  TestResolverContextConstruction.test_all_maps_none_not_loaded: TestResolverContextConstruction#test_all_maps_none_not_loaded().
  TestResolverContextConstruction.test_file_class_methods_loaded_flag_with_prebuilt: TestResolverContextConstruction#test_file_class_methods_loaded_flag_with_prebuilt().
  TestResolverContextConstruction.test_file_class_methods_loaded_flag_without_prebuilt: TestResolverContextConstruction#test_file_class_methods_loaded_flag_without_prebuilt().
  TestResolverContextProperties.test_file_symbols_property: TestResolverContextProperties#test_file_symbols_property().
  TestResolverContextProperties.test_name_to_source_property: TestResolverContextProperties#test_name_to_source_property().
  TestResolverContextProperties.test_file_class_methods_property: TestResolverContextProperties#test_file_class_methods_property().
  TestResolverContextProperties.test_global_name_table_property: TestResolverContextProperties#test_global_name_table_property().
  TestResolverContextProperties.test_import_alias_target_property: TestResolverContextProperties#test_import_alias_target_property().
  TestResolverContextProperties.test_builtins_property: TestResolverContextProperties#test_builtins_property().
  TestResolverContextProperties.test_stdlib_modules_property: TestResolverContextProperties#test_stdlib_modules_property().
  TestResolverContextProperties.test_callee_resolver_property_none: TestResolverContextProperties#test_callee_resolver_property_none().
  TestResolverContextProperties.test_callee_resolver_property_set: TestResolverContextProperties#test_callee_resolver_property_set().
  TestResolveRelativeModule.test_single_dot_sibling: TestResolveRelativeModule#test_single_dot_sibling().
  TestResolveRelativeModule.test_single_dot_init: TestResolveRelativeModule#test_single_dot_init().
  TestResolveRelativeModule.test_double_dot_parent: TestResolveRelativeModule#test_double_dot_parent().
  TestBuildResolverContextCache._build: TestBuildResolverContextCache#_build().
  TestResolveRelativeModule._m2f: TestResolveRelativeModule#_m2f().
  TestIsEnabled.test_enabled_by_default: TestIsEnabled#test_enabled_by_default().
  TestIsEnabled.test_disabled_values: TestIsEnabled#test_disabled_values().
  TestIsEnabled.test_enabled_values: TestIsEnabled#test_enabled_values().
  TestBuildModuleToFile.test_regular_module: TestBuildModuleToFile#test_regular_module().
  TestBuildModuleToFile.test_init_module: TestBuildModuleToFile#test_init_module().
  TestBuildModuleToFile.test_nested_module: TestBuildModuleToFile#test_nested_module().
  TestBuildModuleToFile.test_multiple_files: TestBuildModuleToFile#test_multiple_files().
  TestBuildModuleToFile.test_empty_list: TestBuildModuleToFile#test_empty_list().
  TestBuildModuleToFile.test_non_py_file_excluded: TestBuildModuleToFile#test_non_py_file_excluded().
  TestResolveAbsoluteModule.test_exact_match: TestResolveAbsoluteModule#test_exact_match().
  TestResolveAbsoluteModule.test_partial_match: TestResolveAbsoluteModule#test_partial_match().
  TestResolveAbsoluteModule.test_no_match: TestResolveAbsoluteModule#test_no_match().
  TestResolveAbsoluteModule.test_empty_module_to_file: TestResolveAbsoluteModule#test_empty_module_to_file().
  TestResolveRelativeModule.test_no_match_returns_empty: TestResolveRelativeModule#test_no_match_returns_empty().
  TestBuildResolverContextCache._identity: TestBuildResolverContextCache#_identity().
  TestResolverContextConstruction: TestResolverContextConstruction#
  TestResolverContextProperties: TestResolverContextProperties#
  TestEnsureLoaded: TestEnsureLoaded#
  TestFileClassMethodsLazy: TestFileClassMethodsLazy#
  TestIsEnabled: TestIsEnabled#
  TestBuildModuleToFile: TestBuildModuleToFile#
  TestResolveAbsoluteModule: TestResolveAbsoluteModule#
  TestResolveRelativeModule: TestResolveRelativeModule#
  TestBuildResolverContextCache: TestBuildResolverContextCache#
---
# Module: [`tests/unit/synapse_resolver/test_context.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py)

## Classes
### `TestBuildModuleToFile`
- def: [`tests/unit/synapse_resolver/test_context.py:309`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L309)
- doc: _build_module_to_file maps Python file paths to dotted module names.
- signature: `class TestBuildModuleToFile:`
- members:
  - `test_empty_list(self)` — [`L330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L330)
  - `test_init_module(self)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L316)
  - `test_multiple_files(self)` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L324)
  - `test_nested_module(self)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L320)
  - `test_non_py_file_excluded(self)` — [`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L333)
  - `test_regular_module(self)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L312)
- uses (calls/refs, reference-scoped): [`_build_module_to_file`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#_build_module_to_file)

### `TestBuildResolverContextCache`
- def: [`tests/unit/synapse_resolver/test_context.py:398`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L398)
- doc: build_resolver_context reuses LRU-cached results for same cache snapshot.
- signature: `class TestBuildResolverContextCache:`
- members:
  - `test_clear_cache_forces_rebuild(self, monkeypatch: pytest.MonkeyPatch)` — [`L443`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L443)
  - `test_lru_cache_hit(self, monkeypatch: pytest.MonkeyPatch)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L401)
  - `test_lru_cache_miss_different_identity(self, monkeypatch: pytest.MonkeyPatch)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L416)
- protocol/private: `_build`[`L421`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L421), `_identity`[`L431`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L431)
- uses (calls/refs, reference-scoped): [`build_resolver_context`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#build_resolver_context), [`clear_resolver_context_cache`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#clear_resolver_context_cache)  (2 test-only)

### `TestEnsureLoaded`
- def: [`tests/unit/synapse_resolver/test_context.py:182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L182)
- doc: _ensure_loaded triggers build_resolver_context when cache is present.
- signature: `class TestEnsureLoaded:`
- members:
  - `test_no_cache_marks_loaded_without_build(self)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L185)
  - `test_second_property_access_does_not_rebuild(self, monkeypatch: pytest.MonkeyPatch)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L214)
  - `test_with_cache_calls_build(self, monkeypatch: pytest.MonkeyPatch)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L193)
- uses (calls/refs, reference-scoped): [`_ensure_loaded`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext._ensure_loaded), [`ResolverContext`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext), [`file_symbols`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext.file_symbols), [`_loaded`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext._loaded), [`clear_resolver_context_cache`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#clear_resolver_context_cache), [`name_to_source`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext.name_to_source), [`_file_symbols`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext._file_symbols)  (2 test-only)

### `TestFileClassMethodsLazy`
- def: [`tests/unit/synapse_resolver/test_context.py:237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L237)
- doc: file_class_methods triggers _build_file_class_methods_from_cache lazily.
- signature: `class TestFileClassMethodsLazy:`
- members:
  - `test_lazy_load_from_cache(self, monkeypatch: pytest.MonkeyPatch)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L240)
  - `test_no_double_load(self, monkeypatch: pytest.MonkeyPatch)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L263)
- uses (calls/refs, reference-scoped): [`ResolverContext`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext), [`file_class_methods`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext.file_class_methods), [`_file_class_methods_loaded`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext._file_class_methods_loaded)  (1 test-only)

### `TestIsEnabled`
- def: [`tests/unit/synapse_resolver/test_context.py:286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L286)
- doc: is_enabled() respects the TSA_SYNAPSE environment variable.
- signature: `class TestIsEnabled:`
- members:
  - `test_disabled_values(self, val: str, monkeypatch: pytest.MonkeyPatch)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L294)
  - `test_enabled_by_default(self, monkeypatch: pytest.MonkeyPatch)` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L289)
  - `test_enabled_values(self, val: str, monkeypatch: pytest.MonkeyPatch)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L299)
- uses (calls/refs, reference-scoped): [`is_enabled`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#is_enabled)

### `TestResolveAbsoluteModule`
- def: [`tests/unit/synapse_resolver/test_context.py:343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L343)
- doc: _resolve_absolute_module walks the dotted name to find the file.
- signature: `class TestResolveAbsoluteModule:`
- members:
  - `test_empty_module_to_file(self)` — [`L358`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L358)
  - `test_exact_match(self)` — [`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L346)
  - `test_no_match(self)` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L354)
  - `test_partial_match(self)` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L350)
- uses (calls/refs, reference-scoped): [`_resolve_absolute_module`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#_resolve_absolute_module)

### `TestResolveRelativeModule`
- def: [`tests/unit/synapse_resolver/test_context.py:367`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L367)
- doc: _resolve_relative_module handles leading-dot relative imports.
- signature: `class TestResolveRelativeModule:`
- members:
  - `test_double_dot_parent(self)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L383)
  - `test_no_match_returns_empty(self)` — [`L388`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L388)
  - `test_single_dot_init(self)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L378)
  - `test_single_dot_sibling(self)` — [`L373`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L373)
- protocol/private: `_m2f`[`L370`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L370)
- uses (calls/refs, reference-scoped): [`_resolve_relative_module`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#_resolve_relative_module)

### `TestResolverContextConstruction`
- def: [`tests/unit/synapse_resolver/test_context.py:59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L59)
- doc: ResolverContext builds correctly in both construction modes.
- signature: `class TestResolverContextConstruction:`
- members:
  - `test_all_maps_none_not_loaded(self)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L101)
  - `test_cache_stored(self)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L87)
  - `test_file_class_methods_loaded_flag_with_prebuilt(self)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L105)
  - `test_file_class_methods_loaded_flag_without_prebuilt(self)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L109)
  - `test_no_cache_empty_maps(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L62)
  - `test_no_cache_loaded_flag_false(self)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L75)
  - `test_prebuilt_maps_loaded_flag_true(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L79)
  - `test_project_root_stored(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L83)
  - `test_single_prebuilt_map_sets_loaded(self)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L92) — Even one non-None kwarg marks the context as loaded.
- uses (calls/refs, reference-scoped): [`ResolverContext`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext), [`_loaded`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext._loaded), [`_file_class_methods_loaded`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext._file_class_methods_loaded), [`_file_class_methods`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext._file_class_methods), [`_file_symbols`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext._file_symbols), [`cache`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext.cache), [`_builtins`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext._builtins), [`_callee_resolver`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext._callee_resolver), [`_global_name_table`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext._global_name_table), [`_import_alias_target`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext._import_alias_target), [`_imports_by_file`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext._imports_by_file), [`_name_to_source`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext._name_to_source), [`_stdlib_modules`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext._stdlib_modules), [`project_root`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext.project_root)  (2 test-only)

### `TestResolverContextProperties`
- def: [`tests/unit/synapse_resolver/test_context.py:119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L119)
- doc: Properties return the pre-built maps directly.
- signature: `class TestResolverContextProperties:`
- members:
  - `test_builtins_property(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L157)
  - `test_callee_resolver_property_none(self)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L167)
  - `test_callee_resolver_property_set(self)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L171)
  - `test_file_class_methods_property(self)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L130)
  - `test_file_symbols_property(self)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L122)
  - `test_global_name_table_property(self)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L134)
  - `test_import_alias_target_property(self)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L138)
  - `test_imports_by_file_property(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L142)
  - `test_name_to_source_property(self)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L126)
  - `test_stdlib_modules_property(self)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L162)
- uses (calls/refs, reference-scoped): [`local_name`](../../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry.local_name), [`ImportEntry`](../../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry), [`callee_resolver`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext.callee_resolver), [`module_path`](../../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry.module_path), [`file_class_methods`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext.file_class_methods), [`is_relative`](../../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry.is_relative), [`file_symbols`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext.file_symbols), [`file_path`](../../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry.file_path), [`imports_by_file`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext.imports_by_file), [`language`](../../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry.language), [`builtins`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext.builtins), [`import_alias_target`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext.import_alias_target), [`name_to_source`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext.name_to_source), [`stdlib_modules`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext.stdlib_modules), [`global_name_table`](../../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext.global_name_table)  (1 test-only)

## Functions
- `_make_cache(project_root: str = "/repo", db_path: str = "")` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L27) — Return a minimal ASTCache mock.
- `_prebuilt_ctx(**kwargs)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_context.py#L35) — Build a ResolverContext with all maps pre-supplied (no DB needed).

