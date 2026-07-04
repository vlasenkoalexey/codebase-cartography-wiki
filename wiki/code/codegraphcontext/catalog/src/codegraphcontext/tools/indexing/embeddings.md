---
title: 'Module: src/codegraphcontext/tools/indexing/embeddings.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/indexing/embeddings.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.indexing.embeddings`/
symbols:
  EmbeddingPipeline.run: EmbeddingPipeline#run().
  EmbeddingPipeline._ensure_vector_index: EmbeddingPipeline#_ensure_vector_index().
  _get_embedder: _get_embedder().
  _OpenAIEmbedder.embed_batch: _OpenAIEmbedder#embed_batch().
  EmbeddingPipeline._fetch_unembedded: EmbeddingPipeline#_fetch_unembedded().
  EmbeddingPipeline.invalidate_for_file: EmbeddingPipeline#invalidate_for_file().
  EmbeddingPipeline._backend: EmbeddingPipeline#_backend.
  EmbeddingPipeline: EmbeddingPipeline#
  EmbeddingPipeline.driver: EmbeddingPipeline#driver.
  EmbeddingPipeline.batch_size: EmbeddingPipeline#batch_size.
  _OpenAIEmbedder.dim: _OpenAIEmbedder#dim.
  EmbeddingPipeline._unembedded_predicate: EmbeddingPipeline#_unembedded_predicate().
  EmbeddingPipeline._write_embeddings: EmbeddingPipeline#_write_embeddings().
  detect_graph_backend: detect_graph_backend().
  _LocalEmbedder.dim: _LocalEmbedder#dim.
  _LocalEmbedder.embed_batch: _LocalEmbedder#embed_batch().
  _FastEmbedder.dim: _FastEmbedder#dim.
  _FastEmbedder.embed_batch: _FastEmbedder#embed_batch().
  _VECTOR_INDEX_NAME: _VECTOR_INDEX_NAME.
  cosine_similarity: cosine_similarity().
  _LocalEmbedder: _LocalEmbedder#
  _LocalEmbedder.model: _LocalEmbedder#model.
  _FastEmbedder: _FastEmbedder#
  _DIM_OPENAI: _DIM_OPENAI.
  _DIM_BGE_SMALL: _DIM_BGE_SMALL.
  _build_text: _build_text().
  _OpenAIEmbedder: _OpenAIEmbedder#
  _OpenAIEmbedder.client: _OpenAIEmbedder#client.
  _OpenAIEmbedder.model: _OpenAIEmbedder#model.
  _FastEmbedder._model: _FastEmbedder#_model.
  _DIM_MINILM: _DIM_MINILM.
  _OpenAIEmbedder.__init__: _OpenAIEmbedder#__init__().
  _LocalEmbedder.__init__: _LocalEmbedder#__init__().
  _FastEmbedder.__init__: _FastEmbedder#__init__().
  EmbeddingPipeline.__init__: EmbeddingPipeline#__init__().
---
# Module: [`src/codegraphcontext/tools/indexing/embeddings.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py)

## Classes
### `EmbeddingPipeline`
- def: [`src/codegraphcontext/tools/indexing/embeddings.py:140`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L140)
- doc: Reads Function nodes, generates embeddings, and writes them back.
- signature: `class EmbeddingPipeline:`
- members:
  - `_ensure_vector_index(self, dim: int)` — [`L148`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L148) — Create a native vector index when the backend supports one.
  - `_fetch_unembedded(self, repo_path: str)` — [`L177`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L177) — Return (path, name, props) for Function nodes without an embedding.
  - `invalidate_for_file(self, file_path: str)` — [`L220`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L220) — Clear embeddings for all Function nodes in the given file.
  - `run(self, repo_path: str, model_spec: Optional[str] = None)` — [`L237`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L237) — Generate and persist embeddings for all un-embedded Function nodes in repo. — documented in [codegraphcontext-tools-graph_builder](../../../../../concepts/codegraphcontext-tools-graph_builder.md)
  - `batch_size` — [`L145`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L145)
  - `driver` — [`L144`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L144)
- protocol/private: `__init__`[`L143`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L143), `_backend`[`L146`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L146), `_unembedded_predicate`[`L172`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L172), `_write_embeddings`[`L208`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L208)
- uses (calls/refs, reference-scoped): [`info_logger`](../../utils/debug_log.md#info_logger), [`warning_logger`](../../utils/debug_log.md#warning_logger), [`error_logger`](../../utils/debug_log.md#error_logger), [`_get_embedder`](embeddings.md#_get_embedder), [`embed_batch`](embeddings.md#_OpenAIEmbedder.embed_batch), [`dim`](embeddings.md#_OpenAIEmbedder.dim), [`detect_graph_backend`](embeddings.md#detect_graph_backend), [`_VECTOR_INDEX_NAME`](embeddings.md#_VECTOR_INDEX_NAME), [`_build_text`](embeddings.md#_build_text)
- used by: [`run_tree_sitter_index_async`](pipeline.md#run_tree_sitter_index_async), [`_handle_modification`](../../core/watcher.md#RepositoryEventHandler._handle_modification)

### `_FastEmbedder`
- def: [`src/codegraphcontext/tools/indexing/embeddings.py:109`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L109)
- doc: ONNX-based embedder via fastembed — no torch required, works on Python 3.13.
- signature: `class _FastEmbedder:`
- members:
  - `embed_batch(self, texts: List[str])` — [`L120`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L120)
  - `dim` — [`L118`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L118)
- protocol/private: `__init__`[`L112`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L112), `_model`[`L117`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L117)
- uses (calls/refs, reference-scoped): [`_DIM_BGE_SMALL`](embeddings.md#_DIM_BGE_SMALL)
- used by: [`_get_embedder`](embeddings.md#_get_embedder)

### `_LocalEmbedder`
- def: [`src/codegraphcontext/tools/indexing/embeddings.py:96`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L96)
- signature: `class _LocalEmbedder:`
- members:
  - `embed_batch(self, texts: List[str])` — [`L105`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L105)
  - `dim` — [`L103`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L103)
  - `model` — [`L102`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L102)
- protocol/private: `__init__`[`L97`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L97)
- used by: [`_get_embedder`](embeddings.md#_get_embedder)

### `_OpenAIEmbedder`
- def: [`src/codegraphcontext/tools/indexing/embeddings.py:81`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L81)
- signature: `class _OpenAIEmbedder:`
- members:
  - `embed_batch(self, texts: List[str])` — [`L91`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L91)
  - `client` — [`L87`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L87)
  - `dim` — [`L89`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L89)
  - `model` — [`L88`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L88)
- protocol/private: `__init__`[`L82`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L82)
- uses (calls/refs, reference-scoped): [`_DIM_OPENAI`](embeddings.md#_DIM_OPENAI)
- used by: [`run`](embeddings.md#EmbeddingPipeline.run), [`_get_embedder`](embeddings.md#_get_embedder), [`_embed_query`](vector_resolver.md#VectorResolver._embed_query)

## Functions
- `_build_text(fn: Dict[str, Any])` — [`L67`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L67) — Construct the text to embed for a Function node.
- `_get_embedder(model_spec: Optional[str] = None)` — [`L124`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L124) — Return the appropriate embedder based on CGC_EMBEDDING_MODEL env var.
- `cosine_similarity(a: List[float], b: List[float])` — [`L55`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L55) — Cosine similarity between two equal-length vectors.
- `detect_graph_backend(driver: Any)` — [`L38`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L38) — Return a stable backend id for the active graph driver wrapper.

## Module values
- `_DIM_BGE_SMALL` — [`L33`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L33)
- `_DIM_MINILM` — [`L32`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L32)
- `_DIM_OPENAI` — [`L31`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L31)
- `_VECTOR_INDEX_NAME` — [`L35`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/embeddings.py#L35)

