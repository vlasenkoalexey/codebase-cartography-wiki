---
title: 'Module: tests/unit/test_dependency_matrix.py'
type: catalog
provenance: extracted
module: tests/unit/test_dependency_matrix.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_dependency_matrix`/Test
symbols:
  TestCouplingEntry.test_to_dict: CouplingEntry#test_to_dict().
  TestDependencyMatrixCrossFileIntegration.test_call_count_nonempty_for_cross_file_project: DependencyMatrixCrossFileIntegration#test_call_count_nonempty_for_cross_file_project().
  TestModuleStats.test_to_dict: ModuleStats#test_to_dict().
  TestDependencyMatrixBuild.test_build_with_mock_cache: DependencyMatrixBuild#test_build_with_mock_cache().
  TestDependencyMatrixBuild.test_build_empty_cache: DependencyMatrixBuild#test_build_empty_cache().
  TestDependencyMatrixCallEdges.test_resolved_call_edges_counted: DependencyMatrixCallEdges#test_resolved_call_edges_counted().
  TestDependencyMatrixBuild.test_build_cache_failure: DependencyMatrixBuild#test_build_cache_failure().
  TestDependencyMatrixBuild.test_coupling_between: DependencyMatrixBuild#test_coupling_between().
  TestDependencyMatrixBuild.test_most_coupled: DependencyMatrixBuild#test_most_coupled().
  TestDependencyMatrixBuild.test_unstable_modules: DependencyMatrixBuild#test_unstable_modules().
  TestDependencyMatrixBuild.test_high_coupling_pairs: DependencyMatrixBuild#test_high_coupling_pairs().
  TestDependencyMatrixSelfCallFilter.test_self_edges_filtered: DependencyMatrixSelfCallFilter#test_self_edges_filtered().
  TestDependencyMatrixCallEdges.test_unresolved_call_edge_skipped: DependencyMatrixCallEdges#test_unresolved_call_edge_skipped().
  TestDependencyMatrixResult.test_to_dict_empty: DependencyMatrixResult#test_to_dict_empty().
  TestDependencyMatrixBuild.test_coupling_between_not_found: DependencyMatrixBuild#test_coupling_between_not_found().
  TestDependencyMatrixBuild.test_summary: DependencyMatrixBuild#test_summary().
  TestPairKey.test_ordering: PairKey#test_ordering().
  TestPairKey.test_same: PairKey#test_same().
  TestPairKey: PairKey#
  TestCouplingEntry: CouplingEntry#
  TestModuleStats: ModuleStats#
  TestDependencyMatrixResult: DependencyMatrixResult#
  TestDependencyMatrixBuild: DependencyMatrixBuild#
  TestDependencyMatrixSelfCallFilter: DependencyMatrixSelfCallFilter#
  TestDependencyMatrixCallEdges: DependencyMatrixCallEdges#
  TestDependencyMatrixCrossFileIntegration: DependencyMatrixCrossFileIntegration#
---
# Module: [`tests/unit/test_dependency_matrix.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py)

## Classes
### `TestCouplingEntry`
- def: [`tests/unit/test_dependency_matrix.py:21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L21)
- signature: `class TestCouplingEntry:`
- members:
  - `test_to_dict(self)` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L22)
- uses (calls/refs, reference-scoped): [`to_dict`](../../tree_sitter_analyzer/dependency_matrix.md#CouplingEntry.to_dict), [`score`](../../tree_sitter_analyzer/dependency_matrix.md#CouplingEntry.score), [`file_a`](../../tree_sitter_analyzer/dependency_matrix.md#CouplingEntry.file_a), [`file_b`](../../tree_sitter_analyzer/dependency_matrix.md#CouplingEntry.file_b), [`CouplingEntry`](../../tree_sitter_analyzer/dependency_matrix.md#CouplingEntry), [`call_count`](../../tree_sitter_analyzer/dependency_matrix.md#CouplingEntry.call_count), [`import_count`](../../tree_sitter_analyzer/dependency_matrix.md#CouplingEntry.import_count)

### `TestDependencyMatrixBuild`
- def: [`tests/unit/test_dependency_matrix.py:50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L50)
- signature: `class TestDependencyMatrixBuild:`
- members:
  - `test_build_cache_failure(self, tmp_path)` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L91)
  - `test_build_empty_cache(self, tmp_path)` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L78)
  - `test_build_with_mock_cache(self, tmp_path)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L51)
  - `test_coupling_between(self, tmp_path)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L100)
  - `test_coupling_between_not_found(self, tmp_path)` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L116)
  - `test_high_coupling_pairs(self, tmp_path)` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L184)
  - `test_most_coupled(self, tmp_path)` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L128)
  - `test_summary(self, tmp_path)` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L168)
  - `test_unstable_modules(self, tmp_path)` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L151)
- uses (calls/refs, reference-scoped): [`build`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrix.build), [`summary`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrix.summary), [`coupling_between`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrix.coupling_between), [`coupling_pairs`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrixResult.coupling_pairs), [`DependencyMatrix`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrix), [`unstable_modules`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrix.unstable_modules), [`most_coupled`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrix.most_coupled), [`score`](../../tree_sitter_analyzer/dependency_matrix.md#CouplingEntry.score), [`modules`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrixResult.modules), [`call_count`](../../tree_sitter_analyzer/dependency_matrix.md#CouplingEntry.call_count), [`high_coupling_pairs`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrixResult.high_coupling_pairs), [`import_count`](../../tree_sitter_analyzer/dependency_matrix.md#CouplingEntry.import_count), [`file`](../../tree_sitter_analyzer/dependency_matrix.md#ModuleStats.file)

### `TestDependencyMatrixCallEdges`
- def: [`tests/unit/test_dependency_matrix.py:224`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L224)
- doc: Regression for the latent call-edge dead-dimension bug.
- signature: `class TestDependencyMatrixCallEdges:`
- members:
  - `test_resolved_call_edges_counted(self, tmp_path)` — [`L235`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L235)
  - `test_unresolved_call_edge_skipped(self, tmp_path)` — [`L252`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L252)
- uses (calls/refs, reference-scoped): [`build`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrix.build), [`coupling_between`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrix.coupling_between), [`coupling_pairs`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrixResult.coupling_pairs), [`DependencyMatrix`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrix), [`call_count`](../../tree_sitter_analyzer/dependency_matrix.md#CouplingEntry.call_count)

### `TestDependencyMatrixCrossFileIntegration`
- def: [`tests/unit/test_dependency_matrix.py:267`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L267)
- doc: End-to-end: a real cross-file Python project must produce a non-empty
- signature: `class TestDependencyMatrixCrossFileIntegration:`
- members:
  - `test_call_count_nonempty_for_cross_file_project(self, tmp_path)` — [`L271`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L271)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project), [`build`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrix.build), [`coupling_between`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrix.coupling_between), [`DependencyMatrix`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrix), [`call_count`](../../tree_sitter_analyzer/dependency_matrix.md#CouplingEntry.call_count)

### `TestDependencyMatrixResult`
- def: [`tests/unit/test_dependency_matrix.py:42`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L42)
- signature: `class TestDependencyMatrixResult:`
- members:
  - `test_to_dict_empty(self)` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L43)
- uses (calls/refs, reference-scoped): [`to_dict`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrixResult.to_dict), [`DependencyMatrixResult`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrixResult)

### `TestDependencyMatrixSelfCallFilter`
- def: [`tests/unit/test_dependency_matrix.py:206`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L206)
- signature: `class TestDependencyMatrixSelfCallFilter:`
- members:
  - `test_self_edges_filtered(self, tmp_path)` — [`L207`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L207)
- uses (calls/refs, reference-scoped): [`build`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrix.build), [`coupling_pairs`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrixResult.coupling_pairs), [`DependencyMatrix`](../../tree_sitter_analyzer/dependency_matrix.md#DependencyMatrix)

### `TestModuleStats`
- def: [`tests/unit/test_dependency_matrix.py:32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L32)
- signature: `class TestModuleStats:`
- members:
  - `test_to_dict(self)` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L33)
- uses (calls/refs, reference-scoped): [`to_dict`](../../tree_sitter_analyzer/dependency_matrix.md#ModuleStats.to_dict), [`ModuleStats`](../../tree_sitter_analyzer/dependency_matrix.md#ModuleStats), [`file`](../../tree_sitter_analyzer/dependency_matrix.md#ModuleStats.file), [`instability`](../../tree_sitter_analyzer/dependency_matrix.md#ModuleStats.instability), [`afferent_coupling`](../../tree_sitter_analyzer/dependency_matrix.md#ModuleStats.afferent_coupling), [`efferent_coupling`](../../tree_sitter_analyzer/dependency_matrix.md#ModuleStats.efferent_coupling)

### `TestPairKey`
- def: [`tests/unit/test_dependency_matrix.py:12`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L12)
- signature: `class TestPairKey:`
- members:
  - `test_ordering(self)` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L13)
  - `test_same(self)` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dependency_matrix.py#L17)
- uses (calls/refs, reference-scoped): [`_pair_key`](../../tree_sitter_analyzer/dependency_matrix.md#_pair_key)

