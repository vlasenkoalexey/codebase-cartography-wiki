---
title: 'Module: tests/unit/mcp/tools/test_health_facade.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_health_facade.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_health_facade`/
symbols:
  test_health_facade_builds_and_has_all_actions: test_health_facade_builds_and_has_all_actions().
  test_health_facade_does_not_contain_viz_actions: test_health_facade_does_not_contain_viz_actions().
  test_set_project_path_rebinds_all_action_map_inners: test_set_project_path_rebinds_all_action_map_inners().
  test_health_facade_total_action_count: test_health_facade_total_action_count().
  test_project_action_routes_and_strips_action_key: test_project_action_routes_and_strips_action_key().
  test_file_action_routes_and_strips_action_key: test_file_action_routes_and_strips_action_key().
  test_deps_action_routes_and_preserves_mode: test_deps_action_routes_and_preserves_mode().
  test_deps_mode_summary: test_deps_mode_summary().
  test_deps_mode_blast: test_deps_mode_blast().
  test_deps_mode_file_deps: test_deps_mode_file_deps().
  test_sibling_param_does_not_reach_project_inner: test_sibling_param_does_not_reach_project_inner().
  test_sibling_param_does_not_reach_scale_inner: test_sibling_param_does_not_reach_scale_inner().
  test_r3_normalize_symbol_to_function_name_for_heatmap: test_r3_normalize_symbol_to_function_name_for_heatmap().
  test_r3_explicit_function_name_wins_over_symbol: test_r3_explicit_function_name_wins_over_symbol().
  test_envelope_preserved_verbatim: test_envelope_preserved_verbatim().
  test_missing_action_returns_error_envelope: test_missing_action_returns_error_envelope().
  test_schema_lists_action_and_core_params: test_schema_lists_action_and_core_params().
  test_facade_description_mentions_all_actions: test_facade_description_mentions_all_actions().
  _ALL_ACTIONS: _ALL_ACTIONS.
  test_health_facade_annotations_read_only: test_health_facade_annotations_read_only().
  test_unknown_action_returns_error_envelope: test_unknown_action_returns_error_envelope().
  test_health_facade_factory_returns_facade_tool: test_health_facade_factory_returns_facade_tool().
  test_project_action_no_strict_leak: test_project_action_no_strict_leak().
  test_deps_action_no_strict_leak: test_deps_action_no_strict_leak().
  _FakeInner: _FakeInner#
  _FakeInner.__init__: _FakeInner#__init__().
  _FakeInner.get_tool_definition: _FakeInner#get_tool_definition().
  _FakeInner._on_project_root_changed: _FakeInner#_on_project_root_changed().
  _FakeInner.execute: _FakeInner#execute().
  _FakeFunctionNameInner: _FakeFunctionNameInner#
  _FakeFunctionNameInner.__init__: _FakeFunctionNameInner#__init__().
  _FakeFunctionNameInner.get_tool_definition: _FakeFunctionNameInner#get_tool_definition().
  _FakeFunctionNameInner.execute: _FakeFunctionNameInner#execute().
  _VIZ_ACTIONS: _VIZ_ACTIONS.
  _FakeInner.last_args: _FakeInner#last_args.
  _FakeInner.rebound_to: _FakeInner#rebound_to.
  _FakeInner.get_tool_schema: _FakeInner#get_tool_schema().
  _FakeFunctionNameInner.last_args: _FakeFunctionNameInner#last_args.
  _FakeFunctionNameInner.get_tool_schema: _FakeFunctionNameInner#get_tool_schema().
  _FakeInner.validate_arguments: _FakeInner#validate_arguments().
  _FakeFunctionNameInner.validate_arguments: _FakeFunctionNameInner#validate_arguments().
---
# Module: [`tests/unit/mcp/tools/test_health_facade.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py)

## Classes
### `_FakeFunctionNameInner`  ·  implements/extends BaseMCPTool
- def: [`tests/unit/mcp/tools/test_health_facade.py:127`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L127)
- doc: Inner that declares `function_name` — used to test R3 normalize.
- signature: `class _FakeFunctionNameInner(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L147`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L147)
  - `get_tool_definition(self)` — [`L141`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L141)
  - `get_tool_schema(self)` — [`L134`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L134)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L144`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L144)
  - `last_args` — [`L132`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L132)
- protocol/private: `__init__`[`L130`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L130)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`__init__`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.__init__)
- used by: [`BaseMCPTool`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.validate_arguments)

### `_FakeInner`  ·  implements/extends BaseMCPTool
- def: [`tests/unit/mcp/tools/test_health_facade.py:85`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L85)
- doc: Lightweight BaseMCPTool that records the args it receives.
- signature: `class _FakeInner(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L114`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L114)
  - `get_tool_definition(self)` — [`L103`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L103)
  - `get_tool_schema(self)` — [`L93`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L93)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L106`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L106)
  - `last_args` — [`L90`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L90)
  - `rebound_to` — [`L91`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L91)
- protocol/private: `__init__`[`L88`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L88), `_on_project_root_changed`[`L109`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L109)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`__init__`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.__init__)
- used by: [`BaseMCPTool`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool._on_project_root_changed)

## Functions
- `test_deps_action_no_strict_leak(tmp_path: Any)` — [`L451`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L451) — Route action=deps through the REAL DependencyAnalysisTool.
- `test_deps_action_routes_and_preserves_mode()` — [`L226`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L226) — R5: deps maps to DependencyAnalysisTool; ``mode`` must reach the inner
- `test_deps_mode_blast()` — [`L253`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L253)
- `test_deps_mode_file_deps()` — [`L265`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L265)
- `test_deps_mode_summary()` — [`L243`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L243)
- `test_envelope_preserved_verbatim()` — [`L360`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L360)
- `test_facade_description_mentions_all_actions()` — [`L493`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L493) — Every action name should appear in the description string.
- `test_file_action_routes_and_strips_action_key()` — [`L211`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L211)
- `test_health_facade_annotations_read_only()` — [`L182`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L182) — All health actions are read-only — annotation honesty per spec §6.
- `test_health_facade_builds_and_has_all_actions()` — [`L157`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L157)
- `test_health_facade_does_not_contain_viz_actions()` — [`L174`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L174) — uml/graph/similarity must not appear in health — they live in viz.
- `test_health_facade_factory_returns_facade_tool()` — [`L424`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L424)
- `test_health_facade_total_action_count()` — [`L167`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L167) — 12 actions total — uml/graph/similarity moved to viz; test_gap wired (RFC-0003).
- `test_missing_action_returns_error_envelope()` — [`L383`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L383)
- `test_project_action_no_strict_leak(tmp_path: Any)` — [`L436`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L436) — Route action=project through the REAL ProjectHealthTool. Verify that
- `test_project_action_routes_and_strips_action_key()` — [`L198`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L198) — action=project should not forward ``action`` to the inner.
- `test_r3_explicit_function_name_wins_over_symbol()` — [`L337`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L337)
- `test_r3_normalize_symbol_to_function_name_for_heatmap()` — [`L325`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L325) — heatmap inner (CodeGraphComplexityHeatmapTool) declares ``function_name``.
- `test_schema_lists_action_and_core_params()` — [`L465`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L465) — Wave D slim schema: ``action`` (required) + core shared params only.
- `test_set_project_path_rebinds_all_action_map_inners(tmp_path: Any)` — [`L408`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L408) — G3: set_project_path on the facade must propagate to every action_map inner.
- `test_sibling_param_does_not_reach_project_inner()` — [`L284`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L284) — A param for action=file (file_path) must not leak to project inner.
- `test_sibling_param_does_not_reach_scale_inner()` — [`L301`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L301) — Param for action=dead (include_test_files) must not leak to scale inner.
- `test_unknown_action_returns_error_envelope()` — [`L393`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L393)

## Module values
- `_ALL_ACTIONS` — [`L60`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L60)
- `_VIZ_ACTIONS` — [`L78`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_health_facade.py#L78)

