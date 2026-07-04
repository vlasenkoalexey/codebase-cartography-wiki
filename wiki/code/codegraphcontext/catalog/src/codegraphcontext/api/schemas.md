---
title: 'Module: src/codegraphcontext/api/schemas.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/api/schemas.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.api.schemas`/
symbols:
  ApiResponse: ApiResponse#
  ApiResponse.status: ApiResponse#status.
  ApiResponse.data: ApiResponse#data.
  ApiResponse.error: ApiResponse#error.
  IndexRequest: IndexRequest#
  QueryRequest: QueryRequest#
  ToolCallRequest: ToolCallRequest#
  ApiResponse.message: ApiResponse#message.
  IndexRequest.path: IndexRequest#path.
  QueryRequest.query: QueryRequest#query.
  QueryRequest.params: QueryRequest#params.
  SearchRequest: SearchRequest#
  ToolCallRequest.name: ToolCallRequest#name.
  ToolCallRequest.arguments: ToolCallRequest#arguments.
  IndexRequest.repo_name: IndexRequest#repo_name.
  IndexRequest.branch: IndexRequest#branch.
  IndexRequest.force: IndexRequest#force.
  SearchRequest.query: SearchRequest#query.
  SearchRequest.top_k: SearchRequest#top_k.
---
# Module: [`src/codegraphcontext/api/schemas.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py)

## Classes
### `ApiResponse`  ·  implements/extends BaseModel
- def: [`src/codegraphcontext/api/schemas.py:23`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py#L23)
- signature: `class ApiResponse(BaseModel):`
- members:
  - `data` — [`L26`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py#L26)
  - `error` — [`L27`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py#L27)
  - `message` — [`L25`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py#L25)
  - `status` — [`L24`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py#L24)
- used by: [`call_tool`](router.md#call_tool), [`execute_query`](router.md#execute_query), [`get_status`](router.md#get_status), [`index_repository`](router.md#index_repository), [`list_repositories`](router.md#list_repositories), [`list_tools`](router.md#list_tools)

### `IndexRequest`  ·  implements/extends BaseModel
- def: [`src/codegraphcontext/api/schemas.py:5`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py#L5)
- signature: `class IndexRequest(BaseModel):`
- members:
  - `branch` — [`L8`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py#L8)
  - `force` — [`L9`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py#L9)
  - `path` — [`L6`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py#L6)
  - `repo_name` — [`L7`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py#L7)
- used by: [`index_repository`](router.md#index_repository)

### `QueryRequest`  ·  implements/extends BaseModel
- def: [`src/codegraphcontext/api/schemas.py:11`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py#L11)
- signature: `class QueryRequest(BaseModel):`
- members:
  - `params` — [`L13`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py#L13)
  - `query` — [`L12`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py#L12)
- used by: [`execute_query`](router.md#execute_query)

### `SearchRequest`  ·  implements/extends BaseModel
- def: [`src/codegraphcontext/api/schemas.py:15`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py#L15)
- signature: `class SearchRequest(BaseModel):`
- members:
  - `query` — [`L16`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py#L16)
  - `top_k` — [`L17`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py#L17)

### `ToolCallRequest`  ·  implements/extends BaseModel
- def: [`src/codegraphcontext/api/schemas.py:19`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py#L19)
- signature: `class ToolCallRequest(BaseModel):`
- members:
  - `arguments` — [`L21`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py#L21)
  - `name` — [`L20`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/api/schemas.py#L20)
- used by: [`call_tool`](router.md#call_tool)

