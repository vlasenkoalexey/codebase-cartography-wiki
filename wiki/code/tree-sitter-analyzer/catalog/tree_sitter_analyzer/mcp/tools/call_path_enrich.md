---
title: 'Module: tree_sitter_analyzer/mcp/tools/call_path_enrich.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/call_path_enrich.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.call_path_enrich`/
symbols:
  inline_path_bodies: inline_path_bodies().
  _build_def_index: _build_def_index().
  _read_body: _read_body().
  _endpoint_block: _endpoint_block().
  build_dead_end: build_dead_end().
  _resolve_def: _resolve_def().
  _lang_hint_for_path: _lang_hint_for_path().
  _neighbor_list: _neighbor_list().
  MAX_TOTAL_BODY_LINES: MAX_TOTAL_BODY_LINES.
  _build_def_index_scan: _build_def_index_scan().
  MAX_BODY_LINES: MAX_BODY_LINES.
  MAX_NEIGHBORS: MAX_NEIGHBORS.
  _collect_path_functions: _collect_path_functions().
---
# Module: [`tree_sitter_analyzer/mcp/tools/call_path_enrich.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_enrich.py)

## Functions
- `_build_def_index(cache: Any, names: set[str])` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_enrich.py#L53) — Return ``name -> [ {file, line, end_line, language, class} ]`` for ``names``.
- `_build_def_index_scan(conn: Any, names: set[str])` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_enrich.py#L104) — Legacy fallback: scan ``ast_index`` + JSON-parse (no ``ast_symbol_rows``).
- `_collect_path_functions(paths: list[dict[str, Any]])` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_enrich.py#L246) — Ordered unique ``(name, file_hint)`` pairs across all path hops.
- `_endpoint_block(project_root: str, cache: Any, index: dict[str, list[dict[str, Any]]], name: str, file_hint: str | None, budget: list[int])` — [`L364`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_enrich.py#L364) — Build one endpoint block: body + direct callers + direct callees.
- `_lang_hint_for_path(path: str)` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_enrich.py#L266) — Language hint for ``path``, returning empty string for ``.h`` headers.
- `_neighbor_list(rows: list[dict[str, Any]], name_key: str)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_enrich.py#L341) — Compact, de-duplicated neighbour list (name + file + line).
- `_read_body(project_root: str, defn: dict[str, Any], budget: list[int], max_body_lines: int | None = None)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_enrich.py#L182) — Read a verbatim function body, honouring per-body and total caps.
- `_resolve_def(index: dict[str, list[dict[str, Any]]], name: str, file_hint: str | None, lang_hint: str | None = None)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_enrich.py#L140) — Pick the best definition span for ``name``, preferring ``file_hint``.
- `build_dead_end(project_root: str, cache: Any, source: str, target: str, source_file: str | None, target_file: str | None)` — [`L392`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_enrich.py#L392) — Return a dead-end payload with both endpoints inlined + neighbours.
- `inline_path_bodies(project_root: str, cache: Any, paths: list[dict[str, Any]], endpoint_hints: dict[str, str] | None = None)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_enrich.py#L282) — Return ``(source_bodies, any_truncated)`` for a found path.

## Module values
- `MAX_BODY_LINES` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_enrich.py#L41)
- `MAX_NEIGHBORS` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_enrich.py#L45)
- `MAX_TOTAL_BODY_LINES` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_enrich.py#L43)

