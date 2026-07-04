---
title: 'Module: tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools._codegraph_query_dsl`/
symbols:
  _ChainStep: _ChainStep#
  parse_chain: parse_chain().
  _ChainStep.kwargs: _ChainStep#kwargs.
  _ChainStep.name: _ChainStep#name.
  int_kw: int_kw().
  bool_kw: bool_kw().
  _parse_step: _parse_step().
  string_args: string_args().
  _ChainStep.args: _ChainStep#args.
  first_str: first_str().
  first_int: first_int().
  step_to_dict: step_to_dict().
  _literal: _literal().
  _FILTER_KWARGS: _FILTER_KWARGS.
  _MAX_STRING_ARG_LENGTH: _MAX_STRING_ARG_LENGTH.
  _ALLOWED_KWARGS._ALLOWED_KWARGS: _ALLOWED_KWARGS._ALLOWED_KWARGS.
  _MAX_QUERY_LENGTH: _MAX_QUERY_LENGTH.
  _MAX_STEPS: _MAX_STEPS.
  _MAX_LIST_ARGS: _MAX_LIST_ARGS.
  _JS_BARE_LITERALS._JS_BARE_LITERALS: _JS_BARE_LITERALS._JS_BARE_LITERALS.
  _SUPPORTED_STEPS: _SUPPORTED_STEPS.
  _has_unquoted_pipe: _has_unquoted_pipe().
  _split_chain: _split_chain().
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py)

## Classes
### `_ChainStep`
- def: [`tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py:96`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L96)
- signature: `class _ChainStep:`
- members:
  - `args` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L98)
  - `kwargs` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L99)
  - `name` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L97)
- used by: [`_apply_step`](codegraph_query_tool.md#CodeGraphQueryTool._apply_step), [`_include_facets`](codegraph_query_tool.md#_include_facets), [`parse_chain`](_codegraph_query_dsl.md#parse_chain), [`_relation_step`](codegraph_query_tool.md#_relation_step), [`_filter_selection_by_related_symbols`](codegraph_query_tool.md#_filter_selection_by_related_symbols), [`sort_state`](_codegraph_query_selection.md#sort_state), [`bool_kw`](_codegraph_query_dsl.md#bool_kw), [`int_kw`](_codegraph_query_dsl.md#int_kw), [`_parse_step`](_codegraph_query_dsl.md#_parse_step), [`filter_current_selection`](_codegraph_query_selection.md#filter_current_selection), [`string_args`](_codegraph_query_dsl.md#string_args), [`filter_concept_entries`](_codegraph_query_selection.md#filter_concept_entries), [`_compile_symbol_predicate`](_codegraph_query_filters.md#_compile_symbol_predicate), [`filter_symbols`](_codegraph_query_filters.md#filter_symbols), [`first_str`](_codegraph_query_dsl.md#first_str), [`first_int`](_codegraph_query_dsl.md#first_int), [`step_to_dict`](_codegraph_query_dsl.md#step_to_dict), [`apply_selection_filters`](_codegraph_query_selection.md#apply_selection_filters), [`selection_filters`](_codegraph_query_state.md#_QueryState.selection_filters), [`_field_predicates`](_codegraph_query_filters.md#_field_predicates), [`concept_file_matches`](_codegraph_query_selection.md#concept_file_matches), [`selection_filters_are_file_only`](_codegraph_query_selection.md#selection_filters_are_file_only)  (27 test-only)

## Functions
- `_has_unquoted_pipe(query: str)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L102) — True when ``query`` has a ``|`` outside any single/double-quoted span.
- `_literal(node: ast.AST)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L280)
- `_parse_step(part: str)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L245)
- `_split_chain(query: str)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L210)
- `bool_kw(step: _ChainStep, name: str, default: bool)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L205)
- `first_int(step: _ChainStep, default: int)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L187)
- `first_str(step: _ChainStep, *, required: bool)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L157)
- `int_kw(step: _ChainStep, name: str, default: int, cap: int)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L196)
- `parse_chain(query: str)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L123) — Parse a safe chained query into steps.
- `step_to_dict(step: _ChainStep)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L153)
- `string_args(step: _ChainStep, *, required: bool)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L168)

## Module values
- `_ALLOWED_KWARGS` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L46)
- `_FILTER_KWARGS` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L33)
- `_JS_BARE_LITERALS` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L272)
- `_MAX_LIST_ARGS` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L12)
- `_MAX_QUERY_LENGTH` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L10)
- `_MAX_STEPS` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L11)
- `_MAX_STRING_ARG_LENGTH` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L13)
- `_SUPPORTED_STEPS` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L14)
- `__all__` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.py#L303)

