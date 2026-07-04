---
title: 'Module: graphify/affected.py'
type: catalog
provenance: extracted
module: graphify/affected.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.affected`/
symbols:
  resolve_seed: resolve_seed().
  format_affected: format_affected().
  affected_nodes: affected_nodes().
  _normalize_label: _normalize_label().
  AffectedHit.node_id: AffectedHit#node_id.
  load_graph: load_graph().
  _bare_name: _bare_name().
  DEFAULT_AFFECTED_RELATIONS: DEFAULT_AFFECTED_RELATIONS.
  _prefer_file_node: _prefer_file_node().
  AffectedHit: AffectedHit#
  _node_label: _node_label().
  AffectedHit.via_relation: AffectedHit#via_relation.
  _format_location: _format_location().
  AffectedHit.depth: AffectedHit#depth.
---
# Module: [`graphify/affected.py`](../../../../../raw/code/graphify/graphify/affected.py)

## Classes
### `AffectedHit`
- def: [`graphify/affected.py:29`](../../../../../raw/code/graphify/graphify/affected.py#L29)
- signature: `class AffectedHit:`
- members:
  - `depth` — [`L31`](../../../../../raw/code/graphify/graphify/affected.py#L31)
  - `node_id` — [`L30`](../../../../../raw/code/graphify/graphify/affected.py#L30)
  - `via_relation` — [`L32`](../../../../../raw/code/graphify/graphify/affected.py#L32)
- used by: [`format_affected`](affected.md#format_affected), [`affected_nodes`](affected.md#affected_nodes)  (4 test-only)

## Functions
- `_bare_name(label: str)` — [`L48`](../../../../../raw/code/graphify/graphify/affected.py#L48) — Lowercased label with the callable decoration (trailing "()") removed.
- `_format_location(data: dict)` — [`L40`](../../../../../raw/code/graphify/graphify/affected.py#L40)
- `_node_label(graph: nx.Graph, node_id: str)` — [`L35`](../../../../../raw/code/graphify/graphify/affected.py#L35)
- `_normalize_label(label: str)` — [`L54`](../../../../../raw/code/graphify/graphify/affected.py#L54)
- `_prefer_file_node(graph: nx.Graph, node_ids: list[str], query: str)` — [`L58`](../../../../../raw/code/graphify/graphify/affected.py#L58) — Return the file-level node when a source_file query matches many nodes.
- `affected_nodes(graph: nx.Graph, seed: str, *, relations: Iterable[str] = DEFAULT_AFFECTED_RELATIONS, depth: int = 2)` — [`L140`](../../../../../raw/code/graphify/graphify/affected.py#L140)
- `format_affected(graph: nx.Graph, query: str, *, relations: Iterable[str] = DEFAULT_AFFECTED_RELATIONS, depth: int = 2)` — [`L179`](../../../../../raw/code/graphify/graphify/affected.py#L179)
- `load_graph(path: Path)` — [`L209`](../../../../../raw/code/graphify/graphify/affected.py#L209)
- `resolve_seed(graph: nx.Graph, query: str)` — [`L93`](../../../../../raw/code/graphify/graphify/affected.py#L93)

## Module values
- `DEFAULT_AFFECTED_RELATIONS` — [`L12`](../../../../../raw/code/graphify/graphify/affected.py#L12)

