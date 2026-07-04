---
title: 'Module: understand-anything-plugin/skills/understand/merge-subdomain-graphs.py'
type: catalog
provenance: extracted
module: understand-anything-plugin/skills/understand/merge-subdomain-graphs.py
status: fresh
symbol_base: scip-python python understand-anything 0.0.0 `understand-anything-plugin.skills.understand.merge-subdomain-graphs`/
symbols:
  main: main().
  merge_graphs: merge_graphs().
  _num: _num().
  load_graph: load_graph().
---
# Module: [`understand-anything-plugin/skills/understand/merge-subdomain-graphs.py`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-subdomain-graphs.py)

## Functions
- `_num(v: Any)` — [`L28`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-subdomain-graphs.py#L28) — Coerce a value to float for safe comparison (handles string weights).
- `load_graph(path: Path)` — [`L36`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-subdomain-graphs.py#L36) — Load and minimally validate a knowledge graph JSON file.
- `main()` — [`L235`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-subdomain-graphs.py#L235)
- `merge_graphs(graphs: list[dict[str, Any]])` — [`L52`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-subdomain-graphs.py#L52) — Merge multiple knowledge graph dicts into one. Returns (merged, report_lines).

