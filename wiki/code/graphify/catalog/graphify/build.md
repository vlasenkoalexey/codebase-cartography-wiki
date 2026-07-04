---
title: 'Module: graphify/build.py'
type: catalog
provenance: extracted
module: graphify/build.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.build`/
symbols:
  build_from_json: build_from_json().
  build_merge: build_merge().
  edge_data: edge_data().
  graph_has_legacy_ids: graph_has_legacy_ids().
  _semantic_id_remap: _semantic_id_remap().
  build: build().
  _norm_source_file: _norm_source_file().
  prefix_graph_for_global: prefix_graph_for_global().
  dedupe_edges: dedupe_edges().
  prune_repo_from_graph: prune_repo_from_graph().
  _normalize_hyperedge_members: _normalize_hyperedge_members().
  dedupe_nodes: dedupe_nodes().
  _old_file_stems: _old_file_stems().
  edge_datas: edge_datas().
  build_merge._kept: build_merge()._kept().
  _infer_merge_root: _infer_merge_root().
  deduplicate_by_label: deduplicate_by_label().
  _HE_MEMBER_ALIASES: _HE_MEMBER_ALIASES.
  _FILE_TYPE_SYNONYMS: _FILE_TYPE_SYNONYMS.
  _norm_label: _norm_label().
---
# Module: [`graphify/build.py`](../../../../../raw/code/graphify/graphify/build.py)

## Functions
- `_infer_merge_root(graph_path: Path)` — [`L133`](../../../../../raw/code/graphify/graphify/build.py#L133) — Best-effort scan root for relativizing paths in build_merge when the caller
- `_kept(item: dict)` — [`L816`](../../../../../raw/code/graphify/graphify/build.py#L816)
- `_norm_label(label: str | None)` — [`L673`](../../../../../raw/code/graphify/graphify/build.py#L673) — Canonical dedup key — Unicode-aware, preserves CJK/word characters.
- `_norm_source_file(p: str | None, root: str | None = None)` — [`L106`](../../../../../raw/code/graphify/graphify/build.py#L106) — Normalize path separators and relativize absolute paths. — documented in [graphify-build](../../concepts/graphify-build.md)
- `_normalize_hyperedge_members(he: object)` — [`L64`](../../../../../raw/code/graphify/graphify/build.py#L64) — Canonicalize a hyperedge's member list onto the `nodes` key, in place.
- `_old_file_stems(rel: Path)` — [`L220`](../../../../../raw/code/graphify/graphify/build.py#L220) — Pre-migration stem forms a semantic fragment may have used for ``rel``.
- `_semantic_id_remap(nodes: list, root: str | None)` — [`L237`](../../../../../raw/code/graphify/graphify/build.py#L237) — Re-derive non-AST node ids from ``source_file`` using the canonical — documented in [graphify-build](../../concepts/graphify-build.md)
- `build(extractions: list[dict], *, directed: bool = False, dedup: bool = True, dedup_llm_backend: str | None = None, root: str | Path | None = None)` — [`L635`](../../../../../raw/code/graphify/graphify/build.py#L635) — Merge multiple extraction results into one graph. — documented in [graphify-build](../../concepts/graphify-build.md)
- `build_from_json(extraction: dict, *, directed: bool = False, root: str | Path | None = None)` — [`L331`](../../../../../raw/code/graphify/graphify/build.py#L331) — Build a NetworkX graph from an extraction dict. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `build_merge(new_chunks: list[dict], graph_path: str | Path | None = None, prune_sources: list[str] | None = None, *, directed: bool = False, dedup: bool = True, dedup_llm_backend: str | None = None, root: str | Path | None = None)` — [`L735`](../../../../../raw/code/graphify/graphify/build.py#L735) — Load existing graph.json, merge new chunks into it, and save back. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `dedupe_edges(edges: list[dict])` — [`L197`](../../../../../raw/code/graphify/graphify/build.py#L197) — Collapse exact parallel edges by ``(source, target, relation)``, keeping the
- `dedupe_nodes(nodes: list[dict])` — [`L178`](../../../../../raw/code/graphify/graphify/build.py#L178) — Collapse nodes sharing an ``id``, last-writer-wins on attributes.
- `deduplicate_by_label(nodes: list[dict], edges: list[dict])` — [`L681`](../../../../../raw/code/graphify/graphify/build.py#L681) — Merge nodes that share a normalised label, rewriting edge references.
- `edge_data(G: nx.Graph, u: str, v: str)` — [`L157`](../../../../../raw/code/graphify/graphify/build.py#L157) — Return one edge attribute dict for (u, v), tolerating MultiGraph. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `edge_datas(G: nx.Graph, u: str, v: str)` — [`L170`](../../../../../raw/code/graphify/graphify/build.py#L170) — Return every edge attribute dict for (u, v); always a list.
- `graph_has_legacy_ids(nodes: list, root: str | Path | None = None, sample: int = 300)` — [`L287`](../../../../../raw/code/graphify/graphify/build.py#L287) — Whether a loaded graph still uses pre-#1504 node IDs (parent-dir / filename — documented in [graphify-build](../../concepts/graphify-build.md)
- `prefix_graph_for_global(G: nx.Graph, repo_tag: str)` — [`L912`](../../../../../raw/code/graphify/graphify/build.py#L912) — Return a copy of G with all node IDs prefixed with repo_tag::.
- `prune_repo_from_graph(G: nx.Graph, repo_tag: str)` — [`L928`](../../../../../raw/code/graphify/graphify/build.py#L928) — Remove all nodes tagged with repo_tag from G in-place. Returns count removed.

## Module values
- `_FILE_TYPE_SYNONYMS` — [`L39`](../../../../../raw/code/graphify/graphify/build.py#L39)
- `_HE_MEMBER_ALIASES` — [`L61`](../../../../../raw/code/graphify/graphify/build.py#L61)

