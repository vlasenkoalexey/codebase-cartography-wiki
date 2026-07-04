---
title: 'Module: tests/unit/core/test_file_output_manager_factory.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_file_output_manager_factory.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_file_output_manager_factory`/
symbols:
  TestFileOutputManagerFactory.test_update_project_root: TestFileOutputManagerFactory#test_update_project_root().
  TestFileOutputManagerBackwardCompatibility.test_existing_methods_unchanged: TestFileOutputManagerBackwardCompatibility#test_existing_methods_unchanged().
  MockMCPTool.file_output_manager: MockMCPTool#file_output_manager.
  TestFileOutputManagerFactory.test_clear_instance: TestFileOutputManagerFactory#test_clear_instance().
  TestFileOutputManagerFactory.test_clear_all_instances: TestFileOutputManagerFactory#test_clear_all_instances().
  TestFileOutputManagerFactoryThreadSafety.get_instance: TestFileOutputManagerFactoryThreadSafety#get_instance().
  TestFileOutputManagerBackwardCompatibility.test_direct_instantiation_still_works: TestFileOutputManagerBackwardCompatibility#test_direct_instantiation_still_works().
  TestFileOutputManagerBackwardCompatibility.test_none_project_root_still_works: TestFileOutputManagerBackwardCompatibility#test_none_project_root_still_works().
  TestFileOutputManagerBackwardCompatibility.test_set_project_root_method: TestFileOutputManagerBackwardCompatibility#test_set_project_root_method().
  TestFileOutputManagerFactory.test_get_managed_project_roots: TestFileOutputManagerFactory#test_get_managed_project_roots().
  TestFileOutputManagerClassMethods.test_get_managed_instance: TestFileOutputManagerClassMethods#test_get_managed_instance().
  TestFileOutputManagerClassMethods.test_create_instance: TestFileOutputManagerClassMethods#test_create_instance().
  TestFileOutputManagerClassMethods.test_get_managed_instance_fallback: TestFileOutputManagerClassMethods#test_get_managed_instance_fallback().
  TestConvenienceFunction.test_get_file_output_manager_function: TestConvenienceFunction#test_get_file_output_manager_function().
  TestIntegrationWithExistingCode.test_new_mcp_tool_pattern_with_factory: TestIntegrationWithExistingCode#test_new_mcp_tool_pattern_with_factory().
  TestFileOutputManagerFactory.setup_method: TestFileOutputManagerFactory#setup_method().
  TestFileOutputManagerFactory.teardown_method: TestFileOutputManagerFactory#teardown_method().
  TestFileOutputManagerFactory.test_singleton_behavior_per_project_root: TestFileOutputManagerFactory#test_singleton_behavior_per_project_root().
  TestFileOutputManagerFactory.test_none_project_root_normalization: TestFileOutputManagerFactory#test_none_project_root_normalization().
  TestFileOutputManagerFactory.test_path_normalization: TestFileOutputManagerFactory#test_path_normalization().
  TestFileOutputManagerFactoryThreadSafety.setup_method: TestFileOutputManagerFactoryThreadSafety#setup_method().
  TestFileOutputManagerFactoryThreadSafety.teardown_method: TestFileOutputManagerFactoryThreadSafety#teardown_method().
  TestFileOutputManagerClassMethods.setup_method: TestFileOutputManagerClassMethods#setup_method().
  TestFileOutputManagerClassMethods.teardown_method: TestFileOutputManagerClassMethods#teardown_method().
  TestConvenienceFunction.setup_method: TestConvenienceFunction#setup_method().
  TestConvenienceFunction.teardown_method: TestConvenienceFunction#teardown_method().
  TestIntegrationWithExistingCode.setup_method: TestIntegrationWithExistingCode#setup_method().
  TestIntegrationWithExistingCode.teardown_method: TestIntegrationWithExistingCode#teardown_method().
  TestIntegrationWithExistingCode.test_new_mcp_tool_pattern_with_factory.NewMCPTool.__init__: TestIntegrationWithExistingCode#test_new_mcp_tool_pattern_with_factory().NewMCPTool#__init__().
  NewMCPTool.file_output_manager: NewMCPTool#file_output_manager.
  TestFileOutputManagerFactoryThreadSafety.test_concurrent_access_same_project_root: TestFileOutputManagerFactoryThreadSafety#test_concurrent_access_same_project_root().
  TestFileOutputManagerFactoryThreadSafety.test_concurrent_access_different_project_roots: TestFileOutputManagerFactoryThreadSafety#test_concurrent_access_different_project_roots().
  TestIntegrationWithExistingCode.test_existing_mcp_tool_pattern.MockMCPTool.__init__: TestIntegrationWithExistingCode#test_existing_mcp_tool_pattern().MockMCPTool#__init__().
  TestIntegrationWithExistingCode.test_existing_mcp_tool_pattern.MockMCPTool: TestIntegrationWithExistingCode#test_existing_mcp_tool_pattern().MockMCPTool#
  TestIntegrationWithExistingCode.test_new_mcp_tool_pattern_with_factory.NewMCPTool: TestIntegrationWithExistingCode#test_new_mcp_tool_pattern_with_factory().NewMCPTool#
  TestFileOutputManagerBackwardCompatibility: TestFileOutputManagerBackwardCompatibility#
  TestFileOutputManagerFactory: TestFileOutputManagerFactory#
  TestFileOutputManagerFactoryThreadSafety: TestFileOutputManagerFactoryThreadSafety#
  TestFileOutputManagerClassMethods: TestFileOutputManagerClassMethods#
  TestConvenienceFunction: TestConvenienceFunction#
  TestIntegrationWithExistingCode: TestIntegrationWithExistingCode#
  TestIntegrationWithExistingCode.test_existing_mcp_tool_pattern: TestIntegrationWithExistingCode#test_existing_mcp_tool_pattern().
  MockMCPTool.project_root: MockMCPTool#project_root.
  NewMCPTool.project_root: NewMCPTool#project_root.
---
# Module: [`tests/unit/core/test_file_output_manager_factory.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py)

## Classes
### `MockMCPTool`
- def: [`tests/unit/core/test_file_output_manager_factory.py:374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L374)
- signature: `class MockMCPTool:`
- members:
  - `file_output_manager` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L377)
  - `project_root` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L376)
- protocol/private: `__init__`[`L375`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L375)
- uses (calls/refs, reference-scoped): [`FileOutputManager`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager), [`project_root`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.project_root)

### `NewMCPTool`
- def: [`tests/unit/core/test_file_output_manager_factory.py:394`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L394)
- signature: `class NewMCPTool:`
- members:
  - `file_output_manager` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L397)
  - `project_root` — [`L396`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L396)
- protocol/private: `__init__`[`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L395)
- uses (calls/refs, reference-scoped): [`FileOutputManager`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager), [`get_managed_instance`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.get_managed_instance)
- used by: (1 test-only callers)

### `TestConvenienceFunction`
- def: [`tests/unit/core/test_file_output_manager_factory.py:336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L336)
- doc: Test convenience function.
- signature: `class TestConvenienceFunction:`
- members:
  - `setup_method(self)` — [`L339`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L339) — Clear factory instances before each test.
  - `teardown_method(self)` — [`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L343) — Clear factory instances after each test.
  - `test_get_file_output_manager_function(self)` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L347) — Test get_file_output_manager convenience function.
- uses (calls/refs, reference-scoped): [`FileOutputManagerFactory`](../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory), [`get_instance`](../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.get_instance), [`clear_all_instances`](../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.clear_all_instances), [`get_file_output_manager`](../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#get_file_output_manager)

### `TestFileOutputManagerBackwardCompatibility`
- def: [`tests/unit/core/test_file_output_manager_factory.py:23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L23)
- doc: Test backward compatibility of FileOutputManager.
- signature: `class TestFileOutputManagerBackwardCompatibility:`
- members:
  - `test_direct_instantiation_still_works(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L26) — Test that direct instantiation of FileOutputManager still works.
  - `test_existing_methods_unchanged(self)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L41) — Test that all existing methods work unchanged.
  - `test_none_project_root_still_works(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L34) — Test that None project_root still works as before.
  - `test_set_project_root_method(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L68) — Test that set_project_root method works as before.
- uses (calls/refs, reference-scoped): [`FileOutputManager`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager), [`project_root`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.project_root), [`detect_content_type`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.detect_content_type), [`save_to_file`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.save_to_file), [`get_output_path`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.get_output_path), [`generate_output_filename`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.generate_output_filename), [`get_file_extension`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.get_file_extension), [`set_project_root`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.set_project_root)

### `TestFileOutputManagerClassMethods`
- def: [`tests/unit/core/test_file_output_manager_factory.py:287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L287)
- doc: Test new class methods in FileOutputManager.
- signature: `class TestFileOutputManagerClassMethods:`
- members:
  - `setup_method(self)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L290) — Clear factory instances before each test.
  - `teardown_method(self)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L294) — Clear factory instances after each test.
  - `test_create_instance(self)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L308) — Test create_instance class method.
  - `test_get_managed_instance(self)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L298) — Test get_managed_instance class method.
  - `test_get_managed_instance_fallback(self)` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L321) — Test get_managed_instance fallback when factory not available.
- uses (calls/refs, reference-scoped): [`FileOutputManagerFactory`](../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory), [`FileOutputManager`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager), [`project_root`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.project_root), [`clear_all_instances`](../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.clear_all_instances), [`get_managed_instance`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.get_managed_instance), [`_instances`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager._instances), [`create_instance`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.create_instance)

### `TestFileOutputManagerFactory`
- def: [`tests/unit/core/test_file_output_manager_factory.py:79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L79)
- doc: Test FileOutputManagerFactory functionality.
- signature: `class TestFileOutputManagerFactory:`
- members:
  - `setup_method(self)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L82) — Clear factory instances before each test.
  - `teardown_method(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L86) — Clear factory instances after each test.
  - `test_clear_all_instances(self)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L135) — Test clearing all instances.
  - `test_clear_instance(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L120) — Test clearing specific instances.
  - `test_get_managed_project_roots(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L147) — Test getting list of managed project roots.
  - `test_none_project_root_normalization(self)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L104) — Test that None project root is normalized consistently.
  - `test_path_normalization(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L110) — Test that different path representations are normalized.
  - `test_singleton_behavior_per_project_root(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L90) — Test that factory returns same instance for same project root.
  - `test_update_project_root(self)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L159) — Test updating project root for existing instance.
- uses (calls/refs, reference-scoped): [`FileOutputManagerFactory`](../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory), [`get_instance`](../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.get_instance), [`project_root`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.project_root), [`clear_all_instances`](../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.clear_all_instances), [`get_instance_count`](../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.get_instance_count), [`update_project_root`](../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.update_project_root), [`clear_instance`](../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.clear_instance), [`get_managed_project_roots`](../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.get_managed_project_roots)

### `TestFileOutputManagerFactoryThreadSafety`
- def: [`tests/unit/core/test_file_output_manager_factory.py:185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L185)
- doc: Test thread safety of FileOutputManagerFactory.
- signature: `class TestFileOutputManagerFactoryThreadSafety:`
- members:
  - `get_instance()` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L202)
  - `setup_method(self)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L188) — Clear factory instances before each test.
  - `teardown_method(self)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L192) — Clear factory instances after each test.
  - `test_concurrent_access_different_project_roots(self)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L232) — Test concurrent access to different project roots.
  - `test_concurrent_access_same_project_root(self)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L196) — Test concurrent access to same project root returns same instance.
- uses (calls/refs, reference-scoped): [`FileOutputManagerFactory`](../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory), [`get_instance`](../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.get_instance), [`clear_all_instances`](../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.clear_all_instances)

### `TestIntegrationWithExistingCode`
- def: [`tests/unit/core/test_file_output_manager_factory.py:359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L359)
- doc: Test integration with existing MCP tool patterns.
- signature: `class TestIntegrationWithExistingCode:`
- members:
  - `setup_method(self)` — [`L362`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L362) — Clear factory instances before each test.
  - `teardown_method(self)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L366) — Clear factory instances after each test.
  - `test_existing_mcp_tool_pattern(self)` — [`L370`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L370) — Test that existing MCP tool initialization pattern still works.
  - `test_new_mcp_tool_pattern_with_factory(self)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_manager_factory.py#L390) — Test new MCP tool pattern using factory.
- uses (calls/refs, reference-scoped): [`FileOutputManagerFactory`](../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory), [`project_root`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.project_root), [`clear_all_instances`](../../../tree_sitter_analyzer/mcp/utils/file_output_factory.md#FileOutputManagerFactory.clear_all_instances)  (2 test-only)

