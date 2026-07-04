---
title: 'Module: graphify/callflow_html.py'
type: catalog
provenance: extracted
module: graphify/callflow_html.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.callflow_html`/
symbols:
  write_callflow_html: write_callflow_html().
  pick_text: pick_text().
  generate_section_flowchart: generate_section_flowchart().
  derive_sections_from_communities: derive_sections_from_communities().
  load_graph: load_graph().
  generate_overview_graph: generate_overview_graph().
  generate_call_table_rows: generate_call_table_rows().
  first_present: first_present().
  select_diagram_nodes: select_diagram_nodes().
  select_diagram_nodes.fallback_key: select_diagram_nodes().fallback_key().
  generate_section_cards: generate_section_cards().
  format_node_refs: format_node_refs().
  safe_mermaid_text: safe_mermaid_text().
  normalize_edge: normalize_edge().
  normalize_sections: normalize_sections().
  node_label: node_label().
  generate_section_intro: generate_section_intro().
  relation_label: relation_label().
  mermaid_section_id: mermaid_section_id().
  safe_file_path: safe_file_path().
  node_mermaid_id: node_mermaid_id().
  preferred_edges: preferred_edges().
  should_include_edge: should_include_edge().
  load_labels: load_labels().
  resolve_graphify_paths: resolve_graphify_paths().
  label_for_community: label_for_community().
  generate_overview_cards: generate_overview_cards().
  humanize_label: humanize_label().
  edge_score: edge_score().
  endpoint_id: endpoint_id().
  select_diagram_nodes.add_node: select_diagram_nodes().add_node().
  section_edge_summary: section_edge_summary().
  node_display_name: node_display_name().
  to_float: to_float().
  node_kind: node_kind().
  normalize_node: normalize_node().
  load_sections: load_sections().
  infer_project_name: infer_project_name().
  node_degree_scores: node_degree_scores().
  node_importance: node_importance().
  group_nodes_by_file: group_nodes_by_file().
  _suggest_tag: _suggest_tag().
  _describe_node: _describe_node().
  generate_header: generate_header().
  derive_flow_chain: derive_flow_chain().
  _report_highlights: _report_highlights().
  main: main().
  read_json: read_json().
  first_list: first_list().
  is_zh: is_zh().
  mermaid_class_defs: mermaid_class_defs().
  stable_ascii_id: stable_ascii_id().
  mermaid_init: mermaid_init().
  build_community_index: build_community_index().
  section_keywords: section_keywords().
  CallflowOptions.output: CallflowOptions#output.
  CallflowOptions.diagram_scale: CallflowOptions#diagram_scale.
  CSS: CSS.
  _node_link_payload: _node_link_payload().
  load_report: load_report().
  html_comment_text: html_comment_text().
  safe_filename: safe_filename().
  detect_lang: detect_lang().
  truncate_text: truncate_text().
  html_anchor_id: html_anchor_id().
  normalize_communities: normalize_communities().
  SECTION_ARCHETYPES: SECTION_ARCHETYPES.
  _community_text: _community_text().
  _keyword_score: _keyword_score().
  _rank_grouped_sections: _rank_grouped_sections().
  build_section_node_map: build_section_node_map().
  classify_edges: classify_edges().
  generate_nav: generate_nav().
  CallflowOptions: CallflowOptions#
  CallflowOptions.lang: CallflowOptions#lang.
  CallflowOptions.max_sections: CallflowOptions#max_sections.
  CallflowOptions.max_diagram_nodes: CallflowOptions#max_diagram_nodes.
  CallflowOptions.max_diagram_edges: CallflowOptions#max_diagram_edges.
  node_in_section: node_in_section().
  CallflowOptions.__init__: CallflowOptions#__init__().
  CallflowOptions.project: CallflowOptions#project.
  CallflowOptions.graphify_out: CallflowOptions#graphify_out.
  CallflowOptions.graph: CallflowOptions#graph.
  CallflowOptions.report: CallflowOptions#report.
  CallflowOptions.labels: CallflowOptions#labels.
  CallflowOptions.sections: CallflowOptions#sections.
---
# Module: [`graphify/callflow_html.py`](../../../../../raw/code/graphify/graphify/callflow_html.py)

## Classes
### `CallflowOptions`
- def: [`graphify/callflow_html.py:1511`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1511)
- doc: Options for call-flow architecture HTML generation.
- signature: `class CallflowOptions:`
- members:
  - `diagram_scale` — [`L1539`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1539) — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
  - `graph` — [`L1532`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1532)
  - `graphify_out` — [`L1531`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1531)
  - `labels` — [`L1534`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1534)
  - `lang` — [`L1537`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1537)
  - `max_diagram_edges` — [`L1541`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1541)
  - `max_diagram_nodes` — [`L1540`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1540)
  - `max_sections` — [`L1538`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1538)
  - `output` — [`L1536`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1536) — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
  - `project` — [`L1530`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1530)
  - `report` — [`L1533`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1533)
  - `sections` — [`L1535`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1535)
- protocol/private: `__init__`[`L1514`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1514)
- used by: [`write_callflow_html`](callflow_html.md#write_callflow_html)

## Functions
- `_community_text(nodes: list, label: str = "")` — [`L799`](../../../../../raw/code/graphify/graphify/callflow_html.py#L799)
- `_describe_node(label: str, source_file: str, file_type: str, lang: str)` — [`L1295`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1295) — Generate a compact human-readable description for a graph node. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `_keyword_score(text: str, keywords: set[str])` — [`L809`](../../../../../raw/code/graphify/graphify/callflow_html.py#L809)
- `_node_link_payload(data: dict)` — [`L222`](../../../../../raw/code/graphify/graphify/callflow_html.py#L222) — Read current graphify graph.json via NetworkX's node-link parser.
- `_rank_grouped_sections(grouped: dict, max_sections: int)` — [`L816`](../../../../../raw/code/graphify/graphify/callflow_html.py#L816) — Return selected grouped sections and overflow communities.
- `_report_highlights(report_text: str, lang: str)` — [`L1544`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1544) — Extract a compact highlights card from GRAPH_REPORT.md. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `_suggest_tag(label: str, file_type: str, lang: str, kind: str = "")` — [`L1260`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1260) — Heuristic tag suggestion based on label name and file type. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `add_node(nid: str)` — [`L993`](../../../../../raw/code/graphify/graphify/callflow_html.py#L993) — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `build_community_index(nodes: list)` — [`L637`](../../../../../raw/code/graphify/graphify/callflow_html.py#L637) — Map community_id (str) -> list of nodes. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `build_section_node_map(sections: list, comm_idx: dict)` — [`L886`](../../../../../raw/code/graphify/graphify/callflow_html.py#L886) — Map section_id -> list of nodes belonging to its communities.
- `classify_edges(edges: list, section_nodes_map: dict)` — [`L910`](../../../../../raw/code/graphify/graphify/callflow_html.py#L910) — Classify edges as intra-section or inter-section.
- `derive_flow_chain(sections: list, classified_edges: dict)` — [`L1357`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1357) — Derive a readable section flow from inter-section edges. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `derive_sections_from_communities(nodes: list, labels: dict, lang: str, max_sections: int)` — [`L831`](../../../../../raw/code/graphify/graphify/callflow_html.py#L831) — Derive architecture-oriented sections when no sections JSON is supplied. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `detect_lang(lang: str, nodes: list, labels: dict)` — [`L451`](../../../../../raw/code/graphify/graphify/callflow_html.py#L451) — Resolve auto language from labels and node names.
- `edge_score(edge: dict)` — [`L572`](../../../../../raw/code/graphify/graphify/callflow_html.py#L572) — Rank edges by confidence and usefulness for diagrams. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `endpoint_id(value)` — [`L131`](../../../../../raw/code/graphify/graphify/callflow_html.py#L131) — Normalize edge endpoints that may be strings or node-like objects. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `fallback_key(node: dict)` — [`L1019`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1019) — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `first_list(*values)` — [`L115`](../../../../../raw/code/graphify/graphify/callflow_html.py#L115) — Return the first list from a set of possible schema locations. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `first_present(mapping: dict, *keys, default=None)` — [`L107`](../../../../../raw/code/graphify/graphify/callflow_html.py#L107) — Return the first non-empty value for any candidate key. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `format_node_refs(node_ids: set, node_by_id: dict, lang: str, empty_text: str, limit: int = 3)` — [`L1191`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1191) — Render node references as readable labels instead of internal IDs. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `generate_call_table_rows(nodes: list, section_edges: list, lang: str)` — [`L1209`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1209) — Generate call table row scaffolding for a section's nodes. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `generate_header(sections: list, meta: dict, lang: str)` — [`L1330`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1330) — Generate the HTML header, title, subtitle, and nav. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `generate_nav(sections: list)` — [`L1175`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1175) — Generate the sticky navigation bar.
- `generate_overview_cards(meta: dict, report_text: str, sections: list, section_nodes_map: dict, classified_edges: dict, lang: str)` — [`L1389`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1389) — Generate generic overview cards. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `generate_overview_graph(sections: list, section_nodes_map: dict, classified_edges: dict, labels: dict, lang: str, diagram_scale: float)` — [`L1075`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1075) — Generate a readable section-level architecture overview. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `generate_section_cards(sec: dict, nodes: list, section_edges: list, lang: str)` — [`L1464`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1464) — Generate key file and design-note cards for a section. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `generate_section_flowchart(section_id: str, section_name: str, nodes: list, edges: list, lang: str, diagram_scale: float, max_nodes: int, max_edges: int)` — [`L1110`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1110) — Generate a compact, human-readable call-flow chart for a section. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `generate_section_intro(sec: dict, nodes: list, edge_count: int, lang: str)` — [`L1440`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1440) — Generate the section introductory paragraph. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `group_nodes_by_file(nodes: list)` — [`L1049`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1049) — Group selected nodes by source file for Mermaid subgraphs. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `html_anchor_id(raw: str, fallback: str, used: set)` — [`L646`](../../../../../raw/code/graphify/graphify/callflow_html.py#L646) — Generate a stable, unique HTML anchor ID.
- `html_comment_text(text: str)` — [`L358`](../../../../../raw/code/graphify/graphify/callflow_html.py#L358) — Keep generated HTML comments well-formed.
- `humanize_label(label: str, source_file: str = "")` — [`L471`](../../../../../raw/code/graphify/graphify/callflow_html.py#L471) — Convert graph labels into short labels people can scan in a diagram. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `infer_project_name(graph_path: str, meta: dict)` — [`L404`](../../../../../raw/code/graphify/graphify/callflow_html.py#L404) — Infer a display project name when graph metadata does not include one. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `is_zh(lang: str)` — [`L441`](../../../../../raw/code/graphify/graphify/callflow_html.py#L441) — Return true when localized strings should be Chinese. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `label_for_community(cid: str, labels: dict, nodes: list, lang: str)` — [`L701`](../../../../../raw/code/graphify/graphify/callflow_html.py#L701) — Choose a readable section name for a community. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `load_graph(path: str | Path)` — [`L255`](../../../../../raw/code/graphify/graphify/callflow_html.py#L255) — Load graph.json. Returns normalized (nodes, edges, hyperedges, metadata). — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `load_labels(path: str | Path | None)` — [`L298`](../../../../../raw/code/graphify/graphify/callflow_html.py#L298) — Load community labels from .graphify_labels.json, tolerating wrapper keys. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `load_report(path: str | Path | None)` — [`L325`](../../../../../raw/code/graphify/graphify/callflow_html.py#L325) — Load GRAPH_REPORT.md if it exists.
- `load_sections(path: str | Path | None)` — [`L315`](../../../../../raw/code/graphify/graphify/callflow_html.py#L315) — Load section definitions from JSON file. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `main()` — [`L1982`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1982) — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `mermaid_class_defs()` — [`L618`](../../../../../raw/code/graphify/graphify/callflow_html.py#L618) — Shared Mermaid-native styles for readable diagrams. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `mermaid_init(scale: float, direction: str = "LR")` — [`L589`](../../../../../raw/code/graphify/graphify/callflow_html.py#L589) — Return a Mermaid init directive that scales diagrams using Mermaid config. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `mermaid_section_id(section_id: str)` — [`L384`](../../../../../raw/code/graphify/graphify/callflow_html.py#L384) — Convert a section ID (like 'cli-entry') to a safe Mermaid ID (like 'CLI_ENTRY'). — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `node_degree_scores(edges: list)` — [`L963`](../../../../../raw/code/graphify/graphify/callflow_html.py#L963) — Score nodes by useful edge participation. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `node_display_name(node: dict | None, fallback: str = "")` — [`L1183`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1183) — Readable node label for tables and summaries. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `node_importance(node: dict)` — [`L973`](../../../../../raw/code/graphify/graphify/callflow_html.py#L973) — Use graphify centrality fields when available.
- `node_in_section(node_id: str, section_node_ids: set)` — [`L901`](../../../../../raw/code/graphify/graphify/callflow_html.py#L901) — Check if a node belongs to a section.
- `node_kind(node: dict)` — [`L487`](../../../../../raw/code/graphify/graphify/callflow_html.py#L487) — Classify a graph node for Mermaid styling and table tags. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `node_label(node: dict)` — [`L1040`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1040) — Build a readable Mermaid node label. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `node_mermaid_id(node: dict)` — [`L376`](../../../../../raw/code/graphify/graphify/callflow_html.py#L376) — Generate a safe Mermaid node ID from a graph node. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `normalize_communities(value)` — [`L666`](../../../../../raw/code/graphify/graphify/callflow_html.py#L666) — Normalize section community lists from JSON or simple strings.
- `normalize_edge(raw: dict, index: int)` — [`L201`](../../../../../raw/code/graphify/graphify/callflow_html.py#L201) — Normalize graphify edges while preserving original fields. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `normalize_node(raw: dict, index: int)` — [`L138`](../../../../../raw/code/graphify/graphify/callflow_html.py#L138) — Normalize a graphify node across common graph.json schema variants. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `normalize_sections(sections: list, lang: str)` — [`L677`](../../../../../raw/code/graphify/graphify/callflow_html.py#L677) — Ensure sections have safe unique IDs and an overview section first. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `pick_text(lang: str, zh: str, en: str)` — [`L446`](../../../../../raw/code/graphify/graphify/callflow_html.py#L446) — Small localization helper for generated copy. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `preferred_edges(edges: list, allow_structure: bool = False)` — [`L556`](../../../../../raw/code/graphify/graphify/callflow_html.py#L556) — Filter to edges that make a readable call-flow diagram. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `read_json(path: str | Path, default=None)` — [`L94`](../../../../../raw/code/graphify/graphify/callflow_html.py#L94) — Read JSON with a useful error message.
- `relation_label(relation: str, lang: str)` — [`L525`](../../../../../raw/code/graphify/graphify/callflow_html.py#L525) — Map graph edge relation names to short diagram labels. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `resolve_graphify_paths(args)` — [`L414`](../../../../../raw/code/graphify/graphify/callflow_html.py#L414) — Resolve project root, graphify output dir, and optional files. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `safe_file_path(path: str)` — [`L389`](../../../../../raw/code/graphify/graphify/callflow_html.py#L389) — Return a short, safe display path. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `safe_filename(text: str, fallback: str = "project")` — [`L398`](../../../../../raw/code/graphify/graphify/callflow_html.py#L398) — Create a conservative filename stem from a project name.
- `safe_mermaid_text(text: str)` — [`L336`](../../../../../raw/code/graphify/graphify/callflow_html.py#L336) — Sanitize text for use inside a Mermaid node label. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `section_edge_summary(classified_edges: dict)` — [`L1058`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1058) — Aggregate inter-section edge counts and relation names. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `section_keywords(nodes: list, limit: int = 5)` — [`L1422`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1422) — Pick representative words from labels and file names.
- `select_diagram_nodes(nodes: list, edges: list, max_nodes: int)` — [`L981`](../../../../../raw/code/graphify/graphify/callflow_html.py#L981) — Select a compact, connected subset of nodes for readable diagrams. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `should_include_edge(edge: dict)` — [`L946`](../../../../../raw/code/graphify/graphify/callflow_html.py#L946) — Decide whether to auto-include an edge in Mermaid output. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `stable_ascii_id(raw: str, prefix: str = "node", limit: int = 48)` — [`L363`](../../../../../raw/code/graphify/graphify/callflow_html.py#L363) — Build a Mermaid-safe ASCII identifier with a hash suffix to avoid collisions.
- `to_float(value, default: float = 0)` — [`L123`](../../../../../raw/code/graphify/graphify/callflow_html.py#L123) — Convert graph numeric fields that may be serialized as strings. — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `truncate_text(text: str, limit: int)` — [`L463`](../../../../../raw/code/graphify/graphify/callflow_html.py#L463) — Truncate without splitting Mermaid syntax.
- `write_callflow_html(project: str | Path | None = None, *, graphify_out: str | Path | None = None, graph: str | Path | None = None, report: str | Path | None = None, labels: str | Path | None = None, sections: str | Path | None = None, output: str | Path | None = None, lang: str = "auto", max_sections: int = 15, diagram_scale: float = 1, max_diagram_nodes: int = 18, max_diagram_edges: int = 24, verbose: bool = False)` — [`L1579`](../../../../../raw/code/graphify/graphify/callflow_html.py#L1579) — Generate call-flow architecture HTML from graphify output files. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)

## Module values
- `CSS` — [`L40`](../../../../../raw/code/graphify/graphify/callflow_html.py#L40)
- `SECTION_ARCHETYPES` — [`L711`](../../../../../raw/code/graphify/graphify/callflow_html.py#L711)

