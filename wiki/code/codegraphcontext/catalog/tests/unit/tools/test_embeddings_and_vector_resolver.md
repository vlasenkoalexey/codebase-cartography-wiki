---
title: 'Module: tests/unit/tools/test_embeddings_and_vector_resolver.py'
type: catalog
provenance: extracted
module: tests/unit/tools/test_embeddings_and_vector_resolver.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.tools.test_embeddings_and_vector_resolver`/
symbols:
  _FakeResult: _FakeResult#
  TestVectorResolver.test_returns_none_on_db_failure: TestVectorResolver#test_returns_none_on_db_failure().
  _RecordingSession: _RecordingSession#
  _RecordingSession.run: _RecordingSession#run().
  TestEmbeddingPipeline.test_run_writes_embeddings_back_to_neo4j: TestEmbeddingPipeline#test_run_writes_embeddings_back_to_neo4j().
  TestEmbeddingPipeline.test_vector_index_creation_is_first_call: TestEmbeddingPipeline#test_vector_index_creation_is_first_call().
  TestVectorResolver.test_returns_path_above_threshold: TestVectorResolver#test_returns_path_above_threshold().
  TestVectorResolver.test_returns_none_below_threshold: TestVectorResolver#test_returns_none_below_threshold().
  TestVectorResolver.test_resolve_bulk_maps_indices_to_paths: TestVectorResolver#test_resolve_bulk_maps_indices_to_paths().
  TestVectorResolver._make_resolver: TestVectorResolver#_make_resolver().
  TestEmbeddingPipeline._make_pipeline: TestEmbeddingPipeline#_make_pipeline().
  TestEmbeddingPipeline.test_run_does_nothing_when_no_unembedded_nodes: TestEmbeddingPipeline#test_run_does_nothing_when_no_unembedded_nodes().
  TestEmbeddingPipeline.test_run_calls_embed_batch_for_each_batch: TestEmbeddingPipeline#test_run_calls_embed_batch_for_each_batch().
  TestEmbeddingPipeline.test_embed_batch_failure_skips_batch_but_continues: TestEmbeddingPipeline#test_embed_batch_failure_skips_batch_but_continues().
  TestVectorResolver.test_returns_none_when_no_candidates: TestVectorResolver#test_returns_none_when_no_candidates().
  TestVectorResolver.test_resolve_bulk_empty_input: TestVectorResolver#test_resolve_bulk_empty_input().
  TestVectorResolver._patch_embedder: TestVectorResolver#_patch_embedder().
  _FakeResult.single: _FakeResult#single().
  _FakeResult.__iter__: _FakeResult#__iter__().
  TestVectorResolver.test_returns_none_on_embedder_failure: TestVectorResolver#test_returns_none_on_embedder_failure().
  _FakeResult._rows: _FakeResult#_rows.
  _RecordingSession.calls: _RecordingSession#calls.
  _RecordingSession._idx: _RecordingSession#_idx.
  _FakeDriver.session: _FakeDriver#session().
  _FakeRow: _FakeRow#
  _RecordingSession._responses: _RecordingSession#_responses.
  _FakeDriver: _FakeDriver#
  _FakeDriver._session: _FakeDriver#_session.
  _FakeRow.__getattr__: _FakeRow#__getattr__().
  _FakeResult.__init__: _FakeResult#__init__().
  _RecordingSession.__init__: _RecordingSession#__init__().
  _RecordingSession.__enter__: _RecordingSession#__enter__().
  _RecordingSession.__exit__: _RecordingSession#__exit__().
  _FakeDriver.__init__: _FakeDriver#__init__().
  TestEmbeddingPipeline: TestEmbeddingPipeline#
  TestBuildText: TestBuildText#
  TestBuildText.test_includes_qualified_name_when_present: TestBuildText#test_includes_qualified_name_when_present().
  TestBuildText.test_falls_back_to_name_without_qualified_name: TestBuildText#test_falls_back_to_name_without_qualified_name().
  TestBuildText.test_includes_docstring_when_present: TestBuildText#test_includes_docstring_when_present().
  TestBuildText.test_includes_parameters: TestBuildText#test_includes_parameters().
  TestBuildText.test_empty_function_node_does_not_crash: TestBuildText#test_empty_function_node_does_not_crash().
  TestVectorResolver: TestVectorResolver#
---
# Module: [`tests/unit/tools/test_embeddings_and_vector_resolver.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py)

## Classes
### `TestBuildText`
- def: [`tests/unit/tools/test_embeddings_and_vector_resolver.py:200`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L200)
- signature: `class TestBuildText:`
- members:
  - `test_empty_function_node_does_not_crash(self)` — [`L227`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L227)
  - `test_falls_back_to_name_without_qualified_name(self)` — [`L208`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L208)
  - `test_includes_docstring_when_present(self)` — [`L214`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L214)
  - `test_includes_parameters(self)` — [`L220`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L220)
  - `test_includes_qualified_name_when_present(self)` — [`L202`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L202)

### `TestEmbeddingPipeline`
- def: [`tests/unit/tools/test_embeddings_and_vector_resolver.py:68`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L68)
- signature: `class TestEmbeddingPipeline:`
- members:
  - `test_embed_batch_failure_skips_batch_but_continues(self)` — [`L169`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L169) — An embedder failure on one batch must not crash the pipeline.
  - `test_run_calls_embed_batch_for_each_batch(self)` — [`L91`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L91) — With 3 nodes and batch_size=2, embed_batch must be called twice.
  - `test_run_does_nothing_when_no_unembedded_nodes(self)` — [`L75`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L75) — If the fetch query returns no rows, no embed or write calls should occur.
  - `test_run_writes_embeddings_back_to_neo4j(self)` — [`L120`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L120) — Each Write call must include an UNWIND query that sets f.embedding.
  - `test_vector_index_creation_is_first_call(self)` — [`L144`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L144) — Vector index DDL must be issued before any embed or write calls.
- protocol/private: `_make_pipeline`[`L70`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L70)
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `TestVectorResolver`
- def: [`tests/unit/tools/test_embeddings_and_vector_resolver.py:237`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L237)
- signature: `class TestVectorResolver:`
- members:
  - `_patch_embedder(self, resolver, vec=None)` — [`L245`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L245) — Inject a mock embedder that returns a fixed vector.
  - `test_resolve_bulk_empty_input(self)` — [`L322`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L322)
  - `test_resolve_bulk_maps_indices_to_paths(self)` — [`L303`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L303) — resolve_bulk must return a dict mapping call index → resolved path.
  - `test_returns_none_below_threshold(self)` — [`L274`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L274)
  - `test_returns_none_on_db_failure(self)` — [`L294`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L294)
  - `test_returns_none_on_embedder_failure(self)` — [`L284`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L284)
  - `test_returns_none_when_no_candidates(self)` — [`L251`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L251)
  - `test_returns_path_above_threshold(self)` — [`L259`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L259)
- protocol/private: `_make_resolver`[`L239`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L239)
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `_FakeDriver`
- def: [`tests/unit/tools/test_embeddings_and_vector_resolver.py:56`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L56)
- signature: `class _FakeDriver:`
- members:
  - `session(self)` — [`L60`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L60)
- protocol/private: `__init__`[`L57`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L57), `_session`[`L58`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L58)
- used by: (2 test-only callers)

### `_FakeResult`
- def: [`tests/unit/tools/test_embeddings_and_vector_resolver.py:26`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L26)
- signature: `class _FakeResult:`
- members:
  - `single(self)` — [`L30`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L30)
- protocol/private: `__init__`[`L27`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L27), `__iter__`[`L33`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L33), `_rows`[`L28`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L28)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (10 test-only callers)

### `_FakeRow`  ·  implements/extends dict
- def: [`tests/unit/tools/test_embeddings_and_vector_resolver.py:17`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L17)
- doc: dict that also supports attribute access like a Record.
- signature: `class _FakeRow(dict):`
- protocol/private: `__getattr__`[`L19`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L19)
- used by: (2 test-only callers)

### `_RecordingSession`
- def: [`tests/unit/tools/test_embeddings_and_vector_resolver.py:37`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L37)
- signature: `class _RecordingSession:`
- members:
  - `run(self, query, **kwargs)` — [`L43`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L43)
  - `calls` — [`L39`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L39)
- protocol/private: `__enter__`[`L49`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L49), `__exit__`[`L52`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L52), `__init__`[`L38`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L38), `_idx`[`L41`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L41), `_responses`[`L40`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_embeddings_and_vector_resolver.py#L40)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (12 test-only callers)

