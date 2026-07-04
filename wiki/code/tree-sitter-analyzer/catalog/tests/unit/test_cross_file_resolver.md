---
title: 'Module: tests/unit/test_cross_file_resolver.py'
type: catalog
provenance: extracted
module: tests/unit/test_cross_file_resolver.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_cross_file_resolver`/
symbols:
  TestDataclassSerialization.test_resolved_edge_to_dict: TestDataclassSerialization#test_resolved_edge_to_dict().
  TestDataclassSerialization.test_import_entry_to_dict: TestDataclassSerialization#test_import_entry_to_dict().
  TestDataclassSerialization.test_function_def_key: TestDataclassSerialization#test_function_def_key().
  TestCrossFileResolverBuild.test_import_index_populated: TestCrossFileResolverBuild#test_import_index_populated().
  multi_file_project: multi_file_project().
  TestCrossFileResolverBuild.test_module_map_populated: TestCrossFileResolverBuild#test_module_map_populated().
  TestCrossFileResolverBuild.test_function_index_populated: TestCrossFileResolverBuild#test_function_index_populated().
  TestCrossFileResolution.test_resolve_same_file_callee: TestCrossFileResolution#test_resolve_same_file_callee().
  TestCrossFileResolution.test_resolve_imported_callee: TestCrossFileResolution#test_resolve_imported_callee().
  TestCrossFileResolution.test_resolve_callee_with_confidence: TestCrossFileResolution#test_resolve_callee_with_confidence().
  TestCrossFileResolution.test_resolve_cross_file_via_import: TestCrossFileResolution#test_resolve_cross_file_via_import().
  TestCrossFileResolution.test_find_caller_function: TestCrossFileResolution#test_find_caller_function().
  TestCrossFileResolution.test_find_caller_function_top_level: TestCrossFileResolution#test_find_caller_function_top_level().
  TestCrossFileResolution.test_find_caller_function_past_end: TestCrossFileResolution#test_find_caller_function_past_end().
  TestCrossFileResolution.test_find_caller_function_unknown_file: TestCrossFileResolution#test_find_caller_function_unknown_file().
  TestResolveCallEdges.test_resolved_edges_have_confidence: TestResolveCallEdges#test_resolved_edges_have_confidence().
  TestResolveCallEdges.test_resolved_edges_to_dict: TestResolveCallEdges#test_resolved_edges_to_dict().
  TestCrossFileResolverBuild.test_build_does_not_crash: TestCrossFileResolverBuild#test_build_does_not_crash().
  TestResolveCallEdges.test_resolve_edges_does_not_crash: TestResolveCallEdges#test_resolve_edges_does_not_crash().
  TestCrossFileResolverBuild: TestCrossFileResolverBuild#
  TestCrossFileResolution: TestCrossFileResolution#
  TestResolveCallEdges: TestResolveCallEdges#
  TestASTCacheEnhancedQueries: TestASTCacheEnhancedQueries#
  TestASTCacheEnhancedQueries.test_query_callers_enhanced: TestASTCacheEnhancedQueries#test_query_callers_enhanced().
  TestASTCacheEnhancedQueries.test_query_callees_enhanced: TestASTCacheEnhancedQueries#test_query_callees_enhanced().
  TestASTCacheEnhancedQueries.test_query_callers_enhanced_empty: TestASTCacheEnhancedQueries#test_query_callers_enhanced_empty().
  TestASTCacheEnhancedQueries.test_get_cross_file_resolver: TestASTCacheEnhancedQueries#test_get_cross_file_resolver().
  TestDataclassSerialization: TestDataclassSerialization#
---
# Module: [`tests/unit/test_cross_file_resolver.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py)

## Classes
### `TestASTCacheEnhancedQueries`
- def: [`tests/unit/test_cross_file_resolver.py:191`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L191)
- signature: `class TestASTCacheEnhancedQueries:`
- members:
  - `test_get_cross_file_resolver(self, multi_file_project)` — [`L212`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L212)
  - `test_query_callees_enhanced(self, multi_file_project)` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L200)
  - `test_query_callers_enhanced(self, multi_file_project)` — [`L192`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L192)
  - `test_query_callers_enhanced_empty(self, multi_file_project)` — [`L207`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L207)

### `TestCrossFileResolution`
- def: [`tests/unit/test_cross_file_resolver.py:102`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L102)
- signature: `class TestCrossFileResolution:`
- members:
  - `test_find_caller_function(self, multi_file_project)` — [`L136`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L136)
  - `test_find_caller_function_past_end(self, multi_file_project)` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L150)
  - `test_find_caller_function_top_level(self, multi_file_project)` — [`L143`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L143)
  - `test_find_caller_function_unknown_file(self, multi_file_project)` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L158)
  - `test_resolve_callee_with_confidence(self, multi_file_project)` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L120)
  - `test_resolve_cross_file_via_import(self, multi_file_project)` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L128)
  - `test_resolve_imported_callee(self, multi_file_project)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L112)
  - `test_resolve_same_file_callee(self, multi_file_project)` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L103)
- uses (calls/refs, reference-scoped): [`build`](../../tree_sitter_analyzer/cross_file_resolver.md#CrossFileResolver.build), [`find_caller_function`](../../tree_sitter_analyzer/cross_file_resolver.md#CrossFileResolver.find_caller_function), [`CrossFileResolver`](../../tree_sitter_analyzer/cross_file_resolver.md#CrossFileResolver), [`resolve_callee`](../../tree_sitter_analyzer/cross_file_resolver.md#CrossFileResolver.resolve_callee)

### `TestCrossFileResolverBuild`
- def: [`tests/unit/test_cross_file_resolver.py:69`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L69)
- signature: `class TestCrossFileResolverBuild:`
- members:
  - `test_build_does_not_crash(self, multi_file_project)` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L70)
  - `test_function_index_populated(self, multi_file_project)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L83)
  - `test_import_index_populated(self, multi_file_project)` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L91)
  - `test_module_map_populated(self, multi_file_project)` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L75)
- uses (calls/refs, reference-scoped): [`build`](../../tree_sitter_analyzer/cross_file_resolver.md#CrossFileResolver.build), [`_module_to_file`](../../tree_sitter_analyzer/cross_file_resolver.md#CrossFileResolver._module_to_file), [`CrossFileResolver`](../../tree_sitter_analyzer/cross_file_resolver.md#CrossFileResolver), [`module_path`](../../tree_sitter_analyzer/cross_file_resolver.md#ImportEntry.module_path), [`_functions_by_name`](../../tree_sitter_analyzer/cross_file_resolver.md#CrossFileResolver._functions_by_name), [`_imports_by_file`](../../tree_sitter_analyzer/cross_file_resolver.md#CrossFileResolver._imports_by_file)

### `TestDataclassSerialization`
- def: [`tests/unit/test_cross_file_resolver.py:220`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L220)
- signature: `class TestDataclassSerialization:`
- members:
  - `test_function_def_key(self)` — [`L234`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L234)
  - `test_import_entry_to_dict(self)` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L221)
  - `test_resolved_edge_to_dict(self)` — [`L244`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L244)
- uses (calls/refs, reference-scoped): [`to_dict`](../../tree_sitter_analyzer/cross_file_resolver.md#ResolvedEdge.to_dict), [`to_dict`](../../tree_sitter_analyzer/cross_file_resolver.md#ImportEntry.to_dict), [`ImportEntry`](../../tree_sitter_analyzer/cross_file_resolver.md#ImportEntry), [`line`](../../tree_sitter_analyzer/cross_file_resolver.md#FunctionDef.line), [`module_path`](../../tree_sitter_analyzer/cross_file_resolver.md#ImportEntry.module_path), [`key`](../../tree_sitter_analyzer/cross_file_resolver.md#FunctionDef.key), [`imported_names`](../../tree_sitter_analyzer/cross_file_resolver.md#ImportEntry.imported_names), [`is_relative`](../../tree_sitter_analyzer/cross_file_resolver.md#ImportEntry.is_relative), [`language`](../../tree_sitter_analyzer/cross_file_resolver.md#ImportEntry.language), [`source_file`](../../tree_sitter_analyzer/cross_file_resolver.md#ImportEntry.source_file), [`FunctionDef`](../../tree_sitter_analyzer/cross_file_resolver.md#FunctionDef), [`callee_resolved_file`](../../tree_sitter_analyzer/cross_file_resolver.md#ResolvedEdge.callee_resolved_file), [`name`](../../tree_sitter_analyzer/cross_file_resolver.md#FunctionDef.name), [`ResolvedEdge`](../../tree_sitter_analyzer/cross_file_resolver.md#ResolvedEdge), [`caller_line`](../../tree_sitter_analyzer/cross_file_resolver.md#ResolvedEdge.caller_line), [`end_line`](../../tree_sitter_analyzer/cross_file_resolver.md#FunctionDef.end_line), [`caller_file`](../../tree_sitter_analyzer/cross_file_resolver.md#ResolvedEdge.caller_file), [`caller_name`](../../tree_sitter_analyzer/cross_file_resolver.md#ResolvedEdge.caller_name), [`confidence`](../../tree_sitter_analyzer/cross_file_resolver.md#ResolvedEdge.confidence), [`callee_file`](../../tree_sitter_analyzer/cross_file_resolver.md#ResolvedEdge.callee_file), [`callee_line`](../../tree_sitter_analyzer/cross_file_resolver.md#ResolvedEdge.callee_line), [`callee_name`](../../tree_sitter_analyzer/cross_file_resolver.md#ResolvedEdge.callee_name), [`file`](../../tree_sitter_analyzer/cross_file_resolver.md#FunctionDef.file), [`language`](../../tree_sitter_analyzer/cross_file_resolver.md#FunctionDef.language)

### `TestResolveCallEdges`
- def: [`tests/unit/test_cross_file_resolver.py:166`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L166)
- signature: `class TestResolveCallEdges:`
- members:
  - `test_resolve_edges_does_not_crash(self, multi_file_project)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L167)
  - `test_resolved_edges_have_confidence(self, multi_file_project)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L173)
  - `test_resolved_edges_to_dict(self, multi_file_project)` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L180)
- uses (calls/refs, reference-scoped): [`resolve_call_edges`](../../tree_sitter_analyzer/cross_file_resolver.md#CrossFileResolver.resolve_call_edges), [`to_dict`](../../tree_sitter_analyzer/cross_file_resolver.md#ResolvedEdge.to_dict), [`CrossFileResolver`](../../tree_sitter_analyzer/cross_file_resolver.md#CrossFileResolver), [`confidence`](../../tree_sitter_analyzer/cross_file_resolver.md#ResolvedEdge.confidence)

## Functions
- `multi_file_project(tmp_path)` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cross_file_resolver.py#L16)

