---
title: 'Module: tests/unit/mcp/test_facade_envelope_contract.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_facade_envelope_contract.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_facade_envelope_contract`/
symbols:
  BUILD_FNS: BUILD_FNS.
  FakeInnerTool.execute: FakeInnerTool#execute().
  test_arg_projection_strips_action: test_arg_projection_strips_action().
  test_envelope_preserved: test_envelope_preserved().
  FakeInnerTool: FakeInnerTool#
  _build_with_fake_inner: _build_with_fake_inner().
  FakeInnerTool.last_args: FakeInnerTool#last_args.
  FakeInnerTool._agent_summary: FakeInnerTool#_agent_summary.
  _FIRST_VALID_ACTION._FIRST_VALID_ACTION: _FIRST_VALID_ACTION._FIRST_VALID_ACTION.
  FakeInnerTool.get_tool_definition: FakeInnerTool#get_tool_definition().
  test_missing_action_returns_error_envelope: test_missing_action_returns_error_envelope().
  test_unknown_action_returns_error_envelope: test_unknown_action_returns_error_envelope().
  FakeInnerTool._verdict: FakeInnerTool#_verdict.
  FakeInnerTool.call_count: FakeInnerTool#call_count.
  FakeInnerTool.get_tool_schema: FakeInnerTool#get_tool_schema().
  FakeInnerTool.__init__: FakeInnerTool#__init__().
  FakeInnerTool.validate_arguments: FakeInnerTool#validate_arguments().
---
# Module: [`tests/unit/mcp/test_facade_envelope_contract.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_facade_envelope_contract.py)

## Classes
### `FakeInnerTool`  ·  implements/extends BaseMCPTool
- def: [`tests/unit/mcp/test_facade_envelope_contract.py:43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_facade_envelope_contract.py#L43)
- doc: Minimal inner tool that records calls and returns a configurable envelope.
- signature: `class FakeInnerTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_facade_envelope_contract.py#L85)
  - `get_tool_definition(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_facade_envelope_contract.py#L79)
  - `get_tool_schema(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_facade_envelope_contract.py#L64)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_facade_envelope_contract.py#L82)
  - `call_count` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_facade_envelope_contract.py#L62)
  - `last_args` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_facade_envelope_contract.py#L61)
- protocol/private: `__init__`[`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_facade_envelope_contract.py#L52), `_agent_summary`[`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_facade_envelope_contract.py#L59), `_verdict`[`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_facade_envelope_contract.py#L58)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`__init__`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.__init__)
- used by: [`BaseMCPTool`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.validate_arguments)  (3 test-only)

## Functions
- `_build_with_fake_inner(build_fn: Any)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_facade_envelope_contract.py#L126) — Build a real facade and inject a FakeInnerTool into its action_map.
- `test_arg_projection_strips_action(build_fn: Any)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_facade_envelope_contract.py#L184) — The 'action' key must NOT reach the inner tool (REQ-M-002b / F4).
- `test_envelope_preserved(build_fn: Any)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_facade_envelope_contract.py#L154) — verdict and agent_summary pass through the facade verbatim (REQ-M-002a).
- `test_missing_action_returns_error_envelope(build_fn: Any)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_facade_envelope_contract.py#L212) — Call with no action key returns success=False, verdict ERROR or NOT_FOUND (REQ-M-002c).
- `test_unknown_action_returns_error_envelope(build_fn: Any)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_facade_envelope_contract.py#L237) — Unregistered action returns success=False and lists available_actions (REQ-M-002d).

## Module values
- `BUILD_FNS` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_facade_envelope_contract.py#L114)
- `_FIRST_VALID_ACTION` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_facade_envelope_contract.py#L103)

