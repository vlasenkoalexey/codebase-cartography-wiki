---
title: 'Module: tests/unit/mcp/tools/test_viz_facade.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_viz_facade.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_viz_facade`/
symbols:
  test_viz_facade_builds_and_has_all_actions: test_viz_facade_builds_and_has_all_actions().
  test_set_project_path_rebinds_all_action_map_inners: test_set_project_path_rebinds_all_action_map_inners().
  test_viz_facade_total_action_count: test_viz_facade_total_action_count().
  test_uml_action_routes_and_strips_action_key: test_uml_action_routes_and_strips_action_key().
  test_graph_action_routes_and_strips_action_key: test_graph_action_routes_and_strips_action_key().
  test_similarity_action_routes_and_strips_action_key: test_similarity_action_routes_and_strips_action_key().
  test_sibling_param_does_not_reach_uml_inner: test_sibling_param_does_not_reach_uml_inner().
  test_sibling_param_does_not_reach_similarity_inner: test_sibling_param_does_not_reach_similarity_inner().
  test_envelope_preserved_verbatim: test_envelope_preserved_verbatim().
  test_missing_action_returns_error_envelope: test_missing_action_returns_error_envelope().
  test_schema_lists_action_as_required_with_all_actions: test_schema_lists_action_as_required_with_all_actions().
  test_facade_description_mentions_all_actions: test_facade_description_mentions_all_actions().
  _ALL_ACTIONS: _ALL_ACTIONS.
  test_viz_facade_annotations_read_only: test_viz_facade_annotations_read_only().
  test_unknown_action_returns_error_envelope: test_unknown_action_returns_error_envelope().
  test_viz_facade_factory_returns_facade_tool: test_viz_facade_factory_returns_facade_tool().
  _FakeInner: _FakeInner#
  _FakeInner.__init__: _FakeInner#__init__().
  _FakeInner.get_tool_definition: _FakeInner#get_tool_definition().
  _FakeInner._on_project_root_changed: _FakeInner#_on_project_root_changed().
  _FakeInner.execute: _FakeInner#execute().
  _FakeInner.last_args: _FakeInner#last_args.
  _FakeInner.rebound_to: _FakeInner#rebound_to.
  _FakeInner.get_tool_schema: _FakeInner#get_tool_schema().
  _FakeInner.validate_arguments: _FakeInner#validate_arguments().
---
# Module: [`tests/unit/mcp/tools/test_viz_facade.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py)

## Classes
### `_FakeInner`  ·  implements/extends BaseMCPTool
- def: [`tests/unit/mcp/tools/test_viz_facade.py:57`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L57)
- doc: Lightweight BaseMCPTool that records the args it receives.
- signature: `class _FakeInner(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L85`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L85)
  - `get_tool_definition(self)` — [`L75`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L75)
  - `get_tool_schema(self)` — [`L65`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L65)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L78`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L78)
  - `last_args` — [`L62`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L62)
  - `rebound_to` — [`L63`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L63)
- protocol/private: `__init__`[`L60`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L60), `_on_project_root_changed`[`L81`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L81)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`__init__`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.__init__)
- used by: [`BaseMCPTool`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool._on_project_root_changed)

## Functions
- `test_envelope_preserved_verbatim()` — [`L224`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L224)
- `test_facade_description_mentions_all_actions()` — [`L314`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L314) — Every action name should appear in the description string.
- `test_graph_action_routes_and_strips_action_key()` — [`L151`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L151) — action=graph should not forward ``action`` to the inner.
- `test_missing_action_returns_error_envelope()` — [`L247`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L247)
- `test_schema_lists_action_as_required_with_all_actions()` — [`L300`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L300) — Facade schema must list ``action`` as required with the 3 viz actions.
- `test_set_project_path_rebinds_all_action_map_inners(tmp_path: Any)` — [`L272`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L272) — G3: set_project_path on the facade must propagate to every action_map inner.
- `test_sibling_param_does_not_reach_similarity_inner()` — [`L204`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L204) — Param for action=uml (source) must not leak to similarity inner.
- `test_sibling_param_does_not_reach_uml_inner()` — [`L191`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L191) — Param for action=graph (depth) must not leak to uml inner.
- `test_similarity_action_routes_and_strips_action_key()` — [`L172`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L172) — action=similarity should not forward ``action`` to the inner.
- `test_uml_action_routes_and_strips_action_key()` — [`L136`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L136) — action=uml should not forward ``action`` to the inner.
- `test_unknown_action_returns_error_envelope()` — [`L257`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L257)
- `test_viz_facade_annotations_read_only()` — [`L120`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L120) — All viz actions are read-only — pure generation/analysis, no mutations.
- `test_viz_facade_builds_and_has_all_actions()` — [`L103`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L103)
- `test_viz_facade_factory_returns_facade_tool()` — [`L288`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L288)
- `test_viz_facade_total_action_count()` — [`L113`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L113) — 4 actions total: uml, graph, similarity, knowledge.

## Module values
- `_ALL_ACTIONS` — [`L50`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_viz_facade.py#L50)

