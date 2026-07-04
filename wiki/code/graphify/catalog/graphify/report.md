---
title: 'Module: graphify/report.py'
type: catalog
provenance: extracted
module: graphify/report.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.report`/
symbols:
  generate: generate().
  load_learning_for_report: load_learning_for_report().
  _safe_community_name: _safe_community_name().
  _learning_section: _learning_section().
---
# Module: [`graphify/report.py`](../../../../../raw/code/graphify/graphify/report.py)

## Functions
- `_learning_section(lines: list, learning: dict | None, top_n: int = 10)` — [`L40`](../../../../../raw/code/graphify/graphify/report.py#L40) — Append the ``## Work-memory lessons`` section, or nothing when empty.
- `_safe_community_name(label: str)` — [`L8`](../../../../../raw/code/graphify/graphify/report.py#L8) — Mirrors export.safe_name so community hub filenames and report wikilinks always agree.
- `generate(G: nx.Graph, communities: dict[int, list[str]], cohesion_scores: dict[int, float], community_labels: dict[int, str], god_node_list: list[dict], surprise_list: list[dict], detection_result: dict, token_cost: dict, root: str, suggested_questions: list[dict] | None = None, min_community_size: int = 3, built_at_commit: str | None = None, learning: dict | None = None)` — [`L71`](../../../../../raw/code/graphify/graphify/report.py#L71) — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `load_learning_for_report(graph_path)` — [`L15`](../../../../../raw/code/graphify/graphify/report.py#L15) — Assemble the report's work-memory inputs from sibling artifacts. — documented in [graphify-reflect](../../concepts/graphify-reflect.md)

