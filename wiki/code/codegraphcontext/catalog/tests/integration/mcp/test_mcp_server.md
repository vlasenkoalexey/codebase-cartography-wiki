---
title: 'Module: tests/integration/mcp/test_mcp_server.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_mcp_server.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.integration.mcp.test_mcp_server`/TestMCPServer#
symbols:
  TestMCPServer.run_test: run_test().
  TestMCPServer.test_tool_routing: test_tool_routing().
  TestMCPServer.test_unknown_tool: test_unknown_tool().
  TestMCPServer.test_add_code_to_graph_routing: test_add_code_to_graph_routing().
  TestMCPServer.test_disabled_tool_call_returns_unknown_tool: test_disabled_tool_call_returns_unknown_tool().
  TestMCPServer: ''
  TestMCPServer.mock_server: mock_server().
  TestMCPServer.test_tools_list_omits_disabled_tools_from_mcp_json: test_tools_list_omits_disabled_tools_from_mcp_json().
---
# Module: [`tests/integration/mcp/test_mcp_server.py`](../../../../../../../raw/code/codegraphcontext/tests/integration/mcp/test_mcp_server.py)

## Classes
### `TestMCPServer`
- def: [`tests/integration/mcp/test_mcp_server.py:8`](../../../../../../../raw/code/codegraphcontext/tests/integration/mcp/test_mcp_server.py#L8)
- doc: Integration tests for the MCP Server.
- signature: `class TestMCPServer:`
- members:
  - `mock_server(self)` — [`L15`](../../../../../../../raw/code/codegraphcontext/tests/integration/mcp/test_mcp_server.py#L15)
  - `run_test()` — [`L34`](../../../../../../../raw/code/codegraphcontext/tests/integration/mcp/test_mcp_server.py#L34)
  - `test_add_code_to_graph_routing(self, mock_server)` — [`L56`](../../../../../../../raw/code/codegraphcontext/tests/integration/mcp/test_mcp_server.py#L56) — Verify routing for complex tools.
  - `test_disabled_tool_call_returns_unknown_tool(self, tmp_path)` — [`L110`](../../../../../../../raw/code/codegraphcontext/tests/integration/mcp/test_mcp_server.py#L110) — Disabled tools should not be executable even if invoked explicitly.
  - `test_tool_routing(self, mock_server)` — [`L32`](../../../../../../../raw/code/codegraphcontext/tests/integration/mcp/test_mcp_server.py#L32) — Test that handle_tool_call routes to the correct internal method.
  - `test_tools_list_omits_disabled_tools_from_mcp_json(self, tmp_path)` — [`L74`](../../../../../../../raw/code/codegraphcontext/tests/integration/mcp/test_mcp_server.py#L74) — Tools listed by the server should exclude mcp.json disabledTools entries.
  - `test_unknown_tool(self, mock_server)` — [`L47`](../../../../../../../raw/code/codegraphcontext/tests/integration/mcp/test_mcp_server.py#L47) — Test unknown tool returns error.

