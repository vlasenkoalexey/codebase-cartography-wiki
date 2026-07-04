---
title: 'Module: tree_sitter_analyzer/core/query_filter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/core/query_filter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.core.query_filter`/QueryFilter#
symbols:
  QueryFilter: ''
  QueryFilter.filter_results: filter_results().
  QueryFilter._match_modifier: _match_modifier().
  QueryFilter._match_name: _match_name().
  QueryFilter._matches_single_filter: _matches_single_filter().
  QueryFilter._match_params: _match_params().
  QueryFilter._extract_method_name: _extract_method_name().
  QueryFilter._count_parameters: _count_parameters().
  QueryFilter._parse_filter_expression: _parse_filter_expression().
  QueryFilter._matches_filters: _matches_filters().
  QueryFilter.get_filter_help: get_filter_help().
  QueryFilter._match_visibility: _match_visibility().
  QueryFilter.__init__: __init__().
---
# Module: [`tree_sitter_analyzer/core/query_filter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_filter.py)

## Classes
### `QueryFilter`
- def: [`tree_sitter_analyzer/core/query_filter.py:12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_filter.py#L12)
- doc: Query result filter
- signature: `class QueryFilter:`
- members:
  - `_count_parameters(self, content: str)` — [`L175`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_filter.py#L175) — Count method parameters, handling nested generics/parens.
  - `_extract_method_name(self, content: str)` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_filter.py#L159) — Extract method name from content
  - `_match_modifier(self, result: dict[str, Any], modifier: str, value: str)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_filter.py#L137) — Match modifier as a keyword in the declaration prefix
  - `_match_name(self, result: dict[str, Any], match_type: str, value: str)` — [`L108`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_filter.py#L108) — Match method name
  - `_match_params(self, result: dict[str, Any], match_type: str, value: str)` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_filter.py#L124) — Match parameter count
  - `_match_visibility(self, result: dict[str, Any], value: str)` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_filter.py#L151) — Match visibility modifier in content
  - `_matches_filters(self, result: dict[str, Any], filters: dict[str, Any])` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_filter.py#L71) — Check if result matches all filter conditions
  - `_matches_single_filter(self, result: dict[str, Any], filter_key: str, filter_config: dict[str, Any])` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_filter.py#L78) — Check single filter condition
  - `_parse_filter_expression(self, expression: str)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_filter.py#L48) — Parse filter expression
  - `filter_results(self, results: list[dict[str, Any]], filter_expression: str)` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_filter.py#L18) — Filter query results based on filter expression
  - `get_filter_help(self)` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_filter.py#L200) — Get filter help information
- protocol/private: `__init__`[`L15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_filter.py#L15)
- used by: [`execute_query`](query_service.md#QueryService.execute_query), [`_print_filter_help`](../cli_main.md#_print_filter_help), [`parser`](query_service.md#QueryService.parser)  (77 test-only)

