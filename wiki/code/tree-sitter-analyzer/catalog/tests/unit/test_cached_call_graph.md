---
title: 'Module: tests/unit/test_cached_call_graph.py'
type: catalog
provenance: extracted
module: tests/unit/test_cached_call_graph.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_cached_call_graph`/
symbols:
  TestCachedCallGraphBuild.test_empty_cache_falls_back: TestCachedCallGraphBuild#test_empty_cache_falls_back().
  TestCachedCallGraphBuild.test_build_from_cache: TestCachedCallGraphBuild#test_build_from_cache().
  TestCachedCallGraphBuild.test_build_fallback_when_no_cache: TestCachedCallGraphBuild#test_build_fallback_when_no_cache().
  TestCachedCallGraphBuild.test_build_no_fallback_no_cache: TestCachedCallGraphBuild#test_build_no_fallback_no_cache().
  TestCachedVsFreshParity.test_same_callers: TestCachedVsFreshParity#test_same_callers().
  TestCachedVsFreshParity.test_same_callees: TestCachedVsFreshParity#test_same_callees().
  TestCachedVsFreshParity.test_same_function_count: TestCachedVsFreshParity#test_same_function_count().
  TestASTCacheCallEdgeStorage.test_js_call_edges: TestASTCacheCallEdgeStorage#test_js_call_edges().
  cached_index: cached_index().
  TestCachedCallGraphQueries.test_callers_of: TestCachedCallGraphQueries#test_callers_of().
  TestCachedCallGraphQueries.test_callees_of: TestCachedCallGraphQueries#test_callees_of().
  TestCachedCallGraphQueries.test_callers_of_leaf: TestCachedCallGraphQueries#test_callers_of_leaf().
  TestCachedCallGraphQueries.test_callees_of_leaf: TestCachedCallGraphQueries#test_callees_of_leaf().
  TestCachedCallGraphQueries.test_all_functions: TestCachedCallGraphQueries#test_all_functions().
  TestCachedCallGraphQueries.test_summary: TestCachedCallGraphQueries#test_summary().
  project_with_calls: project_with_calls().
  TestCachedCallGraphBuild: TestCachedCallGraphBuild#
  TestCachedCallGraphQueries: TestCachedCallGraphQueries#
  TestCachedVsFreshParity: TestCachedVsFreshParity#
  TestASTCacheCallEdgeStorage: TestASTCacheCallEdgeStorage#
  TestASTCacheCallEdgeStorage.test_call_edges_stored: TestASTCacheCallEdgeStorage#test_call_edges_stored().
  TestASTCacheCallEdgeStorage.test_functions_stored: TestASTCacheCallEdgeStorage#test_functions_stored().
  TestASTCacheCallEdgeStorage.test_invalidate_clears_edges: TestASTCacheCallEdgeStorage#test_invalidate_clears_edges().
---
# Module: [`tests/unit/test_cached_call_graph.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py)

## Classes
### `TestASTCacheCallEdgeStorage`
- def: [`tests/unit/test_cached_call_graph.py:131`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L131)
- signature: `class TestASTCacheCallEdgeStorage:`
- members:
  - `test_call_edges_stored(self, project_with_calls, cached_index)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L132)
  - `test_functions_stored(self, project_with_calls, cached_index)` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L140)
  - `test_invalidate_clears_edges(self, project_with_calls, cached_index)` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L145)
  - `test_js_call_edges(self, tmp_path)` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L151)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`index_file`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_file), [`get_call_edges`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.get_call_edges)

### `TestCachedCallGraphBuild`
- def: [`tests/unit/test_cached_call_graph.py:39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L39)
- signature: `class TestCachedCallGraphBuild:`
- members:
  - `test_build_fallback_when_no_cache(self, project_with_calls)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L46)
  - `test_build_from_cache(self, project_with_calls, cached_index)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L40)
  - `test_build_no_fallback_no_cache(self, project_with_calls)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L52)
  - `test_empty_cache_falls_back(self, project_with_calls)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L57)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`CachedCallGraph`](../../tree_sitter_analyzer/call_graph.md#CachedCallGraph), [`build`](../../tree_sitter_analyzer/call_graph.md#CachedCallGraph.build), [`summary`](../../tree_sitter_analyzer/call_graph.md#CallGraph.summary), [`_built`](../../tree_sitter_analyzer/call_graph.md#CachedCallGraph._built)

### `TestCachedCallGraphQueries`
- def: [`tests/unit/test_cached_call_graph.py:67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L67)
- signature: `class TestCachedCallGraphQueries:`
- members:
  - `test_all_functions(self, project_with_calls, cached_index)` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L92)
  - `test_callees_of(self, project_with_calls, cached_index)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L74)
  - `test_callees_of_leaf(self, project_with_calls, cached_index)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L87)
  - `test_callers_of(self, project_with_calls, cached_index)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L68)
  - `test_callers_of_leaf(self, project_with_calls, cached_index)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L81)
  - `test_summary(self, project_with_calls, cached_index)` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L98)
- uses (calls/refs, reference-scoped): [`CachedCallGraph`](../../tree_sitter_analyzer/call_graph.md#CachedCallGraph), [`callees_of`](../../tree_sitter_analyzer/call_graph.md#CallGraph.callees_of), [`callers_of`](../../tree_sitter_analyzer/call_graph.md#CallGraph.callers_of), [`all_functions`](../../tree_sitter_analyzer/call_graph.md#CallGraph.all_functions), [`summary`](../../tree_sitter_analyzer/call_graph.md#CallGraph.summary)

### `TestCachedVsFreshParity`
- def: [`tests/unit/test_cached_call_graph.py:106`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L106)
- signature: `class TestCachedVsFreshParity:`
- members:
  - `test_same_callees(self, project_with_calls, cached_index)` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L116)
  - `test_same_callers(self, project_with_calls, cached_index)` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L107)
  - `test_same_function_count(self, project_with_calls, cached_index)` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L125)
- uses (calls/refs, reference-scoped): [`CallGraph`](../../tree_sitter_analyzer/call_graph.md#CallGraph), [`CachedCallGraph`](../../tree_sitter_analyzer/call_graph.md#CachedCallGraph), [`callees_of`](../../tree_sitter_analyzer/call_graph.md#CallGraph.callees_of), [`callers_of`](../../tree_sitter_analyzer/call_graph.md#CallGraph.callers_of), [`summary`](../../tree_sitter_analyzer/call_graph.md#CallGraph.summary)

## Functions
- `cached_index(project_with_calls)` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L33)
- `project_with_calls(tmp_path)` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cached_call_graph.py#L13)

