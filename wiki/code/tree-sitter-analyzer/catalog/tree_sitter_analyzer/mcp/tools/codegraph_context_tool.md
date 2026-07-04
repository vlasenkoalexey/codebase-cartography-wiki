---
title: 'Module: tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.codegraph_context_tool`/
symbols:
  CodeGraphContextTool: CodeGraphContextTool#
  CodeGraphContextTool.execute: CodeGraphContextTool#execute().
  _extract_symbol_candidates: _extract_symbol_candidates().
  _node_id: _node_id().
  CodeGraphContextTool._expand_nodes: CodeGraphContextTool#_expand_nodes().
  _build_code_blocks: _build_code_blocks().
  CodeGraphContextTool._get_call_graph: CodeGraphContextTool#_get_call_graph().
  CodeGraphContextTool._resolve_entry_points: CodeGraphContextTool#_resolve_entry_points().
  _is_test_file: _is_test_file().
  CodeGraphContextTool._cache: CodeGraphContextTool#_cache.
  CodeGraphContextTool._get_edge_store: CodeGraphContextTool#_get_edge_store().
  CodeGraphContextTool._build_edges: CodeGraphContextTool#_build_edges().
  CodeGraphContextTool._get_cache: CodeGraphContextTool#_get_cache().
  _entry_rank_v2: _entry_rank_v2().
  CodeGraphContextTool._call_graph: CodeGraphContextTool#_call_graph.
  _is_non_prod_file: _is_non_prod_file().
  _next_step_lean: _next_step_lean().
  CodeGraphContextTool._edge_store: CodeGraphContextTool#_edge_store.
  CodeGraphContextTool._on_project_root_changed: CodeGraphContextTool#_on_project_root_changed().
  CodeGraphContextTool.add_ref: CodeGraphContextTool#add_ref().
  _node_from_ref: _node_from_ref().
  _safe_refs: _safe_refs().
  _nodes_from_hits: _nodes_from_hits().
  _extract_symbol_candidates._is_anchor: _extract_symbol_candidates()._is_anchor().
  _name_match_score: _name_match_score().
  CodeGraphContextTool._absorb: CodeGraphContextTool#_absorb().
  _bounded_int: _bounded_int().
  _compound_candidates: _compound_candidates().
  _safe_chain: _safe_chain().
  _PATH_FRAGMENT_RE: _PATH_FRAGMENT_RE.
  _coerce_bool: _coerce_bool().
  _MAX_BLOCK_LINES: _MAX_BLOCK_LINES.
  _MAX_INLINE_EDGES: _MAX_INLINE_EDGES.
  _normalise_hit: _normalise_hit().
  _next_step: _next_step().
  _build_related_symbols: _build_related_symbols().
  CodeGraphContextTool.get_tool_definition: CodeGraphContextTool#get_tool_definition().
  _entry_rank: _entry_rank().
  CodeGraphContextTool.validate_arguments: CodeGraphContextTool#validate_arguments().
  _extract_symbol_candidates._is_specific: _extract_symbol_candidates()._is_specific().
  _extract_symbol_candidates._named_explicitly: _extract_symbol_candidates()._named_explicitly().
  _callee_ref_to_hit: _callee_ref_to_hit().
  _STOP_WORDS: _STOP_WORDS.
  _GENERIC_VERBS: _GENERIC_VERBS.
  _CODE_FILE_EXT: _CODE_FILE_EXT.
  _PATH_COMPONENT_SPLIT: _PATH_COMPONENT_SPLIT.
  _MAX_ENTRY_BODY_LINES: _MAX_ENTRY_BODY_LINES.
  _MAX_INLINE_NODES: _MAX_INLINE_NODES.
  _MAX_INLINE_ENTRY_POINTS: _MAX_INLINE_ENTRY_POINTS.
  CodeGraphContextTool.get_tool_schema: CodeGraphContextTool#get_tool_schema().
  CodeGraphContextTool._edge_store_callees: CodeGraphContextTool#_edge_store_callees().
  CodeGraphContextTool._edge_store_callers: CodeGraphContextTool#_edge_store_callers().
  _FALSEY_STRINGS: _FALSEY_STRINGS.
  _caller_ref_to_hit: _caller_ref_to_hit().
  _edge_degrees: _edge_degrees().
  _unique_files: _unique_files().
  _looks_like_trace: _looks_like_trace().
  CodeGraphContextTool.__init__: CodeGraphContextTool#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py)

## Classes
### `CodeGraphContextTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py:111`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L111) — documented in [tree_sitter_analyzer-mcp-server](../../../../concepts/tree_sitter_analyzer-mcp-server.md)
- doc: MCP tool for one-call architecture context and trace expansion.
- signature: `class CodeGraphContextTool(BaseMCPTool):`
- members:
  - `_absorb(raw_hits: list[Any])` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L393) — Merge raw hits into ``agg``; return the count of USABLE hits.
  - `add_ref(ref: dict[str, Any])` — [`L484`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L484)
  - `execute(self, arguments: dict[str, Any])` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L239)
  - `get_tool_definition(self)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L167)
  - `get_tool_schema(self)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L187)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L234)
- protocol/private: `__init__`[`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L114), `_build_edges`[`L536`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L536), `_cache`[`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L115), `_call_graph`[`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L116), `_edge_store`[`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L117), `_edge_store_callees`[`L496`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L496), `_edge_store_callers`[`L504`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L504), `_expand_nodes`[`L471`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L471), `_get_cache`[`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L125), `_get_call_graph`[`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L146), `_get_edge_store`[`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L134), `_on_project_root_changed`[`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L120), `_resolve_entry_points`[`L373`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L373)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`EdgeKind`](../../graph/edge_store.md#EdgeKind), [`CachedCallGraph`](../../call_graph.md#CachedCallGraph), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`_extract_symbol_candidates`](codegraph_context_tool.md#_extract_symbol_candidates), [`EdgeStore`](../../graph/edge_store.md#EdgeStore), [`CALLS`](../../graph/edge_store.md#EdgeKind.CALLS), [`build`](../../call_graph.md#CachedCallGraph.build), [`_build_code_blocks`](codegraph_context_tool.md#_build_code_blocks), [`_entry_rank_v2`](codegraph_context_tool.md#_entry_rank_v2), [`_next_step_lean`](codegraph_context_tool.md#_next_step_lean), [`_node_from_ref`](codegraph_context_tool.md#_node_from_ref), [`_safe_refs`](codegraph_context_tool.md#_safe_refs), [`_nodes_from_hits`](codegraph_context_tool.md#_nodes_from_hits), [`_bounded_int`](codegraph_context_tool.md#_bounded_int), [`_compound_candidates`](codegraph_context_tool.md#_compound_candidates), [`_safe_chain`](codegraph_context_tool.md#_safe_chain), [`_coerce_bool`](codegraph_context_tool.md#_coerce_bool), [`_MAX_INLINE_EDGES`](codegraph_context_tool.md#_MAX_INLINE_EDGES), [`_build_related_symbols`](codegraph_context_tool.md#_build_related_symbols), [`_next_step`](codegraph_context_tool.md#_next_step), [`_normalise_hit`](codegraph_context_tool.md#_normalise_hit), [`_callee_ref_to_hit`](codegraph_context_tool.md#_callee_ref_to_hit), [`_MAX_INLINE_ENTRY_POINTS`](codegraph_context_tool.md#_MAX_INLINE_ENTRY_POINTS), [`_MAX_INLINE_NODES`](codegraph_context_tool.md#_MAX_INLINE_NODES), [`_caller_ref_to_hit`](codegraph_context_tool.md#_caller_ref_to_hit), [`_looks_like_trace`](codegraph_context_tool.md#_looks_like_trace), [`_unique_files`](codegraph_context_tool.md#_unique_files)  (1 test-only)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_nav_facade`](nav_facade.md#build_nav_facade), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`_context_route`](nav_facade.md#build_nav_facade._context_route)  (31 test-only)

## Functions
- `_bounded_int(value: Any, minimum: int, maximum: int)` — [`L601`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L601)
- `_build_code_blocks(nodes: list[dict[str, Any]], edges: list[dict[str, Any]], max_code_blocks: int, project_root: str)` — [`L824`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L824)
- `_build_related_symbols(nodes: list[dict[str, Any]])` — [`L1130`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L1130) — Build a compact CG-style related-symbols list grouped by file.
- `_callee_ref_to_hit(ref: dict[str, Any])` — [`L790`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L790)
- `_caller_ref_to_hit(ref: dict[str, Any])` — [`L801`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L801)
- `_coerce_bool(value: Any, default: bool = False)` — [`L612`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L612) — Coerce an MCP/CLI argument to bool, honouring JS-style string booleans.
- `_compound_candidates(candidates: list[str])` — [`L990`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L990) — Build camelCase joins of ordered task-word pairs.
- `_edge_degrees(nodes: list[dict[str, Any]], edges: list[dict[str, Any]])` — [`L911`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L911)
- `_entry_rank(hit: dict[str, Any])` — [`L963`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L963)
- `_entry_rank_v2(entry: dict[str, Any], candidates: list[str], wants_tests: bool = False)` — [`L1017`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L1017) — Relevance-aware ranking key for an aggregated entry-point hit.
- `_extract_symbol_candidates(task: str)` — [`L629`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L629)
- `_is_anchor(tok: str)` — [`L703`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L703)
- `_is_non_prod_file(file_path: str)` — [`L945`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L945) — Rank-tier: 1 when the file lives under a non-production directory.
- `_is_specific(tok: str)` — [`L668`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L668)
- `_is_test_file(file_path: str)` — [`L934`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L934) — Rank-tier wrapper: 1 for test files, 0 otherwise.
- `_looks_like_trace(task: str)` — [`L1063`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L1063)
- `_name_match_score(name: str, candidates: list[str])` — [`L970`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L970) — Count how many task candidates appear inside a symbol name.
- `_named_explicitly(verb: str)` — [`L671`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L671)
- `_next_step(has_code: bool, has_entry_points: bool)` — [`L1070`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L1070)
- `_next_step_lean(has_code: bool, has_entry_points: bool, entry_points: list[dict[str, Any]] | None = None)` — [`L1081`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L1081) — Next-step hint for the lean (default) response path.
- `_node_from_ref(ref: dict[str, Any])` — [`L758`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L758)
- `_node_id(name: str, file_path: str, line: int)` — [`L774`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L774)
- `_nodes_from_hits(hits: list[dict[str, Any]], max_nodes: int)` — [`L737`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L737)
- `_normalise_hit(hit: dict[str, Any])` — [`L726`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L726)
- `_safe_chain(graph: Any, name: str, file_path: str | None, depth: int)` — [`L812`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L812)
- `_safe_refs(callable_obj: Any, name: str, file_path: str | None)` — [`L778`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L778)
- `_unique_files(nodes: list[dict[str, Any]])` — [`L923`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L923)

## Module values
- `_CODE_FILE_EXT` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L67)
- `_FALSEY_STRINGS` — [`L609`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L609)
- `_GENERIC_VERBS` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L53)
- `_MAX_BLOCK_LINES` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L83)
- `_MAX_ENTRY_BODY_LINES` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L91)
- `_MAX_INLINE_EDGES` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L97)
- `_MAX_INLINE_ENTRY_POINTS` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L108)
- `_MAX_INLINE_NODES` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L104)
- `_PATH_COMPONENT_SPLIT` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L77)
- `_PATH_FRAGMENT_RE` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L71)
- `_STOP_WORDS` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_context_tool.py#L25)

