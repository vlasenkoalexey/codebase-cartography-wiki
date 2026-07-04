---
title: 'Module: src/codegraphcontext/cli/visualizer.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/cli/visualizer.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.cli.visualizer`/
symbols:
  check_visual_flag: check_visual_flag().
  visualize_search_results: visualize_search_results().
  _launch_visualizer: _launch_visualizer().
  visualize_call_graph: visualize_call_graph().
  visualize_call_chain: visualize_call_chain().
  visualize_dependencies: visualize_dependencies().
  visualize_inheritance_tree: visualize_inheritance_tree().
  visualize_overrides: visualize_overrides().
  _file_props: _file_props().
  _escape_cypher_string: _escape_cypher_string().
  visualize_cypher_results: visualize_cypher_results().
  _validate_graph_label: _validate_graph_label().
  ALLOWED_GRAPH_LABELS: ALLOWED_GRAPH_LABELS.
  resolve_visual_flag: resolve_visual_flag().
---
# Module: [`src/codegraphcontext/cli/visualizer.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/visualizer.py)

## Functions
- `_escape_cypher_string(value: str)` — [`L31`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/visualizer.py#L31)
- `_file_props(name: str, file: Optional[str])` — [`L48`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/visualizer.py#L48)
- `_launch_visualizer(cypher_query: str, *, repo_path: Optional[str] = None, context: Optional[str] = None)` — [`L56`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/visualizer.py#L56)
- `_validate_graph_label(label: str)` — [`L35`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/visualizer.py#L35)
- `check_visual_flag(ctx: Any, visual: bool)` — [`L18`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/visualizer.py#L18) — Return whether visualization was requested (does not launch UI).
- `resolve_visual_flag(ctx: Any, visual: bool)` — [`L10`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/visualizer.py#L10) — True when local or global --visual / -V was requested.
- `visualize_call_chain(_results: Any, from_func: str, to_func: str, max_depth: int = 5, from_file: Optional[str] = None, to_file: Optional[str] = None, **_: Any)` — [`L120`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/visualizer.py#L120)
- `visualize_call_graph(_results: Any, function: str, direction: str = "outgoing", file: Optional[str] = None, **_: Any)` — [`L99`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/visualizer.py#L99)
- `visualize_cypher_results(cypher_query: str, **_: Any)` — [`L188`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/visualizer.py#L188)
- `visualize_dependencies(_results: Any, target: str, **_: Any)` — [`L143`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/visualizer.py#L143)
- `visualize_inheritance_tree(_results: Any, class_name: str, file: Optional[str] = None, **_: Any)` — [`L157`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/visualizer.py#L157)
- `visualize_overrides(_results: Any, function_name: str, **_: Any)` — [`L175`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/visualizer.py#L175)
- `visualize_search_results(_results: Any, name: str, search_type: str = "name", **_: Any)` — [`L70`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/visualizer.py#L70)

## Module values
- `ALLOWED_GRAPH_LABELS` — [`L23`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/visualizer.py#L23)

