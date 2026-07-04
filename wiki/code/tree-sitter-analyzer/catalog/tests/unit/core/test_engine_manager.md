---
title: 'Module: tests/unit/core/test_engine_manager.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_engine_manager.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_engine_manager`/TestEngine
symbols:
  TestEngineManagerResetInstances.test_reset_instances_clears_all: ManagerResetInstances#test_reset_instances_clears_all().
  TestEngineManagerResetInstances.test_reset_instances_thread_safety: ManagerResetInstances#test_reset_instances_thread_safety().
  TestEngineManagerEdgeCases.test_reset_clears_all_project_roots: ManagerEdgeCases#test_reset_clears_all_project_roots().
  TestEngineSecurityRegression.test_unsupported_language_handling: SecurityRegression#test_unsupported_language_handling().
  TestEngineManagerResetInstances.reset_and_create: ManagerResetInstances#reset_and_create().
  TestEngineManagerGetInstance.test_get_instance_default_project_root: ManagerGetInstance#test_get_instance_default_project_root().
  TestEngineManagerGetInstance.test_get_instance_with_project_root: ManagerGetInstance#test_get_instance_with_project_root().
  TestEngineManagerGetInstance.test_get_instance_different_project_roots: ManagerGetInstance#test_get_instance_different_project_roots().
  TestEngineManagerGetInstance.test_get_instance_none_project_root: ManagerGetInstance#test_get_instance_none_project_root().
  TestEngineManagerEdgeCases.test_instance_key_generation: ManagerEdgeCases#test_instance_key_generation().
  TestEngineManagerEdgeCases.test_multiple_project_roots: ManagerEdgeCases#test_multiple_project_roots().
  TestEngineSecurityRegression.test_path_traversal_prevention: SecurityRegression#test_path_traversal_prevention().
  TestEngineManagerThreadSafety.create_instance: ManagerThreadSafety#create_instance().
  TestEngineManagerThreadSafety.test_concurrent_get_instance: ManagerThreadSafety#test_concurrent_get_instance().
  TestEngineManagerThreadSafety.test_double_checked_locking: ManagerThreadSafety#test_double_checked_locking().
  TestEngineSecurityRegression.test_singleton_engine_cleanup: SecurityRegression#test_singleton_engine_cleanup().
  TestEngineManagerGetInstance: ManagerGetInstance#
  TestEngineManagerGetInstance.__test__: ManagerGetInstance#__test__.
  TestEngineManagerThreadSafety: ManagerThreadSafety#
  TestEngineManagerThreadSafety.__test__: ManagerThreadSafety#__test__.
  TestEngineManagerResetInstances: ManagerResetInstances#
  TestEngineManagerResetInstances.__test__: ManagerResetInstances#__test__.
  TestEngineManagerEdgeCases: ManagerEdgeCases#
  TestEngineManagerEdgeCases.__test__: ManagerEdgeCases#__test__.
  TestEngineSecurityRegression: SecurityRegression#
  TestEngineSecurityRegression.__test__: SecurityRegression#__test__.
---
# Module: [`tests/unit/core/test_engine_manager.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py)

## Classes
### `TestEngineManagerEdgeCases`
- def: [`tests/unit/core/test_engine_manager.py:193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L193)
- doc: Test cases for edge cases.
- signature: `class TestEngineManagerEdgeCases:`
- members:
  - `test_instance_key_generation(self)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L198) — Test instance key generation for falsy project roots.
  - `test_multiple_project_roots(self)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L213) — Test managing multiple separate project roots.
  - `test_reset_clears_all_project_roots(self)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L237) — Test reset clears all project-root-scoped instances.
- protocol/private: `__test__`[`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L196)
- uses (calls/refs, reference-scoped): [`UnifiedAnalysisEngine`](../../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine), [`EngineManager`](../../../tree_sitter_analyzer/core/engine_manager.md#EngineManager), [`get_instance`](../../../tree_sitter_analyzer/core/engine_manager.md#EngineManager.get_instance), [`reset_instances`](../../../tree_sitter_analyzer/core/engine_manager.md#EngineManager.reset_instances), [`_instances`](../../../tree_sitter_analyzer/core/engine_manager.md#EngineManager._instances), [`_project_root`](../../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine._project_root)

### `TestEngineManagerGetInstance`
- def: [`tests/unit/core/test_engine_manager.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L18)
- doc: Test cases for get_instance method.
- signature: `class TestEngineManagerGetInstance:`
- members:
  - `test_get_instance_default_project_root(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L23) — Test get_instance with default project root.
  - `test_get_instance_different_project_roots(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L49) — Test get_instance with different project roots.
  - `test_get_instance_none_project_root(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L64) — Test get_instance with None project root.
  - `test_get_instance_with_project_root(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L34) — Test get_instance with specific project root.
- protocol/private: `__test__`[`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L21)
- uses (calls/refs, reference-scoped): [`UnifiedAnalysisEngine`](../../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine), [`EngineManager`](../../../tree_sitter_analyzer/core/engine_manager.md#EngineManager), [`get_instance`](../../../tree_sitter_analyzer/core/engine_manager.md#EngineManager.get_instance), [`reset_instances`](../../../tree_sitter_analyzer/core/engine_manager.md#EngineManager.reset_instances)

### `TestEngineManagerResetInstances`
- def: [`tests/unit/core/test_engine_manager.py:123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L123)
- doc: Test cases for reset_instances method.
- signature: `class TestEngineManagerResetInstances:`
- members:
  - `reset_and_create()` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L171)
  - `test_reset_instances_clears_all(self)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L128) — Test that reset_instances clears all instances.
  - `test_reset_instances_thread_safety(self)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L164) — Test that reset_instances remains safe under concurrent access.
- protocol/private: `__test__`[`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L126)
- uses (calls/refs, reference-scoped): [`UnifiedAnalysisEngine`](../../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine), [`EngineManager`](../../../tree_sitter_analyzer/core/engine_manager.md#EngineManager), [`get_instance`](../../../tree_sitter_analyzer/core/engine_manager.md#EngineManager.get_instance), [`reset_instances`](../../../tree_sitter_analyzer/core/engine_manager.md#EngineManager.reset_instances), [`_instances`](../../../tree_sitter_analyzer/core/engine_manager.md#EngineManager._instances), [`_project_root`](../../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine._project_root)

### `TestEngineManagerThreadSafety`
- def: [`tests/unit/core/test_engine_manager.py:75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L75)
- doc: Test cases for thread safety.
- signature: `class TestEngineManagerThreadSafety:`
- members:
  - `create_instance()` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L86)
  - `test_concurrent_get_instance(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L80) — Test concurrent calls to get_instance.
  - `test_double_checked_locking(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L102) — Test concurrent access does not create duplicate instances.
- protocol/private: `__test__`[`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L78)
- uses (calls/refs, reference-scoped): [`UnifiedAnalysisEngine`](../../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine), [`EngineManager`](../../../tree_sitter_analyzer/core/engine_manager.md#EngineManager), [`get_instance`](../../../tree_sitter_analyzer/core/engine_manager.md#EngineManager.get_instance), [`reset_instances`](../../../tree_sitter_analyzer/core/engine_manager.md#EngineManager.reset_instances)

### `TestEngineSecurityRegression`
- def: [`tests/unit/core/test_engine_manager.py:279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L279)
- doc: Regression tests for security boundaries
- signature: `class TestEngineSecurityRegression:`
- members:
  - `test_path_traversal_prevention(self)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L285) — Path traversal attempts should still be blocked.
  - `test_singleton_engine_cleanup(self)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L305) — Cleanup should remain safe after refactoring.
  - `test_unsupported_language_handling(self)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L297) — Unsupported languages should still surface the expected error.
- protocol/private: `__test__`[`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_engine_manager.py#L282)
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`language`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.language), [`get_analysis_engine`](../../../tree_sitter_analyzer/core/analysis_engine.md#get_analysis_engine), [`analyze`](../../../tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.md#UnifiedAnalysisEngineAnalysisMixin.analyze), [`UnsupportedLanguageError`](../../../tree_sitter_analyzer/core/_analysis_engine_errors.md#UnsupportedLanguageError), [`cleanup`](../../../tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.md#UnifiedAnalysisEngineRuntimeMixin.cleanup)

