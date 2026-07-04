---
title: 'Module: tests/unit/hyphae/test_select_tool.py'
type: catalog
provenance: extracted
module: tests/unit/hyphae/test_select_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.hyphae.test_select_tool`/
symbols:
  _tool: _tool().
  test_exactly_max_results_not_truncated: test_exactly_max_results_not_truncated().
  test_not_pseudo_does_not_clobber_counters: test_not_pseudo_does_not_clobber_counters().
  test_multi_selector_recount_covers_remaining_selectors: test_multi_selector_recount_covers_remaining_selectors().
  test_duplicate_symbols_across_selectors_deduped: test_duplicate_symbols_across_selectors_deduped().
  test_execute_capped_at_100_with_150_total: test_execute_capped_at_100_with_150_total().
  test_next_step_includes_narrowing_hint_when_truncated: test_next_step_includes_narrowing_hint_when_truncated().
  test_truncated_results_show_narrowing_hint_on_ready_index: test_truncated_results_show_narrowing_hint_on_ready_index().
  test_any_selector_on_empty_index_warns: test_any_selector_on_empty_index_warns().
  test_selector_on_missing_cache_warns: test_selector_on_missing_cache_warns().
  test_empty_index_reports_missing_state: test_empty_index_reports_missing_state().
  _FakeCacheWithManyCallers: _FakeCacheWithManyCallers#
  test_tool_definition_names_hyphae: test_tool_definition_names_hyphae().
  test_selector_required: test_selector_required().
  test_execute_calls_selector_json: test_execute_calls_selector_json().
  test_execute_syntax_error_is_graceful: test_execute_syntax_error_is_graceful().
  test_execute_under_cap_not_truncated: test_execute_under_cap_not_truncated().
  test_zero_matches_on_ready_index_is_not_a_warning: test_zero_matches_on_ready_index_is_not_a_warning().
  test_valid_matches_on_ready_index_succeeds: test_valid_matches_on_ready_index_succeeds().
  test_ready_zero_matches_reports_indexed_file_count: test_ready_zero_matches_reports_indexed_file_count().
  test_selector_echo_capped_at_200_chars: test_selector_echo_capped_at_200_chars().
  test_short_selector_not_truncated: test_short_selector_not_truncated().
  test_summary_line_uses_capped_echo: test_summary_line_uses_capped_echo().
  test_syntax_error_branch_caps_echo_too: test_syntax_error_branch_caps_echo_too().
  _FakeCacheWithManyCallers._n: _FakeCacheWithManyCallers#_n.
  _FakeCache.search_symbols_cascade: _FakeCache#search_symbols_cascade().
  _FakeCacheWithManyCallers.get_functions: _FakeCacheWithManyCallers#get_functions().
  _FakeCacheWithManyCallers.get_stats: _FakeCacheWithManyCallers#get_stats().
  _FakeCache: _FakeCache#
  _FakeCache.get_functions: _FakeCache#get_functions().
  _EmptyCache: _EmptyCache#
  _BrokenCache: _BrokenCache#
  _FakeCache.get_symbols_by_kind: _FakeCache#get_symbols_by_kind().
  _FakeCache.query_edges: _FakeCache#query_edges().
  _FakeCache.get_stats: _FakeCache#get_stats().
  _FakeCacheWithManyCallers.__init__: _FakeCacheWithManyCallers#__init__().
  _FakeCacheWithManyCallers.search_symbols_cascade: _FakeCacheWithManyCallers#search_symbols_cascade().
  _FakeCacheWithManyCallers.get_symbols_by_kind: _FakeCacheWithManyCallers#get_symbols_by_kind().
  _FakeCacheWithManyCallers.query_edges: _FakeCacheWithManyCallers#query_edges().
  _EmptyCache.get_functions: _EmptyCache#get_functions().
  _EmptyCache.search_symbols_cascade: _EmptyCache#search_symbols_cascade().
  _EmptyCache.get_symbols_by_kind: _EmptyCache#get_symbols_by_kind().
  _EmptyCache.query_edges: _EmptyCache#query_edges().
  _EmptyCache.get_stats: _EmptyCache#get_stats().
  _BrokenCache.get_functions: _BrokenCache#get_functions().
  _BrokenCache.search_symbols_cascade: _BrokenCache#search_symbols_cascade().
  _BrokenCache.get_symbols_by_kind: _BrokenCache#get_symbols_by_kind().
  _BrokenCache.query_edges: _BrokenCache#query_edges().
  _BrokenCache.get_stats: _BrokenCache#get_stats().
---
# Module: [`tests/unit/hyphae/test_select_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py)

## Classes
### `_BrokenCache`
- def: [`tests/unit/hyphae/test_select_tool.py:336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L336)
- doc: A cache that raises an exception on get_stats.
- signature: `class _BrokenCache:`
- members:
  - `get_functions(self)` — [`L339`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L339)
  - `get_stats(self)` — [`L351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L351)
  - `get_symbols_by_kind(self, kind, limit=50000)` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L345)
  - `query_edges(self, kind, caller_name=None, callee_name=None, limit=10000)` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L348)
  - `search_symbols_cascade(self, query, limit=100)` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L342)
- used by: (1 test-only callers)

### `_EmptyCache`
- def: [`tests/unit/hyphae/test_select_tool.py:302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L302)
- doc: A cache that reports zero indexed files (empty).
- signature: `class _EmptyCache:`
- members:
  - `get_functions(self)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L305)
  - `get_stats(self)` — [`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L317)
  - `get_symbols_by_kind(self, kind, limit=50000)` — [`L311`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L311)
  - `query_edges(self, kind, caller_name=None, callee_name=None, limit=10000)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L314)
  - `search_symbols_cascade(self, query, limit=100)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L308)
- used by: (1 test-only callers)

### `_FakeCache`
- def: [`tests/unit/hyphae/test_select_tool.py:10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L10)
- signature: `class _FakeCache:`
- members:
  - `get_functions(self)` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L11)
  - `get_stats(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L46)
  - `get_symbols_by_kind(self, kind, limit=50000)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L32)
  - `query_edges(self, kind, caller_name=None, callee_name=None, limit=10000)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L35)
  - `search_symbols_cascade(self, query, limit=100)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L29)
- used by: (1 test-only callers)

### `_FakeCacheWithManyCallers`
- def: [`tests/unit/hyphae/test_select_tool.py:51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L51)
- doc: Cache that returns `n` callers (default 150 &gt; cap of 100).
- signature: `class _FakeCacheWithManyCallers:`
- members:
  - `get_functions(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L57)
  - `get_stats(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L88)
  - `get_symbols_by_kind(self, kind, limit=50000)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L72)
  - `query_edges(self, kind, caller_name=None, callee_name=None, limit=10000)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L75)
  - `search_symbols_cascade(self, query, limit=100)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L69)
- protocol/private: `__init__`[`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L54), `_n`[`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L55)
- used by: (7 test-only callers)

## Functions
- `_tool()` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L93)
- `test_any_selector_on_empty_index_warns()` — [`L323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L323) — Any selector on empty index → warns about missing index.
- `test_duplicate_symbols_across_selectors_deduped()` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L213) — The same symbol matched by two selectors counts once.
- `test_empty_index_reports_missing_state()` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L230) — Empty index (no files) → count:0 + index_state:missing + next_step warns.
- `test_exactly_max_results_not_truncated()` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L172) — Exactly 100 unique matches is a COMPLETE result, not a capped one.
- `test_execute_calls_selector_json()` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L112)
- `test_execute_capped_at_100_with_150_total()` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L130) — When 150 matches exceed the default cap of 100, truncated=True and total_matches=150.
- `test_execute_syntax_error_is_graceful()` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L122)
- `test_execute_under_cap_not_truncated()` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L145) — When results are under the cap, truncated=False.
- `test_multi_selector_recount_covers_remaining_selectors()` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L198) — Cap hit in selector 1 of a list — selector 2's matches still counted.
- `test_next_step_includes_narrowing_hint_when_truncated()` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L157) — When truncated, next_step should mention narrowing options.
- `test_not_pseudo_does_not_clobber_counters()` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L185) — :not(...) re-enters eval(); outer counters must survive (reentrancy).
- `test_ready_zero_matches_reports_indexed_file_count()` — [`L370`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L370) — opencode P2 (#497): partial cache classifies ready — the indexed-file
- `test_selector_echo_capped_at_200_chars()` — [`L386`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L386) — A 16 KB selector must be echoed back truncated to ≤ ~250 chars.
- `test_selector_on_missing_cache_warns()` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L356) — Selector on missing/broken cache → warns about missing index.
- `test_selector_required()` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L106)
- `test_short_selector_not_truncated()` — [`L407`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L407) — A short selector (≤ 200 chars) must be echoed verbatim.
- `test_summary_line_uses_capped_echo()` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L418) — A long but VALID selector must not flood agent_summary.summary_line
- `test_syntax_error_branch_caps_echo_too()` — [`L430`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L430) — The 16KB GARBAGE selector from the dogfood report hits the
- `test_tool_definition_names_hyphae()` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L99)
- `test_truncated_results_show_narrowing_hint_on_ready_index()` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L287) — Truncated results on ready index → next_step mentions narrowing.
- `test_valid_matches_on_ready_index_succeeds()` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L272) — Valid matches on ready index → count>0 + index_state:ready + info verdict.
- `test_zero_matches_on_ready_index_is_not_a_warning()` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_select_tool.py#L255) — Zero matches on a ready index → count:0 + index_state:ready + normal next_step.

