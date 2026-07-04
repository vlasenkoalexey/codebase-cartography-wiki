---
title: 'Module: tests/unit/test_change_impact_analysis.py'
type: catalog
provenance: extracted
module: tests/unit/test_change_impact_analysis.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_change_impact_analysis`/Test
symbols:
  TestSummaryOnlyFastPath.test_summary_only_skips_ast_cache_enrichment: SummaryOnlyFastPath#test_summary_only_skips_ast_cache_enrichment().
  TestChangeImpactRequest.test_construction: ChangeImpactRequest#test_construction().
  TestChangeImpactRequest.test_default_scope_paths: ChangeImpactRequest#test_default_scope_paths().
  TestEnrichWithCacheSymbols.test_enriches_changed_files: EnrichWithCacheSymbols#test_enriches_changed_files().
  TestFindAffectedSymbols.test_finds_symbols_in_affected_files: FindAffectedSymbols#test_finds_symbols_in_affected_files().
  TestSummaryOnlyFastPath.test_summary_only_skips_ast_cache_enrichment.FakeGraph._nodes: SummaryOnlyFastPath#test_summary_only_skips_ast_cache_enrichment().FakeGraph#_nodes.
  TestFindTestFiles.test_maps_changed_to_tests: FindTestFiles#test_maps_changed_to_tests().
  TestFindTestFiles.test_no_test_nodes: FindTestFiles#test_no_test_nodes().
  TestTestFileMatchesChange.test_matching_stem: TestFileMatchesChange#test_matching_stem().
  TestTestFileMatchesChange.test_non_matching: TestFileMatchesChange#test_non_matching().
  TestIsRunnableTestFile.test_pytest_style: IsRunnableTestFile#test_pytest_style().
  TestIsRunnableTestFile.test_conftest_excluded: IsRunnableTestFile#test_conftest_excluded().
  TestIsRunnableTestFile.test_init_excluded: IsRunnableTestFile#test_init_excluded().
  TestIsRunnableTestFile.test_non_test_file: IsRunnableTestFile#test_non_test_file().
  TestIsTestOnlyChangeSet.test_true_for_runnable_test_files: IsTestOnlyChangeSet#test_true_for_runnable_test_files().
  TestIsTestOnlyChangeSet.test_false_for_runtime_or_test_support_files: IsTestOnlyChangeSet#test_false_for_runtime_or_test_support_files().
  TestAssessRisk.test_no_changes: AssessRisk#test_no_changes().
  TestAssessRisk.test_low_risk: AssessRisk#test_low_risk().
  TestAssessRisk.test_high_risk: AssessRisk#test_high_risk().
  TestBuildFileImpacts.test_none_graph: BuildFileImpacts#test_none_graph().
  TestBuildFileImpacts.test_with_mock_graph: BuildFileImpacts#test_with_mock_graph().
  TestBuildTestPlan.test_include_tests_false: BuildTestPlan#test_include_tests_false().
  TestBuildTestPlan.test_none_graph: BuildTestPlan#test_none_graph().
  TestLoadDependencyGraph.test_none_root_with_empty_cwd: LoadDependencyGraph#test_none_root_with_empty_cwd().
  TestLoadDependencyGraph.test_nonexistent_root: LoadDependencyGraph#test_nonexistent_root().
  TestAppendLargeDirtyHint.test_small_count: AppendLargeDirtyHint#test_small_count().
  TestAppendLargeDirtyHint.test_large_count_appends: AppendLargeDirtyHint#test_large_count_appends().
  TestEnsureASTCache.test_returns_none_for_none_root: EnsureASTCache#test_returns_none_for_none_root().
  TestEnsureASTCache.test_returns_none_for_empty_files: EnsureASTCache#test_returns_none_for_empty_files().
  TestEnsureASTCache.test_auto_indexes_empty_cache: EnsureASTCache#test_auto_indexes_empty_cache().
  TestEnrichWithCacheSymbols.test_returns_empty_for_none_cache: EnrichWithCacheSymbols#test_returns_empty_for_none_cache().
  TestFindAffectedSymbols.test_returns_empty_for_none_cache: FindAffectedSymbols#test_returns_empty_for_none_cache().
  TestSummaryOnlyFastPath.test_summary_only_skips_ast_cache_enrichment.FakeGraph.nodes: SummaryOnlyFastPath#test_summary_only_skips_ast_cache_enrichment().FakeGraph#nodes().
  TestSummaryOnlyFastPath.test_summary_only_skips_ast_cache_enrichment.FakeGraph.all_nodes: SummaryOnlyFastPath#test_summary_only_skips_ast_cache_enrichment().FakeGraph#all_nodes().
  TestSummaryOnlyFastPath.test_summary_only_skips_ast_cache_enrichment.FakeGraph.has_node: SummaryOnlyFastPath#test_summary_only_skips_ast_cache_enrichment().FakeGraph#has_node().
  TestSummaryOnlyFastPath.test_summary_only_skips_ast_cache_enrichment.FakeGraph: SummaryOnlyFastPath#test_summary_only_skips_ast_cache_enrichment().FakeGraph#
  TestSummaryOnlyFastPath.fail_enrichment: SummaryOnlyFastPath#fail_enrichment().
  TestChangeImpactRequest: ChangeImpactRequest#
  TestFindTestFiles: FindTestFiles#
  TestTestFileMatchesChange: TestFileMatchesChange#
  TestIsRunnableTestFile: IsRunnableTestFile#
  TestIsTestOnlyChangeSet: IsTestOnlyChangeSet#
  TestAssessRisk: AssessRisk#
  TestBuildFileImpacts: BuildFileImpacts#
  TestBuildTestPlan: BuildTestPlan#
  TestLoadDependencyGraph: LoadDependencyGraph#
  TestAppendLargeDirtyHint: AppendLargeDirtyHint#
  TestEnsureASTCache: EnsureASTCache#
  TestEnrichWithCacheSymbols: EnrichWithCacheSymbols#
  TestFindAffectedSymbols: FindAffectedSymbols#
  TestSummaryOnlyFastPath: SummaryOnlyFastPath#
  TestSummaryOnlyFastPath.test_summary_only_skips_ast_cache_enrichment.FakeGraph.dependents_of: SummaryOnlyFastPath#test_summary_only_skips_ast_cache_enrichment().FakeGraph#dependents_of().
  TestSummaryOnlyFastPath.test_summary_only_skips_ast_cache_enrichment.FakeGraph.dependencies_of: SummaryOnlyFastPath#test_summary_only_skips_ast_cache_enrichment().FakeGraph#dependencies_of().
---
# Module: [`tests/unit/test_change_impact_analysis.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py)

## Classes
### `FakeGraph`
- def: [`tests/unit/test_change_impact_analysis.py:272`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L272)
- signature: `class FakeGraph:`
- members:
  - `all_nodes(self)` — [`L278`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L278)
  - `dependencies_of(self, file_rel)` — [`L284`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L284)
  - `dependents_of(self, file_rel)` — [`L281`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L281)
  - `has_node(self, file_rel)` — [`L287`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L287)
  - `nodes(self)` — [`L275`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L275)
- protocol/private: `_nodes`[`L273`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L273)
- used by: (1 test-only callers)

### `TestAppendLargeDirtyHint`
- def: [`tests/unit/test_change_impact_analysis.py:172`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L172)
- signature: `class TestAppendLargeDirtyHint:`
- members:
  - `test_large_count_appends(self)` — [`L176`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L176)
  - `test_small_count(self)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L173)
- uses (calls/refs, reference-scoped): [`_append_large_dirty_hint`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#_append_large_dirty_hint)

### `TestAssessRisk`
- def: [`tests/unit/test_change_impact_analysis.py:101`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L101)
- signature: `class TestAssessRisk:`
- members:
  - `test_high_risk(self)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L110)
  - `test_low_risk(self)` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L106)
  - `test_no_changes(self)` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L102)
- uses (calls/refs, reference-scoped): [`_assess_risk`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#_assess_risk)

### `TestBuildFileImpacts`
- def: [`tests/unit/test_change_impact_analysis.py:116`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L116)
- signature: `class TestBuildFileImpacts:`
- members:
  - `test_none_graph(self)` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L117)
  - `test_with_mock_graph(self)` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L123)
- uses (calls/refs, reference-scoped): [`_build_file_impacts`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#_build_file_impacts)

### `TestBuildTestPlan`
- def: [`tests/unit/test_change_impact_analysis.py:136`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L136)
- signature: `class TestBuildTestPlan:`
- members:
  - `test_include_tests_false(self)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L137)
  - `test_none_graph(self)` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L142)
- uses (calls/refs, reference-scoped): [`_build_test_plan`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#_build_test_plan)

### `TestChangeImpactRequest`
- def: [`tests/unit/test_change_impact_analysis.py:21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L21)
- signature: `class TestChangeImpactRequest:`
- members:
  - `test_construction(self)` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L22)
  - `test_default_scope_paths(self)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L34)
- uses (calls/refs, reference-scoped): [`changed_files`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest.changed_files), [`project_root`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest.project_root), [`ChangeImpactRequest`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest), [`include_tests`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest.include_tests), [`mode`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest.mode), [`diff_stat`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest.diff_stat), [`scope_paths`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest.scope_paths)

### `TestEnrichWithCacheSymbols`
- def: [`tests/unit/test_change_impact_analysis.py:213`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L213)
- signature: `class TestEnrichWithCacheSymbols:`
- members:
  - `test_enriches_changed_files(self, tmp_path)` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L221)
  - `test_returns_empty_for_none_cache(self)` — [`L214`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L214)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_file`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_file), [`_enrich_with_cache_symbols`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#_enrich_with_cache_symbols)

### `TestEnsureASTCache`
- def: [`tests/unit/test_change_impact_analysis.py:181`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L181)
- signature: `class TestEnsureASTCache:`
- members:
  - `test_auto_indexes_empty_cache(self, tmp_path)` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L196)
  - `test_returns_none_for_empty_files(self)` — [`L189`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L189)
  - `test_returns_none_for_none_root(self)` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L182)
- uses (calls/refs, reference-scoped): [`_ensure_ast_cache`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#_ensure_ast_cache)

### `TestFindAffectedSymbols`
- def: [`tests/unit/test_change_impact_analysis.py:242`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L242)
- signature: `class TestFindAffectedSymbols:`
- members:
  - `test_finds_symbols_in_affected_files(self, tmp_path)` — [`L250`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L250)
  - `test_returns_empty_for_none_cache(self)` — [`L243`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L243)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_file`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_file), [`_find_affected_symbols`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#_find_affected_symbols)

### `TestFindTestFiles`
- def: [`tests/unit/test_change_impact_analysis.py:45`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L45)
- signature: `class TestFindTestFiles:`
- members:
  - `test_maps_changed_to_tests(self)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L46)
  - `test_no_test_nodes(self)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L51)
- uses (calls/refs, reference-scoped): [`_find_test_files`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#_find_test_files)

### `TestIsRunnableTestFile`
- def: [`tests/unit/test_change_impact_analysis.py:64`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L64)
- signature: `class TestIsRunnableTestFile:`
- members:
  - `test_conftest_excluded(self)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L71)
  - `test_init_excluded(self)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L77)
  - `test_non_test_file(self)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L83)
  - `test_pytest_style(self)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L65)
- uses (calls/refs, reference-scoped): [`_is_runnable_test_file`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#_is_runnable_test_file)

### `TestIsTestOnlyChangeSet`
- def: [`tests/unit/test_change_impact_analysis.py:89`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L89)
- signature: `class TestIsTestOnlyChangeSet:`
- members:
  - `test_false_for_runtime_or_test_support_files(self)` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L95)
  - `test_true_for_runnable_test_files(self)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L90)
- uses (calls/refs, reference-scoped): [`_is_test_only_change_set`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#_is_test_only_change_set)

### `TestLoadDependencyGraph`
- def: [`tests/unit/test_change_impact_analysis.py:148`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L148)
- signature: `class TestLoadDependencyGraph:`
- members:
  - `test_none_root_with_empty_cwd(self, tmp_path, monkeypatch)` — [`L157`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L157)
  - `test_nonexistent_root(self)` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L165)
- uses (calls/refs, reference-scoped): [`_load_dependency_graph`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#_load_dependency_graph)

### `TestSummaryOnlyFastPath`
- def: [`tests/unit/test_change_impact_analysis.py:268`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L268)
- signature: `class TestSummaryOnlyFastPath:`
- members:
  - `fail_enrichment(*args, **kwargs)` — [`L293`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L293)
  - `test_summary_only_skips_ast_cache_enrichment(self, tmp_path, monkeypatch)` — [`L269`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L269)
- uses (calls/refs, reference-scoped): [`_build_change_impact_result`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#_build_change_impact_result), [`changed_files`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest.changed_files), [`project_root`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest.project_root), [`ChangeImpactRequest`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest), [`include_tests`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest.include_tests), [`mode`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest.mode), [`diff_stat`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest.diff_stat), [`agent_summary_only`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest.agent_summary_only)  (1 test-only)

### `TestTestFileMatchesChange`
- def: [`tests/unit/test_change_impact_analysis.py:56`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L56)
- signature: `class TestTestFileMatchesChange:`
- members:
  - `test_matching_stem(self)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L57)
  - `test_non_matching(self)` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_analysis.py#L60)
- uses (calls/refs, reference-scoped): [`_test_file_matches_change`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#_test_file_matches_change)

