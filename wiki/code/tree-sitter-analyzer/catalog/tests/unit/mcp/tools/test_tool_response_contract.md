---
title: 'Module: tests/unit/mcp/tools/test_tool_response_contract.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_tool_response_contract.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_tool_response_contract`/
symbols:
  TestEnvelopeSuccess.test_codegraph_metrics_call_graph_uses_cached_graph: TestEnvelopeSuccess#test_codegraph_metrics_call_graph_uses_cached_graph().
  TestEnvelopeSuccess.test_project_overview_envelope: TestEnvelopeSuccess#test_project_overview_envelope().
  TestEnvelopeSuccess.test_detect_routes_summary_envelope: TestEnvelopeSuccess#test_detect_routes_summary_envelope().
  TestEnvelopeSuccess.test_check_project_health_envelope: TestEnvelopeSuccess#test_check_project_health_envelope().
  TestEnvelopeSuccess.test_ast_cache_stats_envelope: TestEnvelopeSuccess#test_ast_cache_stats_envelope().
  TestEnvelopeSuccess.test_codegraph_metrics_call_graph_is_read_only_on_cold_cache: TestEnvelopeSuccess#test_codegraph_metrics_call_graph_is_read_only_on_cold_cache().
  TestEnvelopeFailure.test_route_detector_file_mode_traversal_returns_envelope: TestEnvelopeFailure#test_route_detector_file_mode_traversal_returns_envelope().
  _run: _run().
  TestExecuteAcrossAllTools.test_every_tool_response_honours_envelope: TestExecuteAcrossAllTools#test_every_tool_response_honours_envelope().
  TestEnvelopeSuccess.test_codegraph_metrics_call_graph_uses_cached_graph.FakeCachedCallGraph.call_edges: TestEnvelopeSuccess#test_codegraph_metrics_call_graph_uses_cached_graph().FakeCachedCallGraph#call_edges().
  TestEnvelopeValidator.test_rejects_non_dict: TestEnvelopeValidator#test_rejects_non_dict().
  TestEnvelopeValidator.test_rejects_missing_success: TestEnvelopeValidator#test_rejects_missing_success().
  TestEnvelopeValidator.test_rejects_non_bool_success: TestEnvelopeValidator#test_rejects_non_bool_success().
  TestEnvelopeValidator.test_failure_without_error_rejected: TestEnvelopeValidator#test_failure_without_error_rejected().
  TestEnvelopeValidator.test_failure_with_non_str_error_rejected: TestEnvelopeValidator#test_failure_with_non_str_error_rejected().
  TestEnvelopeValidator.test_accepts_minimal_success: TestEnvelopeValidator#test_accepts_minimal_success().
  TestEnvelopeValidator.test_accepts_minimal_failure: TestEnvelopeValidator#test_accepts_minimal_failure().
  TestEnvelopeValidator.test_accepts_real_tool_shape: TestEnvelopeValidator#test_accepts_real_tool_shape().
  TestExecuteAcrossAllTools.registered_tools: TestExecuteAcrossAllTools#registered_tools().
  TestEnvelopeSuccess.test_codegraph_metrics_call_graph_uses_cached_graph.FakeCachedCallGraph: TestEnvelopeSuccess#test_codegraph_metrics_call_graph_uses_cached_graph().FakeCachedCallGraph#
  FakeCachedCallGraph._call_edges: FakeCachedCallGraph#_call_edges.
  tiny_project: tiny_project().
  TestEnvelopeSuccess: TestEnvelopeSuccess#
  TestEnvelopeSuccess.test_codegraph_metrics_call_graph_uses_cached_graph.FakeCachedCallGraph.__init__: TestEnvelopeSuccess#test_codegraph_metrics_call_graph_uses_cached_graph().FakeCachedCallGraph#__init__().
  TestEnvelopeSuccess.test_codegraph_metrics_call_graph_uses_cached_graph.FakeCachedCallGraph.build: TestEnvelopeSuccess#test_codegraph_metrics_call_graph_uses_cached_graph().FakeCachedCallGraph#build().
  FakeCachedCallGraph.built: FakeCachedCallGraph#built.
  TestEnvelopeSuccess.test_codegraph_metrics_call_graph_uses_cached_graph.FakeCachedCallGraph.all_functions: TestEnvelopeSuccess#test_codegraph_metrics_call_graph_uses_cached_graph().FakeCachedCallGraph#all_functions().
  TestEnvelopeFailure: TestEnvelopeFailure#
  TestEnvelopeValidator: TestEnvelopeValidator#
  TestExecuteAcrossAllTools: TestExecuteAcrossAllTools#
---
# Module: [`tests/unit/mcp/tools/test_tool_response_contract.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py)

## Classes
### `FakeCachedCallGraph`
- def: [`tests/unit/mcp/tools/test_tool_response_contract.py:114`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L114)
- signature: `class FakeCachedCallGraph:`
- members:
  - `all_functions(self)` — [`L129`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L129)
  - `build(self)` — [`L126`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L126)
  - `call_edges(self)` — [`L135`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L135) — Public accessor used by codegraph_metrics_tool.
  - `built` — [`L127`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L127)
- protocol/private: `__init__`[`L115`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L115), `_call_edges`[`L118`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L118)
- used by: (1 test-only callers)

### `TestEnvelopeFailure`
- def: [`tests/unit/mcp/tools/test_tool_response_contract.py:154`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L154)
- doc: Tools handed bad input return `success=False` + `error` envelope.
- signature: `class TestEnvelopeFailure:`
- members:
  - `test_route_detector_file_mode_traversal_returns_envelope(self, tiny_project: Path)` — [`L157`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L157) — SEC-3 / ARCH-A5 together: failures still produce a valid
- uses (calls/refs, reference-scoped): [`RouteDetectorTool`](../../../../tree_sitter_analyzer/mcp/tools/route_detector_tool.md#RouteDetectorTool), [`validate_tool_response`](../../../../tree_sitter_analyzer/mcp/tools/tool_response.md#validate_tool_response), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/route_detector_tool.md#RouteDetectorTool.execute)  (1 test-only)

### `TestEnvelopeSuccess`
- def: [`tests/unit/mcp/tools/test_tool_response_contract.py:42`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L42)
- doc: Tools that need no arguments and should succeed against a tiny project.
- signature: `class TestEnvelopeSuccess:`
- members:
  - `test_ast_cache_stats_envelope(self, tiny_project: Path)` — [`L71`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L71)
  - `test_check_project_health_envelope(self, tiny_project: Path)` — [`L64`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L64)
  - `test_codegraph_metrics_call_graph_is_read_only_on_cold_cache(self, tiny_project: Path, monkeypatch: pytest.MonkeyPatch)` — [`L78`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L78)
  - `test_codegraph_metrics_call_graph_uses_cached_graph(self, tiny_project: Path, monkeypatch: pytest.MonkeyPatch)` — [`L100`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L100)
  - `test_detect_routes_summary_envelope(self, tiny_project: Path)` — [`L56`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L56)
  - `test_project_overview_envelope(self, tiny_project: Path)` — [`L45`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L45)
- uses (calls/refs, reference-scoped): [`ASTCacheTool`](../../../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool.execute), [`ProjectOverviewTool`](../../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool), [`RouteDetectorTool`](../../../../tree_sitter_analyzer/mcp/tools/route_detector_tool.md#RouteDetectorTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.md#CodeGraphMetricsTool.execute), [`validate_tool_response`](../../../../tree_sitter_analyzer/mcp/tools/tool_response.md#validate_tool_response), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool.execute), [`ProjectHealthTool`](../../../../tree_sitter_analyzer/mcp/tools/project_health_tool.md#ProjectHealthTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/project_health_tool.md#ProjectHealthTool.execute), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/route_detector_tool.md#RouteDetectorTool.execute), [`CodeGraphMetricsTool`](../../../../tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.md#CodeGraphMetricsTool)  (2 test-only)

### `TestEnvelopeValidator`
- def: [`tests/unit/mcp/tools/test_tool_response_contract.py:186`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L186)
- doc: Direct tests for the validator's own contract.
- signature: `class TestEnvelopeValidator:`
- members:
  - `test_accepts_minimal_failure(self)` — [`L212`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L212)
  - `test_accepts_minimal_success(self)` — [`L209`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L209)
  - `test_accepts_real_tool_shape(self)` — [`L215`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L215)
  - `test_failure_with_non_str_error_rejected(self)` — [`L205`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L205)
  - `test_failure_without_error_rejected(self)` — [`L201`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L201)
  - `test_rejects_missing_success(self)` — [`L193`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L193)
  - `test_rejects_non_bool_success(self)` — [`L197`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L197)
  - `test_rejects_non_dict(self)` — [`L189`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L189)
- uses (calls/refs, reference-scoped): [`validate_tool_response`](../../../../tree_sitter_analyzer/mcp/tools/tool_response.md#validate_tool_response)

### `TestExecuteAcrossAllTools`
- def: [`tests/unit/mcp/tools/test_tool_response_contract.py:228`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L228)
- doc: Exercise every registered MCP tool's execute() against a smoke
- signature: `class TestExecuteAcrossAllTools:`
- members:
  - `registered_tools(self, tiny_project: Path)` — [`L235`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L235)
  - `test_every_tool_response_honours_envelope(self, registered_tools, tiny_project: Path)` — [`L252`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L252)
- uses (calls/refs, reference-scoped): [`validate_tool_response`](../../../../tree_sitter_analyzer/mcp/tools/tool_response.md#validate_tool_response), [`_create_tool_registry`](../../../../tree_sitter_analyzer/mcp/server.md#_create_tool_registry)  (1 test-only)

## Functions
- `_run(coro)` — [`L38`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L38)
- `tiny_project(tmp_path: Path)` — [`L31`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_tool_response_contract.py#L31) — A 1-file project that every tool can analyse.

