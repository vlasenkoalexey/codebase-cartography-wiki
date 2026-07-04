---
title: 'Module: tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools._codegraph_explore_helpers`/
symbols:
  _declaration_symbol_from_line: _declaration_symbol_from_line().
  concept_search: concept_search().
  _concept_file_entry: _concept_file_entry().
  _concept_candidate_paths: _concept_candidate_paths().
  extract_snippet_from_lines: extract_snippet_from_lines().
  split_query: split_query().
  extract_snippet: extract_snippet().
  _concept_rank: _concept_rank().
  read_file_lines: read_file_lines().
  _declaration_symbols_from_matches: _declaration_symbols_from_matches().
  _concept_match_rank: _concept_match_rank().
  _block_member_declaration_symbol: _block_member_declaration_symbol().
  _nearby_symbols: _nearby_symbols().
  _is_definition_like_match: _is_definition_like_match().
  _concept_candidate_paths._add_rows: _concept_candidate_paths()._add_rows().
  _block_declaration_bounds: _block_declaration_bounds().
  logger: logger.
  resolve_tokens: resolve_tokens().
  _concept_line_satisfies_declaration_query: _concept_line_satisfies_declaration_query().
  DECLARATION_TERMS: DECLARATION_TERMS.
  file_size: file_size().
  _search_terms: _search_terms().
  _term_position: _term_position().
  _declaration_end_line: _declaration_end_line().
  _dedupe_concept_symbols: _dedupe_concept_symbols().
  _is_test_like_path: _is_test_like_path().
  MIN_TOKEN_LEN: MIN_TOKEN_LEN.
  FILE_EXT_MARKERS: FILE_EXT_MARKERS.
  language_of: language_of().
  signature_from: signature_from().
  concept_response_payload: concept_response_payload().
  _is_noise_nearby_symbol: _is_noise_nearby_symbol().
---
# Module: [`tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py)

## Functions
- `_add_rows(sql: str, params: tuple[Any, ...])` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L217)
- `_block_declaration_bounds(lines: list[str], line_no: int)` — [`L516`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L516)
- `_block_member_declaration_symbol(stripped: str, line_no: int, lines: list[str], terms: list[str])` — [`L489`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L489)
- `_concept_candidate_paths(conn: Any, terms: list[str], file_tokens: list[str], *, max_paths: int)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L197) — Use structured path/symbol indexes to avoid scanning every file.
- `_concept_file_entry(*, project_root: str, rel_path: str, language: str, symbols_json: str, terms: list[str], max_matches: int)` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L296)
- `_concept_line_satisfies_declaration_query(terms_on_line: list[str], terms: list[str])` — [`L351`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L351)
- `_concept_match_rank(match: dict[str, Any], terms: list[str], lines: list[str] | None = None)` — [`L367`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L367)
- `_concept_rank(entry: dict[str, Any], terms: list[str])` — [`L569`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L569)
- `_declaration_end_line(lines: list[str], start_line: int)` — [`L541`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L541)
- `_declaration_symbol_from_line(line: str, line_no: int, lines: list[str], terms: list[str])` — [`L449`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L449)
- `_declaration_symbols_from_matches(lines: list[str], matches: list[dict[str, Any]], terms: list[str])` — [`L417`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L417)
- `_dedupe_concept_symbols(symbols: list[dict[str, Any]])` — [`L557`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L557)
- `_is_definition_like_match(text: str, terms: list[str])` — [`L598`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L598)
- `_is_noise_nearby_symbol(symbol: dict[str, Any])` — [`L611`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L611)
- `_is_test_like_path(path: str)` — [`L617`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L617)
- `_nearby_symbols(symbols_json: str, matches: list[dict[str, Any]])` — [`L384`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L384)
- `_search_terms(query_terms: list[str])` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L283)
- `_term_position(name: object, terms: list[str])` — [`L441`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L441)
- `concept_response_payload(query: str, entries: list[dict[str, Any]], *, query_terms: int)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L259)
- `concept_search(cache: Any, query_terms: list[str], file_tokens: list[str], project_root: str, max_files: int, *, max_matches_per_file: int = 5, max_file_bytes: int = 1000000)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L149) — Return ranked file-level matches for concept/natural-language queries.
- `extract_snippet(file_path: str, start_line: int, end_line: int)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L117) — Slice ``file_path`` lines [start_line, end_line] (1-based, inclusive).
- `extract_snippet_from_lines(lines: list[str], start_line: int, end_line: int)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L135) — Slice an already-read line list without re-opening the file.
- `file_size(file_path: str)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L109) — Return file size in bytes; 0 if the file is missing/unreadable.
- `language_of(defs: list[Any])` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L87) — First non-empty language string in the definitions, or "" if none.
- `read_file_lines(file_path: str)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L126) — Return all lines for ``file_path`` or [] when unreadable.
- `resolve_tokens(resolver: Any, tokens: list[str])` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L68) — Resolve each token, dedupe by (file, line), preserve first-seen order.
- `signature_from(d: Any)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L96) — Best-effort signature: ``context`` field if present, else "".
- `split_query(query: str)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L48) — Return (symbol_tokens, file_tokens) from a whitespace-tokenised query.

## Module values
- `DECLARATION_TERMS` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L45)
- `FILE_EXT_MARKERS` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L24)
- `MIN_TOKEN_LEN` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L21)
- `logger` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.py#L18)

