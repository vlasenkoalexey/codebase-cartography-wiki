---
title: 'Module: tests/unit/mcp/tools/test_edit_facade.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_edit_facade.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_edit_facade`/
symbols:
  _FakeInner.last_args: _FakeInner#last_args.
  _make_fake_facade: _make_fake_facade().
  _FakeInner: _FakeInner#
  test_set_project_path_rebinds_all_inners: test_set_project_path_rebinds_all_inners().
  test_edit_pr_action_missing_pr_url_fails_loudly: test_edit_pr_action_missing_pr_url_fails_loudly().
  test_edit_facade_builds: test_edit_facade_builds().
  test_edit_facade_all_actions_present: test_edit_facade_all_actions_present().
  test_action_routes_to_correct_inner: test_action_routes_to_correct_inner().
  test_arg_projection_strips_action_key: test_arg_projection_strips_action_key().
  test_arg_projection_passes_known_params: test_arg_projection_passes_known_params().
  test_sibling_param_is_dropped: test_sibling_param_is_dropped().
  test_guard_symbol_passes_through_unchanged: test_guard_symbol_passes_through_unchanged().
  test_no_bespoke_routes: test_no_bespoke_routes().
  test_edit_facade_modification_type_has_enum: test_edit_facade_modification_type_has_enum().
  _FakeInner.execute: _FakeInner#execute().
  test_verdict_not_overwritten._execute_with_custom_verdict: test_verdict_not_overwritten()._execute_with_custom_verdict().
  _FakeInner._tool_name: _FakeInner#_tool_name.
  _FakeInner.get_tool_definition: _FakeInner#get_tool_definition().
  test_verdict_preserved_verbatim: test_verdict_preserved_verbatim().
  test_verdict_not_overwritten: test_verdict_not_overwritten().
  test_missing_action_returns_error_envelope: test_missing_action_returns_error_envelope().
  test_unknown_action_returns_error_envelope: test_unknown_action_returns_error_envelope().
  test_build_edit_facade_returns_facade_tool: test_build_edit_facade_returns_facade_tool().
  test_safe_action_does_not_leak_action_to_inner_strict_guard: test_safe_action_does_not_leak_action_to_inner_strict_guard().
  test_constraints_action_does_not_leak_action_to_inner: test_constraints_action_does_not_leak_action_to_inner().
  test_edit_facade_definition_includes_annotations: test_edit_facade_definition_includes_annotations().
  test_edit_facade_schema_includes_action_and_required: test_edit_facade_schema_includes_action_and_required().
  test_edit_facade_schema_lenient_additional_properties: test_edit_facade_schema_lenient_additional_properties().
  test_edit_facade_schema_has_modification_type_property: test_edit_facade_schema_has_modification_type_property().
  test_edit_facade_modification_type_NOT_in_required: test_edit_facade_modification_type_NOT_in_required().
  test_action_pr_without_mode_or_pr_url_fails_loudly: test_action_pr_without_mode_or_pr_url_fails_loudly().
  test_action_pr_explicit_diff_mode_still_reaches_diff: test_action_pr_explicit_diff_mode_still_reaches_diff().
  _FakeInner.rebound_to: _FakeInner#rebound_to.
  _FakeInner._on_project_root_changed: _FakeInner#_on_project_root_changed().
  test_impact_action_description_documents_mode_param: test_impact_action_description_documents_mode_param().
  test_facade_does_not_override_set_project_path: test_facade_does_not_override_set_project_path().
  test_edit_annotations_not_read_only: test_edit_annotations_not_read_only().
  test_edit_annotations_not_destructive: test_edit_annotations_not_destructive().
  test_edit_annotations_all_four_hints_present: test_edit_annotations_all_four_hints_present().
  test_ast_diff_facade_description_uses_real_mode_params: test_ast_diff_facade_description_uses_real_mode_params().
  test_edit_facade_guard_description_marks_modification_type_required: test_edit_facade_guard_description_marks_modification_type_required().
  _FakeInner.get_tool_schema: _FakeInner#get_tool_schema().
  _FakeInner.__init__: _FakeInner#__init__().
  _FakeInner.validate_arguments: _FakeInner#validate_arguments().
---
# Module: [`tests/unit/mcp/tools/test_edit_facade.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py)

## Classes
### `_FakeInner`  ·  implements/extends BaseMCPTool
- def: [`tests/unit/mcp/tools/test_edit_facade.py:61`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L61)
- doc: Minimal inner that records the args it receives.
- signature: `class _FakeInner(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L91`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L91)
  - `get_tool_definition(self)` — [`L81`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L81)
  - `get_tool_schema(self)` — [`L70`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L70)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L84`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L84)
  - `last_args` — [`L67`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L67)
  - `rebound_to` — [`L68`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L68)
- protocol/private: `__init__`[`L64`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L64), `_on_project_root_changed`[`L87`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L87), `_tool_name`[`L65`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L65)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`__init__`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.__init__)
- used by: [`BaseMCPTool`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool._on_project_root_changed)  (8 test-only)

## Functions
- `_execute_with_custom_verdict()` — [`L298`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L298)
- `_make_fake_facade(**kwargs: Any)` — [`L105`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L105) — Build a facade with all 8 edit actions wired to fake inners.
- `test_action_pr_explicit_diff_mode_still_reaches_diff()` — [`L683`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L683) — Direct sub-mode selection stays available through the facade.
- `test_action_pr_without_mode_or_pr_url_fails_loudly()` — [`L664`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L664) — Codex P1 (#483): facade action=pr with NO explicit mode must not
- `test_action_routes_to_correct_inner(action: str)` — [`L186`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L186)
- `test_arg_projection_passes_known_params()` — [`L215`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L215)
- `test_arg_projection_strips_action_key()` — [`L206`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L206)
- `test_ast_diff_facade_description_uses_real_mode_params()` — [`L488`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L488) — Leg D: the ast_diff description in the edit facade must reference the
- `test_build_edit_facade_returns_facade_tool()` — [`L385`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L385)
- `test_constraints_action_does_not_leak_action_to_inner(tmp_path: Any)` — [`L426`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L426) — F4 regression guard for ConstraintCheckTool (no required file_path).
- `test_edit_annotations_all_four_hints_present()` — [`L463`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L463) — test_every_tool_declares_mcp_annotations requires all 4 hint keys.
- `test_edit_annotations_not_destructive()` — [`L456`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L456) — edit facade suggests/analyses; it does not write files.
- `test_edit_annotations_not_read_only()` — [`L447`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L447) — edit facade spans mutating-intent actions — readOnlyHint must be False.
- `test_edit_facade_all_actions_present()` — [`L150`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L150)
- `test_edit_facade_builds()` — [`L131`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L131)
- `test_edit_facade_definition_includes_annotations()` — [`L471`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L471)
- `test_edit_facade_guard_description_marks_modification_type_required()` — [`L640`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L640) — action=guard description must mark modification_type as required (e.g. with *).
- `test_edit_facade_modification_type_NOT_in_required()` — [`L623`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L623) — modification_type must NOT be in facade required[] (runtime-resolved param).
- `test_edit_facade_modification_type_has_enum()` — [`L607`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L607) — modification_type property must carry the full authoritative enum.
- `test_edit_facade_schema_has_modification_type_property()` — [`L589`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L589) — Schema must declare modification_type so schema-reading agents see it.
- `test_edit_facade_schema_includes_action_and_required()` — [`L517`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L517)
- `test_edit_facade_schema_lenient_additional_properties()` — [`L540`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L540) — The merged facade schema must be lenient (additionalProperties not False).
- `test_edit_pr_action_missing_pr_url_fails_loudly()` — [`L555`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L555) — action=pr without pr_url → success:False, ERROR verdict, not 'No changed files'.
- `test_facade_does_not_override_set_project_path()` — [`L380`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L380) — FacadeTool must inherit set_project_path; edit facade must not override it.
- `test_guard_symbol_passes_through_unchanged()` — [`L254`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L254) — ModificationGuardTool declares ``symbol`` in its schema (NOT function_name).
- `test_impact_action_description_documents_mode_param()` — [`L139`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L139) — #998: action=impact supports a ``mode`` param (diff|staged|branch|pr).
- `test_missing_action_returns_error_envelope()` — [`L322`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L322)
- `test_no_bespoke_routes()` — [`L272`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L272)
- `test_safe_action_does_not_leak_action_to_inner_strict_guard(tmp_path: Any)` — [`L397`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L397) — Route 'safe' through the REAL SafeToEditTool. The inner's strict-param
- `test_set_project_path_rebinds_all_inners(tmp_path: Any)` — [`L356`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L356) — G3: facade.set_project_path must forward to every action_map inner.
- `test_sibling_param_is_dropped()` — [`L234`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L234) — ``file_path`` param routed to 'safe'; must NOT appear in 'impact' inner
- `test_unknown_action_returns_error_envelope()` — [`L342`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L342)
- `test_verdict_not_overwritten()` — [`L294`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L294) — Facade must not re-wrap / overwrite the inner's verdict envelope.
- `test_verdict_preserved_verbatim()` — [`L285`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_edit_facade.py#L285)

