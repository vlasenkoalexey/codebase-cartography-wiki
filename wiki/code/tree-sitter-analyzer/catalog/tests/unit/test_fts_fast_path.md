---
title: 'Module: tests/unit/test_fts_fast_path.py'
type: catalog
provenance: extracted
module: tests/unit/test_fts_fast_path.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_fts_fast_path`/
symbols:
  TestTryFts5FastPath.test_finds_symbol_from_index: TestTryFts5FastPath#test_finds_symbol_from_index().
  TestTryFts5FastPath.test_total_only_mode_returns_dict: TestTryFts5FastPath#test_total_only_mode_returns_dict().
  TestTryFts5FastPath.test_count_only_mode: TestTryFts5FastPath#test_count_only_mode().
  TestTryFts5FastPath.test_summary_mode: TestTryFts5FastPath#test_summary_mode().
  TestTryFts5FastPath.test_no_match_returns_none: TestTryFts5FastPath#test_no_match_returns_none().
  TestTryFts5FastPath.test_language_filter_via_extensions: TestTryFts5FastPath#test_language_filter_via_extensions().
  TestTryFts5FastPath.test_multifile_search: TestTryFts5FastPath#test_multifile_search().
  TestSearchContentFtsIntegration._setup_indexed_project: TestSearchContentFtsIntegration#_setup_indexed_project().
  _write_py_file: _write_py_file().
  TestSearchContentFtsIntegration.test_search_content_uses_fts_for_simple_query: TestSearchContentFtsIntegration#test_search_content_uses_fts_for_simple_query().
  TestSearchContentFtsIntegration.test_search_content_falls_through_for_regex: TestSearchContentFtsIntegration#test_search_content_falls_through_for_regex().
  TestIsFtsEligible.test_simple_identifier: TestIsFtsEligible#test_simple_identifier().
  TestIsFtsEligible.test_identifier_with_underscore: TestIsFtsEligible#test_identifier_with_underscore().
  TestIsFtsEligible.test_camel_case: TestIsFtsEligible#test_camel_case().
  TestIsFtsEligible.test_regex_pattern_rejected: TestIsFtsEligible#test_regex_pattern_rejected().
  TestIsFtsEligible.test_empty_query_rejected: TestIsFtsEligible#test_empty_query_rejected().
  TestIsFtsEligible.test_query_with_spaces_rejected: TestIsFtsEligible#test_query_with_spaces_rejected().
  TestIsFtsEligible.test_fixed_strings_rejected: TestIsFtsEligible#test_fixed_strings_rejected().
  TestIsFtsEligible.test_word_flag_rejected: TestIsFtsEligible#test_word_flag_rejected().
  TestIsFtsEligible.test_multiline_rejected: TestIsFtsEligible#test_multiline_rejected().
  TestIsFtsEligible.test_context_before_rejected: TestIsFtsEligible#test_context_before_rejected().
  TestIsFtsEligible.test_context_after_rejected: TestIsFtsEligible#test_context_after_rejected().
  TestIsFtsEligible.test_include_globs_rejected: TestIsFtsEligible#test_include_globs_rejected().
  TestIsFtsEligible.test_exclude_globs_rejected: TestIsFtsEligible#test_exclude_globs_rejected().
  TestIsFtsEligible.test_plain_extensions_allowed: TestIsFtsEligible#test_plain_extensions_allowed().
  TestIsFtsEligible.test_no_query_key: TestIsFtsEligible#test_no_query_key().
  TestTryFts5FastPath.test_returns_none_when_no_index: TestTryFts5FastPath#test_returns_none_when_no_index().
  TestTryFts5FastPath.test_returns_none_for_regex_query: TestTryFts5FastPath#test_returns_none_for_regex_query().
  TestTryFts5FastPath.test_returns_none_when_no_project_root: TestTryFts5FastPath#test_returns_none_when_no_project_root().
  TestIsFtsEligible: TestIsFtsEligible#
  TestTryFts5FastPath: TestTryFts5FastPath#
  TestSearchContentFtsIntegration: TestSearchContentFtsIntegration#
---
# Module: [`tests/unit/test_fts_fast_path.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py)

## Classes
### `TestIsFtsEligible`
- def: [`tests/unit/test_fts_fast_path.py:22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L22)
- signature: `class TestIsFtsEligible:`
- members:
  - `test_camel_case(self)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L29)
  - `test_context_after_rejected(self)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L53)
  - `test_context_before_rejected(self)` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L50)
  - `test_empty_query_rejected(self)` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L35)
  - `test_exclude_globs_rejected(self)` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L59)
  - `test_fixed_strings_rejected(self)` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L41)
  - `test_identifier_with_underscore(self)` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L26)
  - `test_include_globs_rejected(self)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L56)
  - `test_multiline_rejected(self)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L47)
  - `test_no_query_key(self)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L65)
  - `test_plain_extensions_allowed(self)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L62)
  - `test_query_with_spaces_rejected(self)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L38)
  - `test_regex_pattern_rejected(self)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L32)
  - `test_simple_identifier(self)` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L23)
  - `test_word_flag_rejected(self)` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L44)
- uses (calls/refs, reference-scoped): [`_is_fts_eligible`](../../tree_sitter_analyzer/mcp/tools/_fts_fast_path.md#_is_fts_eligible)

### `TestSearchContentFtsIntegration`
- def: [`tests/unit/test_fts_fast_path.py:231`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L231)
- signature: `class TestSearchContentFtsIntegration:`
- members:
  - `test_search_content_falls_through_for_regex(self, tmp_path)` — [`L260`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L260)
  - `test_search_content_uses_fts_for_simple_query(self, tmp_path)` — [`L242`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L242)
- protocol/private: `_setup_indexed_project`[`L232`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L232)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project), [`SearchContentTool`](../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.execute)  (1 test-only)

### `TestTryFts5FastPath`
- def: [`tests/unit/test_fts_fast_path.py:69`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L69)
- signature: `class TestTryFts5FastPath:`
- members:
  - `test_count_only_mode(self, tmp_path)` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L139)
  - `test_finds_symbol_from_index(self, tmp_path)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L94)
  - `test_language_filter_via_extensions(self, tmp_path)` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L196)
  - `test_multifile_search(self, tmp_path)` — [`L215`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L215)
  - `test_no_match_returns_none(self, tmp_path)` — [`L179`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L179)
  - `test_returns_none_for_regex_query(self, tmp_path)` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L78)
  - `test_returns_none_when_no_index(self, tmp_path)` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L70)
  - `test_returns_none_when_no_project_root(self, tmp_path)` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L86)
  - `test_summary_mode(self, tmp_path)` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L159)
  - `test_total_only_mode_returns_dict(self, tmp_path)` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L119)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project), [`try_fts5_fast_path`](../../tree_sitter_analyzer/mcp/tools/_fts_fast_path.md#try_fts5_fast_path), [`get_stats`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.get_stats)  (1 test-only)

## Functions
- `_write_py_file(directory: str, name: str, content: str)` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_fast_path.py#L15)

