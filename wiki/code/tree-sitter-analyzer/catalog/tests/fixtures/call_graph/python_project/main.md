---
title: 'Module: tests/fixtures/call_graph/python_project/main.py'
type: catalog
provenance: extracted
module: tests/fixtures/call_graph/python_project/main.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.fixtures.call_graph.python_project.main`/
symbols:
  main: main().
  run: run().
  UserService.get_user: UserService#get_user().
  UserService._fetch: UserService#_fetch().
  UserService: UserService#
  UserService.delete_user: UserService#delete_user().
  farewell: farewell().
---
# Module: [`tests/fixtures/call_graph/python_project/main.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/call_graph/python_project/main.py)

## Classes
### `UserService`
- def: [`tests/fixtures/call_graph/python_project/main.py:16`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/call_graph/python_project/main.py#L16)
- signature: `class UserService:`
- members:
  - `delete_user(self, uid)` — [`L20`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/call_graph/python_project/main.py#L20)
  - `get_user(self, uid)` — [`L17`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/call_graph/python_project/main.py#L17)
- protocol/private: `_fetch`[`L23`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/call_graph/python_project/main.py#L23)

## Functions
- `farewell()` — [`L27`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/call_graph/python_project/main.py#L27)
- `main()` — [`L5`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/call_graph/python_project/main.py#L5)
- `run()` — [`L12`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/call_graph/python_project/main.py#L12)

