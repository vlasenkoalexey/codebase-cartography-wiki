---
title: 'Module: tests/unit/test_codegraph_explore_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_explore_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_explore_helpers`/TestConcept
symbols:
  TestConceptSearchHelpers.test_declaration_helpers_cover_invalid_lines_and_unclosed_blocks: SearchHelpers#test_declaration_helpers_cover_invalid_lines_and_unclosed_blocks().
  TestConceptSearchHelpers.test_definition_like_and_test_path_helpers_cover_go: SearchHelpers#test_definition_like_and_test_path_helpers_cover_go().
  TestConceptCandidatePathsFts5Path._make_conn: CandidatePathsFts5Path#_make_conn().
  TestConceptSearchHelpers.test_declaration_symbol_from_line_supports_go_const_blocks: SearchHelpers#test_declaration_symbol_from_line_supports_go_const_blocks().
  TestConceptCandidatePathsFts5Path.test_fts5_path_returns_candidate_file: CandidatePathsFts5Path#test_fts5_path_returns_candidate_file().
  TestConceptCandidatePathsFts5Path.test_fts5_path_falls_back_when_no_match: CandidatePathsFts5Path#test_fts5_path_falls_back_when_no_match().
  TestConceptCandidatePathsFts5Path.test_fts5_path_honours_max_paths: CandidatePathsFts5Path#test_fts5_path_honours_max_paths().
  TestConceptSearchHelpers.test_extract_snippet_from_lines_handles_invalid_ranges: SearchHelpers#test_extract_snippet_from_lines_handles_invalid_ranges().
  TestConceptSearchHelpers.test_search_terms_drops_short_and_duplicate_tokens: SearchHelpers#test_search_terms_drops_short_and_duplicate_tokens().
  TestConceptSearchHelpers.test_concept_search_returns_empty_without_search_terms: SearchHelpers#test_concept_search_returns_empty_without_search_terms().
  TestConceptSearchHelpers.test_concept_candidate_paths_handles_tuple_rows_caps_and_fallback: SearchHelpers#test_concept_candidate_paths_handles_tuple_rows_caps_and_fallback().
  TestConceptSearchHelpers.test_concept_candidate_paths_stops_when_already_capped: SearchHelpers#test_concept_candidate_paths_stops_when_already_capped().
  TestConceptSearchHelpers.test_concept_candidate_paths_returns_empty_without_tokens: SearchHelpers#test_concept_candidate_paths_returns_empty_without_tokens().
  TestConceptSearchHelpers.test_concept_candidate_paths_full_scans_declaration_queries: SearchHelpers#test_concept_candidate_paths_full_scans_declaration_queries().
  TestConceptSearchHelpers.test_concept_candidate_paths_breaks_after_term_cap: SearchHelpers#test_concept_candidate_paths_breaks_after_term_cap().
  TestConceptSearchHelpers.test_ranks_src_multi_term_match_above_test_fixture: SearchHelpers#test_ranks_src_multi_term_match_above_test_fixture().
  TestConceptSearchHelpers.test_concept_search_skips_candidate_filters_and_unreadable_files: SearchHelpers#test_concept_search_skips_candidate_filters_and_unreadable_files().
  TestConceptSearchHelpers.test_concept_search_skips_rows_outside_index_candidates: SearchHelpers#test_concept_search_skips_rows_outside_index_candidates().
  TestConceptSearchHelpers.test_concept_file_entry_returns_none_without_text_matches: SearchHelpers#test_concept_file_entry_returns_none_without_text_matches().
  TestConceptSearchHelpers.test_concept_file_entry_stops_at_max_matches: SearchHelpers#test_concept_file_entry_stops_at_max_matches().
  TestConceptSearchHelpers.test_concept_file_entry_prioritizes_type_declaration_matches: SearchHelpers#test_concept_file_entry_prioritizes_type_declaration_matches().
  TestConceptSearchHelpers.test_concept_search_ranks_declaration_file_above_test_usage: SearchHelpers#test_concept_search_ranks_declaration_file_above_test_usage().
  TestConceptSearchHelpers.test_declaration_symbol_from_line_supports_go_type_aliases: SearchHelpers#test_declaration_symbol_from_line_supports_go_type_aliases().
  TestConceptSearchHelpers.test_block_declaration_bounds_cover_invalid_and_unclosed_blocks: SearchHelpers#test_block_declaration_bounds_cover_invalid_and_unclosed_blocks().
  TestConceptSearchHelpers.test_concept_search_ranks_const_block_source_above_test_usage: SearchHelpers#test_concept_search_ranks_const_block_source_above_test_usage().
  TestConceptSearchHelpers.test_dedupe_concept_symbols_skips_invalid_and_duplicates: SearchHelpers#test_dedupe_concept_symbols_skips_invalid_and_duplicates().
  TestConceptSearchHelpers.test_nearby_symbols_skips_far_duplicates_and_caps_results: SearchHelpers#test_nearby_symbols_skips_far_duplicates_and_caps_results().
  TestConceptSearchHelpers.test_nearby_symbols_degrades_on_invalid_json: SearchHelpers#test_nearby_symbols_degrades_on_invalid_json().
  TestConceptSearchHelpers.test_definition_like_match_requires_term_in_text: SearchHelpers#test_definition_like_match_requires_term_in_text().
  TestConceptCandidatePathsFts5Path._SCHEMA: CandidatePathsFts5Path#_SCHEMA.
  TestConceptSearchHelpers: SearchHelpers#
  TestConceptCandidatePathsFts5Path: CandidatePathsFts5Path#
---
# Module: [`tests/unit/test_codegraph_explore_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py)

## Classes
### `TestConceptCandidatePathsFts5Path`
- def: [`tests/unit/test_codegraph_explore_helpers.py:561`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L561)
- doc: Tests for the FTS5 fast path in _concept_candidate_paths (GE optimization).
- signature: `class TestConceptCandidatePathsFts5Path:`
- members:
  - `test_fts5_path_falls_back_when_no_match(self)` — [`L601`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L601)
  - `test_fts5_path_honours_max_paths(self)` — [`L610`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L610)
  - `test_fts5_path_returns_candidate_file(self)` — [`L594`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L594)
- protocol/private: `_SCHEMA`[`L564`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L564), `_make_conn`[`L571`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L571)
- uses (calls/refs, reference-scoped): [`_concept_candidate_paths`](../../tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.md#_concept_candidate_paths)

### `TestConceptSearchHelpers`
- def: [`tests/unit/test_codegraph_explore_helpers.py:12`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L12)
- signature: `class TestConceptSearchHelpers:`
- members:
  - `test_block_declaration_bounds_cover_invalid_and_unclosed_blocks(self)` — [`L426`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L426)
  - `test_concept_candidate_paths_breaks_after_term_cap(self)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L67)
  - `test_concept_candidate_paths_full_scans_declaration_queries(self)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L57)
  - `test_concept_candidate_paths_handles_tuple_rows_caps_and_fallback(self)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L29)
  - `test_concept_candidate_paths_returns_empty_without_tokens(self)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L52)
  - `test_concept_candidate_paths_stops_when_already_capped(self)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L45)
  - `test_concept_file_entry_prioritizes_type_declaration_matches(self, tmp_path)` — [`L254`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L254)
  - `test_concept_file_entry_returns_none_without_text_matches(self, tmp_path)` — [`L223`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L223)
  - `test_concept_file_entry_stops_at_max_matches(self, tmp_path)` — [`L238`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L238)
  - `test_concept_search_ranks_const_block_source_above_test_usage(self, tmp_path)` — [`L438`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L438)
  - `test_concept_search_ranks_declaration_file_above_test_usage(self, tmp_path)` — [`L288`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L288)
  - `test_concept_search_returns_empty_without_search_terms(self)` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L25)
  - `test_concept_search_skips_candidate_filters_and_unreadable_files(self, tmp_path)` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L138)
  - `test_concept_search_skips_rows_outside_index_candidates(self, tmp_path)` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L181)
  - `test_declaration_helpers_cover_invalid_lines_and_unclosed_blocks(self)` — [`L334`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L334)
  - `test_declaration_symbol_from_line_supports_go_const_blocks(self)` — [`L381`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L381)
  - `test_declaration_symbol_from_line_supports_go_type_aliases(self)` — [`L358`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L358)
  - `test_dedupe_concept_symbols_skips_invalid_and_duplicates(self)` — [`L493`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L493)
  - `test_definition_like_and_test_path_helpers_cover_go(self)` — [`L528`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L528)
  - `test_definition_like_match_requires_term_in_text(self)` — [`L552`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L552)
  - `test_extract_snippet_from_lines_handles_invalid_ranges(self)` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L13)
  - `test_nearby_symbols_degrades_on_invalid_json(self)` — [`L525`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L525)
  - `test_nearby_symbols_skips_far_duplicates_and_caps_results(self)` — [`L506`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L506)
  - `test_ranks_src_multi_term_match_above_test_fixture(self, tmp_path)` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L82)
  - `test_search_terms_drops_short_and_duplicate_tokens(self)` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_explore_helpers.py#L19)
- uses (calls/refs, reference-scoped): [`_declaration_symbol_from_line`](../../tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.md#_declaration_symbol_from_line), [`concept_search`](../../tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.md#concept_search), [`_concept_file_entry`](../../tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.md#_concept_file_entry), [`_concept_candidate_paths`](../../tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.md#_concept_candidate_paths), [`extract_snippet_from_lines`](../../tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.md#extract_snippet_from_lines), [`_concept_rank`](../../tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.md#_concept_rank), [`_declaration_symbols_from_matches`](../../tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.md#_declaration_symbols_from_matches), [`_nearby_symbols`](../../tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.md#_nearby_symbols), [`_is_definition_like_match`](../../tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.md#_is_definition_like_match), [`_block_declaration_bounds`](../../tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.md#_block_declaration_bounds), [`_declaration_end_line`](../../tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.md#_declaration_end_line), [`_dedupe_concept_symbols`](../../tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.md#_dedupe_concept_symbols), [`_is_test_like_path`](../../tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.md#_is_test_like_path), [`_search_terms`](../../tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.md#_search_terms), [`_term_position`](../../tree_sitter_analyzer/mcp/tools/_codegraph_explore_helpers.md#_term_position)

