---
title: 'Module: tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools._codegraph_query_state`/_
symbols:
  _QueryState.current: QueryState#current.
  _QueryState: QueryState#
  _QueryState.facets: QueryState#facets.
  _QueryState.relationships: QueryState#relationships.
  _QueryState.symbols: QueryState#symbols.
  _QueryState.files: QueryState#files.
  _QueryState.add_symbols: QueryState#add_symbols().
  _QueryState.selection_filters: QueryState#selection_filters.
  _QueryState.seed_queries: QueryState#seed_queries.
  _QueryState.concept_files_returned: QueryState#concept_files_returned.
  _QueryState.compact: QueryState#compact.
  _QueryState.backend: QueryState#backend.
  _QueryState.reset_seen_symbols: QueryState#reset_seen_symbols().
  _QueryState._seen_symbols: QueryState#_seen_symbols.
  _QueryState.__init__: QueryState#__init__().
  _QueryState.relation_cache: QueryState#relation_cache.
  _RelMap: RelMap.
---
# Module: [`tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py)

## Classes
### `_QueryState`
- def: [`tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py:14`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py#L14)
- signature: `class _QueryState:`
- members:
  - `add_symbols(self, symbols: list[dict[str, Any]])` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py#L43)
  - `reset_seen_symbols(self, seen: set[tuple[str, int, str]])` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py#L39) — Replace the seen-symbols set (for pruning operations).
  - `backend` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py#L37)
  - `compact` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py#L30)
  - `concept_files_returned` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py#L32)
  - `current` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py#L21)
  - `facets` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py#L28)
  - `files` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py#L23)
  - `relation_cache` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py#L33)
  - `relationships` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py#L24)
  - `seed_queries` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py#L31)
  - `selection_filters` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py#L36)
  - `symbols` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py#L22)
- protocol/private: `__init__`[`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py#L15), `_seen_symbols`[`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py#L29)
- uses (calls/refs, reference-scoped): [`_ChainStep`](_codegraph_query_dsl.md#_ChainStep), [`CodeGraphQueryBackend`](../../codegraph_query_backend.md#CodeGraphQueryBackend), [`symbol_key_tuple`](_codegraph_query_symbols.md#symbol_key_tuple), [`_RelMap`](_codegraph_query_state.md#_RelMap)
- used by: [`_apply_step`](codegraph_query_tool.md#CodeGraphQueryTool._apply_step), [`execute`](codegraph_query_tool.md#CodeGraphQueryTool.execute), [`_include_facets`](codegraph_query_tool.md#_include_facets), [`_relation_step`](codegraph_query_tool.md#_relation_step), [`_apply_concept_fallback`](codegraph_query_tool.md#_apply_concept_fallback), [`_filter_selection_by_related_symbols`](codegraph_query_tool.md#_filter_selection_by_related_symbols), [`replace_current_selection`](_codegraph_query_selection.md#replace_current_selection), [`sort_state`](_codegraph_query_selection.md#sort_state), [`filter_current_selection`](_codegraph_query_selection.md#filter_current_selection), [`uml_facet`](_codegraph_query_facets.md#uml_facet), [`risk_facet`](_codegraph_query_facets.md#risk_facet), [`_relation_entries_for_symbol`](codegraph_query_tool.md#_relation_entries_for_symbol), [`affected_tests_facet`](_codegraph_query_facets.md#affected_tests_facet), [`_state_backend`](codegraph_query_tool.md#_state_backend)  (11 test-only)

## Module values
- `_RelMap` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_state.py#L11)

