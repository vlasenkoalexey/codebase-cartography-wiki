---
title: 'Module: tests/unit/test_cross_file_backfill.py'
type: catalog
provenance: extracted
module: tests/unit/test_cross_file_backfill.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_cross_file_backfill`/
symbols:
  multi_file_project: multi_file_project().
  TestBackfillCrossFileEdges.test_index_project_auto_backfill: TestBackfillCrossFileEdges#test_index_project_auto_backfill().
  TestCrossFileStats.test_stats_with_empty_cache: TestCrossFileStats#test_stats_with_empty_cache().
  TestBackfillCrossFileEdges: TestBackfillCrossFileEdges#
  TestBackfillCrossFileEdges.test_backfill_returns_stats: TestBackfillCrossFileEdges#test_backfill_returns_stats().
  TestBackfillCrossFileEdges.test_backfill_writes_resolved_file: TestBackfillCrossFileEdges#test_backfill_writes_resolved_file().
  TestBackfillCrossFileEdges.test_cross_file_stats_after_backfill: TestBackfillCrossFileEdges#test_cross_file_stats_after_backfill().
  TestBackfillCrossFileEdges.test_query_callers_uses_resolved_file: TestBackfillCrossFileEdges#test_query_callers_uses_resolved_file().
  TestBackfillCrossFileEdges.test_query_callees_uses_resolved_file: TestBackfillCrossFileEdges#test_query_callees_uses_resolved_file().
  TestCrossFileStats: TestCrossFileStats#
  TestCrossFileStats.test_stats_after_indexing: TestCrossFileStats#test_stats_after_indexing().
---
# Module: [`tests/unit/test_cross_file_backfill.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_backfill.py)

## Classes
### `TestBackfillCrossFileEdges`
- def: [`tests/unit/test_cross_file_backfill.py:63`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_backfill.py#L63)
- signature: `class TestBackfillCrossFileEdges:`
- members:
  - `test_backfill_returns_stats(self, multi_file_project)` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_backfill.py#L64)
  - `test_backfill_writes_resolved_file(self, multi_file_project)` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_backfill.py#L78)
  - `test_cross_file_stats_after_backfill(self, multi_file_project)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_backfill.py#L90)
  - `test_index_project_auto_backfill(self, tmp_path)` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_backfill.py#L117)
  - `test_query_callees_uses_resolved_file(self, multi_file_project)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_backfill.py#L109)
  - `test_query_callers_uses_resolved_file(self, multi_file_project)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_backfill.py#L100)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project)

### `TestCrossFileStats`
- def: [`tests/unit/test_cross_file_backfill.py:135`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_backfill.py#L135)
- signature: `class TestCrossFileStats:`
- members:
  - `test_stats_after_indexing(self, multi_file_project)` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_backfill.py#L145)
  - `test_stats_with_empty_cache(self, tmp_path)` — [`L136`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_backfill.py#L136)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`get_cross_file_stats`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.get_cross_file_stats)

## Functions
- `multi_file_project(tmp_path)` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_backfill.py#L10)

