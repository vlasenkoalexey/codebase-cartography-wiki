---
title: 'Module: src/codegraphcontext/api/router.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/api/router.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.api.router`/
symbols:
  call_tool: call_tool().
  execute_query: execute_query().
  get_status: get_status().
  index_repository: index_repository().
  list_repositories: list_repositories().
  list_tools: list_tools().
  get_server: get_server().
  router: router.
  _server_instance._server_instance: _server_instance._server_instance.
  raise_service_unavailable: raise_service_unavailable().
---
# Module: [`src/codegraphcontext/api/router.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/router.py)

## Functions
- `call_tool(request: ToolCallRequest, server: MCPServer = Depends(get_server))` — [`L57`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/router.py#L57) — documented in [codegraphcontext-server](../../../../concepts/codegraphcontext-server.md)
- `execute_query(request: QueryRequest, server: MCPServer = Depends(get_server))` — [`L119`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/router.py#L119) — documented in [codegraphcontext-server](../../../../concepts/codegraphcontext-server.md)
- `get_server()` — [`L23`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/router.py#L23)
- `get_status(server: MCPServer = Depends(get_server))` — [`L37`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/router.py#L37) — documented in [codegraphcontext-server](../../../../concepts/codegraphcontext-server.md)
- `index_repository(request: IndexRequest, background_tasks: BackgroundTasks, server: MCPServer = Depends(get_server))` — [`L89`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/router.py#L89) — documented in [codegraphcontext-server](../../../../concepts/codegraphcontext-server.md)
- `list_repositories(server: MCPServer = Depends(get_server))` — [`L140`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/router.py#L140) — documented in [codegraphcontext-server](../../../../concepts/codegraphcontext-server.md)
- `list_tools(server: MCPServer = Depends(get_server))` — [`L50`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/router.py#L50)
- `raise_service_unavailable(exc: Exception)` — [`L30`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/router.py#L30)

## Module values
- `_server_instance` — [`L21`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/router.py#L21)
- `router` — [`L18`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/router.py#L18)

