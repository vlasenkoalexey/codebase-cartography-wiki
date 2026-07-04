---
title: 'Module: tests/unit/mcp/tools/test_symbol_body_inline.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_symbol_body_inline.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_symbol_body_inline`/
symbols:
  _build_cache: _build_cache().
  test_inline_symbol_body_truncates_over_cap: test_inline_symbol_body_truncates_over_cap().
  test_inline_neighbor_bodies_caps_at_top_n: test_inline_neighbor_bodies_caps_at_top_n().
  test_inline_neighbor_body_uses_40_line_tier: test_inline_neighbor_body_uses_40_line_tier().
  test_inline_search_summaries_uses_30_line_tier: test_inline_search_summaries_uses_30_line_tier().
  test_inline_symbol_body_verbatim_with_end_line: test_inline_symbol_body_verbatim_with_end_line().
  test_inline_symbol_body_resolves_missing_end_line: test_inline_symbol_body_resolves_missing_end_line().
  test_inline_neighbor_bodies_attaches_body_to_each: test_inline_neighbor_bodies_attaches_body_to_each().
  test_inline_neighbor_body_does_not_cross_languages: test_inline_neighbor_body_does_not_cross_languages().
  test_inline_neighbor_body_skipped_for_unknown_callee: test_inline_neighbor_body_skipped_for_unknown_callee().
  test_inline_search_summaries_attaches_body: test_inline_search_summaries_attaches_body().
  _SRC_BIG: _SRC_BIG.
  _SRC_SMALL: _SRC_SMALL.
---
# Module: [`tests/unit/mcp/tools/test_symbol_body_inline.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_symbol_body_inline.py)

## Functions
- `_build_cache(tmp_path: Path)` — [`L26`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_symbol_body_inline.py#L26)
- `test_inline_neighbor_bodies_attaches_body_to_each(tmp_path)` — [`L94`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_symbol_body_inline.py#L94)
- `test_inline_neighbor_bodies_caps_at_top_n(tmp_path)` — [`L177`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_symbol_body_inline.py#L177)
- `test_inline_neighbor_body_does_not_cross_languages(tmp_path)` — [`L107`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_symbol_body_inline.py#L107) — A Python callee with no Python def must not inline a foreign-language body.
- `test_inline_neighbor_body_skipped_for_unknown_callee(tmp_path)` — [`L143`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_symbol_body_inline.py#L143) — An unresolved callee gets no inlined body (it would be a bare-name guess).
- `test_inline_neighbor_body_uses_40_line_tier(tmp_path)` — [`L186`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_symbol_body_inline.py#L186)
- `test_inline_search_summaries_attaches_body(tmp_path)` — [`L200`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_symbol_body_inline.py#L200)
- `test_inline_search_summaries_uses_30_line_tier(tmp_path)` — [`L210`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_symbol_body_inline.py#L210)
- `test_inline_symbol_body_resolves_missing_end_line(tmp_path)` — [`L80`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_symbol_body_inline.py#L80)
- `test_inline_symbol_body_truncates_over_cap(tmp_path)` — [`L68`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_symbol_body_inline.py#L68)
- `test_inline_symbol_body_verbatim_with_end_line(tmp_path)` — [`L58`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_symbol_body_inline.py#L58)

## Module values
- `_SRC_BIG` — [`L22`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_symbol_body_inline.py#L22)
- `_SRC_SMALL` — [`L23`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_symbol_body_inline.py#L23)

