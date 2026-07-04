---
title: 'Module: tree_sitter_analyzer/mcp/tools/_call_tree.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/_call_tree.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools._call_tree`/
symbols:
  build_call_tree: build_call_tree().
  DEFAULT_MAX_NODES: DEFAULT_MAX_NODES.
  build_call_tree._dfs: build_call_tree()._dfs().
  DEFAULT_MAX_DEPTH: DEFAULT_MAX_DEPTH.
  Expander: Expander.
  MAX_DEPTH_CAP: MAX_DEPTH_CAP.
  _node_key: _node_key().
---
# Module: [`tree_sitter_analyzer/mcp/tools/_call_tree.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree.py)

## Functions
- `_dfs(node: dict[str, Any], name: str, file: str | None, remaining: int, path: set[str])` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree.py#L88)
- `_node_key(name: str, file: str | None)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree.py#L42)
- `build_call_tree(root_name: str, root_file: str | None, expand: Expander, *, max_depth: int = DEFAULT_MAX_DEPTH, max_nodes: int = DEFAULT_MAX_NODES, children_key: str = "children")` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree.py#L46) — Build a depth-limited nested call tree from ``root_name``.

## Module values
- `DEFAULT_MAX_DEPTH` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree.py#L33)
- `DEFAULT_MAX_NODES` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree.py#L39)
- `Expander` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree.py#L31)
- `MAX_DEPTH_CAP` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree.py#L34)

