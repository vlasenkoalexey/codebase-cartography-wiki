---
title: 'Module: tests/unit/mcp/test_trace_impact_count_fix.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_trace_impact_count_fix.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_trace_impact_count_fix`/
symbols:
  tool: tool().
  TestTraceImpactCountAccuracy.test_unit_count_not_capped_by_mock: TestTraceImpactCountAccuracy#test_unit_count_not_capped_by_mock().
  pytestmark: pytestmark.
  SPRING_BASE: SPRING_BASE.
  TestTraceImpactCountAccuracy: TestTraceImpactCountAccuracy#
  TestTraceImpactCountAccuracy.test_call_count_not_capped_by_max_results: TestTraceImpactCountAccuracy#test_call_count_not_capped_by_max_results().
  TestTraceImpactCountAccuracy.test_impact_level_reflects_true_count: TestTraceImpactCountAccuracy#test_impact_level_reflects_true_count().
  TestTraceImpactCountAccuracy.test_truncated_flag_set_when_results_capped: TestTraceImpactCountAccuracy#test_truncated_flag_set_when_results_capped().
---
# Module: [`tests/unit/mcp/test_trace_impact_count_fix.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_trace_impact_count_fix.py)

## Classes
### `TestTraceImpactCountAccuracy`
- def: [`tests/unit/mcp/test_trace_impact_count_fix.py:32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_trace_impact_count_fix.py#L32)
- doc: call_count must reflect true match total, not the display-capped count.
- signature: `class TestTraceImpactCountAccuracy:`
- members:
  - `test_call_count_not_capped_by_max_results(self, tool)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_trace_impact_count_fix.py#L35) — With max_results=5 and 695 real matches, call_count must be 695.
  - `test_impact_level_reflects_true_count(self, tool)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_trace_impact_count_fix.py#L56) — impact_level must use true total, not capped count.
  - `test_truncated_flag_set_when_results_capped(self, tool)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_trace_impact_count_fix.py#L67) — truncated=True must be returned when results exceed max_results.
  - `test_unit_count_not_capped_by_mock(self)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_trace_impact_count_fix.py#L76) — Unit test without external dependency.
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#TraceImpactTool.execute), [`TraceImpactTool`](../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#TraceImpactTool)

## Functions
- `tool()` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_trace_impact_count_fix.py#L26)

## Module values
- `SPRING_BASE` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_trace_impact_count_fix.py#L17)
- `pytestmark` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_trace_impact_count_fix.py#L19)

