---
title: 'Module: tests/unit/mcp/tools/test_structure_facade.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_structure_facade.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_structure_facade`/
symbols:
  test_set_project_path_rebinds_bespoke_inners: test_set_project_path_rebinds_bespoke_inners().
  test_read_bespoke_action_stripped: test_read_bespoke_action_stripped().
  test_class_detail_query_alias_resolves_to_class_name: test_class_detail_query_alias_resolves_to_class_name().
  test_class_detail_class_name_direct_still_works: test_class_detail_class_name_direct_still_works().
  test_arg_projection_strips_action_key: test_arg_projection_strips_action_key().
  test_sibling_param_not_forwarded: test_sibling_param_not_forwarded().
  test_envelope_preserved: test_envelope_preserved().
  test_bespoke_inner_is_read_partial_tool_registered: test_bespoke_inner_is_read_partial_tool_registered().
  test_structure_facade_has_all_expected_actions: test_structure_facade_has_all_expected_actions().
  test_action_routing_class_detail: test_action_routing_class_detail().
  test_set_project_path_rebinds_action_map_inners: test_set_project_path_rebinds_action_map_inners().
  test_structure_facade_builds: test_structure_facade_builds().
  test_structure_facade_query_not_registered: test_structure_facade_query_not_registered().
  test_structure_facade_read_is_bespoke: test_structure_facade_read_is_bespoke().
  test_structure_facade_action_map_entries: test_structure_facade_action_map_entries().
  test_action_routing_outline: test_action_routing_outline().
  test_action_routing_analyze: test_action_routing_analyze().
  test_action_routing_ast_path: test_action_routing_ast_path().
  test_action_routing_sitemap: test_action_routing_sitemap().
  test_action_routing_class_tree: test_action_routing_class_tree().
  test_action_routing_explore: test_action_routing_explore().
  test_missing_action_returns_error_envelope: test_missing_action_returns_error_envelope().
  test_class_detail_is_bespoke_route: test_class_detail_is_bespoke_route().
  test_read_bespoke_single_mode: test_read_bespoke_single_mode().
  test_read_bespoke_batch_mode: test_read_bespoke_batch_mode().
  test_read_bespoke_missing_required_params: test_read_bespoke_missing_required_params().
  test_unknown_action_returns_error_envelope: test_unknown_action_returns_error_envelope().
  test_factory_returns_facade_tool: test_factory_returns_facade_tool().
  test_end_to_end_no_strict_param_leak: test_end_to_end_no_strict_param_leak().
  test_annotations_set_correctly: test_annotations_set_correctly().
  test_structure_read_coerces_string_bounds: test_structure_read_coerces_string_bounds().
  test_structure_read_rejects_non_numeric_bounds: test_structure_read_rejects_non_numeric_bounds().
  test_structure_read_rejects_fractional_float_bounds: test_structure_read_rejects_fractional_float_bounds().
  test_class_hierarchy_default_mode_is_tree_when_class_named: test_class_hierarchy_default_mode_is_tree_when_class_named().
  test_class_hierarchy_default_mode_is_summary_without_class: test_class_hierarchy_default_mode_is_summary_without_class().
  test_class_hierarchy_explicit_mode_always_honored: test_class_hierarchy_explicit_mode_always_honored().
  test_class_hierarchy_validate_accepts_named_class_without_mode: test_class_hierarchy_validate_accepts_named_class_without_mode().
  test_class_tree_supers_in_schema_enum: test_class_tree_supers_in_schema_enum().
  test_class_tree_supers_alias_normalizes_to_superclasses: test_class_tree_supers_alias_normalizes_to_superclasses().
  test_class_tree_mode_supers_does_not_return_unknown_mode_error: test_class_tree_mode_supers_does_not_return_unknown_mode_error().
  test_class_detail_class_name_in_facade_schema: test_class_detail_class_name_in_facade_schema().
  _EXPECTED_ACTIONS: _EXPECTED_ACTIONS.
  test_facade_does_not_override_set_project_path: test_facade_does_not_override_set_project_path().
  test_arg_projection_strips_action_key.spy_execute: test_arg_projection_strips_action_key().spy_execute().
  test_sibling_param_not_forwarded.spy_execute: test_sibling_param_not_forwarded().spy_execute().
  test_read_bespoke_action_stripped.fake_execute: test_read_bespoke_action_stripped().fake_execute().
  test_envelope_preserved.fake_execute: test_envelope_preserved().fake_execute().
  test_class_detail_query_alias_resolves_to_class_name.spy_execute: test_class_detail_query_alias_resolves_to_class_name().spy_execute().
  test_class_detail_class_name_direct_still_works.spy_execute: test_class_detail_class_name_direct_still_works().spy_execute().
---
# Module: [`tests/unit/mcp/tools/test_structure_facade.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py)

## Functions
- `fake_execute(args: dict[str, Any])` — [`L272`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L272)
- `fake_execute(args: dict[str, Any])` — [`L297`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L297)
- `spy_execute(args: dict[str, Any])` — [`L181`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L181)
- `spy_execute(args: dict[str, Any])` — [`L202`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L202)
- `spy_execute(args: dict)` — [`L678`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L678)
- `spy_execute(args: dict)` — [`L709`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L709)
- `test_action_routing_analyze()` — [`L116`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L116)
- `test_action_routing_ast_path()` — [`L125`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L125)
- `test_action_routing_class_detail()` — [`L148`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L148) — class_detail is a bespoke route (#804) — not in action_map but registered
- `test_action_routing_class_tree()` — [`L141`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L141)
- `test_action_routing_explore()` — [`L161`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L161)
- `test_action_routing_outline()` — [`L109`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L109)
- `test_action_routing_sitemap()` — [`L132`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L132)
- `test_annotations_set_correctly()` — [`L451`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L451)
- `test_arg_projection_strips_action_key()` — [`L175`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L175) — F4 Landmine A: ``action`` must be stripped or the inner raises ValueError.
- `test_bespoke_inner_is_read_partial_tool_registered()` — [`L378`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L378) — ReadPartialTool, AnalyzeCodeStructureTool, and ClassInspectTool must be
- `test_class_detail_class_name_direct_still_works()` — [`L697`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L697) — Passing class_name=X directly (without query) must still work (#804).
- `test_class_detail_class_name_in_facade_schema()` — [`L652`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L652) — class_name must be a declared property in the facade's public schema (#804).
- `test_class_detail_is_bespoke_route()` — [`L729`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L729) — class_detail must be in bespoke_map (not action_map) for the alias to work.
- `test_class_detail_query_alias_resolves_to_class_name()` — [`L664`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L664) — Passing query=X for class_detail must behave the same as class_name=X (#804).
- `test_class_hierarchy_default_mode_is_summary_without_class()` — [`L561`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L561)
- `test_class_hierarchy_default_mode_is_tree_when_class_named()` — [`L554`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L554)
- `test_class_hierarchy_explicit_mode_always_honored()` — [`L568`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L568)
- `test_class_hierarchy_validate_accepts_named_class_without_mode()` — [`L581`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L581) — With a class_name and no mode, validation must pass: the resolved mode is
- `test_class_tree_mode_supers_does_not_return_unknown_mode_error()` — [`L616`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L616) — Calling class_tree with mode='supers' must NOT return 'Unknown mode: supers'.
- `test_class_tree_supers_alias_normalizes_to_superclasses()` — [`L605`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L605) — ClassHierarchyTool._normalize_mode must map 'supers' → 'superclasses'.
- `test_class_tree_supers_in_schema_enum()` — [`L595`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L595) — 'supers' must appear in the mode enum of ClassHierarchyTool's schema.
- `test_end_to_end_no_strict_param_leak(tmp_path: Any)` — [`L417`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L417) — Route one action through the real inner without a ValueError on 'action'.
- `test_envelope_preserved()` — [`L293`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L293)
- `test_facade_does_not_override_set_project_path()` — [`L407`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L407) — FacadeTool must not override set_project_path (BaseMCPTool contract).
- `test_factory_returns_facade_tool()` — [`L401`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L401) — build_structure_facade must return a FacadeTool (no illegal subclass).
- `test_missing_action_returns_error_envelope()` — [`L319`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L319)
- `test_read_bespoke_action_stripped()` — [`L265`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L265) — Action key must not reach the _read_route (bespoke args are cleaned).
- `test_read_bespoke_batch_mode(tmp_path: Any)` — [`L244`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L244) — Batch mode: ``requests`` list is forwarded verbatim to ReadPartialTool.
- `test_read_bespoke_missing_required_params()` — [`L258`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L258) — read bespoke route raises ValueError when file_path/start_line absent.
- `test_read_bespoke_single_mode(tmp_path: Any)` — [`L221`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L221) — Single-file read: reshapes flat params into 11-key full_args.
- `test_set_project_path_rebinds_action_map_inners(tmp_path: Any)` — [`L343`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L343) — G3: action_map inners must get the new project root after set_project_path.
- `test_set_project_path_rebinds_bespoke_inners(tmp_path: Any)` — [`L354`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L354) — G3: all bespoke inners (ReadPartialTool, AnalyzeCodeStructureTool,
- `test_sibling_param_not_forwarded()` — [`L196`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L196) — class_name (for class_tree/class_detail) must not reach outline inner.
- `test_structure_facade_action_map_entries()` — [`L94`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L94) — All non-bespoke actions are in action_map (plain inner tool delegation).
- `test_structure_facade_builds()` — [`L68`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L68)
- `test_structure_facade_has_all_expected_actions()` — [`L74`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L74)
- `test_structure_facade_query_not_registered()` — [`L80`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L80) — F3: query (.scm DSL) belongs to search facade, NOT structure.
- `test_structure_facade_read_is_bespoke()` — [`L87`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L87) — read must be a bespoke route (not in action_map) — it does reshaping.
- `test_structure_read_coerces_string_bounds(tmp_path: Any)` — [`L469`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L469) — Agents pass start_line/end_line as strings (the flat facade schema does
- `test_structure_read_rejects_fractional_float_bounds(tmp_path: Any)` — [`L518`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L518) — Codex P3 #328: a fractional numeric bound (start_line=2.9) must be
- `test_structure_read_rejects_non_numeric_bounds(tmp_path: Any)` — [`L496`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L496) — A genuinely non-numeric bound raises a CLEAR ValueError (caught at the MCP
- `test_unknown_action_returns_error_envelope()` — [`L330`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L330)

## Module values
- `_EXPECTED_ACTIONS` — [`L50`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_structure_facade.py#L50)

