---
title: 'Module: tests/unit/test_codegraph_query_internals_facets.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_query_internals_facets.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_query_internals_facets`/TestCodeGraphQueryInternalsFacets#
symbols:
  TestCodeGraphQueryInternalsFacets.test_quality_facets_cover_empty_error_and_missing_paths: test_quality_facets_cover_empty_error_and_missing_paths().
  TestCodeGraphQueryInternalsFacets.test_sort_state_supports_path_alias_fan_out_and_rejects_unknown_fields: test_sort_state_supports_path_alias_fan_out_and_rejects_unknown_fields().
  TestCodeGraphQueryInternalsFacets.test_include_facets_collects_quality_health_tests_and_risk: test_include_facets_collects_quality_health_tests_and_risk().
  TestCodeGraphQueryInternalsFacets.test_relation_step_skips_symbols_without_names_and_empty_rows: test_relation_step_skips_symbols_without_names_and_empty_rows().
  TestCodeGraphQueryInternalsFacets.test_relation_step_sorts_source_edges_before_tests_then_limits: test_relation_step_sorts_source_edges_before_tests_then_limits().
  TestCodeGraphQueryInternalsFacets.test_relation_step_filters_builtin_runtime_noise_before_limits: test_relation_step_filters_builtin_runtime_noise_before_limits().
  TestCodeGraphQueryInternalsFacets.test_sort_state_by_confidence_desc: test_sort_state_by_confidence_desc().
  TestCodeGraphQueryInternalsFacets.test_source_preference_key_identifies_test_fixture_and_generated_paths: test_source_preference_key_identifies_test_fixture_and_generated_paths().
  TestCodeGraphQueryInternalsFacets.test_relation_noise_symbol_identifies_runtime_helpers: test_relation_noise_symbol_identifies_runtime_helpers().
  TestCodeGraphQueryInternalsFacets.test_build_file_entries_includes_truncated_excerpt_for_long_symbols: test_build_file_entries_includes_truncated_excerpt_for_long_symbols().
  TestCodeGraphQueryInternalsFacets.test_compact_facets_trim_source_relationship_and_quality_shapes: test_compact_facets_trim_source_relationship_and_quality_shapes().
  TestCodeGraphQueryInternalsFacets.test_dedupe_symbols_keeps_first_instance: test_dedupe_symbols_keeps_first_instance().
  TestCodeGraphQueryInternalsFacets: ''
---
# Module: [`tests/unit/test_codegraph_query_internals_facets.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals_facets.py)

## Classes
### `TestCodeGraphQueryInternalsFacets`
- def: [`tests/unit/test_codegraph_query_internals_facets.py:29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals_facets.py#L29)
- signature: `class TestCodeGraphQueryInternalsFacets:`
- members:
  - `test_build_file_entries_includes_truncated_excerpt_for_long_symbols(self, tmp_path)` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals_facets.py#L180)
  - `test_compact_facets_trim_source_relationship_and_quality_shapes(self)` — [`L296`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals_facets.py#L296)
  - `test_dedupe_symbols_keeps_first_instance(self)` — [`L436`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals_facets.py#L436)
  - `test_include_facets_collects_quality_health_tests_and_risk(self, tmp_path)` — [`L225`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals_facets.py#L225)
  - `test_quality_facets_cover_empty_error_and_missing_paths(self, tmp_path)` — [`L381`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals_facets.py#L381)
  - `test_relation_noise_symbol_identifies_runtime_helpers(self)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals_facets.py#L132)
  - `test_relation_step_filters_builtin_runtime_noise_before_limits(self)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals_facets.py#L87)
  - `test_relation_step_skips_symbols_without_names_and_empty_rows(self)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals_facets.py#L30)
  - `test_relation_step_sorts_source_edges_before_tests_then_limits(self)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals_facets.py#L58)
  - `test_sort_state_by_confidence_desc(self)` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals_facets.py#L165)
  - `test_sort_state_supports_path_alias_fan_out_and_rejects_unknown_fields(self)` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals_facets.py#L147)
  - `test_source_preference_key_identifies_test_fixture_and_generated_paths(self)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_internals_facets.py#L137)
- uses (calls/refs, reference-scoped): [`_ChainStep`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.md#_ChainStep), [`_include_facets`](../../tree_sitter_analyzer/mcp/tools/codegraph_query_tool.md#_include_facets), [`current`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_state.md#_QueryState.current), [`_relation_step`](../../tree_sitter_analyzer/mcp/tools/codegraph_query_tool.md#_relation_step), [`_QueryState`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_state.md#_QueryState), [`sort_state`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_selection.md#sort_state), [`health_facet`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_facets.md#health_facet), [`facets`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_state.md#_QueryState.facets), [`complexity_facet`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_facets.md#complexity_facet), [`relationships`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_state.md#_QueryState.relationships), [`symbols`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_state.md#_QueryState.symbols), [`build_file_entries`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.md#build_file_entries), [`compact_facets`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_compact.md#compact_facets), [`source_preference_key`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.md#source_preference_key), [`risk_facet`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_facets.md#risk_facet), [`affected_tests_facet`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_facets.md#affected_tests_facet), [`dedupe_symbols`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.md#dedupe_symbols), [`is_relation_noise_symbol`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_selection.md#is_relation_noise_symbol), [`drop_test_shadow_symbols`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.md#drop_test_shadow_symbols), [`absolute_path`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.md#absolute_path)

