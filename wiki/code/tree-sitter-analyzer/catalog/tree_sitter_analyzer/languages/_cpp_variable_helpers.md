---
title: 'Module: tree_sitter_analyzer/languages/_cpp_variable_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_cpp_variable_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._cpp_variable_helpers`/
symbols:
  _build_variables: _build_variables().
  _apply_variable_child: _apply_variable_child().
  extract_cpp_field_declaration: extract_cpp_field_declaration().
  extract_cpp_variable_declaration: extract_cpp_variable_declaration().
  extract_base_classes: extract_base_classes().
  _variable_parts: _variable_parts().
  _VariableParts.names: _VariableParts#names.
  _VariableParts.modifiers: _VariableParts#modifiers.
  _VariableParts: _VariableParts#
  _VariableParts.type_name: _VariableParts#type_name.
  _base_specifier_names: _base_specifier_names().
  _init_declarator_names: _init_declarator_names().
  _BASE_NAME_NODE_TYPES: _BASE_NAME_NODE_TYPES.
  _append_nonempty_name: _append_nonempty_name().
  _TYPE_NODES_CPP: _TYPE_NODES_CPP.
  _append_text_modifier: _append_text_modifier().
---
# Module: [`tree_sitter_analyzer/languages/_cpp_variable_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_variable_helpers.py)

## Classes
### `_VariableParts`
- def: [`tree_sitter_analyzer/languages/_cpp_variable_helpers.py:22`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_variable_helpers.py#L22)
- signature: `class _VariableParts:`
- members:
  - `modifiers` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_variable_helpers.py#L25)
  - `names` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_variable_helpers.py#L24)
  - `type_name` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_variable_helpers.py#L23)
- used by: [`_build_variables`](_cpp_variable_helpers.md#_build_variables), [`_apply_variable_child`](_cpp_variable_helpers.md#_apply_variable_child), [`extract_cpp_field_declaration`](_cpp_variable_helpers.md#extract_cpp_field_declaration), [`extract_cpp_variable_declaration`](_cpp_variable_helpers.md#extract_cpp_variable_declaration), [`_variable_parts`](_cpp_variable_helpers.md#_variable_parts)

## Functions
- `_append_nonempty_name(names: list[str], node: Any, get_node_text: Callable[..., str])` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_variable_helpers.py#L149)
- `_append_text_modifier(modifiers: list[str], node: Any, get_node_text: Callable[..., str])` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_variable_helpers.py#L129)
- `_apply_variable_child(child: Any, parts: _VariableParts, get_node_text: Callable[..., str], declarator_name_types: tuple[str, ...])` — [`L111`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_variable_helpers.py#L111)
- `_base_specifier_names(node: Any, get_node_text: Callable[..., str])` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_variable_helpers.py#L49)
- `_build_variables(node: Any, parts: _VariableParts, get_node_text: Callable[..., str], is_global_fn: Callable[[Any], bool], determine_vis_fn: Callable[..., str])` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_variable_helpers.py#L159)
- `_init_declarator_names(node: Any, get_node_text: Callable[..., str], declarator_name_types: tuple[str, ...])` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_variable_helpers.py#L137)
- `_variable_parts(node: Any, get_node_text: Callable[..., str], declarator_name_types: tuple[str, ...])` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_variable_helpers.py#L100)
- `extract_base_classes(node: Any, get_node_text: Callable[..., str])` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_variable_helpers.py#L31) — Extract base class names from base_class_clause.
- `extract_cpp_field_declaration(node: Any, get_node_text: Callable[..., str], is_global_fn: Callable[[Any], bool], determine_vis_fn: Callable[..., str])` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_variable_helpers.py#L57) — Extract C++ field declarations.
- `extract_cpp_variable_declaration(node: Any, get_node_text: Callable[..., str], is_global_fn: Callable[[Any], bool], determine_vis_fn: Callable[..., str])` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_variable_helpers.py#L77) — Extract C++ variable declarations outside class member lists.

## Module values
- `_BASE_NAME_NODE_TYPES` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_variable_helpers.py#L28)
- `_TYPE_NODES_CPP` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_variable_helpers.py#L10)

