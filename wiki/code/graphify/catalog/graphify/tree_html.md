---
title: 'Module: graphify/tree_html.py'
type: catalog
provenance: extracted
module: graphify/tree_html.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.tree_html`/
symbols:
  build_tree: build_tree().
  write_tree_html: write_tree_html().
  build_tree._ensure_dir: build_tree()._ensure_dir().
  build_tree._finalise: build_tree()._finalise().
  DEFAULT_MAX_CHILDREN: DEFAULT_MAX_CHILDREN.
  emit_html: emit_html().
  _common_root: _common_root().
  _make_truncation_leaf: _make_truncation_leaf().
  _HTML_TEMPLATE: _HTML_TEMPLATE.
---
# Module: [`graphify/tree_html.py`](../../../../../raw/code/graphify/graphify/tree_html.py)

## Functions
- `_common_root(paths: List[str])` — [`L49`](../../../../../raw/code/graphify/graphify/tree_html.py#L49)
- `_ensure_dir(abs_path: Path)` — [`L102`](../../../../../raw/code/graphify/graphify/tree_html.py#L102)
- `_finalise(d: Dict[str, Any])` — [`L154`](../../../../../raw/code/graphify/graphify/tree_html.py#L154)
- `_make_truncation_leaf(extra: int)` — [`L64`](../../../../../raw/code/graphify/graphify/tree_html.py#L64)
- `build_tree(graph: Dict[str, Any], *, root: Optional[str] = None, max_children: int = DEFAULT_MAX_CHILDREN, project_label: Optional[str] = None)` — [`L68`](../../../../../raw/code/graphify/graphify/tree_html.py#L68) — Build a ``{name, total_count, children}`` hierarchy.
- `emit_html(tree: Dict[str, Any], *, title: str, header: str, svg_width: int = 6000, svg_height: int = 8000)` — [`L542`](../../../../../raw/code/graphify/graphify/tree_html.py#L542)
- `write_tree_html(graph_path: Path, output_path: Path, *, root: Optional[str] = None, max_children: int = DEFAULT_MAX_CHILDREN, project_label: Optional[str] = None, top_k_edges: int = 0)` — [`L562`](../../../../../raw/code/graphify/graphify/tree_html.py#L562) — documented in [graphify-security](../../concepts/graphify-security.md)

## Module values
- `DEFAULT_MAX_CHILDREN` — [`L43`](../../../../../raw/code/graphify/graphify/tree_html.py#L43)
- `_HTML_TEMPLATE` — [`L176`](../../../../../raw/code/graphify/graphify/tree_html.py#L176)

