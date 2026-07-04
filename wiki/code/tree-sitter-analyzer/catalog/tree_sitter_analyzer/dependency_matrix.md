---
title: 'Module: tree_sitter_analyzer/dependency_matrix.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/dependency_matrix.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.dependency_matrix`/
symbols:
  DependencyMatrix._compute_matrix: DependencyMatrix#_compute_matrix().
  DependencyMatrix.build: DependencyMatrix#build().
  DependencyMatrix.summary: DependencyMatrix#summary().
  DependencyMatrix.coupling_between: DependencyMatrix#coupling_between().
  DependencyMatrixResult.coupling_pairs: DependencyMatrixResult#coupling_pairs.
  DependencyMatrix: DependencyMatrix#
  DependencyMatrix.unstable_modules: DependencyMatrix#unstable_modules().
  DependencyMatrix._result: DependencyMatrix#_result.
  CouplingEntry.to_dict: CouplingEntry#to_dict().
  DependencyMatrixResult.to_dict: DependencyMatrixResult#to_dict().
  DependencyMatrix._compute_module_stats: DependencyMatrix#_compute_module_stats().
  DependencyMatrix.most_coupled: DependencyMatrix#most_coupled().
  ModuleStats.to_dict: ModuleStats#to_dict().
  CouplingEntry.score: CouplingEntry#score.
  CouplingEntry.file_a: CouplingEntry#file_a.
  CouplingEntry.file_b: CouplingEntry#file_b.
  CouplingEntry: CouplingEntry#
  DependencyMatrixResult.modules: DependencyMatrixResult#modules.
  CouplingEntry.call_count: CouplingEntry#call_count.
  DependencyMatrix._import_edges: DependencyMatrix#_import_edges.
  DependencyMatrixResult.high_coupling_pairs: DependencyMatrixResult#high_coupling_pairs.
  CouplingEntry.import_count: CouplingEntry#import_count.
  DependencyMatrixResult: DependencyMatrixResult#
  ModuleStats: ModuleStats#
  _pair_key: _pair_key().
  DependencyMatrix._built: DependencyMatrix#_built.
  DependencyMatrix._collect_import_edges: DependencyMatrix#_collect_import_edges().
  DependencyMatrixResult.module_stats: DependencyMatrixResult#module_stats.
  DependencyMatrix._call_edges: DependencyMatrix#_call_edges.
  ModuleStats.file: ModuleStats#file.
  ModuleStats.instability: ModuleStats#instability.
  DependencyMatrix._modules: DependencyMatrix#_modules.
  DependencyMatrix._collect_call_edges: DependencyMatrix#_collect_call_edges().
  DependencyMatrix._resolve_import: DependencyMatrix#_resolve_import().
  ModuleStats.afferent_coupling: ModuleStats#afferent_coupling.
  ModuleStats.efferent_coupling: ModuleStats#efferent_coupling.
  logger: logger.
  IMPORT_FACTOR: IMPORT_FACTOR.
  CALL_FACTOR: CALL_FACTOR.
  HIGH_COUPLING_THRESHOLD: HIGH_COUPLING_THRESHOLD.
  DependencyMatrixResult.matrix: DependencyMatrixResult#matrix.
  DependencyMatrix.project_root: DependencyMatrix#project_root.
  DependencyMatrix._resolve_python_import: DependencyMatrix#_resolve_python_import().
  DependencyMatrix.__init__: DependencyMatrix#__init__().
---
# Module: [`tree_sitter_analyzer/dependency_matrix.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py)

## Classes
### `CouplingEntry`
- def: [`tree_sitter_analyzer/dependency_matrix.py:40`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L40)
- signature: `class CouplingEntry:`
- members:
  - `to_dict(self)` — [`L47`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L47)
  - `call_count` — [`L44`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L44)
  - `file_a` — [`L41`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L41)
  - `file_b` — [`L42`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L42)
  - `import_count` — [`L43`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L43)
  - `score` — [`L45`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L45)
- used by: [`_compute_matrix`](dependency_matrix.md#DependencyMatrix._compute_matrix), [`execute`](mcp/tools/dependency_matrix_tool.md#CodeGraphDependencyMatrixTool.execute), [`summary`](dependency_matrix.md#DependencyMatrix.summary), [`coupling_between`](dependency_matrix.md#DependencyMatrix.coupling_between), [`coupling_pairs`](dependency_matrix.md#DependencyMatrixResult.coupling_pairs), [`to_dict`](dependency_matrix.md#DependencyMatrixResult.to_dict), [`most_coupled`](dependency_matrix.md#DependencyMatrix.most_coupled), [`high_coupling_pairs`](dependency_matrix.md#DependencyMatrixResult.high_coupling_pairs)  (6 test-only)

### `DependencyMatrix`
- def: [`tree_sitter_analyzer/dependency_matrix.py:96`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L96)
- doc: Build a dependency coupling matrix from the pre-indexed AST cache.
- signature: `class DependencyMatrix:`
- members:
  - `build(self)` — [`L117`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L117) — documented in [tree_sitter_analyzer-ast_cache](../../concepts/tree_sitter_analyzer-ast_cache.md)
  - `coupling_between(self, file_a: str, file_b: str)` — [`L288`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L288)
  - `most_coupled(self, top_k: int = 10)` — [`L299`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L299)
  - `summary(self)` — [`L311`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L311)
  - `unstable_modules(self, threshold: float = 0.7)` — [`L305`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L305)
  - `project_root` — [`L106`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L106)
- protocol/private: `__init__`[`L105`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L105), `_built`[`L107`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L107), `_call_edges`[`L111`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L111), `_collect_call_edges`[`L161`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L161), `_collect_import_edges`[`L147`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L147), `_compute_matrix`[`L218`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L218), `_compute_module_stats`[`L268`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L268), `_import_edges`[`L108`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L108), `_modules`[`L114`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L114), `_resolve_import`[`L178`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L178), `_resolve_python_import`[`L188`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L188), `_result`[`L115`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L115)
- uses (calls/refs, reference-scoped): [`ASTCache`](ast_cache.md#ASTCache), [`close`](ast_cache.md#ASTCache.close), [`coupling_pairs`](dependency_matrix.md#DependencyMatrixResult.coupling_pairs), [`score`](dependency_matrix.md#CouplingEntry.score), [`file_a`](dependency_matrix.md#CouplingEntry.file_a), [`file_b`](dependency_matrix.md#CouplingEntry.file_b), [`CouplingEntry`](dependency_matrix.md#CouplingEntry), [`modules`](dependency_matrix.md#DependencyMatrixResult.modules), [`call_count`](dependency_matrix.md#CouplingEntry.call_count), [`high_coupling_pairs`](dependency_matrix.md#DependencyMatrixResult.high_coupling_pairs), [`DependencyMatrixResult`](dependency_matrix.md#DependencyMatrixResult), [`import_count`](dependency_matrix.md#CouplingEntry.import_count), [`ModuleStats`](dependency_matrix.md#ModuleStats), [`_pair_key`](dependency_matrix.md#_pair_key), [`module_stats`](dependency_matrix.md#DependencyMatrixResult.module_stats), [`file`](dependency_matrix.md#ModuleStats.file), [`instability`](dependency_matrix.md#ModuleStats.instability), [`afferent_coupling`](dependency_matrix.md#ModuleStats.afferent_coupling), [`efferent_coupling`](dependency_matrix.md#ModuleStats.efferent_coupling), [`CALL_FACTOR`](dependency_matrix.md#CALL_FACTOR), [`HIGH_COUPLING_THRESHOLD`](dependency_matrix.md#HIGH_COUPLING_THRESHOLD), [`IMPORT_FACTOR`](dependency_matrix.md#IMPORT_FACTOR), [`logger`](dependency_matrix.md#logger), [`matrix`](dependency_matrix.md#DependencyMatrixResult.matrix)
- used by: [`execute`](mcp/tools/dependency_matrix_tool.md#CodeGraphDependencyMatrixTool.execute), [`_get_matrix`](mcp/tools/dependency_matrix_tool.md#CodeGraphDependencyMatrixTool._get_matrix), [`__init__`](mcp/tools/dependency_matrix_tool.md#CodeGraphDependencyMatrixTool.__init__)  (13 test-only)

### `DependencyMatrixResult`
- def: [`tree_sitter_analyzer/dependency_matrix.py:74`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L74)
- signature: `class DependencyMatrixResult:`
- members:
  - `to_dict(self)` — [`L81`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L81)
  - `coupling_pairs` — [`L76`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L76)
  - `high_coupling_pairs` — [`L78`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L78)
  - `matrix` — [`L79`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L79)
  - `module_stats` — [`L77`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L77)
  - `modules` — [`L75`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L75)
- uses (calls/refs, reference-scoped): [`to_dict`](dependency_matrix.md#CouplingEntry.to_dict), [`to_dict`](dependency_matrix.md#ModuleStats.to_dict), [`CouplingEntry`](dependency_matrix.md#CouplingEntry), [`ModuleStats`](dependency_matrix.md#ModuleStats)
- used by: [`_compute_matrix`](dependency_matrix.md#DependencyMatrix._compute_matrix), [`build`](dependency_matrix.md#DependencyMatrix.build), [`execute`](mcp/tools/dependency_matrix_tool.md#CodeGraphDependencyMatrixTool.execute), [`summary`](dependency_matrix.md#DependencyMatrix.summary), [`coupling_between`](dependency_matrix.md#DependencyMatrix.coupling_between), [`unstable_modules`](dependency_matrix.md#DependencyMatrix.unstable_modules), [`_result`](dependency_matrix.md#DependencyMatrix._result), [`most_coupled`](dependency_matrix.md#DependencyMatrix.most_coupled)  (7 test-only)

### `ModuleStats`
- def: [`tree_sitter_analyzer/dependency_matrix.py:58`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L58)
- signature: `class ModuleStats:`
- members:
  - `to_dict(self)` — [`L64`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L64)
  - `afferent_coupling` — [`L60`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L60)
  - `efferent_coupling` — [`L61`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L61)
  - `file` — [`L59`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L59)
  - `instability` — [`L62`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L62)
- used by: [`execute`](mcp/tools/dependency_matrix_tool.md#CodeGraphDependencyMatrixTool.execute), [`unstable_modules`](dependency_matrix.md#DependencyMatrix.unstable_modules), [`_compute_module_stats`](dependency_matrix.md#DependencyMatrix._compute_module_stats), [`to_dict`](dependency_matrix.md#DependencyMatrixResult.to_dict), [`module_stats`](dependency_matrix.md#DependencyMatrixResult.module_stats)  (2 test-only)

## Functions
- `_pair_key(a: str, b: str)` — [`L92`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L92)

## Module values
- `CALL_FACTOR` — [`L35`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L35)
- `HIGH_COUPLING_THRESHOLD` — [`L36`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L36)
- `IMPORT_FACTOR` — [`L34`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L34)
- `logger` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dependency_matrix.py#L32)

