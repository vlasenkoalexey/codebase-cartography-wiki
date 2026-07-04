---
title: 'Module: src/codegraphcontext/api/mcp_sse.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/api/mcp_sse.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.api.mcp_sse`/
symbols:
  handle_call_tool: handle_call_tool().
  handle_sse: handle_sse().
  mcp_server: mcp_server.
  handle_list_tools: handle_list_tools().
  handle_messages: handle_messages().
  sse: sse.
---
# Module: [`src/codegraphcontext/api/mcp_sse.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/mcp_sse.py)

## Functions
- `handle_call_tool(name: str, arguments: dict | None)` — [`L30`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/mcp_sse.py#L30) — Handle tool execution.
- `handle_list_tools()` — [`L17`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/mcp_sse.py#L17) — List available tools (honors disabledTools from mcp.json).
- `handle_messages(request: Request)` — [`L67`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/mcp_sse.py#L67) — Endpoint for receiving messages from the client.
- `handle_sse(request: Request)` — [`L52`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/mcp_sse.py#L52) — Entry point for the SSE connection.

## Module values
- `mcp_server` — [`L14`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/mcp_sse.py#L14)
- `sse` — [`L50`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/mcp_sse.py#L50)

