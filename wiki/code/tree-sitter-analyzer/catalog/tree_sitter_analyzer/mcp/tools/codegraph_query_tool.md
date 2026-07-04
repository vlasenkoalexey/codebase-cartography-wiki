---
title: 'Module: tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.codegraph_query_tool`/
symbols:
  CodeGraphQueryTool._apply_step: CodeGraphQueryTool#_apply_step().
  CodeGraphQueryTool.execute: CodeGraphQueryTool#execute().
  _include_facets: _include_facets().
  CodeGraphQueryTool: CodeGraphQueryTool#
  _relation_step: _relation_step().
  _apply_concept_fallback: _apply_concept_fallback().
  _filter_selection_by_related_symbols: _filter_selection_by_related_symbols().
  _resolve_query_with_backend: _resolve_query_with_backend().
  _resolve_query: _resolve_query().
  _relation_entries_for_symbol: _relation_entries_for_symbol().
  _MAX_SYMBOLS_CAP: _MAX_SYMBOLS_CAP.
  _semantic_queries_with_backend: _semantic_queries_with_backend().
  _query_relation_entries: _query_relation_entries().
  _state_backend: _state_backend().
  _resolve_queries_with_backend: _resolve_queries_with_backend().
  CodeGraphQueryTool._get_cache: CodeGraphQueryTool#_get_cache().
  _filter_declaration_query_symbols: _filter_declaration_query_symbols().
  _resolve_queries: _resolve_queries().
  CodeGraphQueryTool.get_cache: CodeGraphQueryTool#get_cache().
  CodeGraphQueryTool._cache: CodeGraphQueryTool#_cache.
  logger: logger.
  CodeGraphQueryTool.cache_initialized: CodeGraphQueryTool#cache_initialized().
  CodeGraphQueryTool.get_tool_definition: CodeGraphQueryTool#get_tool_definition().
  _MAX_FILES_CAP: _MAX_FILES_CAP.
  _MAX_REL_PER_SYMBOL: _MAX_REL_PER_SYMBOL.
  CodeGraphQueryTool.__init__: CodeGraphQueryTool#__init__().
  CodeGraphQueryTool._on_project_root_changed: CodeGraphQueryTool#_on_project_root_changed().
  CodeGraphQueryTool.get_tool_schema: CodeGraphQueryTool#get_tool_schema().
  CodeGraphQueryTool.validate_arguments: CodeGraphQueryTool#validate_arguments().
  _DECLARATION_QUERY_KINDS: _DECLARATION_QUERY_KINDS.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py)

## Classes
### `CodeGraphQueryTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py:114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L114)
- doc: MCP Tool: one chained query over the pre-indexed code graph.
- signature: `class CodeGraphQueryTool(BaseMCPTool):`
- members:
  - `cache_initialized(self)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L138) — True if the AST cache has been lazily initialized (i.e. cached).
  - `execute(self, arguments: dict[str, Any])` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L218) — documented in [tree_sitter_analyzer-mcp-tools-facade_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-facade_tool.md)
  - `get_cache(self)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L133) — Public alias for _get_cache() — use this instead of accessing _cache directly.
  - `get_tool_definition(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L142)
  - `get_tool_schema(self)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L166)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L212)
- protocol/private: `__init__`[`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L117), `_apply_step`[`L331`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L331), `_cache`[`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L118), `_get_cache`[`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L124), `_on_project_root_changed`[`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L121)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`build_response`](_response_builder.md#build_response), [`_ChainStep`](_codegraph_query_dsl.md#_ChainStep), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`_include_facets`](codegraph_query_tool.md#_include_facets), [`current`](_codegraph_query_state.md#_QueryState.current), [`parse_chain`](_codegraph_query_dsl.md#parse_chain), [`_relation_step`](codegraph_query_tool.md#_relation_step), [`kwargs`](_codegraph_query_dsl.md#_ChainStep.kwargs), [`_apply_concept_fallback`](codegraph_query_tool.md#_apply_concept_fallback), [`_QueryState`](_codegraph_query_state.md#_QueryState), [`name`](_codegraph_query_dsl.md#_ChainStep.name), [`_filter_selection_by_related_symbols`](codegraph_query_tool.md#_filter_selection_by_related_symbols), [`CodeGraphQueryBackend`](../../codegraph_query_backend.md#CodeGraphQueryBackend), [`sort_state`](_codegraph_query_selection.md#sort_state), [`bool_kw`](_codegraph_query_dsl.md#bool_kw), [`int_kw`](_codegraph_query_dsl.md#int_kw), [`facets`](_codegraph_query_state.md#_QueryState.facets), [`relationships`](_codegraph_query_state.md#_QueryState.relationships), [`filter_current_selection`](_codegraph_query_selection.md#filter_current_selection), [`string_args`](_codegraph_query_dsl.md#string_args), [`symbols`](_codegraph_query_state.md#_QueryState.symbols), [`build_file_entries`](_codegraph_query_symbols.md#build_file_entries), [`uml_facet`](_codegraph_query_facets.md#uml_facet), [`files`](_codegraph_query_state.md#_QueryState.files), [`compact_facets`](_codegraph_query_compact.md#compact_facets), [`add_symbols`](_codegraph_query_state.md#_QueryState.add_symbols), [`first_int`](_codegraph_query_dsl.md#first_int), [`step_to_dict`](_codegraph_query_dsl.md#step_to_dict), [`dedupe_symbols`](_codegraph_query_symbols.md#dedupe_symbols), [`_MAX_SYMBOLS_CAP`](codegraph_query_tool.md#_MAX_SYMBOLS_CAP), [`_semantic_queries_with_backend`](codegraph_query_tool.md#_semantic_queries_with_backend), [`_resolve_queries_with_backend`](codegraph_query_tool.md#_resolve_queries_with_backend), [`_state_backend`](codegraph_query_tool.md#_state_backend), [`seed_queries`](_codegraph_query_state.md#_QueryState.seed_queries), [`concept_files_returned`](_codegraph_query_state.md#_QueryState.concept_files_returned), [`compact_relationships`](_codegraph_query_compact.md#compact_relationships)  (+4 more)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_search_facade`](search_facade.md#build_search_facade)  (30 test-only)

## Functions
- `_apply_concept_fallback(*, cache: Any, project_root: str, state: _QueryState, max_files: int, max_symbols: int)` — [`L536`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L536)
- `_filter_declaration_query_symbols(query: str, symbols: list[dict[str, Any]])` — [`L514`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L514)
- `_filter_selection_by_related_symbols(cache: Any, state: _QueryState, step: _ChainStep)` — [`L685`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L685)
- `_include_facets(*, cache: Any, project_root: str, state: _QueryState, step: _ChainStep, default_max_symbols: int, default_max_files: int, default_include_code: bool)` — [`L723`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L723)
- `_query_relation_entries(*, cache: Any, backend: CodeGraphQueryBackend | None = None, direction: str, name: str, file_path: str, depth: int, limit: int)` — [`L660`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L660)
- `_relation_entries_for_symbol(*, cache: Any, state: _QueryState, direction: str, symbol: dict[str, Any], depth: int, limit: int)` — [`L631`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L631)
- `_relation_step(cache: Any, state: _QueryState, *, direction: str, step: _ChainStep)` — [`L602`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L602)
- `_resolve_queries(cache: Any, queries: list[str], limit: int)` — [`L566`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L566)
- `_resolve_queries_with_backend(backend: CodeGraphQueryBackend, queries: list[str], limit: int)` — [`L573`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L573)
- `_resolve_query(cache: Any, query: str, limit: int)` — [`L468`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L468)
- `_resolve_query_with_backend(backend: CodeGraphQueryBackend, query: str, limit: int)` — [`L482`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L482)
- `_semantic_queries_with_backend(backend: CodeGraphQueryBackend, queries: list[str], limit: int)` — [`L586`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L586)
- `_state_backend(state: _QueryState, cache: Any)` — [`L476`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L476)

## Module values
- `_DECLARATION_QUERY_KINDS` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L111)
- `_MAX_FILES_CAP` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L109)
- `_MAX_REL_PER_SYMBOL` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L110)
- `_MAX_SYMBOLS_CAP` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L108)
- `__all__` — [`L796`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L796)
- `logger` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_query_tool.py#L106)

