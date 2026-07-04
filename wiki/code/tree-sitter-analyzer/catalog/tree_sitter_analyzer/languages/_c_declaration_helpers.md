---
title: 'Module: tree_sitter_analyzer/languages/_c_declaration_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_c_declaration_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._c_declaration_helpers`/
symbols:
  _variable: _variable().
  _field_variable: _field_variable().
  extract_field_declaration: extract_field_declaration().
  extract_variable_declaration: extract_variable_declaration().
  _field_parts: _field_parts().
  _variable_parts: _variable_parts().
  _append_child_names: _append_child_names().
  _append_array_fields: _append_array_fields().
  _append_initializer_fields: _append_initializer_fields().
  _append_pointer_fields: _append_pointer_fields().
  _append_pointer_variables: _append_pointer_variables().
  _node_line_range: _node_line_range().
  _append_modifier: _append_modifier().
  _append_nonempty_name: _append_nonempty_name().
  _TYPE_NODES_FIELD: _TYPE_NODES_FIELD.
  _TYPE_NODES_VAR: _TYPE_NODES_VAR.
---
# Module: [`tree_sitter_analyzer/languages/_c_declaration_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_declaration_helpers.py)

## Functions
- `_append_array_fields(node: Any, field_names: list[str], field_type: str | None, get_node_text: Callable[..., str])` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_declaration_helpers.py#L142)
- `_append_child_names(node: Any, names: list[str], node_type: str, get_node_text: Callable[..., str])` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_declaration_helpers.py#L182)
- `_append_initializer_fields(node: Any, field_names: list[str], get_node_text: Callable[..., str])` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_declaration_helpers.py#L152)
- `_append_modifier(modifiers: list[str], node: Any, get_node_text: Callable[..., str])` — [`L205`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_declaration_helpers.py#L205)
- `_append_nonempty_name(names: list[str], node: Any, get_node_text: Callable[..., str])` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_declaration_helpers.py#L195)
- `_append_pointer_fields(node: Any, field_names: list[str], field_type: str | None, get_node_text: Callable[..., str])` — [`L160`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_declaration_helpers.py#L160)
- `_append_pointer_variables(node: Any, var_names: list[str], var_type: str | None, get_node_text: Callable[..., str])` — [`L171`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_declaration_helpers.py#L171)
- `_field_parts(node: Any, get_node_text: Callable[..., str])` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_declaration_helpers.py#L90)
- `_field_variable(name: str, start_line: int, end_line: int, raw_text: str, field_type: str, modifiers: list[str])` — [`L213`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_declaration_helpers.py#L213)
- `_node_line_range(node: Any)` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_declaration_helpers.py#L86)
- `_variable(name: str, start_line: int, end_line: int, raw_text: str, var_type: str, modifiers: list[str], visibility: str)` — [`L234`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_declaration_helpers.py#L234)
- `_variable_parts(node: Any, get_node_text: Callable[..., str])` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_declaration_helpers.py#L118)
- `extract_field_declaration(node: Any, get_node_text: Callable[..., str])` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_declaration_helpers.py#L32) — Extract struct/union field declarations.
- `extract_variable_declaration(node: Any, get_node_text: Callable[..., str])` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_declaration_helpers.py#L54) — Extract C variable declarations (not struct members).

## Module values
- `_TYPE_NODES_FIELD` — [`L9`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_declaration_helpers.py#L9)
- `_TYPE_NODES_VAR` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_declaration_helpers.py#L20)

