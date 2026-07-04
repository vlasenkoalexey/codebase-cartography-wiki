---
title: 'Module: graphify/analyze.py'
type: catalog
provenance: extracted
module: graphify/analyze.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.analyze`/
symbols:
  _surprise_score: _surprise_score().
  god_nodes: god_nodes().
  surprising_connections: surprising_connections().
  _file_category: _file_category().
  suggest_questions: suggest_questions().
  _is_file_node: _is_file_node().
  find_import_cycles: find_import_cycles().
  _cross_file_surprises: _cross_file_surprises().
  _node_community_map: _node_community_map().
  _is_concept_node: _is_concept_node().
  _cross_community_surprises: _cross_community_surprises().
  _is_json_key_node: _is_json_key_node().
  graph_diff: graph_diff().
  _LANG_FAMILY._LANG_FAMILY: _LANG_FAMILY._LANG_FAMILY.
  graph_diff.edge_key: graph_diff().edge_key().
  _cross_language: _cross_language().
  _top_level_dir: _top_level_dir().
  find_import_cycles._endpoint_source_file: find_import_cycles()._endpoint_source_file().
  _BUILTIN_NOISE_LABELS: _BUILTIN_NOISE_LABELS.
  _JSON_NOISE_LABELS._JSON_NOISE_LABELS: _JSON_NOISE_LABELS._JSON_NOISE_LABELS.
---
# Module: [`graphify/analyze.py`](../../../../../raw/code/graphify/graphify/analyze.py)

## Functions
- `_cross_community_surprises(G: nx.Graph, communities: dict[int, list[str]], top_n: int)` — [`L331`](../../../../../raw/code/graphify/graphify/analyze.py#L331) — For single-source corpora: find edges that bridge different communities. — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `_cross_file_surprises(G: nx.Graph, communities: dict[int, list[str]], top_n: int)` — [`L268`](../../../../../raw/code/graphify/graphify/analyze.py#L268) — Cross-file edges between real code/doc entities, ranked by a composite — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `_cross_language(src_a: str, src_b: str)` — [`L39`](../../../../../raw/code/graphify/graphify/analyze.py#L39) — Return True if two source files belong to different language families. — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `_endpoint_source_file(node_id: str)` — [`L652`](../../../../../raw/code/graphify/graphify/analyze.py#L652)
- `_file_category(path: str)` — [`L178`](../../../../../raw/code/graphify/graphify/analyze.py#L178) — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `_is_concept_node(G: nx.Graph, node_id: str)` — [`L156`](../../../../../raw/code/graphify/graphify/analyze.py#L156) — Return True if this node is a manually-injected semantic concept node — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `_is_file_node(G: nx.Graph, node_id: str)` — [`L55`](../../../../../raw/code/graphify/graphify/analyze.py#L55) — Return True if this node is a file-level hub node (e.g. 'client', 'models') — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `_is_json_key_node(G: nx.Graph, node_id: str)` — [`L91`](../../../../../raw/code/graphify/graphify/analyze.py#L91) — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `_node_community_map(communities: dict[int, list[str]])` — [`L50`](../../../../../raw/code/graphify/graphify/analyze.py#L50) — Invert communities dict: node_id -> community_id. — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `_surprise_score(G: nx.Graph, u: str, v: str, data: dict, node_community: dict[str, int], u_source: str, v_source: str, degrees: dict[str, int] | None = None)` — [`L194`](../../../../../raw/code/graphify/graphify/analyze.py#L194) — Score how surprising a cross-file edge is. Returns (score, reasons). — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `_top_level_dir(path: str)` — [`L189`](../../../../../raw/code/graphify/graphify/analyze.py#L189) — Return the first path component - used to detect cross-repo edges. — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `edge_key(G: nx.Graph, u: str, v: str, data: dict)` — [`L571`](../../../../../raw/code/graphify/graphify/analyze.py#L571)
- `find_import_cycles(G: nx.Graph, max_cycle_length: int = 5, top_n: int = 20)` — [`L628`](../../../../../raw/code/graphify/graphify/analyze.py#L628) — Detect circular import dependencies at the file level.
- `god_nodes(G: nx.Graph, top_n: int = 10)` — [`L100`](../../../../../raw/code/graphify/graphify/analyze.py#L100) — Return the top_n most-connected real entities - the core abstractions. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `graph_diff(G_old: nx.Graph, G_new: nx.Graph)` — [`L544`](../../../../../raw/code/graphify/graphify/analyze.py#L544) — Compare two graph snapshots and return what changed.
- `suggest_questions(G: nx.Graph, communities: dict[int, list[str]], community_labels: dict[int, str], top_n: int = 7)` — [`L419`](../../../../../raw/code/graphify/graphify/analyze.py#L419) — Generate questions the graph is uniquely positioned to answer.
- `surprising_connections(G: nx.Graph, communities: dict[int, list[str]] | None = None, top_n: int = 5)` — [`L124`](../../../../../raw/code/graphify/graphify/analyze.py#L124) — Find connections that are genuinely surprising - not obvious from file structure. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)

## Module values
- `_BUILTIN_NOISE_LABELS` — [`L11`](../../../../../raw/code/graphify/graphify/analyze.py#L11) — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `_JSON_NOISE_LABELS` — [`L83`](../../../../../raw/code/graphify/graphify/analyze.py#L83) — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `_LANG_FAMILY` — [`L24`](../../../../../raw/code/graphify/graphify/analyze.py#L24) — documented in [graphify-analyze](../../concepts/graphify-analyze.md)

