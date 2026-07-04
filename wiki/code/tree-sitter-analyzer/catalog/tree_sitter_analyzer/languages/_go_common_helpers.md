---
title: 'Module: tree_sitter_analyzer/languages/_go_common_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_go_common_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._go_common_helpers`/
symbols:
  extract_method_receiver: extract_method_receiver().
  _strip_generic_suffix: _strip_generic_suffix().
  extract_docstring: extract_docstring().
  extract_parameters: extract_parameters().
  _extract_receiver_from_text: _extract_receiver_from_text().
  _extract_receiver_parts: _extract_receiver_parts().
  go_visibility: go_visibility().
  extract_return_type: extract_return_type().
  _docstring_scan_start: _docstring_scan_start().
  _collect_docstring_lines: _collect_docstring_lines().
---
# Module: [`tree_sitter_analyzer/languages/_go_common_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_common_helpers.py)

## Functions
- `_collect_docstring_lines(content_lines: list[str], scan_start: int)` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_common_helpers.py#L50)
- `_docstring_scan_start(node: Any, content_lines: list[str])` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_common_helpers.py#L43)
- `_extract_receiver_from_text(receiver_text: str)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_common_helpers.py#L113) — Parse a raw receiver tuple text like ``(p *Stack[T])``.
- `_extract_receiver_parts(parameter_node: Any, get_node_text: Callable[..., str])` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_common_helpers.py#L88) — Extract ``(name, normalized_type)`` from a Go ``parameter_declaration``.
- `_strip_generic_suffix(receiver_type: str)` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_common_helpers.py#L139) — Strip trailing Go type arguments like ``[T]`` or ``[A, B]``.
- `extract_docstring(node: Any, content_lines: list[str])` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_common_helpers.py#L33) — Extract doc comments preceding the node.
- `extract_method_receiver(node: Any, get_node_text: Callable[..., str])` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_common_helpers.py#L62) — Extract method receiver name and type.
- `extract_parameters(node: Any, get_node_text: Callable[..., str])` — [`L7`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_common_helpers.py#L7) — Extract function/method parameters.
- `extract_return_type(node: Any, get_node_text: Callable[..., str])` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_common_helpers.py#L25) — Extract function/method return type.
- `go_visibility(name: str)` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_common_helpers.py#L168)

