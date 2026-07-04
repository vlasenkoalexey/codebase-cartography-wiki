---
title: 'Module: tests/unit/tools/test_kuzu_relationship_queries.py'
type: catalog
provenance: extracted
module: tests/unit/tools/test_kuzu_relationship_queries.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.tools.test_kuzu_relationship_queries`/
symbols:
  _make_finder: _make_finder().
  _FakeSession.run: _FakeSession#run().
  _FakeDriver.session: _FakeDriver#session().
  _FakeDBManager.get_driver: _FakeDBManager#get_driver().
  test_find_all_callers_avoids_list_extract: test_find_all_callers_avoids_list_extract().
  test_find_all_callees_avoids_list_extract: test_find_all_callees_avoids_list_extract().
  test_call_chain_avoids_list_extract: test_call_chain_avoids_list_extract().
  _FakeSession._recorder: _FakeSession#_recorder.
  _FakeResult: _FakeResult#
  _FakeSession: _FakeSession#
  _FakeDriver: _FakeDriver#
  _FakeDriver._recorder: _FakeDriver#_recorder.
  _FakeDBManager: _FakeDBManager#
  _FakeDBManager._recorder: _FakeDBManager#_recorder.
  _FakeResult.data: _FakeResult#data().
  _FakeSession.__init__: _FakeSession#__init__().
  _FakeSession.__enter__: _FakeSession#__enter__().
  _FakeSession.__exit__: _FakeSession#__exit__().
  _FakeDriver.__init__: _FakeDriver#__init__().
  _FakeDBManager.__init__: _FakeDBManager#__init__().
  _FakeDBManager.get_backend_type: _FakeDBManager#get_backend_type().
---
# Module: [`tests/unit/tools/test_kuzu_relationship_queries.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py)

## Classes
### `_FakeDBManager`
- def: [`tests/unit/tools/test_kuzu_relationship_queries.py:30`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L30)
- signature: `class _FakeDBManager:`
- members:
  - `get_backend_type(self)` — [`L38`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L38)
  - `get_driver(self)` — [`L34`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L34)
- protocol/private: `__init__`[`L31`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L31), `_recorder`[`L32`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L32)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `_FakeDriver`
- def: [`tests/unit/tools/test_kuzu_relationship_queries.py:23`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L23)
- signature: `class _FakeDriver:`
- members:
  - `session(self)` — [`L27`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L27)
- protocol/private: `__init__`[`L24`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L24), `_recorder`[`L25`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L25)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `_FakeResult`
- def: [`tests/unit/tools/test_kuzu_relationship_queries.py:4`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L4)
- signature: `class _FakeResult:`
- members:
  - `data(self)` — [`L5`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L5)
- used by: (1 test-only callers)

### `_FakeSession`
- def: [`tests/unit/tools/test_kuzu_relationship_queries.py:8`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L8)
- signature: `class _FakeSession:`
- members:
  - `run(self, query: str, **kwargs: Any)` — [`L12`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L12)
- protocol/private: `__enter__`[`L17`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L17), `__exit__`[`L20`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L20), `__init__`[`L9`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L9), `_recorder`[`L10`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L10)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

## Functions
- `_make_finder(recorder: Optional[Dict[str, Any]] = None)` — [`L41`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L41)
- `test_call_chain_avoids_list_extract()` — [`L64`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L64)
- `test_find_all_callees_avoids_list_extract()` — [`L56`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L56)
- `test_find_all_callers_avoids_list_extract()` — [`L48`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_relationship_queries.py#L48)

