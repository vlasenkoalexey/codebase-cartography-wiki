---
title: 'Module: graphify/wiki.py'
type: catalog
provenance: extracted
module: graphify/wiki.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.wiki`/
symbols:
  to_wiki: to_wiki().
  _community_article: _community_article().
  _md_link: _md_link().
  _god_node_article: _god_node_article().
  _index_md: _index_md().
  _safe_filename: _safe_filename().
  to_wiki._unique_slug: to_wiki()._unique_slug().
  _cross_community_links: _cross_community_links().
---
# Module: [`graphify/wiki.py`](../../../../../raw/code/graphify/graphify/wiki.py)

## Functions
- `_community_article(G: nx.Graph, cid: int, nodes: list[str], label: str, labels: dict[int, str], cohesion: float | None, node_community: dict[str, int] | None = None, resolver: dict[str, str] | None = None)` — [`L62`](../../../../../raw/code/graphify/graphify/wiki.py#L62)
- `_cross_community_links(G: nx.Graph, nodes: list[str], own_cid: int, labels: dict[int, str], node_community: dict[str, int])` — [`L51`](../../../../../raw/code/graphify/graphify/wiki.py#L51) — Return (community_label, edge_count) pairs for cross-community connections, sorted descending.
- `_god_node_article(G: nx.Graph, nid: str, labels: dict[int, str], node_community: dict[str, int] | None = None, resolver: dict[str, str] | None = None)` — [`L132`](../../../../../raw/code/graphify/graphify/wiki.py#L132)
- `_index_md(communities: dict[int, list[str]], labels: dict[int, str], god_nodes_data: list[dict], total_nodes: int, total_edges: int, resolver: dict[str, str] | None = None)` — [`L169`](../../../../../raw/code/graphify/graphify/wiki.py#L169)
- `_md_link(label: str, resolver: dict[str, str])` — [`L27`](../../../../../raw/code/graphify/graphify/wiki.py#L27) — Render a link to another wiki article as a portable relative markdown link.
- `_safe_filename(name: str)` — [`L12`](../../../../../raw/code/graphify/graphify/wiki.py#L12) — Make a label safe for use as a filename across platforms.
- `_unique_slug(base: str)` — [`L280`](../../../../../raw/code/graphify/graphify/wiki.py#L280)
- `to_wiki(G: nx.Graph, communities: dict[int, list[str]], output_dir: str | Path, community_labels: dict[int, str] | None = None, cohesion: dict[int, float] | None = None, god_nodes_data: list[dict] | None = None)` — [`L211`](../../../../../raw/code/graphify/graphify/wiki.py#L211) — Generate a Wikipedia-style wiki from the graph. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)

