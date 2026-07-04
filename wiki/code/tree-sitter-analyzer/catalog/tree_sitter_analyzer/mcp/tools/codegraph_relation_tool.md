---
title: 'Module: tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.codegraph_relation_tool`/
symbols:
  CodeGraphRelationToolMixin._get_call_graph: CodeGraphRelationToolMixin#_get_call_graph().
  CodeGraphRelationToolMixin: CodeGraphRelationToolMixin#
  CodeGraphRelationToolMixin._try_get_cache: CodeGraphRelationToolMixin#_try_get_cache().
  _is_stale_resolution: _is_stale_resolution().
  CodeGraphRelationToolMixin.project_root: CodeGraphRelationToolMixin#project_root.
  classify_callee_resolution: classify_callee_resolution().
  CodeGraphRelationToolMixin._call_graph: CodeGraphRelationToolMixin#_call_graph.
  _STALE_CACHE_WARNING: _STALE_CACHE_WARNING.
  CodeGraphRelationToolMixin._init_relation_state: CodeGraphRelationToolMixin#_init_relation_state().
  CodeGraphRelationToolMixin._reset_relation_state: CodeGraphRelationToolMixin#_reset_relation_state().
  CodeGraphRelationToolMixin._data_source: CodeGraphRelationToolMixin#_data_source.
  CodeGraphRelationToolMixin.get_call_graph: CodeGraphRelationToolMixin#get_call_graph().
  CodeGraphRelationToolMixin.call_graph_initialized: CodeGraphRelationToolMixin#call_graph_initialized().
  CodeGraphRelationToolMixin._cache_call_graph_built: CodeGraphRelationToolMixin#_cache_call_graph_built().
  CodeGraphRelationToolMixin._fetch_activation_map: CodeGraphRelationToolMixin#_fetch_activation_map().
  CodeGraphRelationToolMixin._activation_for: CodeGraphRelationToolMixin#_activation_for().
  _STDLIB_TOP_LEVELS: _STDLIB_TOP_LEVELS.
  _STALE_CACHE_UNKNOWN_RATIO: _STALE_CACHE_UNKNOWN_RATIO.
---
# Module: [`tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py)

## Classes
### `CodeGraphRelationToolMixin`
- def: [`tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py:135`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py#L135)
- doc: Shared cache and graph bootstrap for caller/callee compatibility tools.
- signature: `class CodeGraphRelationToolMixin:`
- members:
  - `_activation_for(activation_map: dict[tuple[str, int], dict[str, Any]], file_path: str, line: int)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py#L225) — Return the activation entry for a relation target, or zero-row defaults.
  - `_fetch_activation_map(cache: Any)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py#L197) — Build a (file_path, line) -> activation map from AST cache rows.
  - `call_graph_initialized(self)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py#L192) — True if the call graph has been lazily initialized (i.e. cached).
  - `get_call_graph(self)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py#L187) — Public alias for _get_call_graph() — use this instead of accessing _call_graph.
  - `project_root` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py#L138)
- protocol/private: `_cache_call_graph_built`[`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py#L168), `_call_graph`[`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py#L139), `_data_source`[`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py#L140), `_get_call_graph`[`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py#L174), `_init_relation_state`[`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py#L142), `_reset_relation_state`[`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py#L146), `_try_get_cache`[`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py#L150)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`close`](../../ast_cache.md#ASTCache.close), [`CallGraph`](../../call_graph.md#CallGraph), [`CachedCallGraph`](../../call_graph.md#CachedCallGraph), [`CodeGraphCallersTool`](callers_tool.md#CodeGraphCallersTool), [`CodeGraphCalleesTool`](callees_tool.md#CodeGraphCalleesTool), [`get_stats`](../../ast_cache.md#ASTCache.get_stats), [`has_call_edges`](../../ast_cache.md#ASTCache.has_call_edges), [`_CallTreeBase`](_call_tree_tool.md#_CallTreeBase)
- used by: [`execute`](callers_tool.md#CodeGraphCallersTool.execute), [`execute`](callees_tool.md#CodeGraphCalleesTool.execute), [`CodeGraphCallersTool`](callers_tool.md#CodeGraphCallersTool), [`CodeGraphCalleesTool`](callees_tool.md#CodeGraphCalleesTool), [`execute`](_call_tree_tool.md#_CallTreeBase.execute), [`_make_expander`](_call_tree_tool.md#_CallTreeBase._make_expander), [`_enrich_graph_callees_with_activation`](callees_tool.md#CodeGraphCalleesTool._enrich_graph_callees_with_activation), [`_CallTreeBase`](_call_tree_tool.md#_CallTreeBase), [`_inline_callee_bodies`](callees_tool.md#CodeGraphCalleesTool._inline_callee_bodies), [`_inline_caller_bodies`](callers_tool.md#CodeGraphCallersTool._inline_caller_bodies), [`_sql_native_callees`](callees_tool.md#CodeGraphCalleesTool._sql_native_callees), [`_resolve_via_enhanced`](callees_tool.md#CodeGraphCalleesTool._resolve_via_enhanced), [`_sql_native_callers`](callers_tool.md#CodeGraphCallersTool._sql_native_callers), [`__init__`](_call_tree_tool.md#_CallTreeBase.__init__), [`__init__`](callees_tool.md#CodeGraphCalleesTool.__init__), [`__init__`](callers_tool.md#CodeGraphCallersTool.__init__), [`_on_project_root_changed`](callees_tool.md#CodeGraphCalleesTool._on_project_root_changed), [`_on_project_root_changed`](callers_tool.md#CodeGraphCallersTool._on_project_root_changed), [`_on_project_root_changed`](_call_tree_tool.md#_CallTreeBase._on_project_root_changed)  (4 test-only)

## Functions
- `_is_stale_resolution(entries: list[dict[str, Any]])` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py#L94) — Return True when a relation response mostly has unknown callee resolution.
- `classify_callee_resolution(callee_name: str, callee_resolved_file: str, caller_file: str)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py#L103) — Classify callee resolution type and determine resolved file.

## Module values
- `_STALE_CACHE_UNKNOWN_RATIO` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py#L84)
- `_STALE_CACHE_WARNING` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py#L86)
- `_STDLIB_TOP_LEVELS` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.py#L11)

