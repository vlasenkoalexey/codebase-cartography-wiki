---
title: 'Module: tree_sitter_analyzer/mcp/tools/query_symbol_search.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/query_symbol_search.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.query_symbol_search`/
symbols:
  execute_symbol_search: execute_symbol_search().
  execute_find_references: execute_find_references().
  _build_match_fn: _build_match_fn().
  _scatter_symbol_search: _scatter_symbol_search().
  _scatter_find_references: _scatter_find_references().
  _collect_source_files: _collect_source_files().
  _build_type_filter: _build_type_filter().
  _scatter_symbol_search._search_file: _scatter_symbol_search()._search_file().
  _try_fts_ranked_search: _try_fts_ranked_search().
  _scatter_find_references._scan_one: _scatter_find_references()._scan_one().
  _classify_element_for_references: _classify_element_for_references().
  _assemble_symbol_search_response: _assemble_symbol_search_response().
  _assemble_find_references_response: _assemble_find_references_response().
  _record_unique_ref: _record_unique_ref().
  _SYMBOL_SEARCH_MAX_FILES: _SYMBOL_SEARCH_MAX_FILES.
  _SYMBOL_SEARCH_BATCH_SIZE: _SYMBOL_SEARCH_BATCH_SIZE.
  _scan_file_for_references: _scan_file_for_references().
  categorize_queries: categorize_queries().
  _fts_symbol_to_match: _fts_symbol_to_match().
  logger: logger.
  _resolve_project_root: _resolve_project_root().
  _make_reference_row: _make_reference_row().
  _TYPE_MAP: _TYPE_MAP.
  _SYMBOL_SEARCH_EXTS: _SYMBOL_SEARCH_EXTS.
  _parse_symbol_search_args: _parse_symbol_search_args().
  _search_one_file_for_symbol: _search_one_file_for_symbol().
  _build_match_fn.fuzzy: _build_match_fn().fuzzy().
  _build_match_fn.wildcard: _build_match_fn().wildcard().
  _build_match_fn.exact: _build_match_fn().exact().
  _build_type_filter.type_check: _build_type_filter().type_check().
  _parse_find_references_args: _parse_find_references_args().
  _is_definition_element: _is_definition_element().
---
# Module: [`tree_sitter_analyzer/mcp/tools/query_symbol_search.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py)

## Functions
- `_assemble_find_references_response(symbol: str, output_format: str, source_files: list[Path], definitions: list[dict[str, Any]], references: list[dict[str, Any]])` — [`L565`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L565) — Build the canonical ``execute_find_references`` envelope.
- `_assemble_symbol_search_response(symbol: str, output_format: str, source_files: list[Path], results: list[dict[str, Any]], *, ranked: bool = False, ranking_method: str = "")` — [`L302`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L302) — Build the canonical ``execute_symbol_search`` envelope.
- `_build_match_fn(symbol: str)` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L342) — Build a name-matching function based on the symbol pattern.
- `_build_type_filter(symbol_type: str | None)` — [`L371`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L371) — Build an element type filter function.
- `_classify_element_for_references(e: Any, rel: str, bare_name: str, seen_refs: set[tuple[str, int]], refs: list[dict[str, Any]], defs: list[dict[str, Any]])` — [`L489`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L489) — Sort a single AST element into definitions / references / related buckets.
- `_collect_source_files(root: Path)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L170) — Walk ``root`` for source files, applying excludes + the 500 cap.
- `_fts_symbol_to_match(row: dict[str, Any], root: Path)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L276) — Convert a fts_search_ranked row to the standard match dict shape.
- `_is_definition_element(etype: str)` — [`L525`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L525) — Return True if an element type string represents a definition/declaration.
- `_make_reference_row(name: str, etype: str, rel: str, start: int, end: int, role: str)` — [`L533`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L533) — Canonical row shape for both definitions + references.
- `_parse_find_references_args(arguments: dict[str, Any])` — [`L414`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L414) — Validate + extract symbol + output_format from arguments.
- `_parse_symbol_search_args(arguments: dict[str, Any])` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L147) — Validate + extract the 4 inputs ``execute_symbol_search`` needs.
- `_record_unique_ref(rel: str, start: int, seen_refs: set[tuple[str, int]], refs: list[dict[str, Any]], name: str, etype: str, end: int, role: str)` — [`L547`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L547) — Append a reference row only if (rel, start) hasn't been seen yet.
- `_resolve_project_root(project_root: str | None)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L160) — Validate ``project_root`` and return its resolved ``Path``.
- `_scan_file_for_references(fp: Path, root: Path, engine: Any, bare_name: str, seen_refs: set[tuple[str, int]], AnalysisRequest: Any, detect_language_from_file: Any)` — [`L461`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L461) — One file's contribution to references + definitions.
- `_scan_one(fp: Path)` — [`L439`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L439)
- `_scatter_find_references(root: Path, source_files: list[Path], bare_name: str)` — [`L423`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L423) — Run per-file reference scan in 50-file batches, return (defs, refs).
- `_scatter_symbol_search(root: Path, source_files: list[Path], language: str | None, match_fn: Any, type_filter: Any)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L199) — Run per-file symbol search in 50-file batches, return flat result list.
- `_search_file(fp: Path)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L214)
- `_search_one_file_for_symbol(fp: Path, root: Path, engine: Any, language: str | None, match_fn: Any, type_filter: Any, AnalysisRequest: Any, detect_language_from_file: Any)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L235) — Per-file symbol search — analyze, filter by name + type, collect hits.
- `_try_fts_ranked_search(root: Path, symbol: str, language: str | None)` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L288) — Try the FTS5 BM25 fast path. Returns [] on any failure or miss.
- `categorize_queries(query_names: list[str], language: str)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L48) — Group query names into categories for better AI agent discoverability.
- `exact(name: str)` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L365)
- `execute_find_references(project_root: str | None, arguments: dict[str, Any])` — [`L387`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L387) — Find all references (call sites / usages) of a symbol across the project.
- `execute_symbol_search(project_root: str | None, arguments: dict[str, Any])` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L107) — Search for a symbol definition across all project source files.
- `fuzzy(name: str)` — [`L352`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L352)
- `type_check(etype: str)` — [`L380`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L380)
- `wildcard(name: str)` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L360)

## Module values
- `_SYMBOL_SEARCH_BATCH_SIZE` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L45)
- `_SYMBOL_SEARCH_EXTS` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L26)
- `_SYMBOL_SEARCH_MAX_FILES` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L44)
- `_TYPE_MAP` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L13)
- `logger` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_symbol_search.py#L11)

