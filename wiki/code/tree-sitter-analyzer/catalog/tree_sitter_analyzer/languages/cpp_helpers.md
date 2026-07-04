---
title: 'Module: tree_sitter_analyzer/languages/cpp_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/cpp_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.cpp_helpers`/
symbols:
  get_access_specifier: get_access_specifier().
  determine_visibility: determine_visibility().
  _VALID_SPECS: _VALID_SPECS.
  _default_class_access: _default_class_access().
  is_global_scope: is_global_scope().
  _EXPLICIT_VISIBILITY: _EXPLICIT_VISIBILITY.
  _CLASS_DEFAULT_ACCESS._CLASS_DEFAULT_ACCESS: _CLASS_DEFAULT_ACCESS._CLASS_DEFAULT_ACCESS.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/languages/cpp_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_helpers.py)

## Functions
- `_default_class_access(class_node: Any)` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_helpers.py#L91) — Return the default access specifier for a class/struct/union node.
- `determine_visibility(modifiers: list[str], is_global: bool = False, node: Any = None, get_node_text: Callable[..., str] | None = None)` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_helpers.py#L123) — Determine visibility from modifiers and context.
- `get_access_specifier(node: Any, get_node_text: Callable[..., str])` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_helpers.py#L98) — Get the current access specifier for a class member.
- `is_global_scope(node: Any)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_helpers.py#L68) — Check if a node is in global scope (not inside a class/struct/union).

## Module values
- `_CLASS_DEFAULT_ACCESS` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_helpers.py#L84)
- `_EXPLICIT_VISIBILITY` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_helpers.py#L82)
- `_VALID_SPECS` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_helpers.py#L83)
- `__all__` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_helpers.py#L40)

