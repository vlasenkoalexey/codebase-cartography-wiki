---
title: 'Module: tests/unit/mcp/tools/test_project_facade.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_project_facade.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_project_facade`/
symbols:
  _run_action: _run_action().
  test_arg_projection_strips_action_key: test_arg_projection_strips_action_key().
  test_sibling_param_dropped_between_actions: test_sibling_param_dropped_between_actions().
  test_all_10_actions_registered: test_all_10_actions_registered().
  test_envelope_preserved_verbatim: test_envelope_preserved_verbatim().
  test_set_project_path_rebinds_all_inners: test_set_project_path_rebinds_all_inners().
  test_smart_action_documented_params_subset_of_inner_schema: test_smart_action_documented_params_subset_of_inner_schema().
  test_build_project_facade_returns_facade_tool: test_build_project_facade_returns_facade_tool().
  test_all_actions_in_action_map_not_bespoke: test_all_actions_in_action_map_not_bespoke().
  test_index_actions_not_in_project_facade: test_index_actions_not_in_project_facade().
  test_unknown_action_returns_error_with_available_actions: test_unknown_action_returns_error_with_available_actions().
  test_schema_includes_action_and_union_params: test_schema_includes_action_and_union_params().
  _ALL_ACTIONS: _ALL_ACTIONS.
  test_action_routes_to_correct_inner: test_action_routes_to_correct_inner().
  test_missing_action_returns_error_envelope: test_missing_action_returns_error_envelope().
  test_no_set_project_path_override: test_no_set_project_path_override().
  test_end_to_end_no_strict_param_leak: test_end_to_end_no_strict_param_leak().
  test_annotations_set_correctly: test_annotations_set_correctly().
  test_journal_description_uses_real_param_names: test_journal_description_uses_real_param_names().
  _mock_result: _mock_result().
  test_arg_projection_strips_action_key._capture: test_arg_projection_strips_action_key()._capture().
  test_sibling_param_dropped_between_actions._capture: test_sibling_param_dropped_between_actions()._capture().
---
# Module: [`tests/unit/mcp/tools/test_project_facade.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py)

## Functions
- `_capture(args: dict[str, Any])` — [`L154`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L154)
- `_capture(args: dict[str, Any])` — [`L178`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L178)
- `_mock_result(action: str)` — [`L117`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L117)
- `_run_action(action: str, extra: dict[str, Any] | None = None)` — [`L130`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L130)
- `test_action_routes_to_correct_inner(action: str)` — [`L139`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L139)
- `test_all_10_actions_registered()` — [`L79`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L79)
- `test_all_actions_in_action_map_not_bespoke()` — [`L87`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L87) — All project facade actions are normal delegates (no bespoke routes).
- `test_annotations_set_correctly()` — [`L330`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L330) — Spec §6: project spans read + mutating (journal/doc_sync) actions.
- `test_arg_projection_strips_action_key()` — [`L150`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L150)
- `test_build_project_facade_returns_facade_tool()` — [`L73`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L73)
- `test_end_to_end_no_strict_param_leak(tmp_path: Any, action: str, extra_args: dict[str, Any])` — [`L296`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L296) — Route action through the REAL inner tool (fresh tmp_path, no index).
- `test_envelope_preserved_verbatim()` — [`L196`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L196)
- `test_index_actions_not_in_project_facade()` — [`L94`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L94) — Index lifecycle actions must have been extracted to the index facade.
- `test_journal_description_uses_real_param_names()` — [`L369`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L369) — project facade journal description must reference real inner params.
- `test_missing_action_returns_error_envelope()` — [`L222`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L222)
- `test_no_set_project_path_override()` — [`L272`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L272) — Factory must return a plain FacadeTool; FacadeTool itself must not
- `test_schema_includes_action_and_union_params()` — [`L351`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L351)
- `test_set_project_path_rebinds_all_inners(tmp_path: Any)` — [`L256`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L256)
- `test_sibling_param_dropped_between_actions()` — [`L172`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L172) — A ``query`` param belonging to the ``cache`` action must not reach the
- `test_smart_action_documented_params_subset_of_inner_schema()` — [`L404`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L404) — #573: the facade's documented params for ``action=smart`` must all exist
- `test_unknown_action_returns_error_with_available_actions()` — [`L232`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L232)

## Module values
- `_ALL_ACTIONS` — [`L54`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_project_facade.py#L54)

