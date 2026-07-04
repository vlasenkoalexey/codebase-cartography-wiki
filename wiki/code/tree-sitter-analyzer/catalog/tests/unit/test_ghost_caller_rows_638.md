---
title: 'Module: tests/unit/test_ghost_caller_rows_638.py'
type: catalog
provenance: extracted
module: tests/unit/test_ghost_caller_rows_638.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_ghost_caller_rows_638`/
symbols:
  _parse: _parse().
  _fmt_edges: _fmt_edges().
  TestCallGraphParseTierAttribution.test_fmt_callers_are_both_execute_methods: TestCallGraphParseTierAttribution#test_fmt_callers_are_both_execute_methods().
  indexed_project: indexed_project().
  TestCallersToolGhostRows.test_real_call_sites_resolve_to_enclosing_methods: TestCallersToolGhostRows#test_real_call_sites_resolve_to_enclosing_methods().
  TestDuplicateNameSpanAttribution.test_call_in_first_same_named_method_attributed: TestDuplicateNameSpanAttribution#test_call_in_first_same_named_method_attributed().
  TestDuplicateNameSpanAttribution.test_call_in_second_same_named_method_attributed: TestDuplicateNameSpanAttribution#test_call_in_second_same_named_method_attributed().
  TestDuplicateNameSpanAttribution.test_module_level_call_unattributed_by_design: TestDuplicateNameSpanAttribution#test_module_level_call_unattributed_by_design().
  TestCallersToolGhostRows.test_no_result_row_has_empty_name_or_line_zero: TestCallersToolGhostRows#test_no_result_row_has_empty_name_or_line_zero().
  TestCallersToolGhostRows.test_module_level_call_counted_not_emitted: TestCallersToolGhostRows#test_module_level_call_counted_not_emitted().
  TestCallersToolGhostRows.test_no_unattributed_key_when_all_attributed: TestCallersToolGhostRows#test_no_unattributed_key_when_all_attributed().
  _HYPHAE_SHAPE: _HYPHAE_SHAPE.
  _FIRST_EXECUTE_DEF_LINE: _FIRST_EXECUTE_DEF_LINE.
  _SECOND_EXECUTE_DEF_LINE: _SECOND_EXECUTE_DEF_LINE.
  TestDuplicateNameSpanAttribution.test_exact_fmt_edge_count: TestDuplicateNameSpanAttribution#test_exact_fmt_edge_count().
  TestCallGraphParseTierAttribution.project: TestCallGraphParseTierAttribution#project().
  _FIRST_EXECUTE_CALL_LINE: _FIRST_EXECUTE_CALL_LINE.
  _SECOND_EXECUTE_CALL_LINE: _SECOND_EXECUTE_CALL_LINE.
  _MODULE_LEVEL_CALL_LINE: _MODULE_LEVEL_CALL_LINE.
  TestDuplicateNameSpanAttribution: TestDuplicateNameSpanAttribution#
  TestCallGraphParseTierAttribution: TestCallGraphParseTierAttribution#
  TestCallersToolGhostRows: TestCallersToolGhostRows#
---
# Module: [`tests/unit/test_ghost_caller_rows_638.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py)

## Classes
### `TestCallGraphParseTierAttribution`
- def: [`tests/unit/test_ghost_caller_rows_638.py:139`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L139)
- signature: `class TestCallGraphParseTierAttribution:`
- members:
  - `project(self, tmp_path: Path)` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L141)
  - `test_fmt_callers_are_both_execute_methods(self, project: str)` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L145) — Callers of fmt at the parse tier resolve to BOTH execute methods.
- uses (calls/refs, reference-scoped): [`CallGraph`](../../tree_sitter_analyzer/call_graph.md#CallGraph), [`callers_of`](../../tree_sitter_analyzer/call_graph.md#CallGraph.callers_of)  (3 test-only)

### `TestCallersToolGhostRows`
- def: [`tests/unit/test_ghost_caller_rows_638.py:179`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L179)
- signature: `class TestCallersToolGhostRows:`
- members:
  - `test_module_level_call_counted_not_emitted(self, indexed_project: str)` — [`L223`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L223) — The module-level fmt() call is excluded with a counted note.
  - `test_no_result_row_has_empty_name_or_line_zero(self, indexed_project: str)` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L181) — Structural pin (#638): a caller row is navigable or it is not a row.
  - `test_no_unattributed_key_when_all_attributed(self, indexed_project: str)` — [`L232`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L232) — helper_a is only called inside a method — no counted note emitted.
  - `test_real_call_sites_resolve_to_enclosing_methods(self, indexed_project: str)` — [`L197`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L197) — Both in-method call sites attribute to their own execute definition.
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool.execute), [`CodeGraphCallersTool`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool)  (2 test-only)

### `TestDuplicateNameSpanAttribution`
- def: [`tests/unit/test_ghost_caller_rows_638.py:94`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L94)
- signature: `class TestDuplicateNameSpanAttribution:`
- members:
  - `test_call_in_first_same_named_method_attributed(self)` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L98) — fmt() at line 15 lives inside SubscribeTool.execute (def line 13).
  - `test_call_in_second_same_named_method_attributed(self)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L113)
  - `test_exact_fmt_edge_count(self)` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L95)
  - `test_module_level_call_unattributed_by_design(self)` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L120) — Module-level fmt() at line 26 has no enclosing function.
- uses (calls/refs, reference-scoped): (6 test-only callers)

## Functions
- `_fmt_edges()` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L83)
- `_parse(source: str, language: str = "python")` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L75)
- `indexed_project(tmp_path: Path)` — [`L169`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L169)

## Module values
- `_FIRST_EXECUTE_CALL_LINE` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L69)
- `_FIRST_EXECUTE_DEF_LINE` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L68)
- `_HYPHAE_SHAPE` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L38)
- `_MODULE_LEVEL_CALL_LINE` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L72)
- `_SECOND_EXECUTE_CALL_LINE` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L71)
- `_SECOND_EXECUTE_DEF_LINE` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ghost_caller_rows_638.py#L70)

