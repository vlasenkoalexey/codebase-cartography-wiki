---
title: 'Module: tree_sitter_analyzer/mcp/tools/_codegraph_query_filters.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/_codegraph_query_filters.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools._codegraph_query_filters`/
symbols:
  _compile_symbol_predicate: _compile_symbol_predicate().
  filter_symbols: filter_symbols().
  _compile_symbol_predicate.predicate: _compile_symbol_predicate().predicate().
  _field_predicates: _field_predicates().
  _text_matches: _text_matches().
  is_test_or_fixture_path: is_test_or_fixture_path().
  _fields_match: _fields_match().
  is_generated_or_vendor_path: is_generated_or_vendor_path().
  _optional_bool: _optional_bool().
  _compile_regex: _compile_regex().
  _regex_matches_symbol: _regex_matches_symbol().
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/mcp/tools/_codegraph_query_filters.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_filters.py)

## Functions
- `_compile_regex(value: Any, *, case_sensitive: bool)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_filters.py#L112)
- `_compile_symbol_predicate(step: _ChainStep)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_filters.py#L49)
- `_field_predicates(step: _ChainStep, *, case_sensitive: bool)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_filters.py#L83)
- `_fields_match(symbol: dict[str, Any], predicates: list[tuple[str, Any, bool]])` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_filters.py#L98)
- `_optional_bool(value: Any)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_filters.py#L137)
- `_regex_matches_symbol(regex: re.Pattern[str], symbol: dict[str, Any])` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_filters.py#L141)
- `_text_matches(value: str, expected: Any, *, case_sensitive: bool)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_filters.py#L124)
- `filter_symbols(symbols: list[dict[str, Any]], step: _ChainStep, *, invert: bool = False)` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_filters.py#L13) — Filter a symbol selection using literal chain predicates.
- `is_generated_or_vendor_path(path: str)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_filters.py#L44)
- `is_test_or_fixture_path(path: str)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_filters.py#L30)
- `predicate(symbol: dict[str, Any])` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_filters.py#L65)

## Module values
- `__all__` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_filters.py#L148)

