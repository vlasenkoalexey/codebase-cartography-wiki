---
title: 'Module: tests/unit/mcp/test_utils/test_file_output_factory.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_utils/test_file_output_factory.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_utils.test_file_output_factory`/
symbols:
  TestFileOutputManagerFactoryUpdateProjectRoot.test_update_project_root_success: TestFileOutputManagerFactoryUpdateProjectRoot#test_update_project_root_success().
  TestFileOutputManagerFactoryClearAllInstances.test_clear_all_instances_with_instances: TestFileOutputManagerFactoryClearAllInstances#test_clear_all_instances_with_instances().
  TestFileOutputManagerFactoryUpdateProjectRoot.test_update_project_root_updates_instance: TestFileOutputManagerFactoryUpdateProjectRoot#test_update_project_root_updates_instance().
  TestFileOutputManagerFactoryIntegration.test_factory_clear_all_and_recreate: TestFileOutputManagerFactoryIntegration#test_factory_clear_all_and_recreate().
  TestFileOutputManagerFactoryGetInstance.test_get_instance_creates_new_instance: TestFileOutputManagerFactoryGetInstance#test_get_instance_creates_new_instance().
  TestFileOutputManagerFactoryGetInstance.test_get_instance_with_none_project_root: TestFileOutputManagerFactoryGetInstance#test_get_instance_with_none_project_root().
  TestFileOutputManagerFactoryGetInstance.test_get_instance_normalizes_path: TestFileOutputManagerFactoryGetInstance#test_get_instance_normalizes_path().
  TestFileOutputManagerFactoryClearInstance.test_clear_instance_existing: TestFileOutputManagerFactoryClearInstance#test_clear_instance_existing().
  TestFileOutputManagerFactoryClearInstance.test_clear_instance_with_none: TestFileOutputManagerFactoryClearInstance#test_clear_instance_with_none().
  TestFileOutputManagerFactoryClearInstance.test_clear_instance_normalizes_path: TestFileOutputManagerFactoryClearInstance#test_clear_instance_normalizes_path().
  TestFileOutputManagerFactoryGetInstanceCount.test_get_instance_count_multiple: TestFileOutputManagerFactoryGetInstanceCount#test_get_instance_count_multiple().
  TestFileOutputManagerFactoryGetInstanceCount.test_get_instance_count_same_project_root: TestFileOutputManagerFactoryGetInstanceCount#test_get_instance_count_same_project_root().
  TestFileOutputManagerFactoryGetManagedProjectRoots.test_get_managed_project_roots_empty: TestFileOutputManagerFactoryGetManagedProjectRoots#test_get_managed_project_roots_empty().
  TestFileOutputManagerFactoryGetManagedProjectRoots.test_get_managed_project_roots_multiple: TestFileOutputManagerFactoryGetManagedProjectRoots#test_get_managed_project_roots_multiple().
  TestFileOutputManagerFactoryUpdateProjectRoot.test_update_project_root_same_path: TestFileOutputManagerFactoryUpdateProjectRoot#test_update_project_root_same_path().
  TestFileOutputManagerFactoryUpdateProjectRoot.test_update_project_root_normalizes_paths: TestFileOutputManagerFactoryUpdateProjectRoot#test_update_project_root_normalizes_paths().
  TestGetFileOutputManager.test_get_file_output_manager_with_path: TestGetFileOutputManager#test_get_file_output_manager_with_path().
  TestGetFileOutputManager.test_get_file_output_manager_uses_factory: TestGetFileOutputManager#test_get_file_output_manager_uses_factory().
  TestFileOutputManagerFactoryIntegration.test_factory_multiple_project_roots: TestFileOutputManagerFactoryIntegration#test_factory_multiple_project_roots().
  TestFileOutputManagerFactoryIntegration.test_factory_clear_and_recreate: TestFileOutputManagerFactoryIntegration#test_factory_clear_and_recreate().
  TestFileOutputManagerFactoryGetInstance.get_instance_thread: TestFileOutputManagerFactoryGetInstance#get_instance_thread().
  clear_factory_instances: clear_factory_instances().
  TestFileOutputManagerFactoryGetInstance.test_get_instance_returns_same_instance: TestFileOutputManagerFactoryGetInstance#test_get_instance_returns_same_instance().
  TestFileOutputManagerFactoryNormalizeProjectRoot.test_normalize_project_root_none: TestFileOutputManagerFactoryNormalizeProjectRoot#test_normalize_project_root_none().
  TestFileOutputManagerFactoryNormalizeProjectRoot.test_normalize_project_root_absolute_path: TestFileOutputManagerFactoryNormalizeProjectRoot#test_normalize_project_root_absolute_path().
  TestFileOutputManagerFactoryNormalizeProjectRoot.test_normalize_project_root_relative_path: TestFileOutputManagerFactoryNormalizeProjectRoot#test_normalize_project_root_relative_path().
  TestFileOutputManagerFactoryNormalizeProjectRoot.test_normalize_project_root_with_dots: TestFileOutputManagerFactoryNormalizeProjectRoot#test_normalize_project_root_with_dots().
  TestFileOutputManagerFactoryNormalizeProjectRoot.test_normalize_project_root_invalid_path: TestFileOutputManagerFactoryNormalizeProjectRoot#test_normalize_project_root_invalid_path().
  TestFileOutputManagerFactoryClearInstance.test_clear_instance_nonexistent: TestFileOutputManagerFactoryClearInstance#test_clear_instance_nonexistent().
  TestFileOutputManagerFactoryClearAllInstances.test_clear_all_instances_no_instances: TestFileOutputManagerFactoryClearAllInstances#test_clear_all_instances_no_instances().
  TestFileOutputManagerFactoryGetInstanceCount.test_get_instance_count_empty: TestFileOutputManagerFactoryGetInstanceCount#test_get_instance_count_empty().
  TestFileOutputManagerFactoryUpdateProjectRoot.test_update_project_root_nonexistent: TestFileOutputManagerFactoryUpdateProjectRoot#test_update_project_root_nonexistent().
  TestGetFileOutputManager.test_get_file_output_manager_with_none: TestGetFileOutputManager#test_get_file_output_manager_with_none().
  TestFileOutputManagerFactoryIntegration.test_factory_singleton_behavior: TestFileOutputManagerFactoryIntegration#test_factory_singleton_behavior().
  TestFileOutputManagerFactoryGetInstance.test_get_instance_thread_safety: TestFileOutputManagerFactoryGetInstance#test_get_instance_thread_safety().
  TestFileOutputManagerFactoryGetInstance: TestFileOutputManagerFactoryGetInstance#
  TestFileOutputManagerFactoryNormalizeProjectRoot: TestFileOutputManagerFactoryNormalizeProjectRoot#
  TestFileOutputManagerFactoryClearInstance: TestFileOutputManagerFactoryClearInstance#
  TestFileOutputManagerFactoryClearAllInstances: TestFileOutputManagerFactoryClearAllInstances#
  TestFileOutputManagerFactoryGetInstanceCount: TestFileOutputManagerFactoryGetInstanceCount#
  TestFileOutputManagerFactoryGetManagedProjectRoots: TestFileOutputManagerFactoryGetManagedProjectRoots#
  TestFileOutputManagerFactoryUpdateProjectRoot: TestFileOutputManagerFactoryUpdateProjectRoot#
  TestGetFileOutputManager: TestGetFileOutputManager#
  TestFileOutputManagerFactoryIntegration: TestFileOutputManagerFactoryIntegration#
---
# Module: [`tests/unit/mcp/test_utils/test_file_output_factory.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py)

## Classes
### `TestFileOutputManagerFactoryClearAllInstances`
- def: [`tests/unit/mcp/test_utils/test_file_output_factory.py:189`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L189)
- doc: Tests for clear_all_instances method.
- signature: `class TestFileOutputManagerFactoryClearAllInstances:`
- members:
  - `test_clear_all_instances_no_instances(self)` — [`L205`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L205) — Test clear_all_instances with no instances.
  - `test_clear_all_instances_with_instances(self)` — [`L192`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L192) — Test clear_all_instances removes all instances.
- uses (calls/refs, reference-scoped): [`FileOutputManagerFactory`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory), [`get_instance`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.get_instance), [`clear_all_instances`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.clear_all_instances), [`get_instance_count`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.get_instance_count)

### `TestFileOutputManagerFactoryClearInstance`
- def: [`tests/unit/mcp/test_utils/test_file_output_factory.py:144`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L144)
- doc: Tests for clear_instance method.
- signature: `class TestFileOutputManagerFactoryClearInstance:`
- members:
  - `test_clear_instance_existing(self)` — [`L147`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L147) — Test clear_instance removes existing instance.
  - `test_clear_instance_nonexistent(self)` — [`L160`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L160) — Test clear_instance with nonexistent instance.
  - `test_clear_instance_normalizes_path(self)` — [`L176`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L176) — Test clear_instance normalizes project root path.
  - `test_clear_instance_with_none(self)` — [`L166`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L166) — Test clear_instance with None clears default instance.
- uses (calls/refs, reference-scoped): [`FileOutputManagerFactory`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory), [`get_instance`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.get_instance), [`clear_instance`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.clear_instance)

### `TestFileOutputManagerFactoryGetInstance`
- def: [`tests/unit/mcp/test_utils/test_file_output_factory.py:27`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L27)
- doc: Tests for get_instance method.
- signature: `class TestFileOutputManagerFactoryGetInstance:`
- members:
  - `get_instance_thread()` — [`L75`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L75)
  - `test_get_instance_creates_new_instance(self)` — [`L30`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L30) — Test get_instance creates new instance for new project root.
  - `test_get_instance_normalizes_path(self)` — [`L59`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L59) — Test get_instance normalizes project root path.
  - `test_get_instance_returns_same_instance(self)` — [`L43`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L43) — Test get_instance returns same instance for same project root.
  - `test_get_instance_thread_safety(self)` — [`L68`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L68) — Test get_instance is thread-safe.
  - `test_get_instance_with_none_project_root(self)` — [`L50`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L50) — Test get_instance with None uses current working directory.
- uses (calls/refs, reference-scoped): [`FileOutputManagerFactory`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory), [`get_instance`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.get_instance), [`project_root`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.project_root)

### `TestFileOutputManagerFactoryGetInstanceCount`
- def: [`tests/unit/mcp/test_utils/test_file_output_factory.py:212`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L212)
- doc: Tests for get_instance_count method.
- signature: `class TestFileOutputManagerFactoryGetInstanceCount:`
- members:
  - `test_get_instance_count_empty(self)` — [`L215`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L215) — Test get_instance_count with no instances.
  - `test_get_instance_count_multiple(self)` — [`L221`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L221) — Test get_instance_count with multiple instances.
  - `test_get_instance_count_same_project_root(self)` — [`L231`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L231) — Test get_instance_count doesn't increase for same project root.
- uses (calls/refs, reference-scoped): [`FileOutputManagerFactory`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory), [`get_instance`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.get_instance), [`get_instance_count`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.get_instance_count)

### `TestFileOutputManagerFactoryGetManagedProjectRoots`
- def: [`tests/unit/mcp/test_utils/test_file_output_factory.py:242`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L242)
- doc: Tests for get_managed_project_roots method.
- signature: `class TestFileOutputManagerFactoryGetManagedProjectRoots:`
- members:
  - `test_get_managed_project_roots_empty(self)` — [`L245`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L245) — Test get_managed_project_roots with no instances.
  - `test_get_managed_project_roots_multiple(self)` — [`L254`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L254) — Test get_managed_project_roots with multiple instances.
- uses (calls/refs, reference-scoped): [`FileOutputManagerFactory`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory), [`get_instance`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.get_instance), [`clear_all_instances`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.clear_all_instances), [`get_managed_project_roots`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.get_managed_project_roots)

### `TestFileOutputManagerFactoryIntegration`
- def: [`tests/unit/mcp/test_utils/test_file_output_factory.py:371`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L371)
- doc: Integration tests for factory behavior.
- signature: `class TestFileOutputManagerFactoryIntegration:`
- members:
  - `test_factory_clear_all_and_recreate(self)` — [`L414`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L414) — Test factory can clear all and recreate instances.
  - `test_factory_clear_and_recreate(self)` — [`L400`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L400) — Test factory can clear and recreate instances.
  - `test_factory_multiple_project_roots(self)` — [`L385`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L385) — Test factory manages multiple project roots separately.
  - `test_factory_singleton_behavior(self)` — [`L374`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L374) — Test factory maintains singleton behavior across calls.
- uses (calls/refs, reference-scoped): [`FileOutputManagerFactory`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory), [`get_instance`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.get_instance), [`clear_all_instances`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.clear_all_instances), [`get_instance_count`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.get_instance_count), [`clear_instance`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.clear_instance)

### `TestFileOutputManagerFactoryNormalizeProjectRoot`
- def: [`tests/unit/mcp/test_utils/test_file_output_factory.py:95`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L95)
- doc: Tests for _normalize_project_root method.
- signature: `class TestFileOutputManagerFactoryNormalizeProjectRoot:`
- members:
  - `test_normalize_project_root_absolute_path(self)` — [`L107`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L107) — Test normalize_project_root with absolute path.
  - `test_normalize_project_root_invalid_path(self, monkeypatch)` — [`L127`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L127) — Test normalize_project_root with invalid path returns resolved path.
  - `test_normalize_project_root_none(self)` — [`L98`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L98) — Test normalize_project_root with None returns current directory.
  - `test_normalize_project_root_relative_path(self)` — [`L113`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L113) — Test normalize_project_root with relative path.
  - `test_normalize_project_root_with_dots(self)` — [`L119`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L119) — Test normalize_project_root resolves path with dots.
- uses (calls/refs, reference-scoped): [`FileOutputManagerFactory`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory), [`_normalize_project_root`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory._normalize_project_root)

### `TestFileOutputManagerFactoryUpdateProjectRoot`
- def: [`tests/unit/mcp/test_utils/test_file_output_factory.py:269`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L269)
- doc: Tests for update_project_root method.
- signature: `class TestFileOutputManagerFactoryUpdateProjectRoot:`
- members:
  - `test_update_project_root_nonexistent(self)` — [`L299`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L299) — Test update_project_root with nonexistent instance.
  - `test_update_project_root_normalizes_paths(self)` — [`L317`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L317) — Test update_project_root normalizes both paths.
  - `test_update_project_root_same_path(self)` — [`L307`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L307) — Test update_project_root with same path returns True.
  - `test_update_project_root_success(self)` — [`L272`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L272) — Test update_project_root successfully updates instance.
  - `test_update_project_root_updates_instance(self)` — [`L329`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L329) — Test update_project_root updates instance's internal project root.
- uses (calls/refs, reference-scoped): [`FileOutputManagerFactory`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory), [`get_instance`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.get_instance), [`project_root`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.project_root), [`update_project_root`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.update_project_root), [`_normalize_project_root`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory._normalize_project_root), [`get_managed_project_roots`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.get_managed_project_roots)

### `TestGetFileOutputManager`
- def: [`tests/unit/mcp/test_utils/test_file_output_factory.py:342`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L342)
- doc: Tests for get_file_output_manager convenience function.
- signature: `class TestGetFileOutputManager:`
- members:
  - `test_get_file_output_manager_uses_factory(self)` — [`L362`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L362) — Test get_file_output_manager uses factory.
  - `test_get_file_output_manager_with_none(self)` — [`L353`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L353) — Test get_file_output_manager with None.
  - `test_get_file_output_manager_with_path(self)` — [`L345`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L345) — Test get_file_output_manager with path.
- uses (calls/refs, reference-scoped): [`FileOutputManagerFactory`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory), [`get_instance`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.get_instance), [`project_root`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.project_root), [`get_file_output_manager`](../../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#get_file_output_manager)

## Functions
- `clear_factory_instances()` — [`L20`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_factory.py#L20) — Clear factory instances before and after each test.

