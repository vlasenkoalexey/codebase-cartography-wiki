---
title: 'Module: tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.hyphae_subscribe_tool`/
symbols:
  HyphaeSubscribeTool.execute: HyphaeSubscribeTool#execute().
  HyphaeUnsubscribeTool.execute: HyphaeUnsubscribeTool#execute().
  _SESSION_SESSIONS._SESSION_SESSIONS: _SESSION_SESSIONS._SESSION_SESSIONS.
  get_session_loop: get_session_loop().
  get_session_obj: get_session_obj().
  _SESSION_LOOPS._SESSION_LOOPS: _SESSION_LOOPS._SESSION_LOOPS.
  HyphaeSubscribeTool: HyphaeSubscribeTool#
  HyphaeUnsubscribeTool: HyphaeUnsubscribeTool#
  _selector_to_uri: _selector_to_uri().
  _RESOURCE_SCHEME: _RESOURCE_SCHEME.
  _SESSION_MIN_INTERVALS._SESSION_MIN_INTERVALS: _SESSION_MIN_INTERVALS._SESSION_MIN_INTERVALS.
  _uri_to_selector: _uri_to_selector().
  HyphaeSubscribeTool.get_tool_definition: HyphaeSubscribeTool#get_tool_definition().
  HyphaeUnsubscribeTool.get_tool_definition: HyphaeUnsubscribeTool#get_tool_definition().
  get_session_min_interval: get_session_min_interval().
  _capture_session_id: _capture_session_id().
  _capture_session_obj: _capture_session_obj().
  HyphaeSubscribeTool.get_tool_schema: HyphaeSubscribeTool#get_tool_schema().
  HyphaeSubscribeTool.validate_arguments: HyphaeSubscribeTool#validate_arguments().
  HyphaeUnsubscribeTool.get_tool_schema: HyphaeUnsubscribeTool#get_tool_schema().
  HyphaeUnsubscribeTool.validate_arguments: HyphaeUnsubscribeTool#validate_arguments().
---
# Module: [`tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py)

## Classes
### `HyphaeSubscribeTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py:38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L38)
- doc: `search action=subscribe`: register a Hyphae selector for push updates.
- signature: `class HyphaeSubscribeTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L81)
  - `get_tool_definition(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L45)
  - `get_tool_schema(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L58)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L76)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`build_response`](_response_builder.md#build_response), [`subscribe`](../subscription_registry.md#SubscriptionRegistry.subscribe), [`get_subscription_registry`](../../_singleton_registry.md#get_subscription_registry), [`_SESSION_SESSIONS`](hyphae_subscribe_tool.md#_SESSION_SESSIONS._SESSION_SESSIONS), [`_SESSION_LOOPS`](hyphae_subscribe_tool.md#_SESSION_LOOPS._SESSION_LOOPS), [`_selector_to_uri`](hyphae_subscribe_tool.md#_selector_to_uri), [`_SESSION_MIN_INTERVALS`](hyphae_subscribe_tool.md#_SESSION_MIN_INTERVALS._SESSION_MIN_INTERVALS), [`_capture_session_id`](hyphae_subscribe_tool.md#_capture_session_id), [`_capture_session_obj`](hyphae_subscribe_tool.md#_capture_session_obj)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_search_facade`](search_facade.md#build_search_facade)

### `HyphaeUnsubscribeTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py:115`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L115)
- doc: `search action=unsubscribe`: cancel a Hyphae subscription.
- signature: `class HyphaeUnsubscribeTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L143)
  - `get_tool_definition(self)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L118)
  - `get_tool_schema(self)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L125)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L138)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`build_response`](_response_builder.md#build_response), [`get_subscription_registry`](../../_singleton_registry.md#get_subscription_registry), [`remove_session`](../subscription_registry.md#SubscriptionRegistry.remove_session), [`_SESSION_SESSIONS`](hyphae_subscribe_tool.md#_SESSION_SESSIONS._SESSION_SESSIONS), [`unsubscribe`](../subscription_registry.md#SubscriptionRegistry.unsubscribe), [`_SESSION_LOOPS`](hyphae_subscribe_tool.md#_SESSION_LOOPS._SESSION_LOOPS), [`_SESSION_MIN_INTERVALS`](hyphae_subscribe_tool.md#_SESSION_MIN_INTERVALS._SESSION_MIN_INTERVALS), [`_capture_session_id`](hyphae_subscribe_tool.md#_capture_session_id)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_search_facade`](search_facade.md#build_search_facade)

## Functions
- `_capture_session_id()` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L180) — Return a stable session identifier for the current MCP request.
- `_capture_session_obj()` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L196) — Capture the MCP ServerSession from the current request context.
- `_selector_to_uri(selector: str)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L28)
- `_uri_to_selector(uri: str)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L32)
- `get_session_loop(session_id: str)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L214) — Return the captured event loop for *session_id*, or None.
- `get_session_min_interval(session_id: str)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L224) — Return the min_interval_s for *session_id* (default 2.0).
- `get_session_obj(session_id: str)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L219) — Return the captured MCP ServerSession for *session_id*, or None.

## Module values
- `_RESOURCE_SCHEME` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L25)
- `_SESSION_LOOPS` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L173)
- `_SESSION_MIN_INTERVALS` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L175)
- `_SESSION_SESSIONS` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.py#L177)

