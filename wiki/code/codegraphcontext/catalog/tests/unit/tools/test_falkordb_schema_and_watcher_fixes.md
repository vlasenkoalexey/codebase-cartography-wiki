---
title: 'Module: tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py'
type: catalog
provenance: extracted
module: tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.tools.test_falkordb_schema_and_watcher_fixes`/
symbols:
  TestCreateGraphSchemaFalkorDB._run_schema: TestCreateGraphSchemaFalkorDB#_run_schema().
  TestUpdateFileInGraphGenericFiles._make_graph_builder_stub: TestUpdateFileInGraphGenericFiles#_make_graph_builder_stub().
  TestUpdateFileInGraphGenericFiles.test_all_generic_extensions_reach_minimal_node: TestUpdateFileInGraphGenericFiles#test_all_generic_extensions_reach_minimal_node().
  _RecordingSession: _RecordingSession#
  _RecordingSession.run: _RecordingSession#run().
  _FakeDriver.__init__: _FakeDriver#__init__().
  _FakeDriver.session: _FakeDriver#session().
  TestCreateGraphSchemaFalkorDB.test_embedded_falkordb_sends_no_create_constraint: TestCreateGraphSchemaFalkorDB#test_embedded_falkordb_sends_no_create_constraint().
  TestCreateGraphSchemaFalkorDB.test_remote_falkordb_sends_no_create_constraint: TestCreateGraphSchemaFalkorDB#test_remote_falkordb_sends_no_create_constraint().
  TestCreateGraphSchemaFalkorDB.test_neo4j_sends_create_constraint: TestCreateGraphSchemaFalkorDB#test_neo4j_sends_create_constraint().
  TestCreateGraphSchemaFalkorDB.test_embedded_falkordb_still_sends_create_index: TestCreateGraphSchemaFalkorDB#test_embedded_falkordb_still_sends_create_index().
  TestCreateGraphSchemaFalkorDB.test_remote_falkordb_still_sends_create_index: TestCreateGraphSchemaFalkorDB#test_remote_falkordb_still_sends_create_index().
  TestUpdateFileInGraphGenericFiles.test_generic_file_calls_add_minimal_file_node: TestUpdateFileInGraphGenericFiles#test_generic_file_calls_add_minimal_file_node().
  TestUpdateFileInGraphGenericFiles.test_unsupported_file_is_still_skipped: TestUpdateFileInGraphGenericFiles#test_unsupported_file_is_still_skipped().
  TestUpdateFileInGraphGenericFiles.test_code_file_calls_add_file_to_graph: TestUpdateFileInGraphGenericFiles#test_code_file_calls_add_file_to_graph().
  TestUpdateFileInGraphGenericFiles.test_deleted_file_returns_deleted_sentinel: TestUpdateFileInGraphGenericFiles#test_deleted_file_returns_deleted_sentinel().
  _RecordingSession.queries: _RecordingSession#queries.
  _FakeDriver: _FakeDriver#
  _FakeDriver._session: _FakeDriver#_session.
  _make_db_manager: _make_db_manager().
  TestUpdateFileInGraphGenericFiles._generic_extensions_sample: TestUpdateFileInGraphGenericFiles#_generic_extensions_sample().
  _RecordingSession.__init__: _RecordingSession#__init__().
  _RecordingSession.__enter__: _RecordingSession#__enter__().
  _RecordingSession.__exit__: _RecordingSession#__exit__().
  TestCreateGraphSchemaFalkorDB: TestCreateGraphSchemaFalkorDB#
  TestUpdateFileInGraphGenericFiles: TestUpdateFileInGraphGenericFiles#
---
# Module: [`tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py)

## Classes
### `TestCreateGraphSchemaFalkorDB`
- def: [`tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py:62`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L62)
- signature: `class TestCreateGraphSchemaFalkorDB:`
- members:
  - `test_embedded_falkordb_sends_no_create_constraint(self)` — [`L73`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L73) — Backend 'falkordb' (embedded Lite) must not receive CREATE CONSTRAINT.
  - `test_embedded_falkordb_still_sends_create_index(self)` — [`L100`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L100) — Indices are always sent — they are what makes MERGE deduplication work.
  - `test_neo4j_sends_create_constraint(self)` — [`L94`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L94) — Neo4j backend must still receive CREATE CONSTRAINT statements.
  - `test_remote_falkordb_sends_no_create_constraint(self)` — [`L81`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L81) — Backend 'falkordb-remote' must not receive CREATE CONSTRAINT.
  - `test_remote_falkordb_still_sends_create_index(self)` — [`L106`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L106) — Indices are always sent for 'falkordb-remote' too.
- protocol/private: `_run_schema`[`L64`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L64)
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `TestUpdateFileInGraphGenericFiles`
- def: [`tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py:117`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L117)
- doc: update_file_in_graph is the watcher's incremental update path.
- signature: `class TestUpdateFileInGraphGenericFiles:`
- members:
  - `_make_graph_builder_stub(self)` — [`L125`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L125) — Build a minimal GraphBuilder stub with the real update_file_in_graph method.
  - `test_all_generic_extensions_reach_minimal_node(self, tmp_path)` — [`L222`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L222) — Parametric check: every generic extension must reach add_minimal_file_node.
  - `test_code_file_calls_add_file_to_graph(self, tmp_path)` — [`L181`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L181) — A parseable code file must still go through add_file_to_graph (not minimal).
  - `test_deleted_file_returns_deleted_sentinel(self, tmp_path)` — [`L201`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L201) — A file that no longer exists on disk must return the deleted sentinel.
  - `test_generic_file_calls_add_minimal_file_node(self, tmp_path)` — [`L141`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L141) — A .md file must trigger add_minimal_file_node, not be silently dropped.
  - `test_unsupported_file_is_still_skipped(self, tmp_path)` — [`L161`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L161) — A truly unsupported extension (unsupported=True) must NOT call add_minimal_file_node.
- protocol/private: `_generic_extensions_sample`[`L219`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L219)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `_FakeDriver`
- def: [`tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py:44`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L44)
- signature: `class _FakeDriver:`
- members:
  - `session(self)` — [`L48`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L48)
- protocol/private: `__init__`[`L45`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L45), `_session`[`L46`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L46)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `_RecordingSession`
- def: [`tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py:27`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L27)
- doc: Records every query string passed to .run().
- signature: `class _RecordingSession:`
- members:
  - `run(self, query: str, **_kwargs)` — [`L33`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L33)
  - `queries` — [`L31`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L31)
- protocol/private: `__enter__`[`L37`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L37), `__exit__`[`L40`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L40), `__init__`[`L30`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L30)
- used by: (3 test-only callers)

## Functions
- `_make_db_manager(backend_type: str)` — [`L52`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_falkordb_schema_and_watcher_fixes.py#L52)

