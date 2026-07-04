---
title: 'Module: tests/unit/test_codegraph_explore_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_explore_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_explore_tool`/
symbols:
  _make_def: _make_def().
  _patch_resolver_with: _patch_resolver_with().
  _patch_resolver_with._resolve: _patch_resolver_with()._resolve().
  TestExecuteHappyPath.test_two_defs_in_two_files_returns_info: TestExecuteHappyPath#test_two_defs_in_two_files_returns_info().
  TestExecuteHappyPath.test_max_files_cap_trims: TestExecuteHappyPath#test_max_files_cap_trims().
  TestExecuteHappyPath.test_include_code_false_omits_snippets: TestExecuteHappyPath#test_include_code_false_omits_snippets().
  TestExecuteHappyPath.test_relationship_map_dedupes_returned_symbol_callees: TestExecuteHappyPath#test_relationship_map_dedupes_returned_symbol_callees().
  TestExecuteHappyPath.test_concept_matches_merge_before_resolved_file_entries: TestExecuteHappyPath#test_concept_matches_merge_before_resolved_file_entries().
  _patch_cache_with: _patch_cache_with().
  TestExecuteNotFound.test_zero_matches_returns_not_found: TestExecuteNotFound#test_zero_matches_returns_not_found().
  TestExecuteNotFound.test_zero_symbol_matches_returns_concept_matches: TestExecuteNotFound#test_zero_symbol_matches_returns_concept_matches().
  TestExecuteHappyPath.test_relationships_use_sql_cache_not_full_graph: TestExecuteHappyPath#test_relationships_use_sql_cache_not_full_graph().
  tool: tool().
  tool_with_root: tool_with_root().
  TestSplitQuery.test_file_tokens_separated_from_symbols: TestSplitQuery#test_file_tokens_separated_from_symbols().
  TestSplitQuery.test_short_tokens_dropped: TestSplitQuery#test_short_tokens_dropped().
  TestExecuteDegraded.test_empty_cache_returns_warn: TestExecuteDegraded#test_empty_cache_returns_warn().
  TestExtractSnippet.test_valid_range: TestExtractSnippet#test_valid_range().
  TestExtractSnippet.test_missing_file_returns_empty: TestExtractSnippet#test_missing_file_returns_empty().
  TestExtractSnippet.test_invalid_range_returns_empty: TestExtractSnippet#test_invalid_range_returns_empty().
  TestExecuteHappyPath._query_callees: TestExecuteHappyPath#_query_callees().
  TestToolDefinition: TestToolDefinition#
  TestToolDefinition.test_tool_name: TestToolDefinition#test_tool_name().
  TestToolDefinition.test_description_starts_with_bulk_fetch: TestToolDefinition#test_description_starts_with_bulk_fetch().
  TestToolDefinition.test_annotations_all_four_hints: TestToolDefinition#test_annotations_all_four_hints().
  TestToolDefinition.test_schema_query_and_symbol_alias_not_required: TestToolDefinition#test_schema_query_and_symbol_alias_not_required().
  TestToolDefinition.test_symbol_alias_maps_to_query: TestToolDefinition#test_symbol_alias_maps_to_query().
  TestToolDefinition.test_symbols_list_maps_to_query: TestToolDefinition#test_symbols_list_maps_to_query().
  TestToolDefinition.test_symbol_accepts_list_too: TestToolDefinition#test_symbol_accepts_list_too().
  TestToolDefinition.test_symbols_in_schema: TestToolDefinition#test_symbols_in_schema().
  TestToolDefinition.test_missing_query_and_symbol_raises: TestToolDefinition#test_missing_query_and_symbol_raises().
  TestToolDefinition.test_schema_strict_no_additional_properties: TestToolDefinition#test_schema_strict_no_additional_properties().
  TestToolDefinition.test_schema_output_format_default_is_toon: TestToolDefinition#test_schema_output_format_default_is_toon().
  TestToolDefinition.test_schema_caps: TestToolDefinition#test_schema_caps().
  TestValidateArguments: TestValidateArguments#
  TestValidateArguments.test_missing_query_raises: TestValidateArguments#test_missing_query_raises().
  TestValidateArguments.test_blank_query_raises: TestValidateArguments#test_blank_query_raises().
  TestValidateArguments.test_valid_query: TestValidateArguments#test_valid_query().
  TestSplitQuery: TestSplitQuery#
  TestExecuteDegraded: TestExecuteDegraded#
  TestExecuteDegraded.test_no_project_root_returns_warn: TestExecuteDegraded#test_no_project_root_returns_warn().
  TestExecuteNotFound: TestExecuteNotFound#
  TestExecuteHappyPath: TestExecuteHappyPath#
  TestExecuteHappyPath.test_relationship_names_degrades_when_sql_lookup_fails: TestExecuteHappyPath#test_relationship_names_degrades_when_sql_lookup_fails().
  TestExecuteHappyPath.test_relationship_names_caps_caller_and_callee_lists: TestExecuteHappyPath#test_relationship_names_caps_caller_and_callee_lists().
  TestExecuteHappyPath.test_source_path_joins_relative_paths_with_project_root: TestExecuteHappyPath#test_source_path_joins_relative_paths_with_project_root().
  TestExecuteOutputFormat: TestExecuteOutputFormat#
  TestExecuteOutputFormat.test_toon_format_default: TestExecuteOutputFormat#test_toon_format_default().
  TestExecuteOutputFormat.test_json_format_no_toon_blob: TestExecuteOutputFormat#test_json_format_no_toon_blob().
  TestExtractSnippet: TestExtractSnippet#
---
# Module: [`tests/unit/test_codegraph_explore_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py)

## Classes
### `TestExecuteDegraded`
- def: [`tests/unit/test_codegraph_explore_tool.py:167`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L167)
- signature: `class TestExecuteDegraded:`
- members:
  - `test_empty_cache_returns_warn(self, tool_with_root)` — [`L176`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L176)
  - `test_no_project_root_returns_warn(self, tool)` — [`L169`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L169)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestExecuteHappyPath`
- def: [`tests/unit/test_codegraph_explore_tool.py:235`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L235)
- signature: `class TestExecuteHappyPath:`
- members:
  - `test_concept_matches_merge_before_resolved_file_entries(self, tool_with_root, tmp_path)` — [`L360`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L360)
  - `test_include_code_false_omits_snippets(self, tool_with_root, tmp_path)` — [`L280`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L280)
  - `test_max_files_cap_trims(self, tool_with_root, tmp_path)` — [`L260`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L260)
  - `test_relationship_map_dedupes_returned_symbol_callees(self, tool_with_root, tmp_path)` — [`L328`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L328)
  - `test_relationship_names_caps_caller_and_callee_lists(self, tool_with_root)` — [`L410`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L410)
  - `test_relationship_names_degrades_when_sql_lookup_fails(self, tool_with_root)` — [`L400`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L400)
  - `test_relationships_use_sql_cache_not_full_graph(self, tool_with_root, tmp_path)` — [`L295`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L295)
  - `test_source_path_joins_relative_paths_with_project_root(self, tool_with_root)` — [`L424`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L424)
  - `test_two_defs_in_two_files_returns_info(self, tool_with_root, tmp_path)` — [`L237`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L237)
- protocol/private: `_query_callees`[`L341`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L341)
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestExecuteNotFound`
- def: [`tests/unit/test_codegraph_explore_tool.py:188`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L188)
- signature: `class TestExecuteNotFound:`
- members:
  - `test_zero_matches_returns_not_found(self, tool_with_root)` — [`L190`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L190)
  - `test_zero_symbol_matches_returns_concept_matches(self, tool_with_root)` — [`L201`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L201)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestExecuteOutputFormat`
- def: [`tests/unit/test_codegraph_explore_tool.py:428`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L428)
- signature: `class TestExecuteOutputFormat:`
- members:
  - `test_json_format_no_toon_blob(self, tool)` — [`L436`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L436)
  - `test_toon_format_default(self, tool)` — [`L430`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L430)

### `TestExtractSnippet`
- def: [`tests/unit/test_codegraph_explore_tool.py:442`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L442)
- signature: `class TestExtractSnippet:`
- members:
  - `test_invalid_range_returns_empty(self, tmp_path)` — [`L451`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L451)
  - `test_missing_file_returns_empty(self, tmp_path)` — [`L448`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L448)
  - `test_valid_range(self, tmp_path)` — [`L443`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L443)
- uses (calls/refs, reference-scoped): [`extract_snippet`](../../tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.md#extract_snippet)

### `TestSplitQuery`
- def: [`tests/unit/test_codegraph_explore_tool.py:153`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L153)
- signature: `class TestSplitQuery:`
- members:
  - `test_file_tokens_separated_from_symbols(self)` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L154)
  - `test_short_tokens_dropped(self)` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L161)
- uses (calls/refs, reference-scoped): [`split_query`](../../tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.md#split_query)

### `TestToolDefinition`
- def: [`tests/unit/test_codegraph_explore_tool.py:75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L75)
- signature: `class TestToolDefinition:`
- members:
  - `test_annotations_all_four_hints(self, tool)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L83)
  - `test_description_starts_with_bulk_fetch(self, tool)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L79)
  - `test_missing_query_and_symbol_raises(self, tool)` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L120)
  - `test_schema_caps(self, tool)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L132)
  - `test_schema_output_format_default_is_toon(self, tool)` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L127)
  - `test_schema_query_and_symbol_alias_not_required(self, tool)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L90)
  - `test_schema_strict_no_additional_properties(self, tool)` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L124)
  - `test_symbol_accepts_list_too(self, tool)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L109)
  - `test_symbol_alias_maps_to_query(self, tool)` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L98)
  - `test_symbols_in_schema(self, tool)` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L116)
  - `test_symbols_list_maps_to_query(self, tool)` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L103)
  - `test_tool_name(self, tool)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L76)

### `TestValidateArguments`
- def: [`tests/unit/test_codegraph_explore_tool.py:140`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L140)
- signature: `class TestValidateArguments:`
- members:
  - `test_blank_query_raises(self, tool)` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L145)
  - `test_missing_query_raises(self, tool)` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L141)
  - `test_valid_query(self, tool)` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L149)

## Functions
- `_make_def(file: str, name: str, line: int = 1, end_line: int = 5, kind: str = "function", language: str = "python")` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L34)
- `_patch_cache_with(total_files: int = 5)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L68) — Patch ASTCache so the tool's _try_get_cache walks the success branch.
- `_patch_resolver_with(defs_per_token: dict[str, list[DefinitionLocation]])` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L52) — Return a context manager patching SymbolResolver so .resolve(tok)
- `_resolve(tok: str)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L57)
- `tool()` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L25)
- `tool_with_root(tmp_path)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_tool.py#L30)

