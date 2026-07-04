---
title: 'Module: tree_sitter_analyzer/languages/_go_function_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_go_function_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._go_function_helpers`/
symbols:
  _build_go_function: _build_go_function().
  extract_go_method: extract_go_method().
  extract_go_interface_methods: extract_go_interface_methods().
  extract_go_function: extract_go_function().
  _go_calculate_complexity: _go_calculate_complexity().
  _go_function_name: _go_function_name().
  _GO_DECISION_NODE_TYPES._GO_DECISION_NODE_TYPES: _GO_DECISION_NODE_TYPES._GO_DECISION_NODE_TYPES.
---
# Module: [`tree_sitter_analyzer/languages/_go_function_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_function_helpers.py)

## Functions
- `_build_go_function(name: str, node: Any, get_node_text: Callable[..., str], content_lines: list[str])` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_function_helpers.py#L140)
- `_go_calculate_complexity(node: Any)` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_function_helpers.py#L33) — Return cyclomatic complexity (1 + decision points) for a Go function node.
- `_go_function_name(node: Any, get_node_text: Callable[..., str])` — [`L133`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_function_helpers.py#L133)
- `extract_go_function(node: Any, get_node_text: Callable[..., str], content_lines: list[str])` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_function_helpers.py#L49) — Extract Go function declaration.
- `extract_go_interface_methods(type_spec_node: Any, get_node_text: Callable[..., str], content_lines: list[str])` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_function_helpers.py#L88) — Extract interface method signatures as Functions owned by the interface.
- `extract_go_method(node: Any, get_node_text: Callable[..., str], content_lines: list[str])` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_function_helpers.py#L66) — Extract Go method declaration (function with receiver).

## Module values
- `_GO_DECISION_NODE_TYPES` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_function_helpers.py#L20)

