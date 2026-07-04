---
title: 'Module: tests/unit/test_project_graph.py'
type: catalog
provenance: extracted
module: tests/unit/test_project_graph.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_project_graph`/
symbols:
  TestSymbolInDegree.test_R9_js_bare_imports_yield_no_symbol_entry: TestSymbolInDegree#test_R9_js_bare_imports_yield_no_symbol_entry().
  PY_PROJECT: PY_PROJECT.
  TestSymbolInDegree.test_R5_ambiguous_when_two_files_define_same_name: TestSymbolInDegree#test_R5_ambiguous_when_two_files_define_same_name().
  TestSymbolInDegree.test_R6_disambiguate_by_defining_file: TestSymbolInDegree#test_R6_disambiguate_by_defining_file().
  TestImportExtraction.test_extract_python_imports_from_utils: TestImportExtraction#test_extract_python_imports_from_utils().
  TestDependencyGraph.test_empty_project_handled: TestDependencyGraph#test_empty_project_handled().
  TestSymbolInDegree.test_G4_no_self_imports_polluting_count: TestSymbolInDegree#test_G4_no_self_imports_polluting_count().
  TestDependencyGraphCache.test_cache_hit_on_rebuild: TestDependencyGraphCache#test_cache_hit_on_rebuild().
  FIXTURES_DIR: FIXTURES_DIR.
  TestImportExtraction.test_extract_python_imports_from_main: TestImportExtraction#test_extract_python_imports_from_main().
  TestImportExtraction.test_extract_js_imports_from_index: TestImportExtraction#test_extract_js_imports_from_index().
  TestImportExtraction.test_extract_imports_unsupported_language: TestImportExtraction#test_extract_imports_unsupported_language().
  TestImportExtraction.test_extract_go_imports_from_main: TestImportExtraction#test_extract_go_imports_from_main().
  TestImportExtraction.test_extract_rust_imports_from_main: TestImportExtraction#test_extract_rust_imports_from_main().
  TestImportExtraction.test_extract_cpp_imports_from_main: TestImportExtraction#test_extract_cpp_imports_from_main().
  TestImportExtraction.test_extract_java_imports_from_main: TestImportExtraction#test_extract_java_imports_from_main().
  TestDependencyGraph.py_graph: TestDependencyGraph#py_graph().
  TestDependencyGraph.js_graph: TestDependencyGraph#js_graph().
  TestSymbolInDegree.py_graph: TestSymbolInDegree#py_graph().
  TestCycleDetection.py_graph: TestCycleDetection#py_graph().
  TestBlastRadius.py_graph: TestBlastRadius#py_graph().
  JS_PROJECT: JS_PROJECT.
  GO_PROJECT: GO_PROJECT.
  RUST_PROJECT: RUST_PROJECT.
  CPP_PROJECT: CPP_PROJECT.
  JAVA_PROJECT: JAVA_PROJECT.
  TestSymbolInDegree.custom_graph: TestSymbolInDegree#custom_graph().
  TestCycleDetection.test_detect_cycles: TestCycleDetection#test_detect_cycles().
  TestBlastRadius.radius: TestBlastRadius#radius().
  TestDependencyGraphPublicAPI.tiny: TestDependencyGraphPublicAPI#tiny().
  TestDependencyGraphPublicAccessors.small_graph: TestDependencyGraphPublicAccessors#small_graph().
  _is_stdlib: _is_stdlib().
  TestImportExtraction: TestImportExtraction#
  TestDependencyGraph: TestDependencyGraph#
  TestDependencyGraph.test_build_python_graph: TestDependencyGraph#test_build_python_graph().
  TestDependencyGraph.test_build_js_graph: TestDependencyGraph#test_build_js_graph().
  TestDependencyGraph.test_get_dependencies_of_file: TestDependencyGraph#test_get_dependencies_of_file().
  TestDependencyGraph.test_get_dependents_of_file: TestDependencyGraph#test_get_dependents_of_file().
  TestDependencyGraph.test_leaf_file_has_no_dependents: TestDependencyGraph#test_leaf_file_has_no_dependents().
  TestDependencyGraph.test_to_dict_output: TestDependencyGraph#test_to_dict_output().
  TestSymbolInDegree: TestSymbolInDegree#
  TestSymbolInDegree.test_R1_simple_fan_in_count: TestSymbolInDegree#test_R1_simple_fan_in_count().
  TestSymbolInDegree.test_R2_zero_for_unimported_defined_symbol: TestSymbolInDegree#test_R2_zero_for_unimported_defined_symbol().
  TestSymbolInDegree.test_R3_zero_for_unknown_symbol_no_raise: TestSymbolInDegree#test_R3_zero_for_unknown_symbol_no_raise().
  TestSymbolInDegree.test_R4_dedupes_repeated_imports_in_same_file: TestSymbolInDegree#test_R4_dedupes_repeated_imports_in_same_file().
  TestSymbolInDegree.test_R7_relative_import_counts: TestSymbolInDegree#test_R7_relative_import_counts().
  TestSymbolInDegree.test_R8_stdlib_names_not_indexed: TestSymbolInDegree#test_R8_stdlib_names_not_indexed().
  TestSymbolInDegree.test_G1_dependents_of_unchanged: TestSymbolInDegree#test_G1_dependents_of_unchanged().
  TestSymbolInDegree.test_G2_to_dict_backward_compatible: TestSymbolInDegree#test_G2_to_dict_backward_compatible().
  TestSymbolInDegree.test_G3_find_cycles_unchanged: TestSymbolInDegree#test_G3_find_cycles_unchanged().
  TestCycleDetection: TestCycleDetection#
  TestBlastRadius: TestBlastRadius#
  TestBlastRadius.test_blast_radius_forward: TestBlastRadius#test_blast_radius_forward().
  TestBlastRadius.test_blast_radius_reverse: TestBlastRadius#test_blast_radius_reverse().
  TestBlastRadius.test_blast_radius_leaf_file_forward: TestBlastRadius#test_blast_radius_leaf_file_forward().
  TestBlastRadius.test_blast_radius_nonexistent_file: TestBlastRadius#test_blast_radius_nonexistent_file().
  TestBlastRadius.test_blast_radius_to_dict: TestBlastRadius#test_blast_radius_to_dict().
  TestDependencyGraphCache: TestDependencyGraphCache#
  TestDependencyGraphPublicAPI: TestDependencyGraphPublicAPI#
  TestDependencyGraphPublicAPI.test_all_nodes_returns_frozenset: TestDependencyGraphPublicAPI#test_all_nodes_returns_frozenset().
  TestDependencyGraphPublicAPI.test_all_nodes_contains_all_files: TestDependencyGraphPublicAPI#test_all_nodes_contains_all_files().
  TestDependencyGraphPublicAPI.test_all_nodes_consistent_with_nodes: TestDependencyGraphPublicAPI#test_all_nodes_consistent_with_nodes().
  TestDependencyGraphPublicAPI.test_all_nodes_returns_copy: TestDependencyGraphPublicAPI#test_all_nodes_returns_copy().
  TestDependencyGraphPublicAPI.test_all_edges_returns_frozenset: TestDependencyGraphPublicAPI#test_all_edges_returns_frozenset().
  TestDependencyGraphPublicAPI.test_all_edges_consistent_with_edges: TestDependencyGraphPublicAPI#test_all_edges_consistent_with_edges().
  TestDependencyGraphPublicAPI.test_all_edges_returns_copy: TestDependencyGraphPublicAPI#test_all_edges_returns_copy().
  TestDependencyGraphPublicAPI.test_all_deps_returns_dict: TestDependencyGraphPublicAPI#test_all_deps_returns_dict().
  TestDependencyGraphPublicAPI.test_all_deps_values_are_sets: TestDependencyGraphPublicAPI#test_all_deps_values_are_sets().
  TestDependencyGraphPublicAPI.test_all_deps_mutation_does_not_affect_graph: TestDependencyGraphPublicAPI#test_all_deps_mutation_does_not_affect_graph().
  TestDependencyGraphPublicAPI.test_all_deps_covers_dependencies_of: TestDependencyGraphPublicAPI#test_all_deps_covers_dependencies_of().
  TestDependencyGraphPublicAccessors: TestDependencyGraphPublicAccessors#
  TestDependencyGraphPublicAccessors.test_has_node_true_for_existing_node: TestDependencyGraphPublicAccessors#test_has_node_true_for_existing_node().
  TestDependencyGraphPublicAccessors.test_has_node_false_for_missing_node: TestDependencyGraphPublicAccessors#test_has_node_false_for_missing_node().
  TestDependencyGraphPublicAccessors.test_node_count_matches_nodes_length: TestDependencyGraphPublicAccessors#test_node_count_matches_nodes_length().
  TestDependencyGraphPublicAccessors.test_edge_count_matches_edges_length: TestDependencyGraphPublicAccessors#test_edge_count_matches_edges_length().
  TestDependencyGraphPublicAccessors.test_node_count_nonzero: TestDependencyGraphPublicAccessors#test_node_count_nonzero().
---
# Module: [`tests/unit/test_project_graph.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py)

## Classes
### `TestBlastRadius`
- def: [`tests/unit/test_project_graph.py:421`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L421)
- doc: Test blast radius / impact analysis.
- signature: `class TestBlastRadius:`
- members:
  - `py_graph(self)` — [`L425`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L425)
  - `radius(self, py_graph)` — [`L431`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L431)
  - `test_blast_radius_forward(self, radius)` — [`L436`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L436) — Changing a leaf file → impact propagates to its dependents.
  - `test_blast_radius_leaf_file_forward(self, radius)` — [`L456`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L456) — Changing utils.py (no internal deps, imported by main) → only main is impacted.
  - `test_blast_radius_nonexistent_file(self, radius)` — [`L463`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L463) — Nonexistent file returns empty set.
  - `test_blast_radius_reverse(self, radius)` — [`L444`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L444) — To understand what influences a file → trace reverse dependencies.
  - `test_blast_radius_to_dict(self, radius)` — [`L468`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L468) — Can serialize blast radius result.
- uses (calls/refs, reference-scoped): [`DependencyGraph`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph), [`BlastRadius`](../../tree_sitter_analyzer/project_graph.md#BlastRadius)  (1 test-only)

### `TestCycleDetection`
- def: [`tests/unit/test_project_graph.py:400`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L400)
- doc: Test circular dependency detection.
- signature: `class TestCycleDetection:`
- members:
  - `py_graph(self)` — [`L404`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L404)
  - `test_detect_cycles(self, py_graph)` — [`L409`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L409) — Should detect the cycle between main.py and pkg/submodule.py.
- uses (calls/refs, reference-scoped): [`DependencyGraph`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph)  (1 test-only)

### `TestDependencyGraph`
- def: [`tests/unit/test_project_graph.py:142`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L142)
- doc: Test DependencyGraph construction and queries.
- signature: `class TestDependencyGraph:`
- members:
  - `js_graph(self)` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L152)
  - `py_graph(self)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L146)
  - `test_build_js_graph(self, js_graph)` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L164) — Graph should contain JS files.
  - `test_build_python_graph(self, py_graph)` — [`L157`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L157) — Graph should contain all .py files in the project.
  - `test_empty_project_handled(self, tmp_path)` — [`L202`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L202) — Empty project directory produces empty graph.
  - `test_get_dependencies_of_file(self, py_graph)` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L170) — Query what a specific file depends on.
  - `test_get_dependents_of_file(self, py_graph)` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L180) — Query what files depend on a specific file.
  - `test_leaf_file_has_no_dependents(self, py_graph)` — [`L188`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L188) — utils.py only has imports from standard library, no internal deps.
  - `test_to_dict_output(self, py_graph)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L194) — Graph can be serialized to dict.
- uses (calls/refs, reference-scoped): [`DependencyGraph`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph), [`nodes`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph.nodes), [`edges`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph.edges)  (2 test-only)

### `TestDependencyGraphCache`
- def: [`tests/unit/test_project_graph.py:481`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L481)
- doc: Test caching behavior.
- signature: `class TestDependencyGraphCache:`
- members:
  - `test_cache_hit_on_rebuild(self, tmp_path)` — [`L484`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L484) — Rebuilding the same project should use cache (fast second build).
- uses (calls/refs, reference-scoped): [`DependencyGraph`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph), [`nodes`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph.nodes), [`edges`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph.edges)

### `TestDependencyGraphPublicAPI`
- def: [`tests/unit/test_project_graph.py:502`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L502)
- doc: T2 — public adjacency API: all_nodes(), all_edges(), all_deps().
- signature: `class TestDependencyGraphPublicAPI:`
- members:
  - `test_all_deps_covers_dependencies_of(self, tiny)` — [`L564`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L564)
  - `test_all_deps_mutation_does_not_affect_graph(self, tiny)` — [`L554`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L554)
  - `test_all_deps_returns_dict(self, tiny)` — [`L546`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L546)
  - `test_all_deps_values_are_sets(self, tiny)` — [`L550`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L550)
  - `test_all_edges_consistent_with_edges(self, tiny)` — [`L537`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L537)
  - `test_all_edges_returns_copy(self, tiny)` — [`L540`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L540)
  - `test_all_edges_returns_frozenset(self, tiny)` — [`L533`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L533)
  - `test_all_nodes_consistent_with_nodes(self, tiny)` — [`L524`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L524)
  - `test_all_nodes_contains_all_files(self, tiny)` — [`L518`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L518)
  - `test_all_nodes_returns_copy(self, tiny)` — [`L527`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L527)
  - `test_all_nodes_returns_frozenset(self, tiny)` — [`L514`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L514)
  - `tiny(self, tmp_path)` — [`L506`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L506)
- uses (calls/refs, reference-scoped): [`DependencyGraph`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph)

### `TestDependencyGraphPublicAccessors`
- def: [`tests/unit/test_project_graph.py:577`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L577)
- doc: TDD: has_node(), node_count(), edge_count() public API.
- signature: `class TestDependencyGraphPublicAccessors:`
- members:
  - `small_graph(self, tmp_path)` — [`L581`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L581)
  - `test_edge_count_matches_edges_length(self, small_graph)` — [`L604`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L604) — edge_count() equals len(edges()).
  - `test_has_node_false_for_missing_node(self, small_graph)` — [`L596`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L596) — has_node() returns False for a file not in the graph.
  - `test_has_node_true_for_existing_node(self, small_graph)` — [`L590`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L590) — has_node() returns True for a file that is in the graph.
  - `test_node_count_matches_nodes_length(self, small_graph)` — [`L600`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L600) — node_count() equals len(nodes()).
  - `test_node_count_nonzero(self, small_graph)` — [`L608`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L608) — A non-empty project has at least one node.
- uses (calls/refs, reference-scoped): [`DependencyGraph`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph)

### `TestImportExtraction`
- def: [`tests/unit/test_project_graph.py:28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L28)
- doc: Test import extraction from source files.
- signature: `class TestImportExtraction:`
- members:
  - `test_extract_cpp_imports_from_main(self)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L109) — main.cpp should yield local includes, not system includes.
  - `test_extract_go_imports_from_main(self)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L83) — main.go should yield imports to internal packages, not stdlib.
  - `test_extract_imports_unsupported_language(self)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L76) — Unsupported language returns empty list.
  - `test_extract_java_imports_from_main(self)` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L121) — Main.java should yield com.example imports, not java.util.
  - `test_extract_js_imports_from_index(self)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L62) — index.js should yield imports to src/utils, src/models/user, src/formatter.
  - `test_extract_python_imports_from_main(self)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L31) — main.py should yield imports to utils, models.user, models.base, pkg.submodule.
  - `test_extract_python_imports_from_utils(self)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L51) — utils.py has no imports → empty list.
  - `test_extract_rust_imports_from_main(self)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L94) — main.rs should yield crate-local imports, not std.
- uses (calls/refs, reference-scoped): [`extract_imports_from_file`](../../tree_sitter_analyzer/project_graph.md#extract_imports_from_file)  (7 test-only)

### `TestSymbolInDegree`
- def: [`tests/unit/test_project_graph.py:218`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L218)
- doc: Test the PR-0.2 `symbol_in_degree()` API.
- signature: `class TestSymbolInDegree:`
- members:
  - `custom_graph(self, tmp_path)` — [`L234`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L234) — Build a small focused project for the cases the PY_PROJECT
  - `py_graph(self)` — [`L228`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L228)
  - `test_G1_dependents_of_unchanged(self, py_graph)` — [`L355`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L355)
  - `test_G2_to_dict_backward_compatible(self, py_graph)` — [`L359`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L359)
  - `test_G3_find_cycles_unchanged(self, py_graph)` — [`L368`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L368)
  - `test_G4_no_self_imports_polluting_count(self, tmp_path)` — [`L373`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L373)
  - `test_R1_simple_fan_in_count(self, custom_graph)` — [`L258`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L258)
  - `test_R2_zero_for_unimported_defined_symbol(self, custom_graph)` — [`L267`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L267)
  - `test_R3_zero_for_unknown_symbol_no_raise(self, custom_graph)` — [`L274`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L274)
  - `test_R4_dedupes_repeated_imports_in_same_file(self, custom_graph)` — [`L283`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L283)
  - `test_R5_ambiguous_when_two_files_define_same_name(self, tmp_path)` — [`L290`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L290)
  - `test_R6_disambiguate_by_defining_file(self, tmp_path)` — [`L301`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L301)
  - `test_R7_relative_import_counts(self, py_graph)` — [`L318`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L318)
  - `test_R8_stdlib_names_not_indexed(self, py_graph)` — [`L326`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L326)
  - `test_R9_js_bare_imports_yield_no_symbol_entry(self, tmp_path)` — [`L335`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L335)
- uses (calls/refs, reference-scoped): [`DependencyGraph`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph), [`symbol_in_degree`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph.symbol_in_degree), [`dependents_of`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph.dependents_of), [`file_count`](../../tree_sitter_analyzer/project_graph.md#SymbolFanIn.file_count), [`defining_files`](../../tree_sitter_analyzer/project_graph.md#SymbolFanIn.defining_files), [`importer_files`](../../tree_sitter_analyzer/project_graph.md#SymbolFanIn.importer_files), [`ambiguous`](../../tree_sitter_analyzer/project_graph.md#SymbolFanIn.ambiguous)  (1 test-only)

## Functions
- `_is_stdlib(import_dict: dict)` — [`L618`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L618) — Check if an import is a stdlib module (heuristic).

## Module values
- `CPP_PROJECT` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L19)
- `FIXTURES_DIR` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L14)
- `GO_PROJECT` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L17)
- `JAVA_PROJECT` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L20)
- `JS_PROJECT` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L16)
- `PY_PROJECT` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L15)
- `RUST_PROJECT` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph.py#L18)

