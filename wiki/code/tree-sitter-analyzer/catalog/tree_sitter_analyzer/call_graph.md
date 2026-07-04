---
title: 'Module: tree_sitter_analyzer/call_graph.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/call_graph.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.call_graph`/
symbols:
  FunctionRef: FunctionRef#
  CallGraph: CallGraph#
  CallGraph.build: CallGraph#build().
  CachedCallGraph: CachedCallGraph#
  CachedCallGraph.build: CachedCallGraph#build().
  CachedCallGraph._build_from_cache: CachedCallGraph#_build_from_cache().
  CallGraph.callees_of: CallGraph#callees_of().
  CallGraph.callers_of: CallGraph#callers_of().
  FunctionRef.qualified_name: FunctionRef#qualified_name().
  CallGraph.all_functions: CallGraph#all_functions().
  CallGraph.caller_refs_of: CallGraph#caller_refs_of().
  CallGraph.callee_refs_of: CallGraph#callee_refs_of().
  CallGraph.resolve_targets: CallGraph#resolve_targets().
  FunctionRef.to_dict: FunctionRef#to_dict().
  CallGraph.call_chain: CallGraph#call_chain().
  CallGraph.summary: CallGraph#summary().
  CallGraph._resolve_callee: CallGraph#_resolve_callee().
  CallGraph.function_refs: CallGraph#function_refs().
  CallGraph.file_impact: CallGraph#file_impact().
  CallGraph._func_by_name: CallGraph#_func_by_name.
  CallGraph._func_by_file: CallGraph#_func_by_file.
  CallGraph.call_edges: CallGraph#call_edges().
  CallGraph._functions: CallGraph#_functions.
  CallGraph.all_function_refs: CallGraph#all_function_refs().
  CallGraph._resolve_targets: CallGraph#_resolve_targets().
  CallGraph.find_enclosing_func: CallGraph#find_enclosing_func().
  CallGraph._call_edges: CallGraph#_call_edges.
  CallGraph._callees: CallGraph#_callees.
  CallGraph.callers_map: CallGraph#callers_map().
  CallGraph.callees_map: CallGraph#callees_map().
  CallGraph.functions_by_file: CallGraph#functions_by_file().
  CallGraph.all_call_edges: CallGraph#all_call_edges().
  CallGraph._callee_resolver: CallGraph#_callee_resolver.
  CallGraph._callers: CallGraph#_callers.
  CallGraph.functions_in_file: CallGraph#functions_in_file().
  CallGraph.function_refs_in_file: CallGraph#function_refs_in_file().
  CallGraph.resolve_callee: CallGraph#resolve_callee().
  CachedCallGraph._cache: CachedCallGraph#_cache.
  CallGraph._iter_source_files: CallGraph#_iter_source_files().
  CallGraph._func_by_qualified: CallGraph#_func_by_qualified.
  CachedCallGraph._built: CachedCallGraph#_built.
  CallGraph._is_excluded: CallGraph#_is_excluded().
  CallGraph._collect_import_map: CallGraph#_collect_import_map().
  CallGraph.is_built: CallGraph#is_built().
  CallGraph.is_excluded: CallGraph#is_excluded().
  CallGraph._built: CallGraph#_built.
  CallGraph._find_enclosing_func: CallGraph#_find_enclosing_func().
  FunctionRef.__eq__: FunctionRef#__eq__().
  CallGraph._build_module_to_file_map: CallGraph#_build_module_to_file_map().
  CallGraph.iter_source_files: CallGraph#iter_source_files().
  CachedCallGraph.close: CachedCallGraph#close().
  CallGraph.project_root: CallGraph#project_root.
  CallGraph._imported_names: CallGraph#_imported_names.
  FunctionRef.__init__: FunctionRef#__init__().
  FunctionRef.__hash__: FunctionRef#__hash__().
  CachedCallGraph.__init__: CachedCallGraph#__init__().
  CachedCallGraph.__del__: CachedCallGraph#__del__().
  _EXCLUDE_DIRS: _EXCLUDE_DIRS.
  CallGraph.__init__: CallGraph#__init__().
  CallGraph._module_to_file: CallGraph#_module_to_file.
  CallGraph._resolve_import_path: CallGraph#_resolve_import_path().
  CachedCallGraph._fallback: CachedCallGraph#_fallback.
  FunctionRef.__slots__: FunctionRef#__slots__.
  CallGraph._file_imports: CallGraph#_file_imports.
  CallGraph._file_module_map: CallGraph#_file_module_map.
---
# Module: [`tree_sitter_analyzer/call_graph.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py)

## Classes
### `CachedCallGraph`  ·  implements/extends CallGraph
- def: [`tree_sitter_analyzer/call_graph.py:706`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L706) — documented in [tree_sitter_analyzer-call_graph](../../concepts/tree_sitter_analyzer-call_graph.md)
- doc: CallGraph built from pre-indexed AST cache (SQLite).
- signature: `class CachedCallGraph(CallGraph):`
- members:
  - `build(self)` — [`L728`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L728) — documented in [tree_sitter_analyzer-call_graph](../../concepts/tree_sitter_analyzer-call_graph.md)
  - `close(self)` — [`L737`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L737)
- protocol/private: `__del__`[`L741`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L741), `__init__`[`L718`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L718), `_build_from_cache`[`L744`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L744), `_built`[`L839`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L839), `_cache`[`L725`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L725), `_fallback`[`L726`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L726)
- uses (calls/refs, reference-scoped): [`FunctionRef`](call_graph.md#FunctionRef), [`CallGraph`](call_graph.md#CallGraph), [`build`](call_graph.md#CallGraph.build), [`CalleeResolver`](callee_resolution.md#CalleeResolver), [`qualified_name`](call_graph.md#FunctionRef.qualified_name), [`resolve_items`](callee_resolution.md#CalleeResolver.resolve_items), [`_func_by_name`](call_graph.md#CallGraph._func_by_name), [`_func_by_file`](call_graph.md#CallGraph._func_by_file), [`_functions`](call_graph.md#CallGraph._functions), [`_call_edges`](call_graph.md#CallGraph._call_edges), [`_callees`](call_graph.md#CallGraph._callees), [`_callee_resolver`](call_graph.md#CallGraph._callee_resolver), [`_callers`](call_graph.md#CallGraph._callers), [`_func_by_qualified`](call_graph.md#CallGraph._func_by_qualified), [`__init__`](call_graph.md#CallGraph.__init__)
- used by: [`CallGraph`](call_graph.md#CallGraph), [`build`](call_graph.md#CallGraph.build), [`analyze_dead_code`](dead_code_analyzer.md#analyze_dead_code), [`_get_call_graph`](mcp/tools/codegraph_context_tool.md#CodeGraphContextTool._get_call_graph), [`_build_call_graph`](mcp/tools/utils/call_graph_impact.md#_build_call_graph), [`_get_call_graph`](mcp/tools/codegraph_relation_tool.md#CodeGraphRelationToolMixin._get_call_graph), [`_collect_call_graph_metrics`](mcp/tools/codegraph_metrics_tool.md#CodeGraphMetricsTool._collect_call_graph_metrics), [`call_graph`](mcp/tools/codegraph_visualization_hub.md#CodeGraphVisualizationHub.call_graph), [`_get_call_graph`](mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool._get_call_graph), [`_get_call_graph`](mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool._get_call_graph), [`_get_call_graph`](mcp/tools/codegraph_navigate_tool.md#CodeGraphNavigateTool._get_call_graph), [`_get_call_graph`](mcp/tools/codegraph_overview_tool.md#CodeGraphOverviewTool._get_call_graph), [`_init_call_graph`](mcp/tools/codegraph_explore_tool.md#_init_call_graph)  (31 test-only)

### `CallGraph`
- def: [`tree_sitter_analyzer/call_graph.py:101`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L101) — documented in [tree_sitter_analyzer-call_graph](../../concepts/tree_sitter_analyzer-call_graph.md)
- doc: Project-level function call graph.
- signature: `class CallGraph:`
- members:
  - `_find_enclosing_func(self, file_funcs: dict[str, FunctionRef], call_line: int)` — [`L322`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L322) — Find the function whose span contains the given line number.
  - `_iter_source_files(self, supported_exts: set[str])` — [`L244`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L244) — Return source files while pruning generated and hidden work dirs.
  - `_resolve_targets(self, func_name: str, file_path: str | None = None)` — [`L662`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L662) — Resolve a function name (and optional file) to FunctionRef(s).
  - `all_call_edges(self)` — [`L468`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L468) — Return all call edges as (caller, callee, line) tuples.
  - `all_function_refs(self)` — [`L508`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L508) — Return all discovered FunctionRef objects (not serialised dicts).
  - `all_functions(self)` — [`L453`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L453) — Return all discovered functions.
  - `build(self)` — [`L129`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L129) — Scan the project and build the call graph. — documented in [tree_sitter_analyzer-call_graph](../../concepts/tree_sitter_analyzer-call_graph.md)
  - `call_chain(self, func_name: str, file_path: str | None = None, depth: int = 5)` — [`L415`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L415) — Trace the full call chain from a function (callees, transitively).
  - `call_edges(self)` — [`L458`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L458) — Return all discovered call edges as (caller, callee, line) tuples.
  - `callee_refs_of(self, func: FunctionRef)` — [`L486`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L486) — Return callees of *func* as ``FunctionRef`` objects.
  - `callees_map(self)` — [`L527`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L527) — Return a shallow copy of the callee adjacency map.
  - `callees_of(self, func_name: str, file_path: str | None = None)` — [`L390`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L390) — Find all functions called by the given function. — documented in [tree_sitter_analyzer-call_graph](../../concepts/tree_sitter_analyzer-call_graph.md)
  - `caller_refs_of(self, func: FunctionRef)` — [`L497`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L497) — Return callers of *func* as ``FunctionRef`` objects.
  - `callers_map(self)` — [`L518`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L518) — Return a shallow copy of the caller adjacency map.
  - `callers_of(self, func_name: str, file_path: str | None = None)` — [`L365`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L365) — Find all functions that call the given function. — documented in [tree_sitter_analyzer-call_graph](../../concepts/tree_sitter_analyzer-call_graph.md)
  - `file_impact(self, file_path: str)` — [`L569`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L569) — Analyze call-graph impact of changes to a file.
  - `find_enclosing_func(self, file_funcs: dict, line_number: int)` — [`L620`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L620) — Public alias for :meth:`_find_enclosing_func`.
  - `function_refs(self)` — [`L476`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L476) — Return all discovered functions as ``FunctionRef`` objects.
  - `function_refs_in_file(self, file_path: str)` — [`L559`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L559) — Return raw :class:`FunctionRef` objects for functions in *file_path*.
  - `functions_by_file(self)` — [`L536`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L536) — Return a shallow copy of the file → FunctionRef list mapping.
  - `functions_in_file(self, file_path: str)` — [`L554`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L554) — Return all functions defined in the given file.
  - `is_built(self)` — [`L616`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L616) — Return True after :meth:`build` has been called at least once.
  - `is_excluded(self, path: Path)` — [`L646`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L646) — Public alias for :meth:`_is_excluded`.
  - `iter_source_files(self, supported_exts: set)` — [`L654`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L654) — Public alias for :meth:`_iter_source_files`.
  - `resolve_callee(self, call: dict, current_file: str, imports: dict)` — [`L633`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L633) — Public alias for :meth:`_resolve_callee`.
  - `resolve_targets(self, func_name: str, file_path: str | None = None)` — [`L541`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L541) — Public alias for _resolve_targets() — resolve name to FunctionRef(s).
  - `summary(self)` — [`L601`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L601) — Return call graph summary statistics.
  - `project_root` — [`L114`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L114)
- protocol/private: `__init__`[`L113`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L113), `_build_module_to_file_map`[`L310`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L310), `_built`[`L122`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L122), `_call_edges`[`L121`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L121), `_callee_resolver`[`L127`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L127), `_callees`[`L119`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L119), `_callers`[`L120`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L120), `_collect_import_map`[`L260`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L260), `_file_imports`[`L123`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L123), `_file_module_map`[`L124`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L124), `_func_by_file`[`L118`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L118), `_func_by_name`[`L116`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L116), `_func_by_qualified`[`L117`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L117), `_functions`[`L115`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L115), `_imported_names`[`L125`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L125), `_is_excluded`[`L237`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L237), `_module_to_file`[`L126`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L126), `_resolve_callee`[`L344`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L344), `_resolve_import_path`[`L280`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L280)
- uses (calls/refs, reference-scoped): [`FunctionRef`](call_graph.md#FunctionRef), [`Parser`](core/parser.md#Parser), [`tree`](core/parser.md#ParseResult.tree), [`success`](core/parser.md#ParseResult.success), [`_language_from_ext`](project_graph.md#_language_from_ext), [`CachedCallGraph`](call_graph.md#CachedCallGraph), [`parse_file`](core/parser.md#Parser.parse_file), [`walk_imports`](import_extractors/__init__.md#walk_imports), [`build`](call_graph.md#CachedCallGraph.build), [`ParseResult`](core/parser.md#ParseResult), [`walk_tree`](function_extraction.md#walk_tree), [`CalleeResolver`](callee_resolution.md#CalleeResolver), [`source_code`](core/parser.md#ParseResult.source_code), [`qualified_name`](call_graph.md#FunctionRef.qualified_name), [`resolve_items`](callee_resolution.md#CalleeResolver.resolve_items), [`to_dict`](call_graph.md#FunctionRef.to_dict), [`_EXCLUDE_DIRS`](call_graph.md#_EXCLUDE_DIRS)
- used by: [`execute`](mcp/tools/callers_tool.md#CodeGraphCallersTool.execute), [`compute_call_graph_impact`](mcp/tools/utils/call_graph_impact.md#compute_call_graph_impact), [`execute`](mcp/tools/callees_tool.md#CodeGraphCalleesTool.execute), [`CachedCallGraph`](call_graph.md#CachedCallGraph), [`analyze_dead_code`](dead_code_analyzer.md#analyze_dead_code), [`execute`](mcp/tools/call_graph_tool.md#CodeGraphCallTool.execute), [`_fallback_graph`](call_path.md#CallPathFinder._fallback_graph), [`_analyze_call_graph_impact`](mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool._analyze_call_graph_impact), [`build`](call_graph.md#CachedCallGraph.build), [`_build_from_cache`](call_graph.md#CachedCallGraph._build_from_cache), [`find_transitive_dead_code`](dead_code_analyzer.md#find_transitive_dead_code), [`_compute_risk_score`](mcp/tools/codegraph_impact_tool.md#_compute_risk_score), [`_function_impact`](mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool._function_impact), [`_compute_transitive_callers`](mcp/tools/codegraph_impact_tool.md#_compute_transitive_callers), [`_compute_transitive_callees`](mcp/tools/codegraph_impact_tool.md#_compute_transitive_callees), [`_test_map_route`](mcp/tools/nav_facade.md#build_nav_facade._test_map_route), [`execute`](mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool.execute), [`execute`](mcp/tools/codegraph_overview_tool.md#CodeGraphOverviewTool.execute), [`_blast_radius_for_functions`](mcp/tools/codegraph_impact_tool.md#_blast_radius_for_functions), [`_get_call_graph`](mcp/tools/call_graph_tool.md#CodeGraphCallTool._get_call_graph), [`_build_call_graph`](mcp/tools/utils/call_graph_impact.md#_build_call_graph), [`_call_hierarchy`](mcp/tools/codegraph_navigate_tool.md#CodeGraphNavigateTool._call_hierarchy), [`_edges_function`](mcp/tools/codegraph_visualize_tool.md#CodeGraphVisualizeTool._edges_function), [`_make_expander`](mcp/tools/_call_tree_tool.md#_CallTreeBase._make_expander), [`_get_call_graph`](mcp/tools/codegraph_relation_tool.md#CodeGraphRelationToolMixin._get_call_graph), [`_edges_file`](mcp/tools/codegraph_visualize_tool.md#CodeGraphVisualizeTool._edges_file), [`_collect_call_graph_metrics`](mcp/tools/codegraph_metrics_tool.md#CodeGraphMetricsTool._collect_call_graph_metrics), [`call_graph`](mcp/tools/codegraph_visualization_hub.md#CodeGraphVisualizationHub.call_graph), [`_find_entry_points`](mcp/tools/codegraph_overview_tool.md#_find_entry_points), [`_find_hub_functions`](mcp/tools/codegraph_overview_tool.md#_find_hub_functions), [`_get_call_graph`](mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool._get_call_graph), [`_co_change_route`](mcp/tools/nav_facade.md#build_nav_facade._co_change_route), [`_compute_depth_distribution`](mcp/tools/codegraph_overview_tool.md#_compute_depth_distribution), [`_edges_full`](mcp/tools/codegraph_visualize_tool.md#CodeGraphVisualizeTool._edges_full), [`_find_dead_code`](mcp/tools/codegraph_overview_tool.md#_find_dead_code), [`_get_call_graph`](mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool._get_call_graph), [`_get_call_graph`](mcp/tools/codegraph_navigate_tool.md#CodeGraphNavigateTool._get_call_graph), [`_get_call_graph`](mcp/tools/codegraph_overview_tool.md#CodeGraphOverviewTool._get_call_graph), [`_compute_module_coupling`](mcp/tools/codegraph_overview_tool.md#_compute_module_coupling), [`_maybe_bare_name_hint`](mcp/tools/call_graph_tool.md#_maybe_bare_name_hint)  (+21 more; 94 test-only)

### `FunctionRef`
- def: [`tree_sitter_analyzer/call_graph.py:50`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L50) — documented in [tree_sitter_analyzer-call_graph](../../concepts/tree_sitter_analyzer-call_graph.md)
- doc: A qualified reference to a function/method in the project.
- signature: `class FunctionRef:`
- members:
  - `qualified_name(self)` — [`L71`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L71) — documented in [tree_sitter_analyzer-call_graph](../../concepts/tree_sitter_analyzer-call_graph.md)
  - `to_dict(self)` — [`L88`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L88)
- protocol/private: `__eq__`[`L76`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L76), `__hash__`[`L85`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L85), `__init__`[`L55`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L55), `__slots__`[`L53`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L53)
- used by: [`build`](call_graph.md#CallGraph.build), [`execute`](mcp/tools/dead_code_tool.md#CodeGraphDeadCodeTool.execute), [`_analyze_call_graph_impact`](mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool._analyze_call_graph_impact), [`_build_from_cache`](call_graph.md#CachedCallGraph._build_from_cache), [`find_transitive_dead_code`](dead_code_analyzer.md#find_transitive_dead_code), [`_compute_risk_score`](mcp/tools/codegraph_impact_tool.md#_compute_risk_score), [`callees_of`](call_graph.md#CallGraph.callees_of), [`_function_impact`](mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool._function_impact), [`callers_of`](call_graph.md#CallGraph.callers_of), [`_compute_transitive_callers`](mcp/tools/codegraph_impact_tool.md#_compute_transitive_callers), [`_compute_transitive_callees`](mcp/tools/codegraph_impact_tool.md#_compute_transitive_callees), [`_test_map_route`](mcp/tools/nav_facade.md#build_nav_facade._test_map_route), [`_blast_radius_for_functions`](mcp/tools/codegraph_impact_tool.md#_blast_radius_for_functions), [`all_functions`](call_graph.md#CallGraph.all_functions), [`caller_refs_of`](call_graph.md#CallGraph.caller_refs_of), [`callee_refs_of`](call_graph.md#CallGraph.callee_refs_of), [`resolve_targets`](call_graph.md#CallGraph.resolve_targets), [`_edges_function`](mcp/tools/codegraph_visualize_tool.md#CodeGraphVisualizeTool._edges_function), [`call_chain`](call_graph.md#CallGraph.call_chain), [`summary`](call_graph.md#CallGraph.summary), [`_resolve_callee`](call_graph.md#CallGraph._resolve_callee), [`function_refs`](call_graph.md#CallGraph.function_refs), [`_edges_file`](mcp/tools/codegraph_visualize_tool.md#CodeGraphVisualizeTool._edges_file), [`_collect_call_graph_metrics`](mcp/tools/codegraph_metrics_tool.md#CodeGraphMetricsTool._collect_call_graph_metrics), [`file_impact`](call_graph.md#CallGraph.file_impact), [`_find_entry_points`](mcp/tools/codegraph_overview_tool.md#_find_entry_points), [`_find_hub_functions`](mcp/tools/codegraph_overview_tool.md#_find_hub_functions), [`_co_change_route`](mcp/tools/nav_facade.md#build_nav_facade._co_change_route), [`_compute_depth_distribution`](mcp/tools/codegraph_overview_tool.md#_compute_depth_distribution), [`_edges_full`](mcp/tools/codegraph_visualize_tool.md#CodeGraphVisualizeTool._edges_full), [`_find_dead_code`](mcp/tools/codegraph_overview_tool.md#_find_dead_code), [`_func_by_name`](call_graph.md#CallGraph._func_by_name), [`_compute_module_coupling`](mcp/tools/codegraph_overview_tool.md#_compute_module_coupling), [`_func_by_file`](call_graph.md#CallGraph._func_by_file), [`call_edges`](call_graph.md#CallGraph.call_edges), [`DeadFunction`](dead_code_analyzer.md#DeadFunction), [`_functions`](call_graph.md#CallGraph._functions), [`_resolve_targets`](call_graph.md#CallGraph._resolve_targets), [`all_function_refs`](call_graph.md#CallGraph.all_function_refs), [`_serialize_dead_function`](mcp/tools/dead_code_tool.md#_serialize_dead_function)  (+17 more; 75 test-only)

## Module values
- `_EXCLUDE_DIRS` — [`L27`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/call_graph.py#L27)

