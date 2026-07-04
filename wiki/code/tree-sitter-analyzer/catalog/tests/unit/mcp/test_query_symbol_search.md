---
title: 'Module: tests/unit/mcp/test_query_symbol_search.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_query_symbol_search.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_query_symbol_search`/
symbols:
  TestCollectSourceFilesExcludes.test_excludes_dotdir_and_node_modules: TestCollectSourceFilesExcludes#test_excludes_dotdir_and_node_modules().
  TestCollectSourceFilesExcludes.test_find_references_skips_dotdir_vendors: TestCollectSourceFilesExcludes#test_find_references_skips_dotdir_vendors().
  TestBuildMatchFn.test_exact_match: TestBuildMatchFn#test_exact_match().
  TestBuildMatchFn.test_exact_match_case_sensitive: TestBuildMatchFn#test_exact_match_case_sensitive().
  TestBuildMatchFn.test_wildcard_prefix: TestBuildMatchFn#test_wildcard_prefix().
  TestBuildMatchFn.test_wildcard_suffix: TestBuildMatchFn#test_wildcard_suffix().
  TestBuildMatchFn.test_wildcard_both_ends: TestBuildMatchFn#test_wildcard_both_ends().
  TestBuildMatchFn.test_wildcard_case_insensitive: TestBuildMatchFn#test_wildcard_case_insensitive().
  TestBuildMatchFn.test_fuzzy_match: TestBuildMatchFn#test_fuzzy_match().
  TestBuildMatchFn.test_fuzzy_case_insensitive: TestBuildMatchFn#test_fuzzy_case_insensitive().
  TestBuildMatchFn.test_empty_symbol_raises: TestBuildMatchFn#test_empty_symbol_raises().
  TestBuildTypeFilter.test_none_returns_none: TestBuildTypeFilter#test_none_returns_none().
  TestBuildTypeFilter.test_class_filter: TestBuildTypeFilter#test_class_filter().
  TestBuildTypeFilter.test_function_filter: TestBuildTypeFilter#test_function_filter().
  TestBuildTypeFilter.test_method_filter: TestBuildTypeFilter#test_method_filter().
  TestBuildTypeFilter.test_unknown_type_returns_none: TestBuildTypeFilter#test_unknown_type_returns_none().
  TestSymbolSearchIntegration.tool_with_project: TestSymbolSearchIntegration#tool_with_project().
  TestSymbolSearchIntegration.test_symbol_type_in_schema: TestSymbolSearchIntegration#test_symbol_type_in_schema().
  TestFindReferences.ref_project: TestFindReferences#ref_project().
  TestFindReferences.test_find_references_empty_symbol_raises: TestFindReferences#test_find_references_empty_symbol_raises().
  TestFindReferences.test_find_references_flag_in_schema: TestFindReferences#test_find_references_flag_in_schema().
  TestCollectSourceFilesExcludes.test_project_root_under_dotted_ancestor_still_collects: TestCollectSourceFilesExcludes#test_project_root_under_dotted_ancestor_still_collects().
  TestCollectSourceFilesExcludes._make_tree: TestCollectSourceFilesExcludes#_make_tree().
  PROJECT_ROOT: PROJECT_ROOT.
  TestBuildMatchFn: TestBuildMatchFn#
  TestBuildTypeFilter: TestBuildTypeFilter#
  TestSymbolSearchIntegration: TestSymbolSearchIntegration#
  TestSymbolSearchIntegration.test_exact_search_finds_symbol: TestSymbolSearchIntegration#test_exact_search_finds_symbol().
  TestSymbolSearchIntegration.test_wildcard_search_finds_multiple: TestSymbolSearchIntegration#test_wildcard_search_finds_multiple().
  TestSymbolSearchIntegration.test_fuzzy_search_finds_matches: TestSymbolSearchIntegration#test_fuzzy_search_finds_matches().
  TestSymbolSearchIntegration.test_type_filter_classes_only: TestSymbolSearchIntegration#test_type_filter_classes_only().
  TestFindReferences: TestFindReferences#
  TestFindReferences.test_find_references_returns_definitions_and_refs: TestFindReferences#test_find_references_returns_definitions_and_refs().
  TestFindReferences.test_find_references_counts_callers: TestFindReferences#test_find_references_counts_callers().
  TestCollectSourceFilesExcludes: TestCollectSourceFilesExcludes#
---
# Module: [`tests/unit/mcp/test_query_symbol_search.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py)

## Classes
### `TestBuildMatchFn`
- def: [`tests/unit/mcp/test_query_symbol_search.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L19)
- signature: `class TestBuildMatchFn:`
- members:
  - `test_empty_symbol_raises(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L68)
  - `test_exact_match(self)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L20)
  - `test_exact_match_case_sensitive(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L26)
  - `test_fuzzy_case_insensitive(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L63)
  - `test_fuzzy_match(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L55)
  - `test_wildcard_both_ends(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L44)
  - `test_wildcard_case_insensitive(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L49)
  - `test_wildcard_prefix(self)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L31)
  - `test_wildcard_suffix(self)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L38)
- uses (calls/refs, reference-scoped): [`execute_symbol_search`](../../../tree_sitter_analyzer/mcp/tools/query_symbol_search.md#execute_symbol_search), [`_build_match_fn`](../../../tree_sitter_analyzer/mcp/tools/query_symbol_search.md#_build_match_fn)

### `TestBuildTypeFilter`
- def: [`tests/unit/mcp/test_query_symbol_search.py:73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L73)
- signature: `class TestBuildTypeFilter:`
- members:
  - `test_class_filter(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L77)
  - `test_function_filter(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L84)
  - `test_method_filter(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L90)
  - `test_none_returns_none(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L74)
  - `test_unknown_type_returns_none(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L96)
- uses (calls/refs, reference-scoped): [`_build_type_filter`](../../../tree_sitter_analyzer/mcp/tools/query_symbol_search.md#_build_type_filter)

### `TestCollectSourceFilesExcludes`
- def: [`tests/unit/mcp/test_query_symbol_search.py:241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L241)
- doc: #568: _collect_source_files must skip dotdirs AND shared EXCLUDE_DIRS members
- signature: `class TestCollectSourceFilesExcludes:`
- members:
  - `_make_tree(self, tmp_path: Path)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L245) — Create a fixture tree with:
  - `test_excludes_dotdir_and_node_modules(self, tmp_path)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L268)
  - `test_find_references_skips_dotdir_vendors(self, tmp_path)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L294) — find_references must not scan files inside dotdirs (budget pollution).
  - `test_project_root_under_dotted_ancestor_still_collects(self, tmp_path)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L279)
- uses (calls/refs, reference-scoped): [`execute_find_references`](../../../tree_sitter_analyzer/mcp/tools/query_symbol_search.md#execute_find_references), [`_collect_source_files`](../../../tree_sitter_analyzer/mcp/tools/query_symbol_search.md#_collect_source_files)

### `TestFindReferences`
- def: [`tests/unit/mcp/test_query_symbol_search.py:178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L178)
- signature: `class TestFindReferences:`
- members:
  - `ref_project(self, tmp_path)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L180)
  - `test_find_references_counts_callers(self, ref_project)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L221)
  - `test_find_references_empty_symbol_raises(self)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L229)
  - `test_find_references_flag_in_schema(self)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L233)
  - `test_find_references_returns_definitions_and_refs(self, ref_project)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L207)
- uses (calls/refs, reference-scoped): [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool), [`execute_find_references`](../../../tree_sitter_analyzer/mcp/tools/query_symbol_search.md#execute_find_references), [`TOOL_SCHEMA`](../../../tree_sitter_analyzer/mcp/tools/query_helpers.md#TOOL_SCHEMA.TOOL_SCHEMA)

### `TestSymbolSearchIntegration`
- def: [`tests/unit/mcp/test_query_symbol_search.py:100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L100)
- signature: `class TestSymbolSearchIntegration:`
- members:
  - `test_exact_search_finds_symbol(self, tool_with_project)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L133)
  - `test_fuzzy_search_finds_matches(self, tool_with_project)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L155)
  - `test_symbol_type_in_schema(self)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L169)
  - `test_type_filter_classes_only(self, tool_with_project)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L160)
  - `test_wildcard_search_finds_multiple(self, tool_with_project)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L145)
  - `tool_with_project(self, tmp_path)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L102)
- uses (calls/refs, reference-scoped): [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool), [`TOOL_SCHEMA`](../../../tree_sitter_analyzer/mcp/tools/query_helpers.md#TOOL_SCHEMA.TOOL_SCHEMA)

## Module values
- `PROJECT_ROOT` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_symbol_search.py#L16)

