---
title: 'Module: graphify/export.py'
type: catalog
provenance: extracted
module: graphify/export.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.export`/
symbols:
  to_html: to_html().
  to_obsidian: to_obsidian().
  to_json: to_json().
  backup_if_protected: backup_if_protected().
  to_canvas: to_canvas().
  push_to_falkordb: push_to_falkordb().
  to_cypher: to_cypher().
  attach_hyperedges: attach_hyperedges().
  push_to_neo4j: push_to_neo4j().
  COMMUNITY_COLORS: COMMUNITY_COLORS.
  to_graphml: to_graphml().
  to_svg: to_svg().
  to_obsidian.safe_name: to_obsidian().safe_name().
  _cypher_escape: _cypher_escape().
  _cypher_label: _cypher_label().
  to_canvas.safe_name: to_canvas().safe_name().
  _yaml_str: _yaml_str().
  to_html._js_safe: to_html()._js_safe().
  _viz_node_limit: _viz_node_limit().
  _git_head: _git_head().
  to_obsidian._owned_write: to_obsidian()._owned_write().
  to_obsidian._community_name: to_obsidian()._community_name().
  generate_html: generate_html.
  _obsidian_tag: _obsidian_tag().
  MAX_NODES_FOR_VIZ: MAX_NODES_FOR_VIZ.
  _cap_filename: _cap_filename().
  _dedup_node_filenames: _dedup_node_filenames().
  to_obsidian._community_reach: to_obsidian()._community_reach().
  _BACKUP_ARTIFACTS: _BACKUP_ARTIFACTS.
  _strip_diacritics: _strip_diacritics().
  _html_styles: _html_styles().
  _hyperedge_script: _hyperedge_script().
  _html_script: _html_script().
  _CONFIDENCE_SCORE_DEFAULTS: _CONFIDENCE_SCORE_DEFAULTS.
  _CYPHER_IDENT_RE: _CYPHER_IDENT_RE.
  to_obsidian._dominant_confidence: to_obsidian()._dominant_confidence().
  push_to_neo4j._safe_rel: push_to_neo4j()._safe_rel().
  push_to_neo4j._safe_label: push_to_neo4j()._safe_label().
  push_to_falkordb._safe_rel: push_to_falkordb()._safe_rel().
  push_to_falkordb._safe_label: push_to_falkordb()._safe_label().
  prune_dangling_edges: prune_dangling_edges().
---
# Module: [`graphify/export.py`](../../../../../raw/code/graphify/graphify/export.py)

## Functions
- `_cap_filename(s: str, limit: int = 200)` — [`L874`](../../../../../raw/code/graphify/graphify/export.py#L874) — Cap a filename stem to ``limit`` UTF-8 bytes so it stays under the 255-byte
- `_community_name(cid)` — [`L1072`](../../../../../raw/code/graphify/graphify/export.py#L1072) — documented in [graphify-export](../../concepts/graphify-export.md)
- `_community_reach(node_id: str)` — [`L1064`](../../../../../raw/code/graphify/graphify/export.py#L1064)
- `_cypher_escape(s: str)` — [`L560`](../../../../../raw/code/graphify/graphify/export.py#L560) — Escape a string for safe embedding in a Cypher single-quoted literal.
- `_cypher_label(raw: str, fallback: str)` — [`L592`](../../../../../raw/code/graphify/graphify/export.py#L592) — Sanitise a value used in identifier position (node label / rel type).
- `_dedup_node_filenames(G: nx.Graph, safe_name)` — [`L891`](../../../../../raw/code/graphify/graphify/export.py#L891) — Map each node_id to a unique note filename, appending a numeric suffix on
- `_dominant_confidence(node_id: str)` — [`L975`](../../../../../raw/code/graphify/graphify/export.py#L975)
- `_git_head()` — [`L475`](../../../../../raw/code/graphify/graphify/export.py#L475) — Return the current git HEAD commit hash, or None if not in a git repo. — documented in [graphify-export](../../concepts/graphify-export.md)
- `_html_script(nodes_json: str, edges_json: str, legend_json: str)` — [`L260`](../../../../../raw/code/graphify/graphify/export.py#L260)
- `_html_styles()` — [`L176`](../../../../../raw/code/graphify/graphify/export.py#L176)
- `_hyperedge_script(hyperedges_json: str)` — [`L217`](../../../../../raw/code/graphify/graphify/export.py#L217)
- `_js_safe(obj)` — [`L822`](../../../../../raw/code/graphify/graphify/export.py#L822) — documented in [graphify-export](../../concepts/graphify-export.md)
- `_obsidian_tag(name: str)` — [`L97`](../../../../../raw/code/graphify/graphify/export.py#L97) — Sanitize a community name for use as an Obsidian tag.
- `_owned_write(rel_name: str, content: str)` — [`L943`](../../../../../raw/code/graphify/graphify/export.py#L943) — Write a graphify-owned file, refusing to overwrite a pre-existing file — documented in [graphify-export](../../concepts/graphify-export.md)
- `_safe_label(label: str)` — [`L1426`](../../../../../raw/code/graphify/graphify/export.py#L1426) — Sanitize a Neo4j node label to prevent Cypher injection.
- `_safe_label(label: str)` — [`L1514`](../../../../../raw/code/graphify/graphify/export.py#L1514) — Sanitize a FalkorDB node label to prevent Cypher injection.
- `_safe_rel(relation: str)` — [`L1423`](../../../../../raw/code/graphify/graphify/export.py#L1423)
- `_safe_rel(relation: str)` — [`L1511`](../../../../../raw/code/graphify/graphify/export.py#L1511)
- `_strip_diacritics(text: str | None)` — [`L106`](../../../../../raw/code/graphify/graphify/export.py#L106)
- `_viz_node_limit()` — [`L160`](../../../../../raw/code/graphify/graphify/export.py#L160) — Return the effective viz node limit, honoring GRAPHIFY_VIZ_NODE_LIMIT env var. — documented in [graphify-export](../../concepts/graphify-export.md)
- `_yaml_str(s: str)` — [`L114`](../../../../../raw/code/graphify/graphify/export.py#L114) — Escape a value for safe embedding in a YAML double-quoted scalar (F-009). — documented in [graphify-export](../../concepts/graphify-export.md)
- `attach_hyperedges(G: nx.Graph, hyperedges: list)` — [`L464`](../../../../../raw/code/graphify/graphify/export.py#L464) — Store hyperedges in the graph's metadata dict. — documented in [graphify-build](../../concepts/graphify-build.md)
- `backup_if_protected(out_dir: Path)` — [`L33`](../../../../../raw/code/graphify/graphify/export.py#L33) — Snapshot graph artifacts to a dated subfolder before an overwrite. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `prune_dangling_edges(graph_data: dict)` — [`L545`](../../../../../raw/code/graphify/graphify/export.py#L545) — Remove edges whose source or target node is not in the node set.
- `push_to_falkordb(G: nx.Graph, uri: str, user: str | None = None, password: str | None = None, communities: dict[int, list[str]] | None = None, graph_name: str = "graphify")` — [`L1472`](../../../../../raw/code/graphify/graphify/export.py#L1472) — Push graph directly to a running FalkorDB instance via the Python SDK.
- `push_to_neo4j(G: nx.Graph, uri: str, user: str, password: str, communities: dict[int, list[str]] | None = None)` — [`L1400`](../../../../../raw/code/graphify/graphify/export.py#L1400) — Push graph directly to a running Neo4j instance via the Python driver.
- `safe_name(label: str)` — [`L959`](../../../../../raw/code/graphify/graphify/export.py#L959) — documented in [graphify-export](../../concepts/graphify-export.md)
- `safe_name(label: str)` — [`L1238`](../../../../../raw/code/graphify/graphify/export.py#L1238)
- `to_canvas(G: nx.Graph, communities: dict[int, list[str]], output_path: str, community_labels: dict[int, str] | None = None, node_filenames: dict[str, str] | None = None)` — [`L1222`](../../../../../raw/code/graphify/graphify/export.py#L1222) — Export graph as an Obsidian Canvas file - communities as groups, nodes as cards.
- `to_cypher(G: nx.Graph, output_path: str)` — [`L605`](../../../../../raw/code/graphify/graphify/export.py#L605)
- `to_graphml(G: nx.Graph, communities: dict[int, list[str]], output_path: str)` — [`L1568`](../../../../../raw/code/graphify/graphify/export.py#L1568) — Export graph as GraphML - opens in Gephi, yEd, and any GraphML-compatible tool.
- `to_html(G: nx.Graph, communities: dict[int, list[str]], output_path: str, community_labels: dict[int, str] | None = None, member_counts: dict[int, int] | None = None, node_limit: int | None = None, learning_overlay: dict | None = None)` — [`L632`](../../../../../raw/code/graphify/graphify/export.py#L632) — Generate an interactive vis.js HTML visualization of the graph. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `to_json(G: nx.Graph, communities: dict[int, list[str]], output_path: str, *, force: bool = False, built_at_commit: str | None = None, community_labels: dict[int, str] | None = None)` — [`L485`](../../../../../raw/code/graphify/graphify/export.py#L485) — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `to_obsidian(G: nx.Graph, communities: dict[int, list[str]], output_dir: str, community_labels: dict[int, str] | None = None, cohesion: dict[int, float] | None = None)` — [`L913`](../../../../../raw/code/graphify/graphify/export.py#L913) — Export graph as an Obsidian vault - one .md file per node with [[wikilinks]], — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `to_svg(G: nx.Graph, communities: dict[int, list[str]], output_path: str, community_labels: dict[int, str] | None = None, figsize: tuple[int, int] = (20, 14))` — [`L1603`](../../../../../raw/code/graphify/graphify/export.py#L1603) — Export graph as an SVG file using matplotlib + spring layout.

## Module values
- `COMMUNITY_COLORS` — [`L152`](../../../../../raw/code/graphify/graphify/export.py#L152) — documented in [graphify-export](../../concepts/graphify-export.md)
- `MAX_NODES_FOR_VIZ` — [`L157`](../../../../../raw/code/graphify/graphify/export.py#L157)
- `_BACKUP_ARTIFACTS` — [`L22`](../../../../../raw/code/graphify/graphify/export.py#L22)
- `_CONFIDENCE_SCORE_DEFAULTS` — [`L461`](../../../../../raw/code/graphify/graphify/export.py#L461)
- `_CYPHER_IDENT_RE` — [`L589`](../../../../../raw/code/graphify/graphify/export.py#L589)
- `generate_html` — [`L871`](../../../../../raw/code/graphify/graphify/export.py#L871) — documented in [graphify-export](../../concepts/graphify-export.md)

