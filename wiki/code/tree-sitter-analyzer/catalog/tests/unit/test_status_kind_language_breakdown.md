---
title: 'Module: tests/unit/test_status_kind_language_breakdown.py'
type: catalog
provenance: extracted
module: tests/unit/test_status_kind_language_breakdown.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_status_kind_language_breakdown`/
symbols:
  _make_conn_with_symbols: _make_conn_with_symbols().
  TestGetStatsBreakdowns.test_edges_by_kind_present: TestGetStatsBreakdowns#test_edges_by_kind_present().
  TestGetStatsBreakdowns.test_total_edges_reconciles_with_edges_by_kind: TestGetStatsBreakdowns#test_total_edges_reconciles_with_edges_by_kind().
  TestGetStatsBreakdowns.test_all_three_breakdown_keys_present: TestGetStatsBreakdowns#test_all_three_breakdown_keys_present().
  TestASTCacheToolStatsBreakdowns.test_handle_stats_surfaces_symbols_by_kind: TestASTCacheToolStatsBreakdowns#test_handle_stats_surfaces_symbols_by_kind().
  TestASTCacheToolStatsBreakdowns.test_handle_stats_surfaces_symbols_by_language: TestASTCacheToolStatsBreakdowns#test_handle_stats_surfaces_symbols_by_language().
  TestASTCacheToolStatsBreakdowns.test_handle_stats_surfaces_edges_by_kind: TestASTCacheToolStatsBreakdowns#test_handle_stats_surfaces_edges_by_kind().
  TestCLIMCPParity.test_get_stats_breakdown_keys_superset_check: TestCLIMCPParity#test_get_stats_breakdown_keys_superset_check().
  TestGetStatsBreakdowns.test_symbols_by_kind_present_in_stats: TestGetStatsBreakdowns#test_symbols_by_kind_present_in_stats().
  TestGetStatsBreakdowns.test_symbols_by_language_present_in_stats: TestGetStatsBreakdowns#test_symbols_by_language_present_in_stats().
  TestGetStatsBreakdowns.test_symbols_by_kind_values_sum_to_total_symbols: TestGetStatsBreakdowns#test_symbols_by_kind_values_sum_to_total_symbols().
  TestGetStatsBreakdowns.test_symbols_by_language_counts_correct: TestGetStatsBreakdowns#test_symbols_by_language_counts_correct().
  TestGetStatsBreakdowns.test_symbols_by_kind_counts_correct: TestGetStatsBreakdowns#test_symbols_by_kind_counts_correct().
  TestGetStatsBreakdowns.test_symbols_by_kind_includes_constant_bucket: TestGetStatsBreakdowns#test_symbols_by_kind_includes_constant_bucket().
  TestGetStatsBreakdowns.test_degrade_gracefully_when_fts5_unavailable: TestGetStatsBreakdowns#test_degrade_gracefully_when_fts5_unavailable().
  TestGetStatsBreakdowns.test_degrade_gracefully_when_table_absent_but_flag_true: TestGetStatsBreakdowns#test_degrade_gracefully_when_table_absent_but_flag_true().
  TestGetStatsBreakdowns.test_total_edges_zero_when_edges_table_absent: TestGetStatsBreakdowns#test_total_edges_zero_when_edges_table_absent().
  TestGetStatsBreakdowns.test_edges_by_kind_empty_dict_when_edges_table_absent: TestGetStatsBreakdowns#test_edges_by_kind_empty_dict_when_edges_table_absent().
  TestCodeGraphStatusBreakdowns.test_codegraph_status_surfaces_symbols_by_kind: TestCodeGraphStatusBreakdowns#test_codegraph_status_surfaces_symbols_by_kind().
  TestCodeGraphStatusBreakdowns.test_codegraph_status_surfaces_symbols_by_language: TestCodeGraphStatusBreakdowns#test_codegraph_status_surfaces_symbols_by_language().
  TestCodeGraphStatusBreakdowns.test_codegraph_status_surfaces_edges_by_kind: TestCodeGraphStatusBreakdowns#test_codegraph_status_surfaces_edges_by_kind().
  TestCLIMCPParity.test_codegraph_status_flag_registered_in_extended_specs: TestCLIMCPParity#test_codegraph_status_flag_registered_in_extended_specs().
  _add_edges: _add_edges().
  TestGetStatsBreakdowns: TestGetStatsBreakdowns#
  TestASTCacheToolStatsBreakdowns: TestASTCacheToolStatsBreakdowns#
  TestCodeGraphStatusBreakdowns: TestCodeGraphStatusBreakdowns#
  TestCLIMCPParity: TestCLIMCPParity#
---
# Module: [`tests/unit/test_status_kind_language_breakdown.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py)

## Classes
### `TestASTCacheToolStatsBreakdowns`
- def: [`tests/unit/test_status_kind_language_breakdown.py:280`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L280)
- doc: Verify ast_cache mode=stats surfaces the new breakdown keys.
- signature: `class TestASTCacheToolStatsBreakdowns:`
- members:
  - `test_handle_stats_surfaces_edges_by_kind(self, tmp_path: Any)` — [`L334`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L334)
  - `test_handle_stats_surfaces_symbols_by_kind(self, tmp_path: Any)` — [`L284`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L284) — _handle_stats must pass symbols_by_kind through to the envelope.
  - `test_handle_stats_surfaces_symbols_by_language(self, tmp_path: Any)` — [`L309`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L309)
- uses (calls/refs, reference-scoped): [`ASTCacheTool`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool.execute), [`_cache`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool._cache)

### `TestCLIMCPParity`
- def: [`tests/unit/test_status_kind_language_breakdown.py:476`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L476)
- doc: --codegraph-status CLI flag must still route to CodeGraphStatusTool.
- signature: `class TestCLIMCPParity:`
- members:
  - `test_codegraph_status_flag_registered_in_extended_specs(self)` — [`L479`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L479)
  - `test_get_stats_breakdown_keys_superset_check(self)` — [`L491`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L491) — get_stats() must include the three breakdown keys (integration check).
- uses (calls/refs, reference-scoped): [`flag_name`](../../tree_sitter_analyzer/cli/commands/mcp_command_helpers.md#McpCommandSpec.flag_name), [`_EXTENDED_SPECS`](../../tree_sitter_analyzer/cli/commands/mcp_commands/_specs_extended.md#_EXTENDED_SPECS._EXTENDED_SPECS), [`get_stats`](../../tree_sitter_analyzer/_ast_cache_query.md#get_stats)  (2 test-only)

### `TestCodeGraphStatusBreakdowns`
- def: [`tests/unit/test_status_kind_language_breakdown.py:362`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L362)
- doc: Verify codegraph_status exposes the new breakdown keys.
- signature: `class TestCodeGraphStatusBreakdowns:`
- members:
  - `test_codegraph_status_surfaces_edges_by_kind(self, tmp_path: Any)` — [`L439`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L439)
  - `test_codegraph_status_surfaces_symbols_by_kind(self, tmp_path: Any)` — [`L366`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L366)
  - `test_codegraph_status_surfaces_symbols_by_language(self, tmp_path: Any)` — [`L403`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L403)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/codegraph_status_tool.md#CodeGraphStatusTool.execute), [`CodeGraphStatusTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_status_tool.md#CodeGraphStatusTool)

### `TestGetStatsBreakdowns`
- def: [`tests/unit/test_status_kind_language_breakdown.py:111`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L111)
- doc: RED tests: these fail until symbols_by_kind/by_language are added.
- signature: `class TestGetStatsBreakdowns:`
- members:
  - `test_all_three_breakdown_keys_present(self)` — [`L264`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L264) — The stats dict must include symbols_by_kind, symbols_by_language, edges_by_kind.
  - `test_degrade_gracefully_when_fts5_unavailable(self)` — [`L199`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L199) — When fts5_available=False, symbols_by_kind/by_language are empty dicts.
  - `test_degrade_gracefully_when_table_absent_but_flag_true(self)` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L209) — If ast_symbol_rows is absent and fts5_available=True, empty dicts (no raise).
  - `test_edges_by_kind_empty_dict_when_edges_table_absent(self)` — [`L256`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L256) — If edges table is absent, edges_by_kind degrades to {}.
  - `test_edges_by_kind_present(self)` — [`L218`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L218) — edges_by_kind must be present when edges table has a kind column.
  - `test_symbols_by_kind_counts_correct(self)` — [`L171`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L171) — symbols_by_kind must count correctly per kind bucket.
  - `test_symbols_by_kind_includes_constant_bucket(self)` — [`L186`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L186) — Issue #610 — kind='constant' rows (Python module constants) must
  - `test_symbols_by_kind_present_in_stats(self)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L114) — get_stats must return a symbols_by_kind dict.
  - `test_symbols_by_kind_values_sum_to_total_symbols(self)` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L142) — symbols_by_kind values must sum to total_symbols.
  - `test_symbols_by_language_counts_correct(self)` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L158) — symbols_by_language must reflect actual per-language row counts.
  - `test_symbols_by_language_present_in_stats(self)` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L128) — get_stats must return a symbols_by_language dict.
  - `test_total_edges_reconciles_with_edges_by_kind(self)` — [`L231`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L231) — Codex P2 #315: total_edges must equal sum(edges_by_kind) — it counts
  - `test_total_edges_zero_when_edges_table_absent(self)` — [`L248`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L248) — total_edges degrades to 0 (not raising) when the edges table is gone.
- uses (calls/refs, reference-scoped): [`get_stats`](../../tree_sitter_analyzer/_ast_cache_query.md#get_stats)  (2 test-only)

## Functions
- `_add_edges(conn: sqlite3.Connection, edges: list[tuple[str, str]])` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L96) — Insert (source, kind) edge rows into an existing connection.
- `_make_conn_with_symbols(rows: list[tuple[str, str, str]])` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_status_kind_language_breakdown.py#L35) — Return a sqlite3.Connection with ast_symbol_rows populated.

