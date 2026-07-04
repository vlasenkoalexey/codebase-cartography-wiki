---
title: 'Module: tree_sitter_analyzer/_ast_cache_unresolved.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_ast_cache_unresolved.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._ast_cache_unresolved`/
symbols:
  resolve_unresolved_refs: resolve_unresolved_refs().
  _call_refs: _call_refs().
  _resolved_edge: _resolved_edge().
  _candidate_symbols: _candidate_symbols().
  _update_call_edge_resolution: _update_call_edge_resolution().
  _choose_candidate: _choose_candidate().
  _parent_refs: _parent_refs().
  resolution_converged: resolution_converged().
  _pending_refs_for_file: _pending_refs_for_file().
  mark_resolution_converged: mark_resolution_converged().
  _is_obvious_external: _is_obvious_external().
  _candidates_for_name_kind: _candidates_for_name_kind().
  _import_target_hints: _import_target_hints().
  _reference_names: _reference_names().
  _call_rows: _call_rows().
  _base_name: _base_name().
  _line: _line().
  index_resolution_fingerprint: index_resolution_fingerprint().
  _choose_candidate.score: _choose_candidate().score().
  logger: logger.
  _row_to_dict: _row_to_dict().
  _file_language: _file_language().
  _refs_supported: _refs_supported().
  pending_unresolved_count: pending_unresolved_count().
  _ref: _ref().
  _module_path_candidates: _module_path_candidates().
  _matches_import_hint: _matches_import_hint().
  _call_is_resolved: _call_is_resolved().
  _local_names: _local_names().
  _unique: _unique().
  _CALL_ROW_COLUMNS: _CALL_ROW_COLUMNS.
---
# Module: [`tree_sitter_analyzer/_ast_cache_unresolved.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py)

## Functions
- `_base_name(name: str)` — [`L685`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L685)
- `_call_is_resolved(edge: dict[str, Any])` — [`L624`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L624)
- `_call_refs(conn: sqlite3.Connection, rel_path: str, language: str, fallback_edges: list[dict[str, Any]], local_callables: set[str])` — [`L282`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L282)
- `_call_rows(conn: sqlite3.Connection, rel_path: str, fallback_edges: list[dict[str, Any]])` — [`L308`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L308) — Return this file's CALLS rows from the unified ``edges`` table (B1.3).
- `_candidate_symbols(conn: sqlite3.Connection, source_file: str, reference_name: str, reference_kind: str, cache: dict[tuple[str, str], list[dict[str, Any]] | None] | None = None)` — [`L331`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L331) — documented in [tree_sitter_analyzer-graph-edge_store](../../concepts/tree_sitter_analyzer-graph-edge_store.md)
- `_candidates_for_name_kind(conn: sqlite3.Connection, name: str, kind: str, cache: dict[tuple[str, str], list[dict[str, Any]] | None] | None)` — [`L356`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L356) — Built candidate items for one ``(name, kind)``; cached when ``cache`` given.
- `_choose_candidate(conn: sqlite3.Connection, row: dict[str, Any], candidates: list[dict[str, Any]])` — [`L432`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L432)
- `_file_language(conn: sqlite3.Connection, file_path: str)` — [`L611`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L611)
- `_import_target_hints(conn: sqlite3.Connection, source_file: str, reference_name: str)` — [`L569`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L569)
- `_is_obvious_external(language: str, callee_name: str, callee_full: str = "")` — [`L632`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L632) — Return True when ``callee_name`` is clearly a stdlib/builtin call.
- `_line(value: Any)` — [`L689`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L689)
- `_local_names(symbol_items: list[dict[str, Any]], kinds: set[str])` — [`L677`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L677)
- `_matches_import_hint(file_path: str, hints: set[str])` — [`L605`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L605)
- `_module_path_candidates(module_path: str)` — [`L598`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L598)
- `_parent_refs(rel_path: str, symbol_items: list[dict[str, Any]], local_classes: set[str])` — [`L253`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L253)
- `_pending_refs_for_file(conn: sqlite3.Connection, rel_path: str, language: str, symbols: dict[str, Any])` — [`L59`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L59) — Recompute the pending second-pass refs for one Python file.
- `_ref(from_node_id: str, reference_name: str, reference_kind: str, file_path: str, line: int)` — [`L237`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L237)
- `_reference_names(conn: sqlite3.Connection, source_file: str, reference_name: str)` — [`L407`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L407)
- `_refs_supported(language: str)` — [`L46`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L46) — Whether second-pass resolution adds value for a language.
- `_resolved_edge(conn: sqlite3.Connection, row: dict[str, Any], candidate: dict[str, Any], candidate_count: int)` — [`L491`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L491) — documented in [tree_sitter_analyzer-graph-edge_store](../../concepts/tree_sitter_analyzer-graph-edge_store.md)
- `_row_to_dict(row: Any, columns: tuple[str, ...])` — [`L706`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L706)
- `_unique(values: list[str])` — [`L696`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L696)
- `_update_call_edge_resolution(conn: sqlite3.Connection, row: dict[str, Any], candidate: dict[str, Any])` — [`L532`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L532) — documented in [tree_sitter_analyzer-graph-edge_store](../../concepts/tree_sitter_analyzer-graph-edge_store.md)
- `index_resolution_fingerprint(conn: sqlite3.Connection)` — [`L179`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L179) — Cheap fingerprint of the indexed-file set: ``"<count>:<max indexed_at>"``.
- `mark_resolution_converged(conn: sqlite3.Connection)` — [`L217`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L217) — Persist that the resolve pass has converged for the current index state.
- `pending_unresolved_count(conn: sqlite3.Connection)` — [`L158`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L158) — Return a cheap count of references still awaiting cross-file resolution.
- `resolution_converged(conn: sqlite3.Connection)` — [`L200`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L200) — True when the resolve pass already ran for the current index state.
- `resolve_unresolved_refs(conn: sqlite3.Connection)` — [`L83`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L83) — Resolve pending cross-file refs into unified ``edges`` rows. — documented in [tree_sitter_analyzer-ast_cache](../../concepts/tree_sitter_analyzer-ast_cache.md)
- `score(item: dict[str, Any])` — [`L471`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L471)

## Module values
- `_CALL_ROW_COLUMNS` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L32)
- `logger` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_unresolved.py#L30)

