---
title: 'Module: tests/unit/mcp/test_symbol_lineage_fixes.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_symbol_lineage_fixes.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_symbol_lineage_fixes`/
symbols:
  _write_py: _write_py().
  _make_tool: _make_tool().
  TestFilepathsScopeFilter.test_file_paths_filter_references: TestFilepathsScopeFilter#test_file_paths_filter_references().
  TestFilepathsScopeFilter.test_scope_cache_key_does_not_cross_pollute: TestFilepathsScopeFilter#test_scope_cache_key_does_not_cross_pollute().
  TestRefCountIncludesCallers.test_callers_included_in_references: TestRefCountIncludesCallers#test_callers_included_in_references().
  TestRefCountIncludesCallers.test_reference_count_matches_caller_count: TestRefCountIncludesCallers#test_reference_count_matches_caller_count().
  TestRefCountIncludesCallers.test_caller_files_appear_in_references: TestRefCountIncludesCallers#test_caller_files_appear_in_references().
  TestRefCountIncludesCallers.test_no_duplicate_references_from_call_graph: TestRefCountIncludesCallers#test_no_duplicate_references_from_call_graph().
  TestRefCountIncludesCallers.test_multiple_calls_use_call_site_lines: TestRefCountIncludesCallers#test_multiple_calls_use_call_site_lines().
  TestRefCountIncludesCallers.test_qualified_symbol_name_is_preserved_for_callers: TestRefCountIncludesCallers#test_qualified_symbol_name_is_preserved_for_callers().
  TestRefCountIncludesCallers.test_stale_call_graph_does_not_enrich_refs: TestRefCountIncludesCallers#test_stale_call_graph_does_not_enrich_refs().
  TestFilepathsScopeFilter.test_scope_note_absent_when_no_file_paths: TestFilepathsScopeFilter#test_scope_note_absent_when_no_file_paths().
  TestFilepathsScopeFilter.test_scope_note_mentions_filtered_references: TestFilepathsScopeFilter#test_scope_note_mentions_filtered_references().
  TestFilepathsScopeFilter.test_file_paths_in_tool_schema: TestFilepathsScopeFilter#test_file_paths_in_tool_schema().
  TestFilepathsScopeFilter.test_file_paths_not_required: TestFilepathsScopeFilter#test_file_paths_not_required().
  TestFilepathsScopeFilter.test_validate_arguments_accepts_file_paths: TestFilepathsScopeFilter#test_validate_arguments_accepts_file_paths().
  TestFilepathsScopeFilter.test_cli_spec_passes_file_paths: TestFilepathsScopeFilter#test_cli_spec_passes_file_paths().
  TestFilepathsScopeFilter.test_cli_spec_passes_file_paths._FakeArgs.file_paths: TestFilepathsScopeFilter#test_cli_spec_passes_file_paths()._FakeArgs#file_paths.
  TestFilepathsScopeFilter.test_cli_spec_file_paths_none_not_included: TestFilepathsScopeFilter#test_cli_spec_file_paths_none_not_included().
  TestFilepathsScopeFilter.test_cli_spec_file_paths_none_not_included._FakeArgs.file_paths: TestFilepathsScopeFilter#test_cli_spec_file_paths_none_not_included()._FakeArgs#file_paths.
  TestNormalizeScopeFilePaths.test_falsy_entries_are_skipped: TestNormalizeScopeFilePaths#test_falsy_entries_are_skipped().
  TestNormalizeScopeFilePaths.test_absolute_path_outside_root_is_kept_verbatim: TestNormalizeScopeFilePaths#test_absolute_path_outside_root_is_kept_verbatim().
  TestNormalizeScopeFilePaths.test_absolute_path_inside_root_is_relativized: TestNormalizeScopeFilePaths#test_absolute_path_inside_root_is_relativized().
  TestNormalizeScopeFilePaths.test_dot_slash_prefix_is_stripped: TestNormalizeScopeFilePaths#test_dot_slash_prefix_is_stripped().
  TestFilterReferencesToScope.test_empty_scope_returns_references_unchanged: TestFilterReferencesToScope#test_empty_scope_returns_references_unchanged().
  TestFilterReferencesToScope.test_only_in_scope_references_are_kept: TestFilterReferencesToScope#test_only_in_scope_references_are_kept().
  TestFilepathsScopeFilter.test_cli_spec_passes_file_paths._FakeArgs: TestFilepathsScopeFilter#test_cli_spec_passes_file_paths()._FakeArgs#
  TestFilepathsScopeFilter.test_cli_spec_file_paths_none_not_included._FakeArgs: TestFilepathsScopeFilter#test_cli_spec_file_paths_none_not_included()._FakeArgs#
  TestFilepathsScopeFilter: TestFilepathsScopeFilter#
  TestFilepathsScopeFilter.test_cli_spec_passes_file_paths._FakeArgs.symbol_lineage: TestFilepathsScopeFilter#test_cli_spec_passes_file_paths()._FakeArgs#symbol_lineage.
  TestFilepathsScopeFilter.test_cli_spec_passes_file_paths._FakeArgs.max_depth: TestFilepathsScopeFilter#test_cli_spec_passes_file_paths()._FakeArgs#max_depth.
  TestFilepathsScopeFilter.test_cli_spec_passes_file_paths._FakeArgs.file_path: TestFilepathsScopeFilter#test_cli_spec_passes_file_paths()._FakeArgs#file_path.
  TestFilepathsScopeFilter.test_cli_spec_file_paths_none_not_included._FakeArgs.symbol_lineage: TestFilepathsScopeFilter#test_cli_spec_file_paths_none_not_included()._FakeArgs#symbol_lineage.
  TestFilepathsScopeFilter.test_cli_spec_file_paths_none_not_included._FakeArgs.max_depth: TestFilepathsScopeFilter#test_cli_spec_file_paths_none_not_included()._FakeArgs#max_depth.
  TestFilepathsScopeFilter.test_cli_spec_file_paths_none_not_included._FakeArgs.file_path: TestFilepathsScopeFilter#test_cli_spec_file_paths_none_not_included()._FakeArgs#file_path.
  TestRefCountIncludesCallers: TestRefCountIncludesCallers#
  TestNormalizeScopeFilePaths: TestNormalizeScopeFilePaths#
  TestFilterReferencesToScope: TestFilterReferencesToScope#
---
# Module: [`tests/unit/mcp/test_symbol_lineage_fixes.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py)

## Classes
### `TestFilepathsScopeFilter`
- def: [`tests/unit/mcp/test_symbol_lineage_fixes.py:38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L38)
- doc: file_paths filters reference/call-site rows while keeping definitions.
- signature: `class TestFilepathsScopeFilter:`
- members:
  - `test_cli_spec_file_paths_none_not_included(self, tmp_path)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L168) — When CLI --file-paths is not set (None), file_paths must not appear
  - `test_cli_spec_passes_file_paths(self, tmp_path)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L149) — CLI spec build_tool_args must include file_paths when present.
  - `test_file_paths_filter_references(self, tmp_path)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L50)
  - `test_file_paths_in_tool_schema(self, tmp_path)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L130) — file_paths must be declared in the tool schema so MCP callers can pass it.
  - `test_file_paths_not_required(self, tmp_path)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L136) — file_paths must be optional (not in required list).
  - `test_scope_cache_key_does_not_cross_pollute(self, tmp_path)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L100)
  - `test_scope_note_absent_when_no_file_paths(self, tmp_path)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L41) — No file_paths → no scope_note (clean envelope).
  - `test_scope_note_mentions_filtered_references(self, tmp_path)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L84)
  - `test_validate_arguments_accepts_file_paths(self, tmp_path)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L142) — validate_arguments must not raise when file_paths is present.
- uses (calls/refs, reference-scoped): [`ASTCache`](../../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project), [`execute`](../../../tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.md#SymbolLineageTool.execute), [`flag_name`](../../../tree_sitter_analyzer/cli/commands/mcp_command_helpers.md#McpCommandSpec.flag_name), [`_CORE_SPECS`](../../../tree_sitter_analyzer/cli/commands/mcp_commands/_specs_core.md#_CORE_SPECS._CORE_SPECS), [`get_tool_schema`](../../../tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.md#SymbolLineageTool.get_tool_schema), [`validate_arguments`](../../../tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.md#SymbolLineageTool.validate_arguments)  (2 test-only)

### `TestFilterReferencesToScope`
- def: [`tests/unit/mcp/test_symbol_lineage_fixes.py:421`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L421)
- doc: Edge branches of _filter_references_to_scope.
- signature: `class TestFilterReferencesToScope:`
- members:
  - `test_empty_scope_returns_references_unchanged(self)` — [`L424`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L424) — Empty scope set short-circuits and returns the input list.
  - `test_only_in_scope_references_are_kept(self)` — [`L430`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L430) — Backslash paths normalize before matching the scope set.
- uses (calls/refs, reference-scoped): [`_filter_references_to_scope`](../../../tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.md#_filter_references_to_scope)

### `TestNormalizeScopeFilePaths`
- def: [`tests/unit/mcp/test_symbol_lineage_fixes.py:395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L395)
- doc: Edge branches of the new scope-path helpers.
- signature: `class TestNormalizeScopeFilePaths:`
- members:
  - `test_absolute_path_inside_root_is_relativized(self, tmp_path)` — [`L409`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L409) — An absolute path under root is made relative.
  - `test_absolute_path_outside_root_is_kept_verbatim(self, tmp_path)` — [`L403`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L403) — An absolute path not under root keeps its text (ValueError branch).
  - `test_dot_slash_prefix_is_stripped(self, tmp_path)` — [`L415`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L415) — A leading ``./`` is stripped from relative paths.
  - `test_falsy_entries_are_skipped(self, tmp_path)` — [`L398`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L398) — Empty/None entries are dropped (the ``continue`` branch).
- uses (calls/refs, reference-scoped): [`_normalize_scope_file_paths`](../../../tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.md#_normalize_scope_file_paths)

### `TestRefCountIncludesCallers`
- def: [`tests/unit/mcp/test_symbol_lineage_fixes.py:195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L195)
- doc: #757: when the call graph has actual call-site callers, they must
- signature: `class TestRefCountIncludesCallers:`
- members:
  - `test_caller_files_appear_in_references(self, tmp_path)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L260) — Files that contain call sites must appear in references.
  - `test_callers_included_in_references(self, tmp_path)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L200) — Call-site callers appear in references list.
  - `test_multiple_calls_use_call_site_lines(self, tmp_path)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L307)
  - `test_no_duplicate_references_from_call_graph(self, tmp_path)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L283) — Call-graph callers must not create duplicate reference entries.
  - `test_qualified_symbol_name_is_preserved_for_callers(self, tmp_path)` — [`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L336)
  - `test_reference_count_matches_caller_count(self, tmp_path)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L235) — reference_count must equal len(references) — no hidden inflation.
  - `test_stale_call_graph_does_not_enrich_refs(self, tmp_path)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L366)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project), [`execute`](../../../tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.md#SymbolLineageTool.execute)  (2 test-only)

### `_FakeArgs`
- def: [`tests/unit/mcp/test_symbol_lineage_fixes.py:177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L177)
- signature: `class _FakeArgs:`
- members:
  - `file_path` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L160)
  - `file_path` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L180)
  - `file_paths` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L161)
  - `file_paths` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L181)
  - `max_depth` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L159)
  - `max_depth` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L179)
  - `symbol_lineage` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L158)
  - `symbol_lineage` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L178)
- uses (calls/refs, reference-scoped): [`build_tool_args`](../../../tree_sitter_analyzer/cli/commands/mcp_command_helpers.md#McpCommandSpec.build_tool_args)  (1 test-only)

## Functions
- `_make_tool(tmp_path: Path)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L27)
- `_write_py(tmp_path: Path, name: str, content: str)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_fixes.py#L21)

