---
title: 'Module: tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_guard_caller_count_excludes_non_calls`/
symbols:
  TestFStringCallSitesNotFiltered._only_in_strings: TestFStringCallSitesNotFiltered#_only_in_strings().
  TestTraceImpactExcludesImportAndStringMatches.test_call_count_excludes_import_and_string_literal: TestTraceImpactExcludesImportAndStringMatches#test_call_count_excludes_import_and_string_literal().
  TestTraceImpactExcludesImportAndStringMatches.test_reconciliation_invariant_guard_matches_nav_callers: TestTraceImpactExcludesImportAndStringMatches#test_reconciliation_invariant_guard_matches_nav_callers().
  _rg_match_line: _rg_match_line().
  TestNonCodeLineAndStringEdges._only_in_strings: TestNonCodeLineAndStringEdges#_only_in_strings().
  TestFilterCommentDocstringMatchesWithNonCallExclusion.test_import_line_excluded: TestFilterCommentDocstringMatchesWithNonCallExclusion#test_import_line_excluded().
  TestFilterCommentDocstringMatchesWithNonCallExclusion.test_string_literal_line_excluded: TestFilterCommentDocstringMatchesWithNonCallExclusion#test_string_literal_line_excluded().
  TestFilterCommentDocstringMatchesWithNonCallExclusion.test_real_calls_all_kept: TestFilterCommentDocstringMatchesWithNonCallExclusion#test_real_calls_all_kept().
  TestCLikeAndEscapePaths.test_c_block_comment_unclosed_spans_lines: TestCLikeAndEscapePaths#test_c_block_comment_unclosed_spans_lines().
  TestNonCodeLineAndStringEdges._noncode: TestNonCodeLineAndStringEdges#_noncode().
  TestCLikeAndEscapePaths._only_in_strings: TestCLikeAndEscapePaths#_only_in_strings().
  TestFilterCommentDocstringMatchesWithNonCallExclusion._make_py_file: TestFilterCommentDocstringMatchesWithNonCallExclusion#_make_py_file().
  TestPythonNonCodeLinesImportDetection.test_from_import_line_flagged: TestPythonNonCodeLinesImportDetection#test_from_import_line_flagged().
  TestPythonNonCodeLinesImportDetection.test_bare_import_line_flagged: TestPythonNonCodeLinesImportDetection#test_bare_import_line_flagged().
  TestIsSymbolOnlyInStrings.test_symbol_inside_double_quoted_string: TestIsSymbolOnlyInStrings#test_symbol_inside_double_quoted_string().
  TestIsSymbolOnlyInStrings.test_symbol_outside_string_is_call: TestIsSymbolOnlyInStrings#test_symbol_outside_string_is_call().
  TestIsSymbolOnlyInStrings.test_symbol_inside_single_quoted_string: TestIsSymbolOnlyInStrings#test_symbol_inside_single_quoted_string().
  TestIsSymbolOnlyInStrings.test_symbol_only_outside_mixed_line: TestIsSymbolOnlyInStrings#test_symbol_only_outside_mixed_line().
  TestFStringCallSitesNotFiltered.test_fstring_replacement_field_call_is_code: TestFStringCallSitesNotFiltered#test_fstring_replacement_field_call_is_code().
  TestFStringCallSitesNotFiltered.test_fstring_literal_text_mention_is_string: TestFStringCallSitesNotFiltered#test_fstring_literal_text_mention_is_string().
  TestFStringCallSitesNotFiltered.test_fstring_mixed_literal_and_field: TestFStringCallSitesNotFiltered#test_fstring_mixed_literal_and_field().
  TestFStringCallSitesNotFiltered.test_escaped_brace_keeps_literal_string: TestFStringCallSitesNotFiltered#test_escaped_brace_keeps_literal_string().
  TestFStringCallSitesNotFiltered.test_nested_brace_in_replacement_field_call_is_code: TestFStringCallSitesNotFiltered#test_nested_brace_in_replacement_field_call_is_code().
  TestFStringCallSitesNotFiltered.test_plain_string_still_filtered: TestFStringCallSitesNotFiltered#test_plain_string_still_filtered().
  TestNonCodeLineAndStringEdges.test_comment_line_is_non_code: TestNonCodeLineAndStringEdges#test_comment_line_is_non_code().
  TestNonCodeLineAndStringEdges.test_import_line_is_non_code: TestNonCodeLineAndStringEdges#test_import_line_is_non_code().
  TestNonCodeLineAndStringEdges.test_symbol_absent_returns_false: TestNonCodeLineAndStringEdges#test_symbol_absent_returns_false().
  TestNonCodeLineAndStringEdges.test_triple_quote_same_line_symbol_filtered: TestNonCodeLineAndStringEdges#test_triple_quote_same_line_symbol_filtered().
  TestNonCodeLineAndStringEdges.test_escaped_char_inside_string: TestNonCodeLineAndStringEdges#test_escaped_char_inside_string().
  TestCLikeAndEscapePaths.test_escaped_char_before_symbol_in_string: TestCLikeAndEscapePaths#test_escaped_char_before_symbol_in_string().
  TestCLikeAndEscapePaths.test_symbol_before_triple_quote_is_code: TestCLikeAndEscapePaths#test_symbol_before_triple_quote_is_code().
  TestCLikeAndEscapePaths._make_file: TestCLikeAndEscapePaths#_make_file().
  TestPythonNonCodeLinesImportDetection: TestPythonNonCodeLinesImportDetection#
  TestIsSymbolOnlyInStrings: TestIsSymbolOnlyInStrings#
  TestFilterCommentDocstringMatchesWithNonCallExclusion: TestFilterCommentDocstringMatchesWithNonCallExclusion#
  TestTraceImpactExcludesImportAndStringMatches: TestTraceImpactExcludesImportAndStringMatches#
  TestFStringCallSitesNotFiltered: TestFStringCallSitesNotFiltered#
  TestNonCodeLineAndStringEdges: TestNonCodeLineAndStringEdges#
  TestCLikeAndEscapePaths: TestCLikeAndEscapePaths#
---
# Module: [`tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py)

## Classes
### `TestCLikeAndEscapePaths`
- def: [`tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py:380`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L380)
- doc: Cover the c-like block-comment path + escaped-char string path (codecov).
- signature: `class TestCLikeAndEscapePaths:`
- members:
  - `test_c_block_comment_unclosed_spans_lines(self, tmp_path)` — [`L396`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L396)
  - `test_escaped_char_before_symbol_in_string(self)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L412)
  - `test_symbol_before_triple_quote_is_code(self)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L416)
- protocol/private: `_make_file`[`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L383), `_only_in_strings`[`L389`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L389)
- uses (calls/refs, reference-scoped): [`_filter_comment_docstring_matches`](../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#_filter_comment_docstring_matches), [`_is_symbol_only_in_strings`](../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#_is_symbol_only_in_strings)

### `TestFStringCallSitesNotFiltered`
- def: [`tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py:308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L308)
- doc: Codex P2 on #661: a call inside an f-string replacement field is real
- signature: `class TestFStringCallSitesNotFiltered:`
- members:
  - `test_escaped_brace_keeps_literal_string(self)` — [`L330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L330)
  - `test_fstring_literal_text_mention_is_string(self)` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L324)
  - `test_fstring_mixed_literal_and_field(self)` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L327)
  - `test_fstring_replacement_field_call_is_code(self)` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L321)
  - `test_nested_brace_in_replacement_field_call_is_code(self)` — [`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L333)
  - `test_plain_string_still_filtered(self)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L338)
- protocol/private: `_only_in_strings`[`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L314)
- uses (calls/refs, reference-scoped): [`_is_symbol_only_in_strings`](../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#_is_symbol_only_in_strings)

### `TestFilterCommentDocstringMatchesWithNonCallExclusion`
- def: [`tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py:105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L105)
- doc: _filter_comment_docstring_matches must drop import-line and
- signature: `class TestFilterCommentDocstringMatchesWithNonCallExclusion:`
- members:
  - `_make_py_file(self, tmp_path, name: str, content: str)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L110) — Write a .py fixture and return the absolute path string.
  - `test_import_line_excluded(self, tmp_path)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L116)
  - `test_real_calls_all_kept(self, tmp_path)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L150)
  - `test_string_literal_line_excluded(self, tmp_path)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L133)
- uses (calls/refs, reference-scoped): [`_filter_comment_docstring_matches`](../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#_filter_comment_docstring_matches)

### `TestIsSymbolOnlyInStrings`
- def: [`tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py:76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L76)
- doc: _is_symbol_only_in_strings must return True when every occurrence of
- signature: `class TestIsSymbolOnlyInStrings:`
- members:
  - `test_symbol_inside_double_quoted_string(self)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L82)
  - `test_symbol_inside_single_quoted_string(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L90)
  - `test_symbol_only_outside_mixed_line(self)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L94)
  - `test_symbol_outside_string_is_call(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L86)
- uses (calls/refs, reference-scoped): [`_is_symbol_only_in_strings`](../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#_is_symbol_only_in_strings)

### `TestNonCodeLineAndStringEdges`
- def: [`tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py:342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L342)
- doc: Cover the #655/#661 diff lines: import detection, triple-quote, escape,
- signature: `class TestNonCodeLineAndStringEdges:`
- members:
  - `test_comment_line_is_non_code(self)` — [`L362`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L362)
  - `test_escaped_char_inside_string(self)` — [`L375`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L375)
  - `test_import_line_is_non_code(self)` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L365)
  - `test_symbol_absent_returns_false(self)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L369)
  - `test_triple_quote_same_line_symbol_filtered(self)` — [`L372`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L372)
- protocol/private: `_noncode`[`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L347), `_only_in_strings`[`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L355)
- uses (calls/refs, reference-scoped): [`_is_symbol_only_in_strings`](../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#_is_symbol_only_in_strings), [`_python_non_code_lines`](../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#_python_non_code_lines)

### `TestPythonNonCodeLinesImportDetection`
- def: [`tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py:34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L34)
- doc: _python_non_code_lines must flag import lines as non-code.
- signature: `class TestPythonNonCodeLinesImportDetection:`
- members:
  - `test_bare_import_line_flagged(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L56) — 'import module' lines must be flagged.
  - `test_from_import_line_flagged(self)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L37) — 'from module import symbol' is not a call site — must be flagged.
- uses (calls/refs, reference-scoped): [`_python_non_code_lines`](../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#_python_non_code_lines)

### `TestTraceImpactExcludesImportAndStringMatches`
- def: [`tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py:192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L192)
- doc: End-to-end fixture: 4 ripgrep hits, only 2 are real calls.
- signature: `class TestTraceImpactExcludesImportAndStringMatches:`
- members:
  - `test_call_count_excludes_import_and_string_literal(self, tmp_path)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L196)
  - `test_reconciliation_invariant_guard_matches_nav_callers(self, tmp_path)` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L257) — Reconciliation invariant: guard call_count must equal the number
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#TraceImpactTool.execute), [`TraceImpactTool`](../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#TraceImpactTool)  (1 test-only)

## Functions
- `_rg_match_line(file_path: str, line_no: int, text: str)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_guard_caller_count_excludes_non_calls.py#L177)

