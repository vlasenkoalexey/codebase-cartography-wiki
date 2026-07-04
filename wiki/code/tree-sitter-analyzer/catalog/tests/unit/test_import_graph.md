---
title: 'Module: tests/unit/test_import_graph.py'
type: catalog
provenance: extracted
module: tests/unit/test_import_graph.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_import_graph`/
symbols:
  _graph: _graph().
  _np: _np().
  TestImportGraphBuild.test_build_resolves_edges_from_cache: TestImportGraphBuild#test_build_resolves_edges_from_cache().
  TestImportGraphBuild.test_build_handles_cache_failure_gracefully: TestImportGraphBuild#test_build_handles_cache_failure_gracefully().
  ROOT: ROOT.
  TestResolvePythonImport.test_bare_dotted_import_resolves_to_module_file: TestResolvePythonImport#test_bare_dotted_import_resolves_to_module_file().
  TestResolvePythonImport.test_from_import_resolves_to_submodule: TestResolvePythonImport#test_from_import_resolves_to_submodule().
  TestResolvePythonImport.test_import_resolves_to_package_init: TestResolvePythonImport#test_import_resolves_to_package_init().
  TestResolvePythonImport.test_stdlib_import_is_not_resolved: TestResolvePythonImport#test_stdlib_import_is_not_resolved().
  TestResolvePythonImport.test_unresolvable_import_returns_none: TestResolvePythonImport#test_unresolvable_import_returns_none().
  TestResolvePythonImport.test_relative_import_with_module_resolves_to_sibling: TestResolvePythonImport#test_relative_import_with_module_resolves_to_sibling().
  TestResolvePythonImport.test_bare_relative_import_is_unresolved: TestResolvePythonImport#test_bare_relative_import_is_unresolved().
  TestResolveJsImport.test_require_relative: TestResolveJsImport#test_require_relative().
  TestResolveJsImport.test_esm_import_relative: TestResolveJsImport#test_esm_import_relative().
  TestResolveJsImport.test_index_resolution: TestResolveJsImport#test_index_resolution().
  TestResolveJsImport.test_bare_module_not_resolved: TestResolveJsImport#test_bare_module_not_resolved().
  TestImportGraphQueries.test_detect_cycles: TestImportGraphQueries#test_detect_cycles().
  TestImportGraphQueries.test_no_cycles_in_dag: TestImportGraphQueries#test_no_cycles_in_dag().
  TestImportGraphQueries.test_dependencies_of_forward: TestImportGraphQueries#test_dependencies_of_forward().
  TestImportGraphQueries.test_dependents_of_reverse: TestImportGraphQueries#test_dependents_of_reverse().
  TestImportGraphQueries.test_dependents_of_unknown_file_is_empty: TestImportGraphQueries#test_dependents_of_unknown_file_is_empty().
  TestImportGraphQueries.test_blast_radius_transitive: TestImportGraphQueries#test_blast_radius_transitive().
  TestImportGraphQueries.test_blast_radius_respects_max_depth: TestImportGraphQueries#test_blast_radius_respects_max_depth().
  TestImportGraphQueries.test_summary_statistics: TestImportGraphQueries#test_summary_statistics().
  TestImportGraphBuild.test_build_resolves_edges_from_cache._FakeCache: TestImportGraphBuild#test_build_resolves_edges_from_cache()._FakeCache#
  TestImportGraphBuild.test_build_handles_cache_failure_gracefully._BoomCache: TestImportGraphBuild#test_build_handles_cache_failure_gracefully()._BoomCache#
  TestResolvePythonImport: TestResolvePythonImport#
  TestResolveJsImport: TestResolveJsImport#
  TestImportGraphQueries: TestImportGraphQueries#
  TestImportGraphBuild: TestImportGraphBuild#
  TestImportGraphBuild.test_build_resolves_edges_from_cache._FakeCache.__init__: TestImportGraphBuild#test_build_resolves_edges_from_cache()._FakeCache#__init__().
  TestImportGraphBuild.test_build_resolves_edges_from_cache._FakeCache.get_imports: TestImportGraphBuild#test_build_resolves_edges_from_cache()._FakeCache#get_imports().
  TestImportGraphBuild.test_build_resolves_edges_from_cache._FakeCache.close: TestImportGraphBuild#test_build_resolves_edges_from_cache()._FakeCache#close().
  TestImportGraphBuild.test_build_handles_cache_failure_gracefully._BoomCache.__init__: TestImportGraphBuild#test_build_handles_cache_failure_gracefully()._BoomCache#__init__().
---
# Module: [`tests/unit/test_import_graph.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py)

## Classes
### `TestImportGraphBuild`
- def: [`tests/unit/test_import_graph.py:206`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L206)
- signature: `class TestImportGraphBuild:`
- members:
  - `test_build_handles_cache_failure_gracefully(self, monkeypatch)` — [`L232`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L232)
  - `test_build_resolves_edges_from_cache(self, monkeypatch)` — [`L207`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L207)
- uses (calls/refs, reference-scoped): [`build`](../../tree_sitter_analyzer/import_graph.md#ImportGraph.build), [`edges`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult.edges), [`ImportGraph`](../../tree_sitter_analyzer/import_graph.md#ImportGraph), [`ImportGraphResult`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult), [`edge_count`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult.edge_count), [`source_file`](../../tree_sitter_analyzer/import_graph.md#ImportEdge.source_file), [`target_file`](../../tree_sitter_analyzer/import_graph.md#ImportEdge.target_file)  (3 test-only)

### `TestImportGraphQueries`
- def: [`tests/unit/test_import_graph.py:150`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L150)
- signature: `class TestImportGraphQueries:`
- members:
  - `test_blast_radius_respects_max_depth(self)` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L174)
  - `test_blast_radius_transitive(self)` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L165)
  - `test_dependencies_of_forward(self)` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L151)
  - `test_dependents_of_reverse(self)` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L156)
  - `test_dependents_of_unknown_file_is_empty(self)` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L161)
  - `test_detect_cycles(self)` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L182)
  - `test_no_cycles_in_dag(self)` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L187)
  - `test_summary_statistics(self)` — [`L191`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L191)
- uses (calls/refs, reference-scoped): [`_make_result`](../../tree_sitter_analyzer/import_graph.md#ImportGraph._make_result), [`summary`](../../tree_sitter_analyzer/import_graph.md#ImportGraph.summary), [`blast_radius`](../../tree_sitter_analyzer/import_graph.md#ImportGraph.blast_radius), [`dependents_of`](../../tree_sitter_analyzer/import_graph.md#ImportGraph.dependents_of), [`dependencies_of`](../../tree_sitter_analyzer/import_graph.md#ImportGraph.dependencies_of), [`cycles`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult.cycles)  (1 test-only)

### `TestResolveJsImport`
- def: [`tests/unit/test_import_graph.py:93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L93)
- signature: `class TestResolveJsImport:`
- members:
  - `test_bare_module_not_resolved(self)` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L118)
  - `test_esm_import_relative(self)` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L102)
  - `test_index_resolution(self)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L110)
  - `test_require_relative(self)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L94)
- uses (calls/refs, reference-scoped): [`_resolve_js_import`](../../tree_sitter_analyzer/import_graph.md#_resolve_js_import)  (2 test-only)

### `TestResolvePythonImport`
- def: [`tests/unit/test_import_graph.py:37`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L37)
- signature: `class TestResolvePythonImport:`
- members:
  - `test_bare_dotted_import_resolves_to_module_file(self)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L38)
  - `test_bare_relative_import_is_unresolved(self)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L76)
  - `test_from_import_resolves_to_submodule(self)` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L43)
  - `test_import_resolves_to_package_init(self)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L48)
  - `test_relative_import_with_module_resolves_to_sibling(self)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L67)
  - `test_stdlib_import_is_not_resolved(self)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L53)
  - `test_unresolvable_import_returns_none(self)` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L59)
- uses (calls/refs, reference-scoped): [`_resolve_python_import`](../../tree_sitter_analyzer/import_graph.md#_resolve_python_import)  (2 test-only)

### `_BoomCache`
- def: [`tests/unit/test_import_graph.py:233`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L233)
- signature: `class _BoomCache:`
- protocol/private: `__init__`[`L234`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L234)
- used by: (1 test-only callers)

### `_FakeCache`
- def: [`tests/unit/test_import_graph.py:213`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L213)
- signature: `class _FakeCache:`
- members:
  - `close(self)` — [`L220`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L220)
  - `get_imports(self)` — [`L217`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L217)
- protocol/private: `__init__`[`L214`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L214)
- used by: (1 test-only callers)

## Functions
- `_graph(edges: list[tuple[str, str]])` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L135) — Construct an already-built ImportGraph from (source, target) pairs.
- `_np(path: str)` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L23) — Normalize a POSIX-style test path to the host OS separator.

## Module values
- `ROOT` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph.py#L20)

