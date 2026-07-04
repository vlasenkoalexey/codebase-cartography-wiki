---
title: 'Module: tests/unit/test_call_graph_integration.py'
type: catalog
provenance: extracted
module: tests/unit/test_call_graph_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_call_graph_integration`/
symbols:
  PY_PROJECT: PY_PROJECT.
  TestCallGraphBuild.test_build_python_project: TestCallGraphBuild#test_build_python_project().
  TestCallGraphCallersOf.test_callers_of_called_function: TestCallGraphCallersOf#test_callers_of_called_function().
  TestCallGraphCalleesOf.test_callees_of_main: TestCallGraphCalleesOf#test_callees_of_main().
  TestCallChain.test_call_chain_from_main: TestCallChain#test_call_chain_from_main().
  TestCallGraphInternalMethods.test_resolve_callee_same_file: TestCallGraphInternalMethods#test_resolve_callee_same_file().
  TestCallGraphInternalMethods.test_resolve_callee_different_file: TestCallGraphInternalMethods#test_resolve_callee_different_file().
  TestCallGraphInternalMethods.test_resolve_targets_with_file_path: TestCallGraphInternalMethods#test_resolve_targets_with_file_path().
  TestCallGraphInternalMethods.test_resolve_targets_by_name_only: TestCallGraphInternalMethods#test_resolve_targets_by_name_only().
  TestCallGraphBuild.test_build_js_project: TestCallGraphBuild#test_build_js_project().
  TestCallGraphBuild.test_build_c_project: TestCallGraphBuild#test_build_c_project().
  TestCallGraphBuild.test_build_empty_dir: TestCallGraphBuild#test_build_empty_dir().
  TestCallGraphBuild.test_build_idempotent: TestCallGraphBuild#test_build_idempotent().
  TestCallGraphBuild.test_summary: TestCallGraphBuild#test_summary().
  TestCallGraphCallersOf.test_callers_of_uncalled_function: TestCallGraphCallersOf#test_callers_of_uncalled_function().
  TestCallGraphCallersOf.test_callers_with_file_path: TestCallGraphCallersOf#test_callers_with_file_path().
  TestCallGraphCalleesOf.test_callees_leaf_function: TestCallGraphCalleesOf#test_callees_leaf_function().
  TestCallChain.test_call_chain_depth_limit: TestCallChain#test_call_chain_depth_limit().
  TestCallChain.test_call_chain_nonexistent_function: TestCallChain#test_call_chain_nonexistent_function().
  TestCallGraphPythonClassMethods.test_class_method_discovered: TestCallGraphPythonClassMethods#test_class_method_discovered().
  TestCallGraphPythonClassMethods.test_class_method_receiver: TestCallGraphPythonClassMethods#test_class_method_receiver().
  TestCallGraphGoProject.test_go_functions_discovered: TestCallGraphGoProject#test_go_functions_discovered().
  TestCallGraphGoProject.test_go_callees: TestCallGraphGoProject#test_go_callees().
  TestCallGraphJavaProject.test_java_methods_discovered: TestCallGraphJavaProject#test_java_methods_discovered().
  TestCallGraphJavaProject.test_java_callers: TestCallGraphJavaProject#test_java_callers().
  TestCallGraphInternalMethods.test_find_enclosing_func: TestCallGraphInternalMethods#test_find_enclosing_func().
  TestCallGraphInternalMethods.test_find_enclosing_func_tightest: TestCallGraphInternalMethods#test_find_enclosing_func_tightest().
  TestCallGraphInternalMethods.test_find_enclosing_func_no_match: TestCallGraphInternalMethods#test_find_enclosing_func_no_match().
  TestCallGraphPublicAdjacencyAPI.test_all_function_refs_returns_function_refs: TestCallGraphPublicAdjacencyAPI#test_all_function_refs_returns_function_refs().
  TestCallGraphPublicAdjacencyAPI.test_all_function_refs_count_matches_all_functions: TestCallGraphPublicAdjacencyAPI#test_all_function_refs_count_matches_all_functions().
  TestCallGraphPublicAdjacencyAPI.test_callers_map_returns_dict: TestCallGraphPublicAdjacencyAPI#test_callers_map_returns_dict().
  TestCallGraphPublicAdjacencyAPI.test_callees_map_returns_dict: TestCallGraphPublicAdjacencyAPI#test_callees_map_returns_dict().
  TestCallGraphPublicAdjacencyAPI.test_functions_by_file_keys_are_strings: TestCallGraphPublicAdjacencyAPI#test_functions_by_file_keys_are_strings().
  TestCallGraphPublicAdjacencyAPI.test_resolve_targets_returns_function_refs: TestCallGraphPublicAdjacencyAPI#test_resolve_targets_returns_function_refs().
  TestCallGraphPublicAdjacencyAPI.test_resolve_targets_consistent_with_callers_of: TestCallGraphPublicAdjacencyAPI#test_resolve_targets_consistent_with_callers_of().
  TestCallGraphAllCallEdges.test_all_call_edges_returns_list: TestCallGraphAllCallEdges#test_all_call_edges_returns_list().
  TestCallGraphAllCallEdges.test_all_call_edges_triggers_build: TestCallGraphAllCallEdges#test_all_call_edges_triggers_build().
  TestCallGraphAllCallEdges.test_all_call_edges_count_matches_summary: TestCallGraphAllCallEdges#test_all_call_edges_count_matches_summary().
  TestCallGraphGoProject.test_go_method_selector_callees: TestCallGraphGoProject#test_go_method_selector_callees().
  TestCallGraphInternalMethods.test_resolve_callee_no_match: TestCallGraphInternalMethods#test_resolve_callee_no_match().
  TestCallGraphInternalMethods.test_is_excluded: TestCallGraphInternalMethods#test_is_excluded().
  TestCallGraphInternalMethods.test_resolve_targets_no_match: TestCallGraphInternalMethods#test_resolve_targets_no_match().
  TestCallGraphPublicAdjacencyAPI.test_all_function_refs_returns_copy: TestCallGraphPublicAdjacencyAPI#test_all_function_refs_returns_copy().
  TestCallGraphPublicAdjacencyAPI.test_callers_map_returns_copy: TestCallGraphPublicAdjacencyAPI#test_callers_map_returns_copy().
  TestCallGraphPublicAdjacencyAPI.test_callees_map_returns_copy: TestCallGraphPublicAdjacencyAPI#test_callees_map_returns_copy().
  TestCallGraphPublicAdjacencyAPI.test_functions_by_file_returns_copy: TestCallGraphPublicAdjacencyAPI#test_functions_by_file_returns_copy().
  TestCallGraphPublicAdjacencyAPI.test_resolve_targets_returns_empty_for_unknown: TestCallGraphPublicAdjacencyAPI#test_resolve_targets_returns_empty_for_unknown().
  TestCallGraphAllCallEdges.test_all_call_edges_returns_copy: TestCallGraphAllCallEdges#test_all_call_edges_returns_copy().
  FIXTURES_DIR: FIXTURES_DIR.
  TestCallGraphInternalMethods.test_iter_source_files_prunes_hidden_and_generated_dirs: TestCallGraphInternalMethods#test_iter_source_files_prunes_hidden_and_generated_dirs().
  JAVA_PROJECT: JAVA_PROJECT.
  GO_PROJECT: GO_PROJECT.
  JS_PROJECT: JS_PROJECT.
  C_PROJECT: C_PROJECT.
  _WINDOWS_SKIP_PY_FIXTURE: _WINDOWS_SKIP_PY_FIXTURE.
  TestCallGraphBuild: TestCallGraphBuild#
  TestCallGraphCallersOf: TestCallGraphCallersOf#
  TestCallGraphCalleesOf: TestCallGraphCalleesOf#
  TestCallChain: TestCallChain#
  TestCallGraphPythonClassMethods: TestCallGraphPythonClassMethods#
  TestCallGraphGoProject: TestCallGraphGoProject#
  TestCallGraphJavaProject: TestCallGraphJavaProject#
  TestCallGraphInternalMethods: TestCallGraphInternalMethods#
  TestCallGraphPublicAdjacencyAPI: TestCallGraphPublicAdjacencyAPI#
  TestCallGraphAllCallEdges: TestCallGraphAllCallEdges#
---
# Module: [`tests/unit/test_call_graph_integration.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py)

## Classes
### `TestCallChain`
- def: [`tests/unit/test_call_graph_integration.py:128`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L128)
- signature: `class TestCallChain:`
- members:
  - `test_call_chain_depth_limit(self)` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L141)
  - `test_call_chain_from_main(self)` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L130)
  - `test_call_chain_nonexistent_function(self)` — [`L148`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L148)
- uses (calls/refs, reference-scoped): [`CallGraph`](../../tree_sitter_analyzer/call_graph.md#CallGraph), [`build`](../../tree_sitter_analyzer/call_graph.md#CallGraph.build), [`call_chain`](../../tree_sitter_analyzer/call_graph.md#CallGraph.call_chain)  (2 test-only)

### `TestCallGraphAllCallEdges`
- def: [`tests/unit/test_call_graph_integration.py:412`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L412)
- signature: `class TestCallGraphAllCallEdges:`
- members:
  - `test_all_call_edges_count_matches_summary(self)` — [`L431`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L431) — all_call_edges() count must match the summary call_edge_count.
  - `test_all_call_edges_returns_copy(self)` — [`L438`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L438) — Mutating the returned list must not affect the internal state.
  - `test_all_call_edges_returns_list(self)` — [`L413`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L413) — all_call_edges() must return a list of 3-tuples.
  - `test_all_call_edges_triggers_build(self)` — [`L423`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L423) — all_call_edges() must build the graph if not yet built.
- uses (calls/refs, reference-scoped): [`FunctionRef`](../../tree_sitter_analyzer/call_graph.md#FunctionRef), [`CallGraph`](../../tree_sitter_analyzer/call_graph.md#CallGraph), [`all_functions`](../../tree_sitter_analyzer/call_graph.md#CallGraph.all_functions), [`summary`](../../tree_sitter_analyzer/call_graph.md#CallGraph.summary), [`all_call_edges`](../../tree_sitter_analyzer/call_graph.md#CallGraph.all_call_edges)  (1 test-only)

### `TestCallGraphBuild`
- def: [`tests/unit/test_call_graph_integration.py:38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L38)
- signature: `class TestCallGraphBuild:`
- members:
  - `test_build_c_project(self)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L57)
  - `test_build_empty_dir(self, tmp_path)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L65)
  - `test_build_idempotent(self)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L71)
  - `test_build_js_project(self)` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L50)
  - `test_build_python_project(self)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L39)
  - `test_summary(self)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L79)
- uses (calls/refs, reference-scoped): [`CallGraph`](../../tree_sitter_analyzer/call_graph.md#CallGraph), [`build`](../../tree_sitter_analyzer/call_graph.md#CallGraph.build), [`all_functions`](../../tree_sitter_analyzer/call_graph.md#CallGraph.all_functions), [`summary`](../../tree_sitter_analyzer/call_graph.md#CallGraph.summary), [`is_built`](../../tree_sitter_analyzer/call_graph.md#CallGraph.is_built)  (3 test-only)

### `TestCallGraphCalleesOf`
- def: [`tests/unit/test_call_graph_integration.py:110`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L110)
- signature: `class TestCallGraphCalleesOf:`
- members:
  - `test_callees_leaf_function(self)` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L121)
  - `test_callees_of_main(self)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L112)
- uses (calls/refs, reference-scoped): [`CallGraph`](../../tree_sitter_analyzer/call_graph.md#CallGraph), [`build`](../../tree_sitter_analyzer/call_graph.md#CallGraph.build), [`callees_of`](../../tree_sitter_analyzer/call_graph.md#CallGraph.callees_of)  (2 test-only)

### `TestCallGraphCallersOf`
- def: [`tests/unit/test_call_graph_integration.py:88`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L88)
- signature: `class TestCallGraphCallersOf:`
- members:
  - `test_callers_of_called_function(self)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L90)
  - `test_callers_of_uncalled_function(self)` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L97)
  - `test_callers_with_file_path(self)` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L103)
- uses (calls/refs, reference-scoped): [`CallGraph`](../../tree_sitter_analyzer/call_graph.md#CallGraph), [`build`](../../tree_sitter_analyzer/call_graph.md#CallGraph.build), [`callers_of`](../../tree_sitter_analyzer/call_graph.md#CallGraph.callers_of)  (2 test-only)

### `TestCallGraphGoProject`
- def: [`tests/unit/test_call_graph_integration.py:176`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L176)
- signature: `class TestCallGraphGoProject:`
- members:
  - `test_go_callees(self)` — [`L186`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L186)
  - `test_go_functions_discovered(self)` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L177)
  - `test_go_method_selector_callees(self, tmp_path)` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L193)
- uses (calls/refs, reference-scoped): [`CallGraph`](../../tree_sitter_analyzer/call_graph.md#CallGraph), [`build`](../../tree_sitter_analyzer/call_graph.md#CallGraph.build), [`callees_of`](../../tree_sitter_analyzer/call_graph.md#CallGraph.callees_of), [`all_functions`](../../tree_sitter_analyzer/call_graph.md#CallGraph.all_functions)  (1 test-only)

### `TestCallGraphInternalMethods`
- def: [`tests/unit/test_call_graph_integration.py:226`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L226)
- signature: `class TestCallGraphInternalMethods:`
- members:
  - `test_find_enclosing_func(self)` — [`L227`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L227)
  - `test_find_enclosing_func_no_match(self)` — [`L245`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L245)
  - `test_find_enclosing_func_tightest(self)` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L236)
  - `test_is_excluded(self)` — [`L275`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L275)
  - `test_iter_source_files_prunes_hidden_and_generated_dirs(self, tmp_path)` — [`L281`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L281)
  - `test_resolve_callee_different_file(self)` — [`L261`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L261)
  - `test_resolve_callee_no_match(self)` — [`L269`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L269)
  - `test_resolve_callee_same_file(self)` — [`L252`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L252)
  - `test_resolve_targets_by_name_only(self)` — [`L308`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L308)
  - `test_resolve_targets_no_match(self)` — [`L315`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L315)
  - `test_resolve_targets_with_file_path(self)` — [`L300`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L300)
- uses (calls/refs, reference-scoped): [`FunctionRef`](../../tree_sitter_analyzer/call_graph.md#FunctionRef), [`CallGraph`](../../tree_sitter_analyzer/call_graph.md#CallGraph), [`resolve_targets`](../../tree_sitter_analyzer/call_graph.md#CallGraph.resolve_targets), [`_func_by_name`](../../tree_sitter_analyzer/call_graph.md#CallGraph._func_by_name), [`find_enclosing_func`](../../tree_sitter_analyzer/call_graph.md#CallGraph.find_enclosing_func), [`resolve_callee`](../../tree_sitter_analyzer/call_graph.md#CallGraph.resolve_callee), [`_func_by_qualified`](../../tree_sitter_analyzer/call_graph.md#CallGraph._func_by_qualified), [`is_excluded`](../../tree_sitter_analyzer/call_graph.md#CallGraph.is_excluded), [`iter_source_files`](../../tree_sitter_analyzer/call_graph.md#CallGraph.iter_source_files)  (1 test-only)

### `TestCallGraphJavaProject`
- def: [`tests/unit/test_call_graph_integration.py:211`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L211)
- signature: `class TestCallGraphJavaProject:`
- members:
  - `test_java_callers(self)` — [`L219`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L219)
  - `test_java_methods_discovered(self)` — [`L212`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L212)
- uses (calls/refs, reference-scoped): [`CallGraph`](../../tree_sitter_analyzer/call_graph.md#CallGraph), [`build`](../../tree_sitter_analyzer/call_graph.md#CallGraph.build), [`callers_of`](../../tree_sitter_analyzer/call_graph.md#CallGraph.callers_of), [`all_functions`](../../tree_sitter_analyzer/call_graph.md#CallGraph.all_functions)  (1 test-only)

### `TestCallGraphPublicAdjacencyAPI`
- def: [`tests/unit/test_call_graph_integration.py:321`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L321)
- doc: Tests for the public API surface that replaces direct _callers/_callees/_functions access.
- signature: `class TestCallGraphPublicAdjacencyAPI:`
- members:
  - `test_all_function_refs_count_matches_all_functions(self)` — [`L338`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L338)
  - `test_all_function_refs_returns_copy(self)` — [`L331`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L331)
  - `test_all_function_refs_returns_function_refs(self)` — [`L324`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L324)
  - `test_callees_map_returns_copy(self)` — [`L365`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L365)
  - `test_callees_map_returns_dict(self)` — [`L357`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L357)
  - `test_callers_map_returns_copy(self)` — [`L350`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L350)
  - `test_callers_map_returns_dict(self)` — [`L342`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L342)
  - `test_functions_by_file_keys_are_strings(self)` — [`L372`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L372)
  - `test_functions_by_file_returns_copy(self)` — [`L382`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L382)
  - `test_resolve_targets_consistent_with_callers_of(self)` — [`L402`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L402) — resolve_targets results should match what callers_of uses internally.
  - `test_resolve_targets_returns_empty_for_unknown(self)` — [`L397`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L397)
  - `test_resolve_targets_returns_function_refs(self)` — [`L389`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L389)
- uses (calls/refs, reference-scoped): [`FunctionRef`](../../tree_sitter_analyzer/call_graph.md#FunctionRef), [`CallGraph`](../../tree_sitter_analyzer/call_graph.md#CallGraph), [`callers_of`](../../tree_sitter_analyzer/call_graph.md#CallGraph.callers_of), [`all_functions`](../../tree_sitter_analyzer/call_graph.md#CallGraph.all_functions), [`resolve_targets`](../../tree_sitter_analyzer/call_graph.md#CallGraph.resolve_targets), [`all_function_refs`](../../tree_sitter_analyzer/call_graph.md#CallGraph.all_function_refs), [`callees_map`](../../tree_sitter_analyzer/call_graph.md#CallGraph.callees_map), [`callers_map`](../../tree_sitter_analyzer/call_graph.md#CallGraph.callers_map), [`functions_by_file`](../../tree_sitter_analyzer/call_graph.md#CallGraph.functions_by_file)  (1 test-only)

### `TestCallGraphPythonClassMethods`
- def: [`tests/unit/test_call_graph_integration.py:155`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L155)
- signature: `class TestCallGraphPythonClassMethods:`
- members:
  - `test_class_method_discovered(self)` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L156)
  - `test_class_method_receiver(self)` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L163)
- uses (calls/refs, reference-scoped): [`CallGraph`](../../tree_sitter_analyzer/call_graph.md#CallGraph), [`build`](../../tree_sitter_analyzer/call_graph.md#CallGraph.build), [`all_functions`](../../tree_sitter_analyzer/call_graph.md#CallGraph.all_functions)  (1 test-only)

## Module values
- `C_PROJECT` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L30)
- `FIXTURES_DIR` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L25)
- `GO_PROJECT` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L29)
- `JAVA_PROJECT` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L28)
- `JS_PROJECT` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L27)
- `PY_PROJECT` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L26)
- `_WINDOWS_SKIP_PY_FIXTURE` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_integration.py#L21)

