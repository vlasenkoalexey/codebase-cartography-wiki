---
title: 'Module: tests/integration/test_ast_cache_lifecycle.py'
type: catalog
provenance: extracted
module: tests/integration/test_ast_cache_lifecycle.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.test_ast_cache_lifecycle`/
symbols:
  TestASTCacheLifecycle.test_invalidate_removes_entry: TestASTCacheLifecycle#test_invalidate_removes_entry().
  TestASTCacheLifecycle.test_index_and_retrieve: TestASTCacheLifecycle#test_index_and_retrieve().
  TestASTCacheLifecycle.test_cache_miss_empty_project: TestASTCacheLifecycle#test_cache_miss_empty_project().
  TestASTCacheLifecycle.test_double_index_replaces_entry: TestASTCacheLifecycle#test_double_index_replaces_entry().
  TestASTCacheLifecycle.test_stats_reflect_indexed_files: TestASTCacheLifecycle#test_stats_reflect_indexed_files().
  cache: cache().
  project: project().
  TestASTCacheLifecycle: TestASTCacheLifecycle#
---
# Module: [`tests/integration/test_ast_cache_lifecycle.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_ast_cache_lifecycle.py)

## Classes
### `TestASTCacheLifecycle`
- def: [`tests/integration/test_ast_cache_lifecycle.py:33`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_ast_cache_lifecycle.py#L33)
- signature: `class TestASTCacheLifecycle:`
- members:
  - `test_cache_miss_empty_project(self, tmp_path: Path)` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_ast_cache_lifecycle.py#L42) — get_functions() on an empty cache returns an empty list.
  - `test_double_index_replaces_entry(self, cache: ASTCache, project: Path)` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_ast_cache_lifecycle.py#L59) — Re-indexing an updated file replaces the cached version.
  - `test_index_and_retrieve(self, cache: ASTCache, project: Path)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_ast_cache_lifecycle.py#L34) — Indexing a file makes it visible via get_functions().
  - `test_invalidate_removes_entry(self, cache: ASTCache, project: Path)` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_ast_cache_lifecycle.py#L50) — Invalidating a file removes it from the index.
  - `test_stats_reflect_indexed_files(self, cache: ASTCache, project: Path)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_ast_cache_lifecycle.py#L68) — get_stats() shows at least one file after indexing.
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_file`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_file), [`get_stats`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.get_stats), [`invalidate`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.invalidate), [`get_functions`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.get_functions)

## Functions
- `cache(project: Path)` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_ast_cache_lifecycle.py#L27)
- `project(tmp_path: Path)` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_ast_cache_lifecycle.py#L14) — A tiny project with one Python file.

