---
title: 'Module: tests/unit/mcp/tools/test_index_facade.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_index_facade.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_index_facade`/
symbols:
  _run_action: _run_action().
  test_arg_projection_strips_action_key: test_arg_projection_strips_action_key().
  test_sibling_param_dropped_between_actions: test_sibling_param_dropped_between_actions().
  test_all_7_actions_registered: test_all_7_actions_registered().
  test_envelope_preserved_verbatim: test_envelope_preserved_verbatim().
  test_set_project_path_rebinds_all_inners: test_set_project_path_rebinds_all_inners().
  test_build_index_facade_returns_facade_tool: test_build_index_facade_returns_facade_tool().
  test_all_actions_in_action_map_not_bespoke: test_all_actions_in_action_map_not_bespoke().
  test_unknown_action_returns_error_with_available_actions: test_unknown_action_returns_error_with_available_actions().
  test_schema_includes_action_and_union_params: test_schema_includes_action_and_union_params().
  _ALL_ACTIONS: _ALL_ACTIONS.
  test_action_routes_to_correct_inner: test_action_routes_to_correct_inner().
  test_missing_action_returns_error_envelope: test_missing_action_returns_error_envelope().
  test_no_set_project_path_override: test_no_set_project_path_override().
  test_end_to_end_no_strict_param_leak_status: test_end_to_end_no_strict_param_leak_status().
  test_annotations_set_correctly: test_annotations_set_correctly().
  test_cache_action_description_lists_mutating_modes: test_cache_action_description_lists_mutating_modes().
  _mock_result: _mock_result().
  test_arg_projection_strips_action_key._capture: test_arg_projection_strips_action_key()._capture().
  test_sibling_param_dropped_between_actions._capture: test_sibling_param_dropped_between_actions()._capture().
---
# Module: [`tests/unit/mcp/tools/test_index_facade.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py)

## Functions
- `_capture(args: dict[str, Any])` — [`L150`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L150)
- `_capture(args: dict[str, Any])` — [`L174`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L174)
- `_mock_result(action: str)` — [`L113`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L113)
- `_run_action(action: str, extra: dict[str, Any] | None = None)` — [`L126`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L126)
- `test_action_routes_to_correct_inner(action: str)` — [`L135`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L135)
- `test_all_7_actions_registered()` — [`L93`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L93)
- `test_all_actions_in_action_map_not_bespoke()` — [`L101`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L101) — All index facade actions are normal delegates (no bespoke routes).
- `test_annotations_set_correctly()` — [`L301`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L301) — Spec §6: index facade spans read-only (status/cache) and mutating
- `test_arg_projection_strips_action_key()` — [`L146`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L146)
- `test_build_index_facade_returns_facade_tool()` — [`L74`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L74)
- `test_cache_action_description_lists_mutating_modes()` — [`L80`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L80) — #992: action=cache also exposes mutating modes (index/sync/watch_*).
- `test_end_to_end_no_strict_param_leak_status(tmp_path: Any)` — [`L271`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L271) — Route status through the REAL inner tool (fresh tmp_path, no index).
- `test_envelope_preserved_verbatim()` — [`L192`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L192)
- `test_missing_action_returns_error_envelope()` — [`L218`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L218)
- `test_no_set_project_path_override()` — [`L258`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L258) — Factory must return a plain FacadeTool; FacadeTool itself must not
- `test_schema_includes_action_and_union_params()` — [`L322`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L322)
- `test_set_project_path_rebinds_all_inners(tmp_path: Any)` — [`L242`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L242)
- `test_sibling_param_dropped_between_actions()` — [`L168`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L168) — A ``query`` param belonging to the ``cache`` action must not reach the
- `test_unknown_action_returns_error_with_available_actions()` — [`L228`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L228)

## Module values
- `_ALL_ACTIONS` — [`L58`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_index_facade.py#L58)

