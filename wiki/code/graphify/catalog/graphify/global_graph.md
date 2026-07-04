---
title: 'Module: graphify/global_graph.py'
type: catalog
provenance: extracted
module: graphify/global_graph.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.global_graph`/
symbols:
  global_add: global_add().
  global_remove: global_remove().
  _load_global_graph: _load_global_graph().
  _GLOBAL_MANIFEST: _GLOBAL_MANIFEST.
  _GLOBAL_GRAPH: _GLOBAL_GRAPH.
  _save_manifest: _save_manifest().
  _save_global_graph: _save_global_graph().
  global_list: global_list().
  global_path: global_path().
  _load_manifest: _load_manifest().
  _GLOBAL_DIR: _GLOBAL_DIR.
  _file_hash: _file_hash().
---
# Module: [`graphify/global_graph.py`](../../../../../raw/code/graphify/graphify/global_graph.py)

## Functions
- `_file_hash(path: Path)` — [`L71`](../../../../../raw/code/graphify/graphify/global_graph.py#L71)
- `_load_global_graph()` — [`L48`](../../../../../raw/code/graphify/graphify/global_graph.py#L48) — documented in [graphify-security](../../concepts/graphify-security.md)
- `_load_manifest()` — [`L15`](../../../../../raw/code/graphify/graphify/global_graph.py#L15)
- `_save_global_graph(G: nx.Graph)` — [`L62`](../../../../../raw/code/graphify/graphify/global_graph.py#L62)
- `_save_manifest(manifest: dict)` — [`L43`](../../../../../raw/code/graphify/graphify/global_graph.py#L43)
- `global_add(source_path: Path, repo_tag: str)` — [`L77`](../../../../../raw/code/graphify/graphify/global_graph.py#L77) — Add or update a project graph in the global graph. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `global_list()` — [`L176`](../../../../../raw/code/graphify/graphify/global_graph.py#L176) — Return the manifest repos dict.
- `global_path()` — [`L181`](../../../../../raw/code/graphify/graphify/global_graph.py#L181)
- `global_remove(repo_tag: str)` — [`L159`](../../../../../raw/code/graphify/graphify/global_graph.py#L159) — Remove all nodes for repo_tag from the global graph. Returns count removed.

## Module values
- `_GLOBAL_DIR` — [`L10`](../../../../../raw/code/graphify/graphify/global_graph.py#L10)
- `_GLOBAL_GRAPH` — [`L11`](../../../../../raw/code/graphify/graphify/global_graph.py#L11)
- `_GLOBAL_MANIFEST` — [`L12`](../../../../../raw/code/graphify/graphify/global_graph.py#L12)

