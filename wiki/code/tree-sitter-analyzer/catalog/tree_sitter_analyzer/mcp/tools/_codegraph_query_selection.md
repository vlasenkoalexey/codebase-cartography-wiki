---
title: 'Module: tree_sitter_analyzer/mcp/tools/_codegraph_query_selection.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/_codegraph_query_selection.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools._codegraph_query_selection`/
symbols:
  replace_current_selection: replace_current_selection().
  sort_state: sort_state().
  filter_current_selection: filter_current_selection().
  filter_concept_entries: filter_concept_entries().
  apply_selection_filters: apply_selection_filters().
  is_relation_noise_symbol: is_relation_noise_symbol().
  concept_file_matches: concept_file_matches().
  selection_filters_are_file_only: selection_filters_are_file_only().
  sort_state.sort_key: sort_state().sort_key().
  prune_relationships: prune_relationships().
  _RELATION_NOISE_SYMBOLS: _RELATION_NOISE_SYMBOLS.
  concept_symbol_to_query_symbol: concept_symbol_to_query_symbol().
---
# Module: [`tree_sitter_analyzer/mcp/tools/_codegraph_query_selection.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_selection.py)

## Functions
- `apply_selection_filters(symbols: list[dict[str, Any]], selection_filters: list[tuple[_ChainStep, bool]])` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_selection.py#L79)
- `concept_file_matches(entry: dict[str, Any], selection_filters: list[tuple[_ChainStep, bool]], file_only: bool)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_selection.py#L119)
- `concept_symbol_to_query_symbol(entry: dict[str, Any], symbol: dict[str, Any])` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_selection.py#L145)
- `filter_concept_entries(entries: list[dict[str, Any]], selection_filters: list[tuple[_ChainStep, bool]])` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_selection.py#L89)
- `filter_current_selection(state: _QueryState, step: _ChainStep, *, invert: bool)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_selection.py#L50)
- `is_relation_noise_symbol(symbol: dict[str, Any])` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_selection.py#L179)
- `prune_relationships(relationships: dict[str, dict[str, list[dict[str, Any]]]], *, keep_tuples: set[tuple[str, int, str]], keep_keys: set[str])` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_selection.py#L160)
- `replace_current_selection(state: _QueryState, selected: list[dict[str, Any]])` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_selection.py#L61)
- `selection_filters_are_file_only(selection_filters: list[tuple[_ChainStep, bool]])` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_selection.py#L136)
- `sort_key(symbol: dict[str, Any])` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_selection.py#L199)
- `sort_state(state: _QueryState, step: _ChainStep)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_selection.py#L184)

## Module values
- `_RELATION_NOISE_SYMBOLS` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_selection.py#L24)

