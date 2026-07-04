---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.call_graph_impact`/
symbols:
  compute_call_graph_impact: compute_call_graph_impact().
  FunctionImpact.to_dict: FunctionImpact#to_dict().
  CallGraphImpactResult.to_dict: CallGraphImpactResult#to_dict().
  _build_call_graph: _build_call_graph().
  CallGraphImpactResult: CallGraphImpactResult#
  CallGraphImpactResult.functions_analyzed: CallGraphImpactResult#functions_analyzed.
  FunctionImpact: FunctionImpact#
  FunctionImpact.name: FunctionImpact#name.
  FunctionImpact.file: FunctionImpact#file.
  FunctionImpact.line: FunctionImpact#line.
  FunctionImpact.upstream_callers: FunctionImpact#upstream_callers.
  FunctionImpact.fan_in: FunctionImpact#fan_in.
  CallGraphImpactResult.total_upstream: CallGraphImpactResult#total_upstream.
  CallGraphImpactResult.total_downstream: CallGraphImpactResult#total_downstream.
  CallGraphImpactResult.high_risk_functions: CallGraphImpactResult#high_risk_functions.
  FunctionImpact.downstream_callees: FunctionImpact#downstream_callees.
  CallGraphImpactResult.function_impacts: CallGraphImpactResult#function_impacts.
  CallGraphImpactResult.affected_functions_by_file: CallGraphImpactResult#affected_functions_by_file.
  CallGraphImpactResult.cross_file_callers: CallGraphImpactResult#cross_file_callers.
  CallGraphImpactResult.cross_file_callees: CallGraphImpactResult#cross_file_callees.
  _MAX_FUNCTIONS_PER_FILE: _MAX_FUNCTIONS_PER_FILE.
  FunctionImpact.fan_out: FunctionImpact#fan_out.
  logger: logger.
  _MAX_UPSTREAM: _MAX_UPSTREAM.
  _MAX_DOWNSTREAM: _MAX_DOWNSTREAM.
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py)

## Classes
### `CallGraphImpactResult`
- def: [`tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py:61`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L61)
- signature: `class CallGraphImpactResult:`
- members:
  - `to_dict(self)` — [`L71`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L71)
  - `affected_functions_by_file` — [`L69`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L69)
  - `cross_file_callees` — [`L67`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L67)
  - `cross_file_callers` — [`L66`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L66)
  - `function_impacts` — [`L68`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L68)
  - `functions_analyzed` — [`L62`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L62)
  - `high_risk_functions` — [`L65`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L65)
  - `total_downstream` — [`L64`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L64)
  - `total_upstream` — [`L63`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L63)
- uses (calls/refs, reference-scoped): [`_MAX_FUNCTIONS_PER_FILE`](call_graph_impact.md#_MAX_FUNCTIONS_PER_FILE)
- used by: [`_build_change_impact_result`](change_impact_analysis.md#_build_change_impact_result), [`compute_call_graph_impact`](call_graph_impact.md#compute_call_graph_impact)  (6 test-only)

### `FunctionImpact`
- def: [`tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py:36`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L36)
- signature: `class FunctionImpact:`
- members:
  - `to_dict(self)` — [`L45`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L45)
  - `downstream_callees` — [`L41`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L41)
  - `fan_in` — [`L42`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L42)
  - `fan_out` — [`L43`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L43)
  - `file` — [`L38`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L38)
  - `line` — [`L39`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L39)
  - `name` — [`L37`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L37)
  - `upstream_callers` — [`L40`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L40)
- uses (calls/refs, reference-scoped): [`_MAX_DOWNSTREAM`](call_graph_impact.md#_MAX_DOWNSTREAM), [`_MAX_UPSTREAM`](call_graph_impact.md#_MAX_UPSTREAM)
- used by: [`compute_call_graph_impact`](call_graph_impact.md#compute_call_graph_impact)  (3 test-only)

## Functions
- `_build_call_graph(project_root: str, *, allow_full_scan: bool = True)` — [`L84`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L84)
- `compute_call_graph_impact(project_root: str, changed_files: list[str], *, allow_full_scan: bool = True)` — [`L112`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L112)

## Module values
- `_MAX_DOWNSTREAM` — [`L32`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L32)
- `_MAX_FUNCTIONS_PER_FILE` — [`L30`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L30)
- `_MAX_UPSTREAM` — [`L31`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L31)
- `logger` — [`L28`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/call_graph_impact.py#L28)

