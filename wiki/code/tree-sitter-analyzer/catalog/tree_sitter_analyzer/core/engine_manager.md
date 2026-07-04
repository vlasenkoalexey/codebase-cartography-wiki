---
title: 'Module: tree_sitter_analyzer/core/engine_manager.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/core/engine_manager.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.core.engine_manager`/EngineManager#
symbols:
  EngineManager: ''
  EngineManager.get_instance: get_instance().
  EngineManager.reset_instances: reset_instances().
  EngineManager._instances: _instances.
  EngineManager._lock: _lock.
---
# Module: [`tree_sitter_analyzer/core/engine_manager.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/engine_manager.py)

## Classes
### `EngineManager`
- def: [`tree_sitter_analyzer/core/engine_manager.py:13`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/engine_manager.py#L13)
- doc: Manages UnifiedAnalysisEngine singleton instances
- signature: `class EngineManager:`
- members:
  - `get_instance(cls, engine_class: type[UnifiedAnalysisEngine], project_root: str | None = None)` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/engine_manager.py#L20) — Get or create singleton instance of the analysis engine
  - `reset_instances(cls)` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/engine_manager.py#L41) — Reset all singleton instances (for testing)
- protocol/private: `_instances`[`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/engine_manager.py#L16), `_lock`[`L17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/engine_manager.py#L17)
- uses (calls/refs, reference-scoped): [`UnifiedAnalysisEngine`](analysis_engine.md#UnifiedAnalysisEngine)
- used by: [`_reset_instance`](_analysis_engine_runtime_mixin.md#UnifiedAnalysisEngineRuntimeMixin._reset_instance)  (16 test-only)

