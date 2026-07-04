---
title: 'Module: tests/unit/mcp/tools/test_nav_facade.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_nav_facade.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_nav_facade`/
symbols:
  _build_facade_with_mock_inners: _build_facade_with_mock_inners().
  test_arg_projection_strips_action_from_navigate: test_arg_projection_strips_action_from_navigate().
  test_arg_projection_strips_action_from_impact: test_arg_projection_strips_action_from_impact().
  test_sibling_param_not_forwarded_to_navigate: test_sibling_param_not_forwarded_to_navigate().
  test_sibling_param_not_forwarded_to_trace: test_sibling_param_not_forwarded_to_trace().
  test_r3_symbol_normalized_for_action_map_routes: test_r3_symbol_normalized_for_action_map_routes().
  test_set_project_path_rebinds_action_map_inners: test_set_project_path_rebinds_action_map_inners().
  test_set_project_path_rebinds_bespoke_inners: test_set_project_path_rebinds_bespoke_inners().
  test_nav_facade_builds_returns_facade_tool: test_nav_facade_builds_returns_facade_tool().
  test_nav_facade_all_actions_present: test_nav_facade_all_actions_present().
  test_nav_facade_bespoke_actions_are_context_callers_callees: test_nav_facade_bespoke_actions_are_context_callers_callees().
  test_navigate_action_routes_to_navigate_inner: test_navigate_action_routes_to_navigate_inner().
  test_call_path_action_routes_to_call_path_inner: test_call_path_action_routes_to_call_path_inner().
  test_xref_action_routes_to_xref_inner: test_xref_action_routes_to_xref_inner().
  test_resolve_action_routes_to_resolve_inner: test_resolve_action_routes_to_resolve_inner().
  test_lineage_action_routes_to_lineage_inner: test_lineage_action_routes_to_lineage_inner().
  test_impact_action_routes_to_impact_inner: test_impact_action_routes_to_impact_inner().
  test_trace_action_routes_to_trace_inner: test_trace_action_routes_to_trace_inner().
  _capture_inner: _capture_inner().
  test_envelope_verdict_preserved: test_envelope_verdict_preserved().
  test_envelope_not_rewrapped: test_envelope_not_rewrapped().
  test_callers_scope_point_uses_callers_tool: test_callers_scope_point_uses_callers_tool().
  test_callers_default_scope_is_point: test_callers_default_scope_is_point().
  test_callers_scope_graph_uses_call_graph_tool: test_callers_scope_graph_uses_call_graph_tool().
  test_callees_scope_point_uses_callees_tool: test_callees_scope_point_uses_callees_tool().
  test_callees_scope_graph_uses_call_graph_tool: test_callees_scope_graph_uses_call_graph_tool().
  test_callers_bespoke_r3_symbol_to_function_name: test_callers_bespoke_r3_symbol_to_function_name().
  test_scope_not_forwarded_to_callers_point_inner: test_scope_not_forwarded_to_callers_point_inner().
  test_scope_not_forwarded_to_callees_graph_inner: test_scope_not_forwarded_to_callees_graph_inner().
  test_missing_action_returns_error_envelope: test_missing_action_returns_error_envelope().
  test_unknown_action_returns_error_envelope: test_unknown_action_returns_error_envelope().
  test_six_bespoke_inners_registered: test_six_bespoke_inners_registered().
  test_nav_facade_returns_facade_tool_not_subclass: test_nav_facade_returns_facade_tool_not_subclass().
  test_navigate_action_no_strict_leak: test_navigate_action_no_strict_leak().
  test_callers_point_action_no_strict_leak: test_callers_point_action_no_strict_leak().
  test_nav_facade_schema_contains_action: test_nav_facade_schema_contains_action().
  test_nav_facade_schema_action_enum_complete: test_nav_facade_schema_action_enum_complete().
  test_nav_facade_annotations_read_only: test_nav_facade_annotations_read_only().
  test_nav_facade_description_contains_codegraph_keyword: test_nav_facade_description_contains_codegraph_keyword().
  test_context_action_with_symbol_normalizes_to_task_no_valueerror: test_context_action_with_symbol_normalizes_to_task_no_valueerror().
  test_context_action_with_query_normalizes_to_task_no_valueerror: test_context_action_with_query_normalizes_to_task_no_valueerror().
  test_call_path_in_running_event_loop_returns_dict: test_call_path_in_running_event_loop_returns_dict().
  test_callers_limit_forwarded_to_point_inner: test_callers_limit_forwarded_to_point_inner().
  test_callees_limit_forwarded_to_point_inner: test_callees_limit_forwarded_to_point_inner().
  _capture_inner._capture: _capture_inner()._capture().
  test_arg_projection_strips_action_from_navigate._spy: test_arg_projection_strips_action_from_navigate()._spy().
  test_arg_projection_strips_action_from_impact._spy: test_arg_projection_strips_action_from_impact()._spy().
  test_sibling_param_not_forwarded_to_navigate._spy: test_sibling_param_not_forwarded_to_navigate()._spy().
  test_sibling_param_not_forwarded_to_trace._spy: test_sibling_param_not_forwarded_to_trace()._spy().
  test_r3_symbol_normalized_for_action_map_routes._spy: test_r3_symbol_normalized_for_action_map_routes()._spy().
---
# Module: [`tests/unit/mcp/tools/test_nav_facade.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py)

## Functions
- `_build_facade_with_mock_inners()` — [`L334`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L334) — Build a nav facade and replace all bespoke backing instances with mocks.
- `_capture(args: dict[str, Any])` — [`L193`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L193)
- `_capture_inner(facade: FacadeTool, action: str)` — [`L188`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L188) — Patch an action_map inner's execute to capture received args.
- `_spy(args: dict[str, Any])` — [`L205`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L205)
- `_spy(args: dict[str, Any])` — [`L223`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L223)
- `_spy(args: dict[str, Any])` — [`L252`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L252)
- `_spy(args: dict[str, Any])` — [`L276`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L276)
- `_spy(args: dict[str, Any])` — [`L308`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L308)
- `test_arg_projection_strips_action_from_impact()` — [`L218`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L218)
- `test_arg_projection_strips_action_from_navigate()` — [`L200`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L200)
- `test_call_path_action_routes_to_call_path_inner()` — [`L113`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L113)
- `test_call_path_in_running_event_loop_returns_dict(tmp_path: Any)` — [`L763`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L763) — Fix ③: nav action=call_path in an already-running event loop must not
- `test_callees_limit_forwarded_to_point_inner()` — [`L812`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L812) — DF-13: limit= must reach callees_point inner when action=callees scope=point.
- `test_callees_scope_graph_uses_call_graph_tool()` — [`L430`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L430)
- `test_callees_scope_point_uses_callees_tool()` — [`L414`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L414)
- `test_callers_bespoke_r3_symbol_to_function_name()` — [`L448`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L448) — Bespoke route: symbol= should be defensively copied to function_name= by
- `test_callers_default_scope_is_point()` — [`L379`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L379) — scope=point is the default; omitting scope should behave the same.
- `test_callers_limit_forwarded_to_point_inner()` — [`L789`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L789) — DF-13: limit= must reach callers_point inner when action=callers scope=point.
- `test_callers_point_action_no_strict_leak(tmp_path: Any)` — [`L624`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L624) — Bespoke callers route (scope=point) must not trip the inner's strict-param guard.
- `test_callers_scope_graph_uses_call_graph_tool()` — [`L395`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L395)
- `test_callers_scope_point_uses_callers_tool()` — [`L363`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L363)
- `test_context_action_with_query_normalizes_to_task_no_valueerror(tmp_path: Any)` — [`L747`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L747) — Fix ③: nav action=context with query= (alternate alias) must also work.
- `test_context_action_with_symbol_normalizes_to_task_no_valueerror(tmp_path: Any)` — [`L720`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L720) — Fix ③: nav action=context with symbol= must NOT raise ValueError('task is
- `test_envelope_not_rewrapped()` — [`L516`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L516) — The facade must not nest the inner envelope inside another dict.
- `test_envelope_verdict_preserved()` — [`L502`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L502)
- `test_impact_action_routes_to_impact_inner()` — [`L157`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L157)
- `test_lineage_action_routes_to_lineage_inner()` — [`L148`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L148)
- `test_missing_action_returns_error_envelope()` — [`L531`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L531)
- `test_nav_facade_all_actions_present()` — [`L60`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L60)
- `test_nav_facade_annotations_read_only()` — [`L686`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L686) — All nav actions are read-only — annotations must reflect this honestly.
- `test_nav_facade_bespoke_actions_are_context_callers_callees()` — [`L84`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L84)
- `test_nav_facade_builds_returns_facade_tool()` — [`L54`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L54)
- `test_nav_facade_description_contains_codegraph_keyword()` — [`L702`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L702) — Fix ②: nav description must contain 'codegraph' so ToolSearch/keyword
- `test_nav_facade_returns_facade_tool_not_subclass()` — [`L592`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L592) — The factory returns an instance of FacadeTool — no subclassing means
- `test_nav_facade_schema_action_enum_complete()` — [`L661`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L661)
- `test_nav_facade_schema_contains_action()` — [`L650`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L650)
- `test_navigate_action_no_strict_leak(tmp_path: Any)` — [`L604`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L604) — Route navigate through the REAL CodeGraphNavigateTool in a fresh tmp dir.
- `test_navigate_action_routes_to_navigate_inner()` — [`L101`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L101)
- `test_r3_symbol_normalized_for_action_map_routes()` — [`L299`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L299) — navigate inner reads ``symbol`` — normalization should NOT overwrite it.
- `test_resolve_action_routes_to_resolve_inner()` — [`L139`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L139)
- `test_scope_not_forwarded_to_callees_graph_inner()` — [`L482`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L482)
- `test_scope_not_forwarded_to_callers_point_inner()` — [`L466`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L466) — scope is a facade control key; must not leak into the callers_point inner.
- `test_set_project_path_rebinds_action_map_inners(tmp_path: Any)` — [`L555`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L555)
- `test_set_project_path_rebinds_bespoke_inners(tmp_path: Any)` — [`L565`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L565) — G3: all four bespoke inners (callers_point, callers_graph, callees_point,
- `test_sibling_param_not_forwarded_to_navigate()` — [`L246`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L246) — source_function (call_path param) must not reach navigate inner.
- `test_sibling_param_not_forwarded_to_trace()` — [`L270`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L270) — function_names (impact param) must not reach trace inner.
- `test_six_bespoke_inners_registered()` — [`L577`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L577) — Exactly 6 bespoke inners: context_inner, callers_point, callers_graph,
- `test_trace_action_routes_to_trace_inner()` — [`L174`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L174)
- `test_unknown_action_returns_error_envelope()` — [`L540`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L540)
- `test_xref_action_routes_to_xref_inner()` — [`L130`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_facade.py#L130)

