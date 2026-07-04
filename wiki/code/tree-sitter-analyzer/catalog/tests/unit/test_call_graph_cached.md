---
title: 'Module: tests/unit/test_call_graph_cached.py'
type: catalog
provenance: extracted
module: tests/unit/test_call_graph_cached.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_call_graph_cached`/
symbols:
  TestCallEdgesPublicAccessor.test_call_edges_returns_list: TestCallEdgesPublicAccessor#test_call_edges_returns_list().
  TestCallGraphInternalAccessors.test_callee_refs_of_returns_list: TestCallGraphInternalAccessors#test_callee_refs_of_returns_list().
  TestCallGraphInternalAccessors.test_caller_refs_of_returns_list: TestCallGraphInternalAccessors#test_caller_refs_of_returns_list().
  _parse_source: _parse_source().
  TestCallEdgesPublicAccessor.test_call_edges_matches_private_attribute: TestCallEdgesPublicAccessor#test_call_edges_matches_private_attribute().
  TestCallEdgesPublicAccessor.test_call_edges_returns_tuples: TestCallEdgesPublicAccessor#test_call_edges_returns_tuples().
  TestCallGraphInternalAccessors.test_function_refs_returns_function_ref_objects: TestCallGraphInternalAccessors#test_function_refs_returns_function_ref_objects().
  TestCallGraphInternalAccessors.test_function_refs_same_as_private_functions: TestCallGraphInternalAccessors#test_function_refs_same_as_private_functions().
  TestCallGraphInternalAccessors.test_callee_refs_of_unknown_func_returns_empty: TestCallGraphInternalAccessors#test_callee_refs_of_unknown_func_returns_empty().
  TestCallGraphInternalAccessors.test_caller_refs_of_unknown_func_returns_empty: TestCallGraphInternalAccessors#test_caller_refs_of_unknown_func_returns_empty().
  TestCallGraphInternalAccessors._two_func_cache: TestCallGraphInternalAccessors#_two_func_cache().
  TestCachedCallGraphImportResolution.test_same_file_resolution: TestCachedCallGraphImportResolution#test_same_file_resolution().
  TestCachedCallGraphImportResolution.test_cross_file_import_resolution: TestCachedCallGraphImportResolution#test_cross_file_import_resolution().
  TestCachedCallGraphImportResolution.test_dotted_callee_resolution: TestCachedCallGraphImportResolution#test_dotted_callee_resolution().
  TestCachedCallGraphImportResolution.test_fallback_to_first_candidate: TestCachedCallGraphImportResolution#test_fallback_to_first_candidate().
  TestCachedCallGraphImportResolution.test_empty_cache_falls_back: TestCachedCallGraphImportResolution#test_empty_cache_falls_back().
  TestCachedCallGraphImportResolution.test_no_fallback_skips_parse: TestCachedCallGraphImportResolution#test_no_fallback_skips_parse().
  TestCachedCallGraphImportResolution.test_reverse_callers: TestCachedCallGraphImportResolution#test_reverse_callers().
  TestCachedCallGraphImportResolution.test_cache_passes_end_line: TestCachedCallGraphImportResolution#test_cache_passes_end_line().
  TestFileImpact.test_file_impact_basic: TestFileImpact#test_file_impact_basic().
  TestFileImpact.test_file_impact_returns_upstream_downstream: TestFileImpact#test_file_impact_returns_upstream_downstream().
  TestFileImpact.test_file_impact_nonexistent_file: TestFileImpact#test_file_impact_nonexistent_file().
  PY_PROJECT: PY_PROJECT.
  TestFindEnclosingFuncRange.test_range_containment: TestFindEnclosingFuncRange#test_range_containment().
  TestFindEnclosingFuncRange.test_range_picks_tighter_scope: TestFindEnclosingFuncRange#test_range_picks_tighter_scope().
  TestFindEnclosingFuncRange.test_module_level_gap_returns_none: TestFindEnclosingFuncRange#test_module_level_gap_returns_none().
  TestCachedCallGraphImportResolution._make_mock_cache: TestCachedCallGraphImportResolution#_make_mock_cache().
  TestFunctionRefEndLine.test_to_dict_includes_end_line: TestFunctionRefEndLine#test_to_dict_includes_end_line().
  TestNodeTextUtf8.test_node_text_multibyte_comment_before_func: TestNodeTextUtf8#test_node_text_multibyte_comment_before_func().
  TestNodeTextUtf8.test_node_text_cjk_identifier: TestNodeTextUtf8#test_node_text_cjk_identifier().
  TestNodeTextUtf8.test_extract_call_after_multibyte: TestNodeTextUtf8#test_extract_call_after_multibyte().
  TestFunctionRefEndLine.test_end_line_defaults_to_start: TestFunctionRefEndLine#test_end_line_defaults_to_start().
  TestFunctionRefEndLine.test_end_line_explicit: TestFunctionRefEndLine#test_end_line_explicit().
  TestNodeTextUtf8.test_node_text_none_returns_empty: TestNodeTextUtf8#test_node_text_none_returns_empty().
  TestCallEdgesPublicAccessor._make_mock_cache: TestCallEdgesPublicAccessor#_make_mock_cache().
  FIXTURES_DIR: FIXTURES_DIR.
  TestCallGraphInternalAccessors: TestCallGraphInternalAccessors#
  TestCallGraphInternalAccessors._make_mock_cache: TestCallGraphInternalAccessors#_make_mock_cache().
  TestCachedCallGraphImportResolution: TestCachedCallGraphImportResolution#
  TestFunctionRefEndLine: TestFunctionRefEndLine#
  TestFindEnclosingFuncRange: TestFindEnclosingFuncRange#
  TestFileImpact: TestFileImpact#
  TestNodeTextUtf8: TestNodeTextUtf8#
  TestCallEdgesPublicAccessor: TestCallEdgesPublicAccessor#
---
# Module: [`tests/unit/test_call_graph_cached.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py)

## Classes
### `TestCachedCallGraphImportResolution`
- def: [`tests/unit/test_call_graph_cached.py:35`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L35)
- doc: Tests for import-aware cross-file resolution in CachedCallGraph.
- signature: `class TestCachedCallGraphImportResolution:`
- members:
  - `test_cache_passes_end_line(self)` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L193)
  - `test_cross_file_import_resolution(self)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L73)
  - `test_dotted_callee_resolution(self)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L99)
  - `test_empty_cache_falls_back(self)` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L152)
  - `test_fallback_to_first_candidate(self)` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L125)
  - `test_no_fallback_skips_parse(self)` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L161)
  - `test_reverse_callers(self)` — [`L169`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L169)
  - `test_same_file_resolution(self)` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L50)
- protocol/private: `_make_mock_cache`[`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L39)
- uses (calls/refs, reference-scoped): [`CachedCallGraph`](../../tree_sitter_analyzer/call_graph.md#CachedCallGraph), [`build`](../../tree_sitter_analyzer/call_graph.md#CachedCallGraph.build), [`callees_of`](../../tree_sitter_analyzer/call_graph.md#CallGraph.callees_of), [`callers_of`](../../tree_sitter_analyzer/call_graph.md#CallGraph.callers_of), [`all_functions`](../../tree_sitter_analyzer/call_graph.md#CallGraph.all_functions), [`is_built`](../../tree_sitter_analyzer/call_graph.md#CallGraph.is_built)  (1 test-only)

### `TestCallEdgesPublicAccessor`
- def: [`tests/unit/test_call_graph_cached.py:348`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L348)
- doc: call_edges() must expose the same data as the private _call_edges.
- signature: `class TestCallEdgesPublicAccessor:`
- members:
  - `test_call_edges_matches_private_attribute(self)` — [`L371`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L371) — call_edges() must return the edges that were built (data contract).
  - `test_call_edges_returns_list(self)` — [`L359`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L359) — call_edges() must return a list (not None).
  - `test_call_edges_returns_tuples(self)` — [`L408`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L408) — Each entry must be a (FunctionRef, FunctionRef, int) tuple.
- protocol/private: `_make_mock_cache`[`L352`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L352)
- uses (calls/refs, reference-scoped): [`FunctionRef`](../../tree_sitter_analyzer/call_graph.md#FunctionRef), [`CallGraph`](../../tree_sitter_analyzer/call_graph.md#CallGraph), [`CachedCallGraph`](../../tree_sitter_analyzer/call_graph.md#CachedCallGraph), [`build`](../../tree_sitter_analyzer/call_graph.md#CachedCallGraph.build), [`_func_by_name`](../../tree_sitter_analyzer/call_graph.md#CallGraph._func_by_name), [`call_edges`](../../tree_sitter_analyzer/call_graph.md#CallGraph.call_edges), [`_functions`](../../tree_sitter_analyzer/call_graph.md#CallGraph._functions), [`_call_edges`](../../tree_sitter_analyzer/call_graph.md#CallGraph._call_edges), [`_built`](../../tree_sitter_analyzer/call_graph.md#CallGraph._built)

### `TestCallGraphInternalAccessors`
- def: [`tests/unit/test_call_graph_cached.py:456`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L456)
- doc: function_refs(), callees_of(), callers_of() must expose FunctionRef data.
- signature: `class TestCallGraphInternalAccessors:`
- members:
  - `test_callee_refs_of_returns_list(self)` — [`L517`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L517) — callee_refs_of(func) must return the callees of a given FunctionRef.
  - `test_callee_refs_of_unknown_func_returns_empty(self)` — [`L541`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L541) — callee_refs_of(unknown) must return empty list, not raise.
  - `test_caller_refs_of_returns_list(self)` — [`L529`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L529) — caller_refs_of(func) must return the callers of a given FunctionRef.
  - `test_caller_refs_of_unknown_func_returns_empty(self)` — [`L549`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L549) — caller_refs_of(unknown) must return empty list, not raise.
  - `test_function_refs_returns_function_ref_objects(self)` — [`L497`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L497) — function_refs() must return FunctionRef objects (not dicts).
  - `test_function_refs_same_as_private_functions(self)` — [`L507`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L507) — function_refs() must return the functions that were built (data contract).
- protocol/private: `_make_mock_cache`[`L460`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L460), `_two_func_cache`[`L468`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L468)
- uses (calls/refs, reference-scoped): [`FunctionRef`](../../tree_sitter_analyzer/call_graph.md#FunctionRef), [`CachedCallGraph`](../../tree_sitter_analyzer/call_graph.md#CachedCallGraph), [`build`](../../tree_sitter_analyzer/call_graph.md#CachedCallGraph.build), [`caller_refs_of`](../../tree_sitter_analyzer/call_graph.md#CallGraph.caller_refs_of), [`callee_refs_of`](../../tree_sitter_analyzer/call_graph.md#CallGraph.callee_refs_of), [`function_refs`](../../tree_sitter_analyzer/call_graph.md#CallGraph.function_refs)

### `TestFileImpact`
- def: [`tests/unit/test_call_graph_cached.py:272`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L272)
- signature: `class TestFileImpact:`
- members:
  - `test_file_impact_basic(self)` — [`L273`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L273)
  - `test_file_impact_nonexistent_file(self)` — [`L288`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L288)
  - `test_file_impact_returns_upstream_downstream(self)` — [`L279`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L279)
- uses (calls/refs, reference-scoped): [`CallGraph`](../../tree_sitter_analyzer/call_graph.md#CallGraph), [`build`](../../tree_sitter_analyzer/call_graph.md#CallGraph.build), [`file_impact`](../../tree_sitter_analyzer/call_graph.md#CallGraph.file_impact), [`functions_in_file`](../../tree_sitter_analyzer/call_graph.md#CallGraph.functions_in_file)  (1 test-only)

### `TestFindEnclosingFuncRange`
- def: [`tests/unit/test_call_graph_cached.py:236`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L236)
- signature: `class TestFindEnclosingFuncRange:`
- members:
  - `test_module_level_gap_returns_none(self)` — [`L252`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L252) — A call between two non-overlapping functions has no enclosing function.
  - `test_range_containment(self)` — [`L237`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L237)
  - `test_range_picks_tighter_scope(self)` — [`L244`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L244)
- uses (calls/refs, reference-scoped): [`FunctionRef`](../../tree_sitter_analyzer/call_graph.md#FunctionRef), [`CallGraph`](../../tree_sitter_analyzer/call_graph.md#CallGraph), [`find_enclosing_func`](../../tree_sitter_analyzer/call_graph.md#CallGraph.find_enclosing_func)

### `TestFunctionRefEndLine`
- def: [`tests/unit/test_call_graph_cached.py:216`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L216)
- signature: `class TestFunctionRefEndLine:`
- members:
  - `test_end_line_defaults_to_start(self)` — [`L217`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L217)
  - `test_end_line_explicit(self)` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L221)
  - `test_to_dict_includes_end_line(self)` — [`L225`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L225)
- uses (calls/refs, reference-scoped): [`FunctionRef`](../../tree_sitter_analyzer/call_graph.md#FunctionRef), [`to_dict`](../../tree_sitter_analyzer/call_graph.md#FunctionRef.to_dict)

### `TestNodeTextUtf8`
- def: [`tests/unit/test_call_graph_cached.py:302`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L302)
- signature: `class TestNodeTextUtf8:`
- members:
  - `test_extract_call_after_multibyte(self)` — [`L331`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L331)
  - `test_node_text_cjk_identifier(self)` — [`L317`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L317)
  - `test_node_text_multibyte_comment_before_func(self)` — [`L303`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L303)
  - `test_node_text_none_returns_empty(self)` — [`L338`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L338)
- uses (calls/refs, reference-scoped): [`walk_tree`](../../tree_sitter_analyzer/function_extraction.md#walk_tree), [`node_text`](../../tree_sitter_analyzer/function_extraction.md#node_text)  (1 test-only)

## Functions
- `_parse_source(source: str, language: str)` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L23)

## Module values
- `FIXTURES_DIR` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L19)
- `PY_PROJECT` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_cached.py#L20)

