---
title: 'Module: src/codegraphcontext/tools/indexing/vector_resolver.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/indexing/vector_resolver.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.indexing.vector_resolver`/
symbols:
  VectorResolver._resolve_neo4j: VectorResolver#_resolve_neo4j().
  VectorResolver.resolve: VectorResolver#resolve().
  VectorResolver._resolve_property_scan: VectorResolver#_resolve_property_scan().
  VectorResolver._get_embedder: VectorResolver#_get_embedder().
  VectorResolver._embed_query: VectorResolver#_embed_query().
  VectorResolver.__init__: VectorResolver#__init__().
  VectorResolver: VectorResolver#
  VectorResolver._backend: VectorResolver#_backend.
  VectorResolver._embedder: VectorResolver#_embedder.
  VectorResolver.resolve_bulk: VectorResolver#resolve_bulk().
  VectorResolver.driver: VectorResolver#driver.
  VectorResolver.threshold: VectorResolver#threshold.
  _VECTOR_INDEX_NAME: _VECTOR_INDEX_NAME.
  _DEFAULT_THRESHOLD: _DEFAULT_THRESHOLD.
  _DEFAULT_TOP_K: _DEFAULT_TOP_K.
  VectorResolver.top_k: VectorResolver#top_k.
---
# Module: [`src/codegraphcontext/tools/indexing/vector_resolver.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/vector_resolver.py)

## Classes
### `VectorResolver`
- def: [`src/codegraphcontext/tools/indexing/vector_resolver.py:21`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/vector_resolver.py#L21)
- doc: Pick the best Function among candidates using embedding similarity.
- signature: `class VectorResolver:`
- members:
  - `_resolve_property_scan(self, called_name: str, candidate_paths: List[str], query_vec: List[float])` — [`L78`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/vector_resolver.py#L78) — Brute-force cosine similarity over stored node embeddings.
  - `resolve(self, called_name: str, caller_qualified_name: Optional[str], candidate_paths: List[str], repo_path: str)` — [`L115`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/vector_resolver.py#L115) — Return the file path of the best-matching Function among candidates.
  - `resolve_bulk(self, calls: List[Dict[str, Any]], repo_path: str)` — [`L137`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/vector_resolver.py#L137) — Resolve a list of calls; returns {call_index: resolved_path}.
  - `driver` — [`L30`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/vector_resolver.py#L30)
  - `threshold` — [`L31`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/vector_resolver.py#L31)
  - `top_k` — [`L32`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/vector_resolver.py#L32)
- protocol/private: `__init__`[`L24`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/vector_resolver.py#L24), `_backend`[`L34`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/vector_resolver.py#L34), `_embed_query`[`L43`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/vector_resolver.py#L43), `_embedder`[`L33`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/vector_resolver.py#L33), `_get_embedder`[`L36`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/vector_resolver.py#L36), `_resolve_neo4j`[`L46`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/vector_resolver.py#L46)
- uses (calls/refs, reference-scoped): [`warning_logger`](../../utils/debug_log.md#warning_logger), [`_get_embedder`](embeddings.md#_get_embedder), [`embed_batch`](embeddings.md#_OpenAIEmbedder.embed_batch), [`detect_graph_backend`](embeddings.md#detect_graph_backend), [`cosine_similarity`](embeddings.md#cosine_similarity), [`_DEFAULT_THRESHOLD`](vector_resolver.md#_DEFAULT_THRESHOLD), [`_DEFAULT_TOP_K`](vector_resolver.md#_DEFAULT_TOP_K), [`_VECTOR_INDEX_NAME`](vector_resolver.md#_VECTOR_INDEX_NAME)
- used by: [`run_tree_sitter_index_async`](pipeline.md#run_tree_sitter_index_async), [`_handle_modification`](../../core/watcher.md#RepositoryEventHandler._handle_modification)

## Module values
- `_DEFAULT_THRESHOLD` — [`L17`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/vector_resolver.py#L17)
- `_DEFAULT_TOP_K` — [`L18`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/vector_resolver.py#L18)
- `_VECTOR_INDEX_NAME` — [`L16`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/vector_resolver.py#L16)

