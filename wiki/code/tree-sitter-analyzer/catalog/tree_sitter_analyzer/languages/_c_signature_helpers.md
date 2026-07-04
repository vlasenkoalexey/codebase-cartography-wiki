---
title: 'Module: tree_sitter_analyzer/languages/_c_signature_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_c_signature_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._c_signature_helpers`/
symbols:
  parse_function_signature: parse_function_signature().
  _find_function_declarator: _find_function_declarator().
  _pointer_return_type: _pointer_return_type().
  _function_declarator_info: _function_declarator_info().
  _append_modifier: _append_modifier().
  _RETURN_TYPE_NODES: _RETURN_TYPE_NODES.
  _MODIFIER_NODES: _MODIFIER_NODES.
---
# Module: [`tree_sitter_analyzer/languages/_c_signature_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_signature_helpers.py)

## Functions
- `_append_modifier(modifiers: list[str], node: Any, get_node_text: Callable[..., str])` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_signature_helpers.py#L93)
- `_find_function_declarator(node: Any, get_node_text: Callable[..., str], extract_params_fn: Callable[[Any], list[str]])` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_signature_helpers.py#L70)
- `_function_declarator_info(node: Any, get_node_text: Callable[..., str], extract_params_fn: Callable[[Any], list[str]])` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_signature_helpers.py#L55)
- `_pointer_return_type(return_type: str)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_signature_helpers.py#L87)
- `parse_function_signature(node: Any, get_node_text: Callable[..., str], extract_params_fn: Callable[[Any], list[str]])` — [`L7`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_signature_helpers.py#L7) — Parse C function signature.

## Module values
- `_MODIFIER_NODES` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_signature_helpers.py#L52)
- `_RETURN_TYPE_NODES` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_signature_helpers.py#L44)

