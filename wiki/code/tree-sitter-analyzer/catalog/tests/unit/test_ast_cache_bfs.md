---
title: 'Module: tests/unit/test_ast_cache_bfs.py'
type: catalog
provenance: extracted
module: tests/unit/test_ast_cache_bfs.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_ast_cache_bfs`/
symbols:
  _insert_edge: _insert_edge().
  _make_conn: _make_conn().
  TestBfsCallers.test_single_caller_found_no_file: TestBfsCallers#test_single_caller_found_no_file().
  TestBfsCallers.test_single_caller_found_with_file: TestBfsCallers#test_single_caller_found_with_file().
  TestBfsCallers.test_file_filter_excludes_other_file: TestBfsCallers#test_file_filter_excludes_other_file().
  TestBfsCallers.test_depth_field_populated: TestBfsCallers#test_depth_field_populated().
  TestBfsCallers.test_deduplication_via_visited_set: TestBfsCallers#test_deduplication_via_visited_set().
  TestBfsCallers.test_max_depth_zero_returns_empty: TestBfsCallers#test_max_depth_zero_returns_empty().
  TestBfsCallers.test_callee_file_falls_back_to_file_path: TestBfsCallers#test_callee_file_falls_back_to_file_path().
  TestBfsCallers.test_callee_file_uses_resolved_when_present: TestBfsCallers#test_callee_file_uses_resolved_when_present().
  TestBfsCallers.test_fallback_file_path_query_when_resolved_file_not_found: TestBfsCallers#test_fallback_file_path_query_when_resolved_file_not_found().
  TestBfsCallers.test_multiple_callers_all_returned: TestBfsCallers#test_multiple_callers_all_returned().
  TestBfsCallers.test_transitive_callers_depth2: TestBfsCallers#test_transitive_callers_depth2().
  TestBfsCallees.test_single_callee_found_no_file: TestBfsCallees#test_single_callee_found_no_file().
  TestBfsCallees.test_single_callee_found_with_file: TestBfsCallees#test_single_callee_found_with_file().
  TestBfsCallees.test_file_filter_works: TestBfsCallees#test_file_filter_works().
  TestBfsCallees.test_depth_field_populated: TestBfsCallees#test_depth_field_populated().
  TestBfsCallees.test_deduplication_via_visited_set: TestBfsCallees#test_deduplication_via_visited_set().
  TestBfsCallees.test_max_depth_zero_returns_empty: TestBfsCallees#test_max_depth_zero_returns_empty().
  TestBfsCallees.test_callee_resolved_file_in_result: TestBfsCallees#test_callee_resolved_file_in_result().
  TestBfsCallees.test_callee_file_falls_back_to_file_path: TestBfsCallees#test_callee_file_falls_back_to_file_path().
  TestBfsCallees.test_multiple_callees_all_returned: TestBfsCallees#test_multiple_callees_all_returned().
  TestBfsCallees.test_transitive_callees_depth2: TestBfsCallees#test_transitive_callees_depth2().
  TestBfsCallers.test_no_callers_returns_empty: TestBfsCallers#test_no_callers_returns_empty().
  TestBfsCallees.test_no_callees_returns_empty: TestBfsCallees#test_no_callees_returns_empty().
  TestBfsCallers: TestBfsCallers#
  TestBfsCallees: TestBfsCallees#
---
# Module: [`tests/unit/test_ast_cache_bfs.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py)

## Classes
### `TestBfsCallees`
- def: [`tests/unit/test_ast_cache_bfs.py:230`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L230)
- signature: `class TestBfsCallees:`
- members:
  - `test_callee_file_falls_back_to_file_path(self)` — [`L294`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L294)
  - `test_callee_resolved_file_in_result(self)` — [`L286`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L286)
  - `test_deduplication_via_visited_set(self)` — [`L264`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L264) — Same callee-file-line should appear only once.
  - `test_depth_field_populated(self)` — [`L258`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L258)
  - `test_file_filter_works(self)` — [`L250`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L250)
  - `test_max_depth_zero_returns_empty(self)` — [`L280`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L280)
  - `test_multiple_callees_all_returned(self)` — [`L302`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L302)
  - `test_no_callees_returns_empty(self)` — [`L231`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L231)
  - `test_single_callee_found_no_file(self)` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L236)
  - `test_single_callee_found_with_file(self)` — [`L243`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L243)
  - `test_transitive_callees_depth2(self)` — [`L310`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L310) — With max_depth=2, BFS should also return callees of callees.
- uses (calls/refs, reference-scoped): [`bfs_callees`](../../tree_sitter_analyzer/_ast_cache_graph.md#bfs_callees)  (2 test-only)

### `TestBfsCallers`
- def: [`tests/unit/test_ast_cache_bfs.py:95`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L95)
- signature: `class TestBfsCallers:`
- members:
  - `test_callee_file_falls_back_to_file_path(self)` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L168) — When callee_resolved_file is empty, callee_file in result = file_path.
  - `test_callee_file_uses_resolved_when_present(self)` — [`L179`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L179)
  - `test_deduplication_via_visited_set(self)` — [`L136`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L136) — Same caller-file-line edge should not appear twice.
  - `test_depth_field_populated(self)` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L130)
  - `test_fallback_file_path_query_when_resolved_file_not_found(self)` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L187) — When querying with callee_file, try callee_resolved_file first,
  - `test_file_filter_excludes_other_file(self)` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L118)
  - `test_max_depth_zero_returns_empty(self)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L162)
  - `test_multiple_callers_all_returned(self)` — [`L201`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L201)
  - `test_no_callers_returns_empty(self)` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L96)
  - `test_single_caller_found_no_file(self)` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L101)
  - `test_single_caller_found_with_file(self)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L109)
  - `test_transitive_callers_depth2(self)` — [`L211`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L211) — With max_depth=2, BFS should also return callers-of-callers.
- uses (calls/refs, reference-scoped): [`bfs_callers`](../../tree_sitter_analyzer/_ast_cache_graph.md#bfs_callers)  (2 test-only)

## Functions
- `_insert_edge(conn: sqlite3.Connection, caller_name: str, caller_file: str, callee_name: str, file_path: str, callee_line: int = 10, caller_line: int = 5, callee_resolved_file: str = "", callee_full: str = "")` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L38)
- `_make_conn()` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_bfs.py#L29)

