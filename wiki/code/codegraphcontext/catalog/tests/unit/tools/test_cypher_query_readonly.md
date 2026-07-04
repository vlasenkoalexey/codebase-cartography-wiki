---
title: 'Module: tests/unit/tools/test_cypher_query_readonly.py'
type: catalog
provenance: extracted
module: tests/unit/tools/test_cypher_query_readonly.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.tools.test_cypher_query_readonly`/
symbols:
  tests: tests.
  e: e.
  t: t.
  _FakeSession.run: _FakeSession#run().
  _run_system: _run_system().
  _run_handler: _run_handler().
  _FakeDriver.session: _FakeDriver#session().
  _FakeDBManager.get_driver: _FakeDBManager#get_driver().
  failures: failures.
  test_handler_blocks_load_csv: test_handler_blocks_load_csv().
  test_handler_blocks_foreach_set: test_handler_blocks_foreach_set().
  test_handler_uses_read_only_session: test_handler_uses_read_only_session().
  test_system_blocks_call_apoc: test_system_blocks_call_apoc().
  test_system_blocks_load_csv: test_system_blocks_load_csv().
  test_system_uses_read_only_session: test_system_uses_read_only_session().
  test_system_no_false_positive_on_asset: test_system_no_false_positive_on_asset().
  _FakeSession._recorder: _FakeSession#_recorder.
  _FakeResult.__iter__: _FakeResult#__iter__().
  _FakeDriver._recorder: _FakeDriver#_recorder.
  _FakeDBManager: _FakeDBManager#
  _FakeResult: _FakeResult#
  _FakeResult._records: _FakeResult#_records.
  _FakeSession: _FakeSession#
  _FakeSession._access_mode: _FakeSession#_access_mode.
  _FakeDriver: _FakeDriver#
  _FakeDBManager._recorder: _FakeDBManager#_recorder.
  _FakeResult.__init__: _FakeResult#__init__().
  _FakeResult.data: _FakeResult#data().
  _FakeSession.__init__: _FakeSession#__init__().
  _FakeSession.__enter__: _FakeSession#__enter__().
  _FakeSession.__exit__: _FakeSession#__exit__().
  _FakeDriver.__init__: _FakeDriver#__init__().
  _FakeDBManager.__init__: _FakeDBManager#__init__().
---
# Module: [`tests/unit/tools/test_cypher_query_readonly.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py)

## Classes
### `_FakeDBManager`
- def: [`tests/unit/tools/test_cypher_query_readonly.py:60`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L60)
- doc: Simulates DatabaseManager.
- signature: `class _FakeDBManager:`
- members:
  - `get_driver(self)` — [`L65`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L65)
- protocol/private: `__init__`[`L62`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L62), `_recorder`[`L63`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L63)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `_FakeDriver`
- def: [`tests/unit/tools/test_cypher_query_readonly.py:49`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L49)
- doc: Simulates the Neo4jDriverWrapper.
- signature: `class _FakeDriver:`
- members:
  - `session(self, **kwargs)` — [`L54`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L54)
- protocol/private: `__init__`[`L51`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L51), `_recorder`[`L52`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L52)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `_FakeResult`
- def: [`tests/unit/tools/test_cypher_query_readonly.py:18`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L18)
- doc: Simulates a Neo4j result set.
- signature: `class _FakeResult:`
- members:
  - `data(self)` — [`L23`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L23)
- protocol/private: `__init__`[`L20`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L20), `__iter__`[`L26`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L26), `_records`[`L21`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L21)
- used by: (1 test-only callers)

### `_FakeSession`
- def: [`tests/unit/tools/test_cypher_query_readonly.py:30`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L30)
- doc: Simulates a Neo4j session, recording calls.
- signature: `class _FakeSession:`
- members:
  - `run(self, query, **kwargs)` — [`L36`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L36)
- protocol/private: `__enter__`[`L42`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L42), `__exit__`[`L45`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L45), `__init__`[`L32`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L32), `_access_mode`[`L34`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L34), `_recorder`[`L33`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L33)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

## Functions
- `_run_handler(cypher_query, recorder)` — [`L71`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L71)
- `_run_system(cypher_query, recorder)` — [`L107`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L107)
- `test_handler_blocks_foreach_set()` — [`L88`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L88)
- `test_handler_blocks_load_csv()` — [`L77`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L77)
- `test_handler_uses_read_only_session()` — [`L97`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L97)
- `test_system_blocks_call_apoc()` — [`L115`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L115)
- `test_system_blocks_load_csv()` — [`L126`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L126)
- `test_system_no_false_positive_on_asset()` — [`L145`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L145)
- `test_system_uses_read_only_session()` — [`L137`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L137)

## Module values
- `e` — [`L169`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L169)
- `failures` — [`L164`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L164)
- `t` — [`L165`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L165)
- `tests` — [`L155`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cypher_query_readonly.py#L155)

