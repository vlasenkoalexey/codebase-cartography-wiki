---
title: 'Module: tests/unit/mcp/test_total_count_under_truncation.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_total_count_under_truncation.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_total_count_under_truncation`/
symbols:
  TestSearchContentTotalCountUnderTruncation.test_total_count_above_displayed_when_truncated: TestSearchContentTotalCountUnderTruncation#test_total_count_above_displayed_when_truncated().
  TestSearchContentTotalCountUnderTruncation.test_non_truncated_response_marks_known: TestSearchContentTotalCountUnderTruncation#test_non_truncated_response_marks_known().
  TestListFilesTotalCountUnderLimit.test_total_count_above_displayed_when_limited: TestListFilesTotalCountUnderLimit#test_total_count_above_displayed_when_limited().
  TestListFilesTotalCountUnderLimit.test_non_truncated_response_marks_known: TestListFilesTotalCountUnderLimit#test_non_truncated_response_marks_known().
  big_repo: big_repo().
  TestSearchContentTotalCountUnderTruncation: TestSearchContentTotalCountUnderTruncation#
  TestListFilesTotalCountUnderLimit: TestListFilesTotalCountUnderLimit#
  _assert_honest_total_count: _assert_honest_total_count().
  _assert_non_truncated_known: _assert_non_truncated_known().
  _FD_AVAILABLE: _FD_AVAILABLE.
  _RG_AVAILABLE: _RG_AVAILABLE.
  _make_repo_with_many_def_lines: _make_repo_with_many_def_lines().
---
# Module: [`tests/unit/mcp/test_total_count_under_truncation.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_total_count_under_truncation.py)

## Classes
### `TestListFilesTotalCountUnderLimit`
- def: [`tests/unit/mcp/test_total_count_under_truncation.py:117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_total_count_under_truncation.py#L117)
- signature: `class TestListFilesTotalCountUnderLimit:`
- members:
  - `test_non_truncated_response_marks_known(self, big_repo: Path)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_total_count_under_truncation.py#L137) — Without truncation, total_count == displayed_count and known.
  - `test_total_count_above_displayed_when_limited(self, big_repo: Path)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_total_count_under_truncation.py#L118) — With limit << real_total, total_count must reflect the real count.
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/list_files_tool.md#ListFilesTool.execute), [`ListFilesTool`](../../../tree_sitter_analyzer/mcp/tools/list_files_tool.md#ListFilesTool)  (3 test-only)

### `TestSearchContentTotalCountUnderTruncation`
- def: [`tests/unit/mcp/test_total_count_under_truncation.py:75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_total_count_under_truncation.py#L75)
- signature: `class TestSearchContentTotalCountUnderTruncation:`
- members:
  - `test_non_truncated_response_marks_known(self, big_repo: Path)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_total_count_under_truncation.py#L95) — When ripgrep didn't truncate, total_count_known must be True.
  - `test_total_count_above_displayed_when_truncated(self, big_repo: Path)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_total_count_under_truncation.py#L76) — The recount pass should resolve a real total > displayed_count.
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.execute)  (3 test-only)

## Functions
- `_assert_honest_total_count(result: dict, displayed: int, total: int)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_total_count_under_truncation.py#L30) — H2/H3 contract: truncated response must carry honest count or explicit uncertainty.
- `_assert_non_truncated_known(result: dict)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_total_count_under_truncation.py#L41) — A non-truncated response must mark total_count as known and exact.
- `_make_repo_with_many_def_lines(root: Path, n_files: int = 50)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_total_count_under_truncation.py#L48) — Populate ``root`` with files that collectively contain >>1 'def' line.
- `big_repo()` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_total_count_under_truncation.py#L61) — Temporary tree with many .py files and many 'def' matches.

## Module values
- `_FD_AVAILABLE` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_total_count_under_truncation.py#L26)
- `_RG_AVAILABLE` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_total_count_under_truncation.py#L27)

