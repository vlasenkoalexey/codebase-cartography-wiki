---
title: 'Module: tests/unit/mcp/tools/test_facade_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_facade_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_facade_tool`/
symbols:
  _make_facade: _make_facade().
  test_set_project_path_rebinds_inner_instances: test_set_project_path_rebinds_inner_instances().
  test_facade_schema_does_not_union_inner_only_params: test_facade_schema_does_not_union_inner_only_params().
  test_search_facade_schema_declares_kind_with_enum: test_search_facade_schema_declares_kind_with_enum().
  test_bespoke_route_bypasses_inner_execute: test_bespoke_route_bypasses_inner_execute().
  test_bespoke_handles_int_return: test_bespoke_handles_int_return().
  test_search_facade_builds_and_routes: test_search_facade_builds_and_routes().
  test_arg_projection_strips_action_control_key: test_arg_projection_strips_action_control_key().
  test_arg_projection_drops_sibling_params: test_arg_projection_drops_sibling_params().
  test_symbol_normalized_to_function_name_before_projection: test_symbol_normalized_to_function_name_before_projection().
  test_explicit_function_name_wins_over_symbol: test_explicit_function_name_wins_over_symbol().
  test_symbol_normalized_to_class_name_before_projection: test_symbol_normalized_to_class_name_before_projection().
  test_explicit_class_name_wins_over_symbol: test_explicit_class_name_wins_over_symbol().
  test_facade_schema_lists_action_and_core_params: test_facade_schema_lists_action_and_core_params().
  test_facade_schema_not_strict_additional_properties: test_facade_schema_not_strict_additional_properties().
  _FakeSymbolTool: _FakeSymbolTool#
  test_action_routes_to_inner_tool: test_action_routes_to_inner_tool().
  test_facade_does_not_raise_on_control_keys: test_facade_does_not_raise_on_control_keys().
  test_envelope_preserved_verbatim: test_envelope_preserved_verbatim().
  test_missing_action_returns_error_envelope: test_missing_action_returns_error_envelope().
  test_unknown_action_returns_error_envelope: test_unknown_action_returns_error_envelope().
  test_unknown_action_error_string_enumerates_valid_actions: test_unknown_action_error_string_enumerates_valid_actions().
  test_unknown_action_close_to_valid_suggests_did_you_mean: test_unknown_action_close_to_valid_suggests_did_you_mean().
  test_far_off_unknown_action_has_no_spurious_suggestion: test_far_off_unknown_action_has_no_spurious_suggestion().
  test_search_facade_batch_description_documents_query_item_shape: test_search_facade_batch_description_documents_query_item_shape().
  test_search_facade_symbol_action_does_not_raise_strict: test_search_facade_symbol_action_does_not_raise_strict().
  _FakeFunctionTool: _FakeFunctionTool#
  _FakeClassTool: _FakeClassTool#
  test_facade_schema_does_not_union_inner_only_params._InnerWithBespokeParam: test_facade_schema_does_not_union_inner_only_params()._InnerWithBespokeParam#
  _FakeSymbolTool.rebound_to: _FakeSymbolTool#rebound_to.
  _FakeSymbolTool.__init__: _FakeSymbolTool#__init__().
  _FakeSymbolTool.get_tool_definition: _FakeSymbolTool#get_tool_definition().
  _FakeSymbolTool._on_project_root_changed: _FakeSymbolTool#_on_project_root_changed().
  _FakeSymbolTool.execute: _FakeSymbolTool#execute().
  _FakeFunctionTool.__init__: _FakeFunctionTool#__init__().
  _FakeFunctionTool.get_tool_definition: _FakeFunctionTool#get_tool_definition().
  _FakeFunctionTool.execute: _FakeFunctionTool#execute().
  _FakeClassTool.__init__: _FakeClassTool#__init__().
  _FakeClassTool.get_tool_definition: _FakeClassTool#get_tool_definition().
  _FakeClassTool.execute: _FakeClassTool#execute().
  test_facade_does_not_override_set_project_path: test_facade_does_not_override_set_project_path().
  test_facade_schema_does_not_union_inner_only_params._InnerWithBespokeParam.get_tool_definition: test_facade_schema_does_not_union_inner_only_params()._InnerWithBespokeParam#get_tool_definition().
  _FakeSymbolTool.last_args: _FakeSymbolTool#last_args.
  _FakeSymbolTool.get_tool_schema: _FakeSymbolTool#get_tool_schema().
  _FakeFunctionTool.last_args: _FakeFunctionTool#last_args.
  _FakeFunctionTool.get_tool_schema: _FakeFunctionTool#get_tool_schema().
  _FakeClassTool.last_args: _FakeClassTool#last_args.
  _FakeClassTool.get_tool_schema: _FakeClassTool#get_tool_schema().
  test_bespoke_route_bypasses_inner_execute._bespoke: test_bespoke_route_bypasses_inner_execute()._bespoke().
  test_bespoke_handles_int_return._bespoke: test_bespoke_handles_int_return()._bespoke().
  test_facade_schema_does_not_union_inner_only_params._InnerWithBespokeParam.get_tool_schema: test_facade_schema_does_not_union_inner_only_params()._InnerWithBespokeParam#get_tool_schema().
  _FakeSymbolTool.validate_arguments: _FakeSymbolTool#validate_arguments().
  _FakeFunctionTool.validate_arguments: _FakeFunctionTool#validate_arguments().
  _FakeClassTool.validate_arguments: _FakeClassTool#validate_arguments().
  test_facade_schema_does_not_union_inner_only_params._InnerWithBespokeParam.validate_arguments: test_facade_schema_does_not_union_inner_only_params()._InnerWithBespokeParam#validate_arguments().
  test_facade_schema_does_not_union_inner_only_params._InnerWithBespokeParam.execute: test_facade_schema_does_not_union_inner_only_params()._InnerWithBespokeParam#execute().
---
# Module: [`tests/unit/mcp/tools/test_facade_tool.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py)

## Classes
### `_FakeClassTool`  ·  implements/extends BaseMCPTool
- def: [`tests/unit/mcp/tools/test_facade_tool.py:131`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L131)
- doc: Inner tool that reads `class_name` (mirrors codegraph_class_inspect /
- signature: `class _FakeClassTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L153`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L153)
  - `get_tool_definition(self)` — [`L147`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L147)
  - `get_tool_schema(self)` — [`L139`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L139)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L150`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L150)
  - `last_args` — [`L137`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L137)
- protocol/private: `__init__`[`L135`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L135)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`__init__`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.__init__)
- used by: [`BaseMCPTool`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.validate_arguments)  (1 test-only)

### `_FakeFunctionTool`  ·  implements/extends BaseMCPTool
- def: [`tests/unit/mcp/tools/test_facade_tool.py:105`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L105)
- doc: Inner tool that reads `function_name` (mirrors codegraph_callers).
- signature: `class _FakeFunctionTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L126`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L126)
  - `get_tool_definition(self)` — [`L120`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L120)
  - `get_tool_schema(self)` — [`L112`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L112)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L123`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L123)
  - `last_args` — [`L110`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L110)
- protocol/private: `__init__`[`L108`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L108)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`__init__`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.__init__)
- used by: [`BaseMCPTool`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.validate_arguments)  (1 test-only)

### `_FakeSymbolTool`  ·  implements/extends BaseMCPTool
- def: [`tests/unit/mcp/tools/test_facade_tool.py:57`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L57)
- doc: Inner tool whose schema only allows `query` + `limit`.
- signature: `class _FakeSymbolTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L91`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L91)
  - `get_tool_definition(self)` — [`L80`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L80)
  - `get_tool_schema(self)` — [`L69`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L69)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L83`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L83)
  - `last_args` — [`L66`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L66)
  - `rebound_to` — [`L67`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L67)
- protocol/private: `__init__`[`L64`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L64), `_on_project_root_changed`[`L86`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L86)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`__init__`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.__init__)
- used by: [`BaseMCPTool`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool._on_project_root_changed)  (4 test-only)

### `_InnerWithBespokeParam`  ·  implements/extends BaseMCPTool
- def: [`tests/unit/mcp/tools/test_facade_tool.py:462`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L462)
- signature: `class _InnerWithBespokeParam(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L476`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L476)
  - `get_tool_definition(self)` — [`L470`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L470)
  - `get_tool_schema(self)` — [`L463`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L463)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L473`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L473)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool)
- used by: [`BaseMCPTool`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.validate_arguments)  (1 test-only)

## Functions
- `_bespoke(args: dict[str, Any])` — [`L278`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L278)
- `_bespoke(args: dict[str, Any])` — [`L299`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L299)
- `_make_facade(**kwargs: Any)` — [`L158`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L158)
- `test_action_routes_to_inner_tool()` — [`L175`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L175)
- `test_arg_projection_drops_sibling_params()` — [`L193`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L193) — A param belonging to a sibling action (function_name) must not reach the
- `test_arg_projection_strips_action_control_key()` — [`L182`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L182) — F4 Landmine A: ``action`` must be stripped before forwarding, or the
- `test_bespoke_handles_int_return()` — [`L295`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L295) — F5: search_content/find_and_grep can return a bare int (exit code) when
- `test_bespoke_route_bypasses_inner_execute()` — [`L275`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L275)
- `test_envelope_preserved_verbatim()` — [`L316`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L316)
- `test_explicit_class_name_wins_over_symbol()` — [`L258`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L258)
- `test_explicit_function_name_wins_over_symbol()` — [`L230`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L230)
- `test_facade_does_not_override_set_project_path()` — [`L416`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L416) — FacadeTool must inherit set_project_path from BaseMCPTool, not override
- `test_facade_does_not_raise_on_control_keys()` — [`L205`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L205) — The facade's own strict-param guard must allow action/scope/mode.
- `test_facade_schema_does_not_union_inner_only_params()` — [`L457`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L457) — A param declared ONLY by an inner tool (not a core param) must NOT be
- `test_facade_schema_lists_action_and_core_params()` — [`L427`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L427) — Wave D slim schema: ``action`` + curated core params, NOT a full union.
- `test_facade_schema_not_strict_additional_properties()` — [`L488`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L488) — The facade-level schema must allow control keys; it must NOT be
- `test_far_off_unknown_action_has_no_spurious_suggestion()` — [`L381`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L381) — A far-off action yields no ``did you mean`` hint (no false suggestion),
- `test_missing_action_returns_error_envelope()` — [`L328`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L328)
- `test_search_facade_batch_description_documents_query_item_shape()` — [`L523`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L523) — #569: schema-reading agents must see batch query items use pattern.
- `test_search_facade_builds_and_routes()` — [`L507`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L507)
- `test_search_facade_schema_declares_kind_with_enum()` — [`L560`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L560) — #640: ``kind`` worked at runtime (additionalProperties) but was absent
- `test_search_facade_symbol_action_does_not_raise_strict(tmp_path: Any)` — [`L535`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L535) — End-to-end: routing through the facade to the real symbol_search inner
- `test_set_project_path_rebinds_inner_instances(tmp_path: Any)` — [`L399`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L399) — G3: server.set_project_path loops _tools.values() calling
- `test_symbol_normalized_to_class_name_before_projection()` — [`L250`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L250)
- `test_symbol_normalized_to_function_name_before_projection()` — [`L222`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L222)
- `test_unknown_action_close_to_valid_suggests_did_you_mean()` — [`L362`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L362) — TURN-SAVER: a typo'd action close to a valid one self-heals in-band.
- `test_unknown_action_error_string_enumerates_valid_actions()` — [`L346`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L346) — F4 DX: the bare ``error`` string itself (not just the envelope's
- `test_unknown_action_returns_error_envelope()` — [`L338`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_facade_tool.py#L338)

