---
title: 'Module: tests/unit/mcp/test_symbol_lineage_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_symbol_lineage_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_symbol_lineage_tool`/
symbols:
  _write_py: _write_py().
  TestInheritanceLineage.test_hierarchy_degrades_to_none_on_error: TestInheritanceLineage#test_hierarchy_degrades_to_none_on_error().
  TestAstIndexStaleness.test_empty_ast_index_is_unknown_not_stale: TestAstIndexStaleness#test_empty_ast_index_is_unknown_not_stale().
  TestAstIndexStaleness.test_stale_when_supported_source_file_is_added_after_index: TestAstIndexStaleness#test_stale_when_supported_source_file_is_added_after_index().
  TestAstIndexStaleness.test_stale_when_indexed_source_file_is_deleted: TestAstIndexStaleness#test_stale_when_indexed_source_file_is_deleted().
  TestInheritanceLineage.test_class_symbol_returns_inheritance_hierarchy: TestInheritanceLineage#test_class_symbol_returns_inheritance_hierarchy().
  TestInheritanceLineage.test_function_symbol_has_no_hierarchy: TestInheritanceLineage#test_function_symbol_has_no_hierarchy().
  TestInheritanceLineage.test_qualified_symbol_name_resolves_hierarchy: TestInheritanceLineage#test_qualified_symbol_name_resolves_hierarchy().
  TestInheritanceLineage.test_cache_invalidates_when_index_built_after_first_call: TestInheritanceLineage#test_cache_invalidates_when_index_built_after_first_call().
  TestInheritanceLineage.test_hierarchy_flags_stale_after_source_edit_without_reindex: TestInheritanceLineage#test_hierarchy_flags_stale_after_source_edit_without_reindex().
  TestInheritanceLineage.test_hierarchy_not_stale_when_index_fresh: TestInheritanceLineage#test_hierarchy_not_stale_when_index_fresh().
  TestInheritanceLineage.test_hierarchy_stale_uses_fingerprint_fallback_when_graph_missing: TestInheritanceLineage#test_hierarchy_stale_uses_fingerprint_fallback_when_graph_missing().
  TestInheritanceLineage.test_hierarchy_stale_for_non_source_ext_kotlin_file: TestInheritanceLineage#test_hierarchy_stale_for_non_source_ext_kotlin_file().
  TestInheritanceLineage.test_execute_invalidates_symbol_cache_when_ast_index_is_stale: TestInheritanceLineage#test_execute_invalidates_symbol_cache_when_ast_index_is_stale().
  tool: tool().
  TestExecute.test_no_project_root_raises: TestExecute#test_no_project_root_raises().
  TestGraphCacheFingerprintHelpers.test_walk_supported_source_paths_skips_dotfiles_excluded_and_unsupported: TestGraphCacheFingerprintHelpers#test_walk_supported_source_paths_skips_dotfiles_excluded_and_unsupported().
  TestRiskAssessment.test_unknown_when_no_definitions: TestRiskAssessment#test_unknown_when_no_definitions().
  TestRiskAssessment.test_low_risk: TestRiskAssessment#test_low_risk().
  TestRiskAssessment.test_medium_risk: TestRiskAssessment#test_medium_risk().
  TestRiskAssessment.test_high_risk: TestRiskAssessment#test_high_risk().
  TestIsTestFile.test_detects_test_files: TestIsTestFile#test_detects_test_files().
  TestIsTestFile.test_rejects_non_test_files: TestIsTestFile#test_rejects_non_test_files().
  TestExecute.test_symbol_not_found_returns_unknown_risk: TestExecute#test_symbol_not_found_returns_unknown_risk().
  TestExecute.test_verdict_present_when_symbol_found: TestExecute#test_verdict_present_when_symbol_found().
  TestExecute.test_finds_symbol_returns_success: TestExecute#test_finds_symbol_returns_success().
  TestExecute.test_toon_format_includes_content: TestExecute#test_toon_format_includes_content().
  TestGraphCacheFingerprintHelpers.test_indexed_abs_and_rel_path_absolute_outside_root_falls_back: TestGraphCacheFingerprintHelpers#test_indexed_abs_and_rel_path_absolute_outside_root_falls_back().
  TestGraphCacheFingerprintHelpers.test_indexed_abs_and_rel_path_relative_inside_root: TestGraphCacheFingerprintHelpers#test_indexed_abs_and_rel_path_relative_inside_root().
  TestR37uTopLevelVerdictMirror.test_top_level_verdict_mirrors_agent_summary_when_found: TestR37uTopLevelVerdictMirror#test_top_level_verdict_mirrors_agent_summary_when_found().
  TestR37uTopLevelVerdictMirror.test_top_level_verdict_mirrors_when_not_found: TestR37uTopLevelVerdictMirror#test_top_level_verdict_mirrors_when_not_found().
  TestInheritanceLineage._boom: TestInheritanceLineage#_boom().
  TestRiskAssessment: TestRiskAssessment#
  TestIsTestFile: TestIsTestFile#
  TestValidation: TestValidation#
  TestValidation.test_requires_symbol: TestValidation#test_requires_symbol().
  TestValidation.test_rejects_empty_symbol: TestValidation#test_rejects_empty_symbol().
  TestValidation.test_rejects_bad_depth: TestValidation#test_rejects_bad_depth().
  TestValidation.test_valid_args_pass: TestValidation#test_valid_args_pass().
  TestToolDefinition: TestToolDefinition#
  TestToolDefinition.test_definition_has_name: TestToolDefinition#test_definition_has_name().
  TestToolDefinition.test_schema_requires_symbol: TestToolDefinition#test_schema_requires_symbol().
  TestExecute: TestExecute#
  TestInheritanceLineage: TestInheritanceLineage#
  TestAstIndexStaleness: TestAstIndexStaleness#
  TestGraphCacheFingerprintHelpers: TestGraphCacheFingerprintHelpers#
  TestR37uTopLevelVerdictMirror: TestR37uTopLevelVerdictMirror#
---
# Module: [`tests/unit/mcp/test_symbol_lineage_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py)

## Classes
### `TestAstIndexStaleness`
- def: [`tests/unit/mcp/test_symbol_lineage_tool.py:442`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L442)
- signature: `class TestAstIndexStaleness:`
- members:
  - `test_empty_ast_index_is_unknown_not_stale(self, tool, tmp_path)` — [`L443`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L443) — An empty DB created by a read path is not a completed stale index.
  - `test_stale_when_indexed_source_file_is_deleted(self, tool, tmp_path)` — [`L466`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L466) — #933: deleted indexed files must make the AST index stale.
  - `test_stale_when_supported_source_file_is_added_after_index(self, tool, tmp_path)` — [`L452`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L452) — #931: newly added supported files must invalidate the AST index.
- uses (calls/refs, reference-scoped): [`ASTCache`](../../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project), [`is_ast_index_stale`](../../../tree_sitter_analyzer/_graph_cache_fingerprint.md#is_ast_index_stale)  (1 test-only)

### `TestExecute`
- def: [`tests/unit/mcp/test_symbol_lineage_tool.py:116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L116)
- signature: `class TestExecute:`
- members:
  - `test_finds_symbol_returns_success(self, tool, tmp_path)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L142)
  - `test_no_project_root_raises(self, tmp_path)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L167)
  - `test_symbol_not_found_returns_unknown_risk(self, tool, tmp_path)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L117)
  - `test_toon_format_includes_content(self, tool, tmp_path)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L161)
  - `test_verdict_present_when_symbol_found(self, tool, tmp_path)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L130) — Found symbols must emit a canonical verdict (not None).
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.md#SymbolLineageTool.execute), [`SymbolLineageTool`](../../../tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.md#SymbolLineageTool)  (1 test-only)

### `TestGraphCacheFingerprintHelpers`
- def: [`tests/unit/mcp/test_symbol_lineage_tool.py:480`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L480)
- doc: Direct coverage for the freshness-walk helper branches (#970).
- signature: `class TestGraphCacheFingerprintHelpers:`
- members:
  - `test_indexed_abs_and_rel_path_absolute_outside_root_falls_back(self, tmp_path)` — [`L483`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L483) — An absolute indexed path outside root → relative_to raises ValueError,
  - `test_indexed_abs_and_rel_path_relative_inside_root(self, tmp_path)` — [`L498`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L498) — A relative indexed path is resolved against root and stays relative.
  - `test_walk_supported_source_paths_skips_dotfiles_excluded_and_unsupported(self, tmp_path)` — [`L511`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L511) — The walker yields only supported, non-dot files outside EXCLUDE_DIRS.
- uses (calls/refs, reference-scoped): [`_walk_supported_source_paths`](../../../tree_sitter_analyzer/_graph_cache_fingerprint.md#_walk_supported_source_paths), [`_indexed_abs_and_rel_path`](../../../tree_sitter_analyzer/_graph_cache_fingerprint.md#_indexed_abs_and_rel_path)  (1 test-only)

### `TestInheritanceLineage`
- def: [`tests/unit/mcp/test_symbol_lineage_tool.py:173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L173)
- doc: #568: lineage of a class returns the advertised inheritance/override
- signature: `class TestInheritanceLineage:`
- members:
  - `test_cache_invalidates_when_index_built_after_first_call(self, tool, tmp_path)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L225)
  - `test_class_symbol_returns_inheritance_hierarchy(self, tool, tmp_path)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L178)
  - `test_execute_invalidates_symbol_cache_when_ast_index_is_stale(self, tool, tmp_path)` — [`L406`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L406) — #932: a warm lineage response must not hide stale AST-index data.
  - `test_function_symbol_has_no_hierarchy(self, tool, tmp_path)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L200)
  - `test_hierarchy_degrades_to_none_on_error(self, tool, tmp_path, monkeypatch)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L244)
  - `test_hierarchy_flags_stale_after_source_edit_without_reindex(self, tool, tmp_path)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L261) — #692: index_stale=True when source is newer than the AST index.
  - `test_hierarchy_not_stale_when_index_fresh(self, tool, tmp_path)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L303) — #692: index_stale=False immediately after indexing (no source edits).
  - `test_hierarchy_stale_for_non_source_ext_kotlin_file(self, tool, tmp_path)` — [`L362`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L362) — #703: index_stale=True after editing a Kotlin (.kt) file post-index.
  - `test_hierarchy_stale_uses_fingerprint_fallback_when_graph_missing(self, tool, tmp_path)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L334) — #692: when the dep-graph fingerprint is absent (graph build failed) the
  - `test_qualified_symbol_name_resolves_hierarchy(self, tool, tmp_path)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L210)
- protocol/private: `_boom`[`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L253)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`index_project`](../../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project), [`ClassHierarchy`](../../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy)  (1 test-only)

### `TestIsTestFile`
- def: [`tests/unit/mcp/test_symbol_lineage_tool.py:48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L48)
- signature: `class TestIsTestFile:`
- members:
  - `test_detects_test_files(self, path)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L62)
  - `test_rejects_non_test_files(self, path)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L79)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestR37uTopLevelVerdictMirror`
- def: [`tests/unit/mcp/test_symbol_lineage_tool.py:537`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L537)
- doc: r37u dogfood: `--symbol-lineage` envelope used to omit top-level
- signature: `class TestR37uTopLevelVerdictMirror:`
- members:
  - `test_top_level_verdict_mirrors_agent_summary_when_found(self, tool, tmp_path)` — [`L546`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L546)
  - `test_top_level_verdict_mirrors_when_not_found(self, tool, tmp_path)` — [`L562`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L562) — Even when no definition is found, top-level verdict must mirror.
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestRiskAssessment`
- def: [`tests/unit/mcp/test_symbol_lineage_tool.py:28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L28)
- signature: `class TestRiskAssessment:`
- members:
  - `test_high_risk(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L42)
  - `test_low_risk(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L34)
  - `test_medium_risk(self)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L38)
  - `test_unknown_when_no_definitions(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L29)
- uses (calls/refs, reference-scoped): [`_assess_risk`](../../../tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.md#_assess_risk)

### `TestToolDefinition`
- def: [`tests/unit/mcp/test_symbol_lineage_tool.py:103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L103)
- signature: `class TestToolDefinition:`
- members:
  - `test_definition_has_name(self, tool)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L104)
  - `test_schema_requires_symbol(self, tool)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L110)

### `TestValidation`
- def: [`tests/unit/mcp/test_symbol_lineage_tool.py:83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L83)
- signature: `class TestValidation:`
- members:
  - `test_rejects_bad_depth(self, tool)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L92)
  - `test_rejects_empty_symbol(self, tool)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L88)
  - `test_requires_symbol(self, tool)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L84)
  - `test_valid_args_pass(self, tool)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L98)

## Functions
- `_write_py(tmp_path, name, content)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L22)
- `tool(tmp_path)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_symbol_lineage_tool.py#L16)

