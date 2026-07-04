---
title: 'Module: tree_sitter_analyzer/ast_cache.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/ast_cache.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.ast_cache`/
symbols:
  ASTCache: ASTCache#
  ASTCache.close: ASTCache#close().
  ASTCache.index_project: ASTCache#index_project().
  ASTCache.get_conn: ASTCache#get_conn().
  ASTCache.index_file: ASTCache#index_file().
  ASTCache._get_conn: ASTCache#_get_conn().
  ASTCache._init_db: ASTCache#_init_db().
  ASTCache.get_stats: ASTCache#get_stats().
  ASTCache.call_graph_built: ASTCache#call_graph_built().
  ASTCache.has_call_edges: ASTCache#has_call_edges().
  ASTCache.query_callees: ASTCache#query_callees().
  ASTCache.query_callers: ASTCache#query_callers().
  ASTCache._post_index_backfill: ASTCache#_post_index_backfill().
  ASTCache.fts_search_ranked: ASTCache#fts_search_ranked().
  ASTCache._indexed_source_files_are_complete: ASTCache#_indexed_source_files_are_complete().
  ASTCache._verify_schema_integrity: ASTCache#_verify_schema_integrity().
  ASTCache._walk_and_partition: ASTCache#_walk_and_partition().
  ASTCache.project_root: ASTCache#project_root.
  ASTCache.db_path: ASTCache#db_path.
  ASTCache._fts5_available: ASTCache#_fts5_available.
  ASTCache._mark_single_file_index_complete_if_needed: ASTCache#_mark_single_file_index_complete_if_needed().
  _walk_source_files: _walk_source_files().
  ASTCache.invalidate: ASTCache#invalidate().
  ASTCache._refresh_graph_edges_from_cache: ASTCache#_refresh_graph_edges_from_cache().
  ASTCache.fts_search: ASTCache#fts_search().
  ASTCache.get_functions: ASTCache#get_functions().
  ASTCache._check_cache_or_read: ASTCache#_check_cache_or_read().
  ASTCache._maybe_refresh_edge_store: ASTCache#_maybe_refresh_edge_store().
  ASTCache._index_parallel: ASTCache#_index_parallel().
  ASTCache._insert_index_row: ASTCache#_insert_index_row().
  ASTCache._search_symbols_linear: ASTCache#_search_symbols_linear().
  ASTCache.lookup: ASTCache#lookup().
  ASTCache.search_symbols: ASTCache#search_symbols().
  ASTCache.search_symbols_cascade: ASTCache#search_symbols_cascade().
  _AST_CACHE_EXTRACTOR_VERSION: _AST_CACHE_EXTRACTOR_VERSION.
  ASTCache._run_synapse_backfill: ASTCache#_run_synapse_backfill().
  ASTCache._run_unresolved_refs_backfill: ASTCache#_run_unresolved_refs_backfill().
  ASTCache.fts5_available: ASTCache#fts5_available().
  ASTCache._local: ASTCache#_local.
  ASTCache._parse_and_write: ASTCache#_parse_and_write().
  ASTCache._completed_full_index_sweep: ASTCache#_completed_full_index_sweep().
  ASTCache.backfill_cross_file_edges: ASTCache#backfill_cross_file_edges().
  ASTCache.get_cross_file_stats: ASTCache#get_cross_file_stats().
  ASTCache.get_call_edges: ASTCache#get_call_edges().
  logger: logger.
  SchemaIntegrityError: SchemaIntegrityError#
  ASTCache.parser: ASTCache#parser().
  ASTCache._write_activation_for_file: ASTCache#_write_activation_for_file().
  ASTCache.get_functions_by_file: ASTCache#get_functions_by_file().
  ASTCache._ensure_large_repo_indexes: ASTCache#_ensure_large_repo_indexes().
  ASTCache._parser: ASTCache#_parser.
  ASTCache._clear_activation_for_file: ASTCache#_clear_activation_for_file().
  ASTCache.get_imports: ASTCache#get_imports().
  ASTCache._write_imports_for_file: ASTCache#_write_imports_for_file().
  ASTCache._resolve_call_edges_for_file: ASTCache#_resolve_call_edges_for_file().
  ASTCache.get_resolved_call_edges: ASTCache#get_resolved_call_edges().
  ASTCache.get_symbols_by_kind: ASTCache#get_symbols_by_kind().
  ASTCache.query_edges: ASTCache#query_edges().
  ASTCache.get_cross_file_resolver: ASTCache#get_cross_file_resolver().
  ASTCache.query_callers_enhanced: ASTCache#query_callers_enhanced().
  ASTCache.query_callees_enhanced: ASTCache#query_callees_enhanced().
  ASTCache._resolve_worker_count: ASTCache#_resolve_worker_count().
  ASTCache.__init__: ASTCache#__init__().
  ASTCache._index_lock: ASTCache#_index_lock.
  ASTCache._cross_file_resolver: ASTCache#_cross_file_resolver.
---
# Module: [`tree_sitter_analyzer/ast_cache.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py)

## Classes
### `ASTCache`
- def: [`tree_sitter_analyzer/ast_cache.py:113`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L113) — documented in [tree_sitter_analyzer-ast_cache](../../concepts/tree_sitter_analyzer-ast_cache.md)
- doc: SQLite-backed persistent AST cache. Re-analysis of unchanged files is a simple DB lookup.
- signature: `class ASTCache:`
- members:
  - `_check_cache_or_read(self, conn: sqlite3.Connection, rel_path: str, abs_path: str, stat: os.stat_result)` — [`L249`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L249) — Return cached-response dict, or (source_code, content_hash) if stale.
  - `_clear_activation_for_file(conn: sqlite3.Connection, rel_path: str)` — [`L614`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L614) — Drop stale activation rows when project indexing runs in fast mode.
  - `_completed_full_index_sweep(stats: dict[str, Any])` — [`L448`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L448) — True when this run processed the whole source set without gaps.
  - `_ensure_large_repo_indexes(conn: sqlite3.Connection)` — [`L185`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L185) — Create non-shape-changing indexes for large-repo query hot paths.
  - `_get_conn(self)` — [`L147`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L147) — Private alias kept for backward compatibility — delegates to get_conn(). — documented in [tree_sitter_analyzer-ast_cache](../../concepts/tree_sitter_analyzer-ast_cache.md)
  - `_index_parallel(self, candidates: list[tuple[str, str]], workers: int)` — [`L581`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L581) — Dispatch parse+extract to a spawn process pool (safe on macOS/Linux).
  - `_indexed_source_files_are_complete(self)` — [`L456`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L456) — Return True when ast_index covers exactly the current source set.
  - `_insert_index_row(self, r: dict[str, Any], indexed_at: str, *, include_activation: bool = True)` — [`L594`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L594) — Write one worker result to SQLite (main table + optional FTS5).
  - `_mark_single_file_index_complete_if_needed(self, had_built_marker: bool, result: dict[str, Any])` — [`L240`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L240) — Refresh the built marker after a successful single-file reindex.
  - `_parse_and_write(self, conn: sqlite3.Connection, abs_path: str, rel_path: str, language: str, stat: os.stat_result, source_code: str, content_hash: str)` — [`L263`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L263) — Parse a file and write all cache rows.
  - `_post_index_backfill(self, stats: dict[str, Any])` — [`L482`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L482) — Run cross-file and Synapse backfills after indexing.
  - `_refresh_graph_edges_from_cache(self, file_paths: list[str] | None = None)` — [`L534`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L534) — Refresh unified EdgeStore rows from persisted AST cache rows.
  - `_resolve_call_edges_for_file(self, conn: sqlite3.Connection, rel_path: str)` — [`L313`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L313) — Resolve call edges for ``rel_path`` via Synapse.
  - `_resolve_worker_count(workers: int | None, candidates: list[Any])` — [`L469`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L469) — Pick worker count from env/arg/auto-detection.
  - `_run_synapse_backfill(self)` — [`L321`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L321) — Re-resolve every unresolved call edge. Returns stats dict or None.
  - `_run_unresolved_refs_backfill(self)` — [`L575`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L575) — Resolve persisted unresolved_refs rows into EdgeStore edges.
  - `_walk_and_partition(self, max_files: int, force: bool, activation_enabled: bool, language_filter: str | None = None)` — [`L424`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L424) — Walk source files and partition into (stats, candidates, count).
  - `_write_activation_for_file(self, conn: sqlite3.Connection, rel_path: str, inserted_symbol_rows: list[dict[str, Any]])` — [`L288`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L288) — Refresh ``ast_symbol_activation`` rows for a single file.
  - `_write_imports_for_file(self, conn: sqlite3.Connection, rel_path: str, language: str, imports: list[str] | list[dict[str, Any]])` — [`L301`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L301) — Refresh ``ast_imports`` rows for ``rel_path``.
  - `backfill_cross_file_edges(self)` — [`L942`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L942) — Resolve cross-file call edges and persist callee_resolved_file.
  - `call_graph_built(self)` — [`L910`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L910) — True iff the cache explicitly records a completed call-graph build.
  - `close(self)` — [`L950`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L950) — documented in [tree_sitter_analyzer-ast_cache](../../concepts/tree_sitter_analyzer-ast_cache.md)
  - `fts5_available(self)` — [`L152`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L152) — Return True if the SQLite FTS5 extension is available for this cache.
  - `fts_search(self, query: str, language: str | None = None, limit: int = 100)` — [`L648`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L648)
  - `fts_search_ranked(self, query: str, language: str | None = None, limit: int = 100)` — [`L660`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L660) — BM25-ranked FTS5 symbol search.
  - `get_call_edges(self)` — [`L688`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L688) — Return all stored call edges from the cache.
  - `get_conn(self)` — [`L128`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L128) — Return the thread-local SQLite connection for this cache. — documented in [tree_sitter_analyzer-ast_cache](../../concepts/tree_sitter_analyzer-ast_cache.md)
  - `get_cross_file_resolver(self)` — [`L914`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L914) — Get (or build) the CrossFileResolver for import-aware resolution.
  - `get_cross_file_stats(self)` — [`L946`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L946) — Return cross-file edge resolution statistics.
  - `get_functions(self)` — [`L742`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L742) — Return all indexed function definitions.
  - `get_functions_by_file(self, file_path: str)` — [`L755`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L755) — Return indexed function definitions for a specific file.
  - `get_imports(self)` — [`L773`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L773) — Return per-file import lists from the cache.
  - `get_resolved_call_edges(self)` — [`L717`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L717) — Return CALLS edges paired with their cross-file-resolved target file.
  - `get_stats(self)` — [`L680`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L680)
  - `get_symbols_by_kind(self, kind: str, limit: int = 50000)` — [`L779`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L779) — Return all indexed symbols of a given kind (e.g. 'class', 'variable').
  - `has_call_edges(self)` — [`L895`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L895) — Check whether the cache contains any call edge data.
  - `index_file(self, file_path: str, language: str | None = None)` — [`L210`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L210)
  - `index_project(self, max_files: int = 20000, force: bool = False, *, workers: int | None = None, resolve_only: bool = False, include_activation: bool | None = None, language_filter: str | None = None)` — [`L327`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L327) — Index every source file under ``self.project_root``. — documented in [tree_sitter_analyzer-ast_cache](../../concepts/tree_sitter_analyzer-ast_cache.md)
  - `invalidate(self, file_path: str)` — [`L683`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L683)
  - `lookup(self, file_path: str)` — [`L618`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L618)
  - `parser(self)` — [`L161`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L161) — Public accessor for the tree-sitter Parser instance.
  - `query_callees(self, caller_name: str, caller_file: str | None = None, max_depth: int = 1)` — [`L871`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L871) — SQL-native callees lookup via BFS on unified edges, with legacy fallback. — documented in [tree_sitter_analyzer-graph-edge_store](../../concepts/tree_sitter_analyzer-graph-edge_store.md)
  - `query_callees_enhanced(self, caller_name: str, caller_file: str | None = None, max_depth: int = 1)` — [`L933`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L933) — Enhanced callees lookup with cross-file import resolution.
  - `query_callers(self, callee_name: str, callee_file: str | None = None, max_depth: int = 1)` — [`L847`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L847) — SQL-native callers lookup via BFS on unified edges, with legacy fallback. — documented in [tree_sitter_analyzer-graph-edge_store](../../concepts/tree_sitter_analyzer-graph-edge_store.md)
  - `query_callers_enhanced(self, callee_name: str, callee_file: str | None = None, max_depth: int = 1)` — [`L924`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L924) — Enhanced callers lookup with cross-file import resolution.
  - `query_edges(self, kind: str, caller_name: str | None = None, callee_name: str | None = None, limit: int = 10000)` — [`L812`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L812) — Query the unified ``edges`` table by edge kind and endpoint name.
  - `search_symbols(self, query: str, language: str | None = None)` — [`L621`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L621)
  - `search_symbols_cascade(self, query: str, language: str | None = None, limit: int = 100)` — [`L629`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L629) — Three-tier cascading search: exact → FTS5 BM25 → LIKE.
  - `db_path` — [`L120`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L120)
  - `project_root` — [`L117`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L117)
- protocol/private: `__init__`[`L116`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L116), `_cross_file_resolver`[`L921`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L921), `_fts5_available`[`L124`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L124), `_index_lock`[`L123`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L123), `_init_db`[`L165`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L165), `_local`[`L121`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L121), `_maybe_refresh_edge_store`[`L522`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L522), `_parser`[`L122`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L122), `_search_symbols_linear`[`L675`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L675), `_verify_schema_integrity`[`L189`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L189)
- uses (calls/refs, reference-scoped): [`Parser`](core/parser.md#Parser), [`EdgeKind`](graph/edge_store.md#EdgeKind), [`_language_from_ext`](project_graph.md#_language_from_ext), [`write_graph_edges_for_file`](_ast_cache_write.md#write_graph_edges_for_file), [`fts_search_ranked`](_ast_cache_query.md#fts_search_ranked), [`EdgeStore`](graph/edge_store.md#EdgeStore), [`CALLS`](graph/edge_store.md#EdgeKind.CALLS), [`search_symbols_cascade`](_ast_cache_search.md#search_symbols_cascade), [`_worker_index_file`](_ast_extraction.md#_worker_index_file), [`resolve_unresolved_refs`](_ast_cache_unresolved.md#resolve_unresolved_refs), [`bfs_callers`](_ast_cache_graph.md#bfs_callers), [`bfs_callees`](_ast_cache_graph.md#bfs_callees), [`write_activation_for_file`](_ast_cache_write.md#write_activation_for_file), [`backfill_cross_file_edges`](_ast_cache_query.md#backfill_cross_file_edges), [`CrossFileResolver`](cross_file_resolver.md#CrossFileResolver), [`get_stats`](_ast_cache_query.md#get_stats), [`resolve_call_edges_for_file`](_ast_cache_synapse.md#resolve_call_edges_for_file), [`run_synapse_backfill`](_ast_cache_synapse.md#run_synapse_backfill), [`init_db`](_ast_cache_schema.md#init_db), [`mark_build_in_progress`](_ast_cache_build_state.md#mark_build_in_progress), [`reclaim_storage_after_full_rebuild`](_ast_cache_maintenance.md#reclaim_storage_after_full_rebuild), [`parse_and_write`](_ast_cache_indexer.md#parse_and_write), [`has_edges`](graph/edge_store.md#EdgeStore.has_edges), [`_content_hash`](_ast_extraction.md#_content_hash), [`clear_call_graph_built`](_ast_cache_callgraph_state.md#clear_call_graph_built), [`query_callers`](graph/edge_store.md#EdgeStore.query_callers), [`mark_call_graph_built`](_ast_cache_callgraph_state.md#mark_call_graph_built), [`mark_resolution_converged`](_ast_cache_unresolved.md#mark_resolution_converged), [`_walk_source_files`](ast_cache.md#_walk_source_files), [`query_callees`](graph/edge_store.md#EdgeStore.query_callees), [`call_graph_built`](_ast_cache_callgraph_state.md#call_graph_built), [`write_imports_for_file`](_ast_cache_write.md#write_imports_for_file), [`clear_build_in_progress`](_ast_cache_build_state.md#clear_build_in_progress), [`_has_fts5`](_ast_extraction.md#_has_fts5), [`apply_migration_v10`](_ast_cache_schema.md#apply_migration_v10), [`apply_migration_v12`](_ast_cache_schema.md#apply_migration_v12), [`apply_migration_v8`](_ast_cache_schema.md#apply_migration_v8), [`_commit_index_results`](_ast_cache_helpers.md#_commit_index_results), [`_init_worker_parser`](_ast_extraction.md#_init_worker_parser), [`apply_large_repo_indexes`](_ast_cache_schema.md#apply_large_repo_indexes)  (+28 more; 2 test-only)
- used by: [`_build_resolver_context_uncached`](synapse_resolver/_context.md#_build_resolver_context_uncached), [`audit`](miswire_audit.md#audit), [`build`](import_graph.md#ImportGraph.build), [`build`](knowledge_graph/builder.md#KnowledgeGraphBuilder.build), [`analyze_dead_code`](dead_code_analyzer.md#analyze_dead_code), [`build`](dependency_matrix.md#DependencyMatrix.build), [`analyze_code_similarity`](code_similarity.md#analyze_code_similarity), [`try_fts5_fast_path`](mcp/tools/_fts_fast_path.md#try_fts5_fast_path), [`build_resolver_context`](synapse_resolver/_context.md#build_resolver_context), [`_hierarchy_for`](mcp/tools/symbol_lineage_tool.md#SymbolLineageTool._hierarchy_for), [`_phase_incremental_sync`](mcp/tools/full_index_tool.md#CodeGraphFullIndexTool._phase_incremental_sync), [`run_watch_health`](health_homeostasis.md#run_watch_health), [`_ensure_ast_cache`](mcp/tools/utils/change_impact_analysis.md#_ensure_ast_cache), [`_prepare_index`](mcp/tools/knowledge_graph_tool.md#CodeGraphKnowledgeIndexTool._prepare_index), [`_build_call_graph`](mcp/tools/utils/call_graph_impact.md#_build_call_graph), [`load_cached_dependency_graph`](mcp/tools/utils/change_impact_cached_graph.md#load_cached_dependency_graph), [`_status`](mcp/tools/incremental_sync_tool.md#CodeGraphIncrementalSyncTool._status), [`_try_get_cache`](call_path.md#CallPathFinder._try_get_cache), [`read_hyphae_resource`](mcp/resources/hyphae_resource.md#read_hyphae_resource), [`_try_get_cache`](mcp/tools/codegraph_relation_tool.md#CodeGraphRelationToolMixin._try_get_cache), [`_status`](mcp/tools/auto_index_tool.md#CodeGraphAutoIndexTool._status), [`_get_cache`](mcp/tools/complexity_heatmap_tool.md#CodeGraphComplexityHeatmapTool._get_cache), [`_collect_inherited_methods`](mcp/tools/class_inspect_tool.md#ClassInspectTool._collect_inherited_methods), [`_find_override_source`](mcp/tools/class_inspect_tool.md#ClassInspectTool._find_override_source), [`_enrich_graph_callees_with_activation`](mcp/tools/callees_tool.md#CodeGraphCalleesTool._enrich_graph_callees_with_activation), [`_enrich_references_with_callers`](mcp/tools/symbol_lineage_tool.md#_enrich_references_with_callers), [`_phase_call_edge_stats`](mcp/tools/full_index_tool.md#CodeGraphFullIndexTool._phase_call_edge_stats), [`_safe_get_stats`](mcp/tools/codegraph_status_tool.md#CodeGraphStatusTool._safe_get_stats), [`_try_get_cache`](mcp/tools/codegraph_explore_tool.md#CodeGraphExploreTool._try_get_cache), [`_try_get_cache`](mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool._try_get_cache), [`_cache`](mcp/tools/ast_cache_tool.md#ASTCacheTool._cache), [`_ensure_cache`](mcp/tools/incremental_sync_tool.md#CodeGraphIncrementalSyncTool._ensure_cache), [`_parent_method_names`](mcp/tools/class_inspect_tool.md#ClassInspectTool._parent_method_names), [`_try_get_cache`](mcp/tools/codegraph_impact_tool.md#CodeGraphImpactTool._try_get_cache), [`_get_cache`](mcp/tools/ast_cache_tool.md#ASTCacheTool._get_cache), [`_get_cache`](mcp/tools/codegraph_context_tool.md#CodeGraphContextTool._get_cache), [`_collect_final_stats`](mcp/tools/full_index_tool.md#CodeGraphFullIndexTool._collect_final_stats), [`_evaluate`](mcp/watch_push_bridge.md#_drive_subscriptions._evaluate), [`_get_hierarchy`](mcp/tools/class_hierarchy_tool.md#ClassHierarchyTool._get_hierarchy), [`_phase_ast_cache`](mcp/tools/full_index_tool.md#CodeGraphFullIndexTool._phase_ast_cache)  (+21 more; 275 test-only)

### `SchemaIntegrityError`  ·  implements/extends RuntimeError
- def: [`tree_sitter_analyzer/ast_cache.py:95`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L95)
- doc: Raised when _init_db cannot prove all expected schema versions are present.
- signature: `class SchemaIntegrityError(RuntimeError):`
- used by: [`_verify_schema_integrity`](ast_cache.md#ASTCache._verify_schema_integrity)  (3 test-only)

## Functions
- `_walk_source_files(project_root: str)` — [`L957`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L957)

## Module values
- `_AST_CACHE_EXTRACTOR_VERSION` — [`L92`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L92)
- `logger` — [`L72`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_cache.py#L72)

