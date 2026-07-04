---
title: 'Module: tests/unit/mcp/test_numeric_param_coercion.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_numeric_param_coercion.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_numeric_param_coercion`/Test
symbols:
  TestAstCacheIndexMaxFilesCoercion.test_mode_index_max_files_string_does_not_crash: AstCacheIndexMaxFilesCoercion#test_mode_index_max_files_string_does_not_crash().
  TestAstCacheSyncMaxFilesCoercion.test_mode_sync_max_files_string_does_not_crash: AstCacheSyncMaxFilesCoercion#test_mode_sync_max_files_string_does_not_crash().
  TestAstPathMaxDepthCoercion.test_mode_outline_max_depth_string_does_not_crash: AstPathMaxDepthCoercion#test_mode_outline_max_depth_string_does_not_crash().
  TestClassHierarchyMaxDepthCoercion.test_max_depth_string_does_not_crash: ClassHierarchyMaxDepthCoercion#test_max_depth_string_does_not_crash().
  TestCodegraphSitemapMaxFilesCoercion.test_max_files_string_does_not_crash: CodegraphSitemapMaxFilesCoercion#test_max_files_string_does_not_crash().
  TestDependencyMatrixTopKCoercion.test_top_k_string_does_not_crash: DependencyMatrixTopKCoercion#test_top_k_string_does_not_crash().
  TestFullIndexMaxFilesCoercion.test_max_files_string_does_not_crash: FullIndexMaxFilesCoercion#test_max_files_string_does_not_crash().
  TestImportGraphMaxDepthCoercion.test_blast_radius_max_depth_string_does_not_crash: ImportGraphMaxDepthCoercion#test_blast_radius_max_depth_string_does_not_crash().
  TestProjectOverviewMaxDepthCoercion.test_max_depth_string_does_not_crash: ProjectOverviewMaxDepthCoercion#test_max_depth_string_does_not_crash().
  TestTestGapMaxFilesMaxGapsCoercion.test_max_files_and_max_gaps_string_does_not_crash: TestGapMaxFilesMaxGapsCoercion#test_max_files_and_max_gaps_string_does_not_crash().
  TestTraceImpactMaxResultsCoercion.test_max_results_string_does_not_crash: TraceImpactMaxResultsCoercion#test_max_results_string_does_not_crash().
  TestUnreachableCodeMaxFilesCoercion.test_max_files_string_does_not_crash: UnreachableCodeMaxFilesCoercion#test_max_files_string_does_not_crash().
  TestAstCacheIndexMaxFilesCoercion: AstCacheIndexMaxFilesCoercion#
  TestAstCacheSyncMaxFilesCoercion: AstCacheSyncMaxFilesCoercion#
  TestAstPathMaxDepthCoercion: AstPathMaxDepthCoercion#
  TestClassHierarchyMaxDepthCoercion: ClassHierarchyMaxDepthCoercion#
  TestCodegraphSitemapMaxFilesCoercion: CodegraphSitemapMaxFilesCoercion#
  TestDependencyMatrixTopKCoercion: DependencyMatrixTopKCoercion#
  TestFullIndexMaxFilesCoercion: FullIndexMaxFilesCoercion#
  TestImportGraphMaxDepthCoercion: ImportGraphMaxDepthCoercion#
  TestProjectOverviewMaxDepthCoercion: ProjectOverviewMaxDepthCoercion#
  TestTestGapMaxFilesMaxGapsCoercion: TestGapMaxFilesMaxGapsCoercion#
  TestTraceImpactMaxResultsCoercion: TraceImpactMaxResultsCoercion#
  TestUnreachableCodeMaxFilesCoercion: UnreachableCodeMaxFilesCoercion#
---
# Module: [`tests/unit/mcp/test_numeric_param_coercion.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py)

## Classes
### `TestAstCacheIndexMaxFilesCoercion`
- def: [`tests/unit/mcp/test_numeric_param_coercion.py:23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L23)
- doc: ast_cache_tool.py:435 — max_files passed to cache.index_project().
- signature: `class TestAstCacheIndexMaxFilesCoercion:`
- members:
  - `test_mode_index_max_files_string_does_not_crash(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L27)
- uses (calls/refs, reference-scoped): [`ASTCacheTool`](../../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool.execute)

### `TestAstCacheSyncMaxFilesCoercion`
- def: [`tests/unit/mcp/test_numeric_param_coercion.py:69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L69)
- doc: ast_cache_tool.py:598 — max_files passed to sync_engine.sync().
- signature: `class TestAstCacheSyncMaxFilesCoercion:`
- members:
  - `test_mode_sync_max_files_string_does_not_crash(self, tmp_path: Any)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L73)
- uses (calls/refs, reference-scoped): [`ASTCacheTool`](../../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool.execute)

### `TestAstPathMaxDepthCoercion`
- def: [`tests/unit/mcp/test_numeric_param_coercion.py:113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L113)
- doc: ast_path_tool.py:114 — max_depth passed to nav.outline().
- signature: `class TestAstPathMaxDepthCoercion:`
- members:
  - `test_mode_outline_max_depth_string_does_not_crash(self, tmp_path: Any)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L117)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/ast_path_tool.md#CodeGraphASTPathTool.execute), [`CodeGraphASTPathTool`](../../../tree_sitter_analyzer/mcp/tools/ast_path_tool.md#CodeGraphASTPathTool)

### `TestClassHierarchyMaxDepthCoercion`
- def: [`tests/unit/mcp/test_numeric_param_coercion.py:156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L156)
- doc: class_hierarchy_tool.py:175 — max_depth passed to hierarchy.subclasses_of().
- signature: `class TestClassHierarchyMaxDepthCoercion:`
- members:
  - `test_max_depth_string_does_not_crash(self)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L160)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.md#ClassHierarchyTool.execute), [`ClassHierarchyTool`](../../../tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.md#ClassHierarchyTool)

### `TestCodegraphSitemapMaxFilesCoercion`
- def: [`tests/unit/mcp/test_numeric_param_coercion.py:200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L200)
- doc: codegraph_sitemap_tool.py:152 — max_files used in arithmetic/slice.
- signature: `class TestCodegraphSitemapMaxFilesCoercion:`
- members:
  - `test_max_files_string_does_not_crash(self, tmp_path: Any)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L204)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.md#CodeGraphSitemapTool.execute), [`CodeGraphSitemapTool`](../../../tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.md#CodeGraphSitemapTool)

### `TestDependencyMatrixTopKCoercion`
- def: [`tests/unit/mcp/test_numeric_param_coercion.py:232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L232)
- doc: dependency_matrix_tool.py:141 — top_k used in coupling_pairs\[:top_k\].
- signature: `class TestDependencyMatrixTopKCoercion:`
- members:
  - `test_top_k_string_does_not_crash(self)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L236)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.md#CodeGraphDependencyMatrixTool.execute), [`CodeGraphDependencyMatrixTool`](../../../tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.md#CodeGraphDependencyMatrixTool)

### `TestFullIndexMaxFilesCoercion`
- def: [`tests/unit/mcp/test_numeric_param_coercion.py:268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L268)
- doc: full_index_tool.py:118 — max_files passed to cache.index_project().
- signature: `class TestFullIndexMaxFilesCoercion:`
- members:
  - `test_max_files_string_does_not_crash(self)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L272)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/full_index_tool.md#CodeGraphFullIndexTool.execute), [`CodeGraphFullIndexTool`](../../../tree_sitter_analyzer/mcp/tools/full_index_tool.md#CodeGraphFullIndexTool)

### `TestImportGraphMaxDepthCoercion`
- def: [`tests/unit/mcp/test_numeric_param_coercion.py:307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L307)
- doc: import_graph_tool.py:181 — max_depth passed to graph.blast_radius().
- signature: `class TestImportGraphMaxDepthCoercion:`
- members:
  - `test_blast_radius_max_depth_string_does_not_crash(self, tmp_path: Any)` — [`L311`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L311)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/import_graph_tool.md#CodeGraphImportGraphTool.execute), [`CodeGraphImportGraphTool`](../../../tree_sitter_analyzer/mcp/tools/import_graph_tool.md#CodeGraphImportGraphTool)

### `TestProjectOverviewMaxDepthCoercion`
- def: [`tests/unit/mcp/test_numeric_param_coercion.py:351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L351)
- doc: project_overview_tool.py:192,205 — validate rejects str; coerce first.
- signature: `class TestProjectOverviewMaxDepthCoercion:`
- members:
  - `test_max_depth_string_does_not_crash(self, tmp_path: Any)` — [`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L355)
- uses (calls/refs, reference-scoped): [`ProjectOverviewTool`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool.execute)

### `TestTestGapMaxFilesMaxGapsCoercion`
- def: [`tests/unit/mcp/test_numeric_param_coercion.py:387`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L387)
- doc: test_gap_tool.py:123,124 — both max_files and max_gaps must be coerced.
- signature: `class TestTestGapMaxFilesMaxGapsCoercion:`
- members:
  - `test_max_files_and_max_gaps_string_does_not_crash(self)` — [`L391`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L391)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestTraceImpactMaxResultsCoercion`
- def: [`tests/unit/mcp/test_numeric_param_coercion.py:431`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L431)
- doc: trace_impact_tool.py:891 — max_results used in len()&gt;= and \[:\] slices.
- signature: `class TestTraceImpactMaxResultsCoercion:`
- members:
  - `test_max_results_string_does_not_crash(self)` — [`L435`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L435)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#TraceImpactTool.execute), [`TraceImpactTool`](../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#TraceImpactTool)

### `TestUnreachableCodeMaxFilesCoercion`
- def: [`tests/unit/mcp/test_numeric_param_coercion.py:473`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L473)
- doc: unreachable_code_tool.py:138 — max_files passed to analyze_project_unreachable.
- signature: `class TestUnreachableCodeMaxFilesCoercion:`
- members:
  - `test_max_files_string_does_not_crash(self)` — [`L477`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_numeric_param_coercion.py#L477)
- uses (calls/refs, reference-scoped): [`UnreachableCodeTool`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool.execute)

