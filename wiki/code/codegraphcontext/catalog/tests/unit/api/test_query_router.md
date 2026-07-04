---
title: 'Module: tests/unit/api/test_query_router.py'
type: catalog
provenance: extracted
module: tests/unit/api/test_query_router.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.api.test_query_router`/
symbols:
  test_execute_query_passes_cypher_query_argument: test_execute_query_passes_cypher_query_argument().
  FakeServer.handle_tool_call: FakeServer#handle_tool_call().
  test_execute_query_returns_503_when_database_unavailable: test_execute_query_returns_503_when_database_unavailable().
  FakeServer.tool_name: FakeServer#tool_name.
  FakeServer.arguments: FakeServer#arguments.
  FakeServer: FakeServer#
  FailingServer: FailingServer#
  FakeServer.__init__: FakeServer#__init__().
  FailingServer.handle_tool_call: FailingServer#handle_tool_call().
---
# Module: [`tests/unit/api/test_query_router.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/api/test_query_router.py)

## Classes
### `FailingServer`
- def: [`tests/unit/api/test_query_router.py:46`](../../../../../../../raw/code/codegraphcontext/tests/unit/api/test_query_router.py#L46)
- signature: `class FailingServer:`
- members:
  - `handle_tool_call(self, tool_name, arguments)` — [`L47`](../../../../../../../raw/code/codegraphcontext/tests/unit/api/test_query_router.py#L47)
- used by: (1 test-only callers)

### `FakeServer`
- def: [`tests/unit/api/test_query_router.py:12`](../../../../../../../raw/code/codegraphcontext/tests/unit/api/test_query_router.py#L12)
- signature: `class FakeServer:`
- members:
  - `handle_tool_call(self, tool_name, arguments)` — [`L17`](../../../../../../../raw/code/codegraphcontext/tests/unit/api/test_query_router.py#L17)
  - `arguments` — [`L15`](../../../../../../../raw/code/codegraphcontext/tests/unit/api/test_query_router.py#L15)
  - `tool_name` — [`L14`](../../../../../../../raw/code/codegraphcontext/tests/unit/api/test_query_router.py#L14)
- protocol/private: `__init__`[`L13`](../../../../../../../raw/code/codegraphcontext/tests/unit/api/test_query_router.py#L13)
- used by: (1 test-only callers)

## Functions
- `test_execute_query_passes_cypher_query_argument(monkeypatch)` — [`L23`](../../../../../../../raw/code/codegraphcontext/tests/unit/api/test_query_router.py#L23)
- `test_execute_query_returns_503_when_database_unavailable(monkeypatch)` — [`L51`](../../../../../../../raw/code/codegraphcontext/tests/unit/api/test_query_router.py#L51)

