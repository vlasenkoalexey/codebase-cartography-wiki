---
title: 'Module: tests/unit/mcp/test_graph_cache_invalidation.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_graph_cache_invalidation.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_graph_cache_invalidation`/
symbols:
  TestGraphFingerprint.test_changes_on_modify: TestGraphFingerprint#test_changes_on_modify().
  TestGraphFingerprint.test_handles_missing_root: TestGraphFingerprint#test_handles_missing_root().
  TestCallGraphCacheInvalidatesOnFileChange.test_call_graph_cache_invalidates_on_file_change: TestCallGraphCacheInvalidatesOnFileChange#test_call_graph_cache_invalidates_on_file_change().
  TestDependencyAnalysisCacheInvalidatesOnFileChange.test_dep_graph_cache_invalidates_on_file_change: TestDependencyAnalysisCacheInvalidatesOnFileChange#test_dep_graph_cache_invalidates_on_file_change().
  TestSymbolLineageCacheInvalidatesOnFileChange.test_symbol_lineage_cache_invalidates_on_file_change: TestSymbolLineageCacheInvalidatesOnFileChange#test_symbol_lineage_cache_invalidates_on_file_change().
  TestGraphFingerprint.test_changes_on_add_remove: TestGraphFingerprint#test_changes_on_add_remove().
  TestCallGraphCacheInvalidatesOnFileChange.test_call_graph_cache_age_reported: TestCallGraphCacheInvalidatesOnFileChange#test_call_graph_cache_age_reported().
  project_root: project_root().
  TestGraphFingerprint.test_idempotent_when_unchanged: TestGraphFingerprint#test_idempotent_when_unchanged().
  TestDependencyGraphGlobalCacheRespectsFingerprint.test_global_cache_invalidates_on_file_mtime: TestDependencyGraphGlobalCacheRespectsFingerprint#test_global_cache_invalidates_on_file_mtime().
  _make_small_python_project: _make_small_python_project().
  TestGraphFingerprint: TestGraphFingerprint#
  TestCallGraphCacheInvalidatesOnFileChange: TestCallGraphCacheInvalidatesOnFileChange#
  TestDependencyAnalysisCacheInvalidatesOnFileChange: TestDependencyAnalysisCacheInvalidatesOnFileChange#
  TestSymbolLineageCacheInvalidatesOnFileChange: TestSymbolLineageCacheInvalidatesOnFileChange#
  TestDependencyGraphGlobalCacheRespectsFingerprint: TestDependencyGraphGlobalCacheRespectsFingerprint#
---
# Module: [`tests/unit/mcp/test_graph_cache_invalidation.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_graph_cache_invalidation.py)

## Classes
### `TestCallGraphCacheInvalidatesOnFileChange`
- def: [`tests/unit/mcp/test_graph_cache_invalidation.py:96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_graph_cache_invalidation.py#L96)
- signature: `class TestCallGraphCacheInvalidatesOnFileChange:`
- members:
  - `test_call_graph_cache_age_reported(self, project_root: Path)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_graph_cache_invalidation.py#L125) — cache_age_s should be present and grow on warm reuse.
  - `test_call_graph_cache_invalidates_on_file_change(self, project_root: Path)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_graph_cache_invalidation.py#L97) — Cold build → warm reuse → mtime touch → rebuilt.
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/call_graph_tool.md#CodeGraphCallTool.execute), [`CodeGraphCallTool`](../../../tree_sitter_analyzer/mcp/tools/call_graph_tool.md#CodeGraphCallTool), [`get_call_graph`](../../../tree_sitter_analyzer/mcp/tools/call_graph_tool.md#CodeGraphCallTool.get_call_graph)

### `TestDependencyAnalysisCacheInvalidatesOnFileChange`
- def: [`tests/unit/mcp/test_graph_cache_invalidation.py:141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_graph_cache_invalidation.py#L141)
- signature: `class TestDependencyAnalysisCacheInvalidatesOnFileChange:`
- members:
  - `test_dep_graph_cache_invalidates_on_file_change(self, project_root: Path)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_graph_cache_invalidation.py#L142)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool.execute), [`DependencyAnalysisTool`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool), [`_graph`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool._graph)

### `TestDependencyGraphGlobalCacheRespectsFingerprint`
- def: [`tests/unit/mcp/test_graph_cache_invalidation.py:200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_graph_cache_invalidation.py#L200)
- signature: `class TestDependencyGraphGlobalCacheRespectsFingerprint:`
- members:
  - `test_global_cache_invalidates_on_file_mtime(self, project_root: Path)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_graph_cache_invalidation.py#L201)
- uses (calls/refs, reference-scoped): [`DependencyGraph`](../../../tree_sitter_analyzer/project_graph.md#DependencyGraph)

### `TestGraphFingerprint`
- def: [`tests/unit/mcp/test_graph_cache_invalidation.py:56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_graph_cache_invalidation.py#L56)
- signature: `class TestGraphFingerprint:`
- members:
  - `test_changes_on_add_remove(self, project_root: Path)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_graph_cache_invalidation.py#L67) — Adding a file must bump file_count.
  - `test_changes_on_modify(self, project_root: Path)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_graph_cache_invalidation.py#L57) — Touching a file's mtime must change the fingerprint.
  - `test_handles_missing_root(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_graph_cache_invalidation.py#L84) — Scan over a non-existent root must not raise.
  - `test_idempotent_when_unchanged(self, project_root: Path)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_graph_cache_invalidation.py#L78) — Calling twice without edits returns the same fingerprint.
- uses (calls/refs, reference-scoped): [`compute_graph_fingerprint`](../../../tree_sitter_analyzer/_graph_cache_fingerprint.md#compute_graph_fingerprint), [`file_count`](../../../tree_sitter_analyzer/_graph_cache_fingerprint.md#GraphFingerprint.file_count), [`GraphFingerprint`](../../../tree_sitter_analyzer/_graph_cache_fingerprint.md#GraphFingerprint), [`max_mtime_ns`](../../../tree_sitter_analyzer/_graph_cache_fingerprint.md#GraphFingerprint.max_mtime_ns), [`is_empty`](../../../tree_sitter_analyzer/_graph_cache_fingerprint.md#GraphFingerprint.is_empty)

### `TestSymbolLineageCacheInvalidatesOnFileChange`
- def: [`tests/unit/mcp/test_graph_cache_invalidation.py:168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_graph_cache_invalidation.py#L168)
- signature: `class TestSymbolLineageCacheInvalidatesOnFileChange:`
- members:
  - `test_symbol_lineage_cache_invalidates_on_file_change(self, project_root: Path)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_graph_cache_invalidation.py#L169)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.md#SymbolLineageTool.execute), [`SymbolLineageTool`](../../../tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.md#SymbolLineageTool), [`_dep_graph`](../../../tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.md#SymbolLineageTool._dep_graph)

## Functions
- `_make_small_python_project(root: Path)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_graph_cache_invalidation.py#L32) — Create a tiny but real python project so the graphs have content.
- `project_root()` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_graph_cache_invalidation.py#L44)

