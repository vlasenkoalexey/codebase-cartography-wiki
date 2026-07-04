---
title: 'Module: tests/unit/test_callers_dedup_and_parse_tier_647_648.py'
type: catalog
provenance: extracted
module: tests/unit/test_callers_dedup_and_parse_tier_647_648.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_callers_dedup_and_parse_tier_647_648`/
symbols:
  TestParseTierModuleLevelExclusion.test_execute_22_has_exactly_one_fmt_callee: TestParseTierModuleLevelExclusion#test_execute_22_has_exactly_one_fmt_callee().
  TestParseTierModuleLevelExclusion.test_no_call_edge_at_module_level_line: TestParseTierModuleLevelExclusion#test_no_call_edge_at_module_level_line().
  TestParseTierModuleLevelExclusion.test_call_edge_count_excludes_module_level_call: TestParseTierModuleLevelExclusion#test_call_edge_count_excludes_module_level_call().
  indexed_project_647: indexed_project_647().
  TestSQLTierDedupKeepsBothMethods.test_two_execute_methods_produce_two_rows: TestSQLTierDedupKeepsBothMethods#test_two_execute_methods_produce_two_rows().
  TestSQLTierDedupKeepsBothMethods.test_caller_count_reflects_both_methods: TestSQLTierDedupKeepsBothMethods#test_caller_count_reflects_both_methods().
  TestSQLTierDedupKeepsBothMethods.test_no_ghost_rows_after_dedup_fix: TestSQLTierDedupKeepsBothMethods#test_no_ghost_rows_after_dedup_fix().
  TestSQLTierDedupKeepsBothMethods.test_module_level_call_still_counted_not_emitted: TestSQLTierDedupKeepsBothMethods#test_module_level_call_still_counted_not_emitted().
  TestParseTierModuleLevelExclusion.project: TestParseTierModuleLevelExclusion#project().
  _TWO_EXECUTE_SOURCE: _TWO_EXECUTE_SOURCE.
  _SECOND_EXECUTE_DEF_LINE: _SECOND_EXECUTE_DEF_LINE.
  _MODULE_LEVEL_CALL_LINE: _MODULE_LEVEL_CALL_LINE.
  _FIRST_EXECUTE_DEF_LINE: _FIRST_EXECUTE_DEF_LINE.
  TestParseTierModuleLevelExclusion: TestParseTierModuleLevelExclusion#
  TestSQLTierDedupKeepsBothMethods: TestSQLTierDedupKeepsBothMethods#
---
# Module: [`tests/unit/test_callers_dedup_and_parse_tier_647_648.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_dedup_and_parse_tier_647_648.py)

## Classes
### `TestParseTierModuleLevelExclusion`
- def: [`tests/unit/test_callers_dedup_and_parse_tier_647_648.py:75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_dedup_and_parse_tier_647_648.py#L75)
- doc: _find_enclosing_func must return None for module-level call sites.
- signature: `class TestParseTierModuleLevelExclusion:`
- members:
  - `project(self, tmp_path: Path)` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_dedup_and_parse_tier_647_648.py#L84)
  - `test_call_edge_count_excludes_module_level_call(self, project: str)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_dedup_and_parse_tier_647_648.py#L90) — The parse-tier should produce exactly 3 edges, not 4.
  - `test_execute_22_has_exactly_one_fmt_callee(self, project: str)` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_dedup_and_parse_tier_647_648.py#L122) — UnsubscribeTool.execute calls fmt once (line 23); the module-level
  - `test_no_call_edge_at_module_level_line(self, project: str)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_dedup_and_parse_tier_647_648.py#L109) — No call edge should be sourced from the module-level call line 26.
- uses (calls/refs, reference-scoped): [`FunctionRef`](../../tree_sitter_analyzer/call_graph.md#FunctionRef), [`CallGraph`](../../tree_sitter_analyzer/call_graph.md#CallGraph), [`build`](../../tree_sitter_analyzer/call_graph.md#CallGraph.build), [`_functions`](../../tree_sitter_analyzer/call_graph.md#CallGraph._functions), [`_call_edges`](../../tree_sitter_analyzer/call_graph.md#CallGraph._call_edges), [`_callees`](../../tree_sitter_analyzer/call_graph.md#CallGraph._callees)  (3 test-only)

### `TestSQLTierDedupKeepsBothMethods`
- def: [`tests/unit/test_callers_dedup_and_parse_tier_647_648.py:163`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_dedup_and_parse_tier_647_648.py#L163)
- doc: The SQL dedup key must include caller_line so same-named methods in
- signature: `class TestSQLTierDedupKeepsBothMethods:`
- members:
  - `test_caller_count_reflects_both_methods(self, indexed_project_647: str)` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_dedup_and_parse_tier_647_648.py#L196) — caller_count must be 2 (both execute methods), not 1 (collapsed).
  - `test_module_level_call_still_counted_not_emitted(self, indexed_project_647: str)` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_dedup_and_parse_tier_647_648.py#L221) — The module-level fmt() call is still excluded and counted (#638 invariant
  - `test_no_ghost_rows_after_dedup_fix(self, indexed_project_647: str)` — [`L207`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_dedup_and_parse_tier_647_648.py#L207) — After the dedup fix, no ghost rows (empty name or line=0) are emitted.
  - `test_two_execute_methods_produce_two_rows(self, indexed_project_647: str)` — [`L169`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_dedup_and_parse_tier_647_648.py#L169) — Both execute methods are distinct callers of fmt — both must appear.
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool.execute), [`CodeGraphCallersTool`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool)  (2 test-only)

## Functions
- `indexed_project_647(tmp_path: Path)` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_dedup_and_parse_tier_647_648.py#L151)

## Module values
- `_FIRST_EXECUTE_DEF_LINE` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_dedup_and_parse_tier_647_648.py#L65)
- `_MODULE_LEVEL_CALL_LINE` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_dedup_and_parse_tier_647_648.py#L67)
- `_SECOND_EXECUTE_DEF_LINE` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_dedup_and_parse_tier_647_648.py#L66)
- `_TWO_EXECUTE_SOURCE` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_dedup_and_parse_tier_647_648.py#L35)

