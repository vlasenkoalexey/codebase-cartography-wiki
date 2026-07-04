---
title: 'Module: tests/unit/test_call_graph_impact.py'
type: catalog
provenance: extracted
module: tests/unit/test_call_graph_impact.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_call_graph_impact`/Test
symbols:
  TestChangeImpactIntegration.test_build_result_includes_call_graph: ChangeImpactIntegration#test_build_result_includes_call_graph().
  TestCallGraphImpactResult.test_to_dict: CallGraphImpactResult#test_to_dict().
  TestFunctionImpact.test_to_dict_with_callers: FunctionImpact#test_to_dict_with_callers().
  TestFunctionImpact.test_to_dict_truncates_long_lists: FunctionImpact#test_to_dict_truncates_long_lists().
  TestChangeImpactIntegration.test_build_result_without_call_graph: ChangeImpactIntegration#test_build_result_without_call_graph().
  TestFunctionImpact.test_to_dict_minimal: FunctionImpact#test_to_dict_minimal().
  TestComputeCallGraphImpact.test_basic_impact: ComputeCallGraphImpact#test_basic_impact().
  TestCallGraphImpactResult.test_empty: CallGraphImpactResult#test_empty().
  TestComputeCallGraphImpact.test_high_fan_in_detected: ComputeCallGraphImpact#test_high_fan_in_detected().
  TestComputeCallGraphImpact.test_no_functions_in_changed_file: ComputeCallGraphImpact#test_no_functions_in_changed_file().
  TestComputeCallGraphImpact.test_returns_none_for_empty_files: ComputeCallGraphImpact#test_returns_none_for_empty_files().
  TestComputeCallGraphImpact.test_returns_none_when_cg_fails: ComputeCallGraphImpact#test_returns_none_when_cg_fails().
  TestComputeCallGraphImpact.test_can_disable_full_scan_fallback: ComputeCallGraphImpact#test_can_disable_full_scan_fallback().
  TestFunctionImpact: FunctionImpact#
  TestCallGraphImpactResult: CallGraphImpactResult#
  TestComputeCallGraphImpact: ComputeCallGraphImpact#
  TestChangeImpactIntegration: ChangeImpactIntegration#
---
# Module: [`tests/unit/test_call_graph_impact.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_impact.py)

## Classes
### `TestCallGraphImpactResult`
- def: [`tests/unit/test_call_graph_impact.py:49`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_impact.py#L49)
- signature: `class TestCallGraphImpactResult:`
- members:
  - `test_empty(self)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_impact.py#L68)
  - `test_to_dict(self)` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_impact.py#L50)
- uses (calls/refs, reference-scoped): [`to_dict`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult.to_dict), [`CallGraphImpactResult`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult), [`functions_analyzed`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult.functions_analyzed), [`high_risk_functions`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult.high_risk_functions), [`total_downstream`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult.total_downstream), [`total_upstream`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult.total_upstream), [`affected_functions_by_file`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult.affected_functions_by_file), [`function_impacts`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult.function_impacts), [`cross_file_callees`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult.cross_file_callees), [`cross_file_callers`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult.cross_file_callers)

### `TestChangeImpactIntegration`
- def: [`tests/unit/test_call_graph_impact.py:143`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_impact.py#L143)
- signature: `class TestChangeImpactIntegration:`
- members:
  - `test_build_result_includes_call_graph(self)` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_impact.py#L144)
  - `test_build_result_without_call_graph(self, tmp_path, monkeypatch)` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_impact.py#L182)
- uses (calls/refs, reference-scoped): [`_build_change_impact_result`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#_build_change_impact_result), [`changed_files`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest.changed_files), [`project_root`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest.project_root), [`ChangeImpactRequest`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest), [`include_tests`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest.include_tests), [`mode`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest.mode), [`diff_stat`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest.diff_stat), [`CallGraphImpactResult`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult), [`agent_summary_only`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#ChangeImpactRequest.agent_summary_only), [`functions_analyzed`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult.functions_analyzed), [`total_downstream`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult.total_downstream), [`total_upstream`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult.total_upstream), [`function_impacts`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult.function_impacts)

### `TestComputeCallGraphImpact`
- def: [`tests/unit/test_call_graph_impact.py:75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_impact.py#L75)
- signature: `class TestComputeCallGraphImpact:`
- members:
  - `test_basic_impact(self, mock_build)` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_impact.py#L96)
  - `test_can_disable_full_scan_fallback(self, mock_build)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_impact.py#L87)
  - `test_high_fan_in_detected(self, mock_build)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_impact.py#L114)
  - `test_no_functions_in_changed_file(self, mock_build)` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_impact.py#L131)
  - `test_returns_none_for_empty_files(self)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_impact.py#L76)
  - `test_returns_none_when_cg_fails(self, mock_build)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_impact.py#L81)
- uses (calls/refs, reference-scoped): [`compute_call_graph_impact`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#compute_call_graph_impact), [`functions_analyzed`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult.functions_analyzed), [`high_risk_functions`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult.high_risk_functions), [`total_downstream`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult.total_downstream), [`total_upstream`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult.total_upstream), [`affected_functions_by_file`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#CallGraphImpactResult.affected_functions_by_file)

### `TestFunctionImpact`
- def: [`tests/unit/test_call_graph_impact.py:14`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_impact.py#L14)
- signature: `class TestFunctionImpact:`
- members:
  - `test_to_dict_minimal(self)` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_impact.py#L15)
  - `test_to_dict_truncates_long_lists(self)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_impact.py#L36)
  - `test_to_dict_with_callers(self)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_impact.py#L24)
- uses (calls/refs, reference-scoped): [`to_dict`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#FunctionImpact.to_dict), [`FunctionImpact`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#FunctionImpact), [`fan_in`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#FunctionImpact.fan_in), [`file`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#FunctionImpact.file), [`line`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#FunctionImpact.line), [`name`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#FunctionImpact.name), [`upstream_callers`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#FunctionImpact.upstream_callers), [`downstream_callees`](../../tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.md#FunctionImpact.downstream_callees)

