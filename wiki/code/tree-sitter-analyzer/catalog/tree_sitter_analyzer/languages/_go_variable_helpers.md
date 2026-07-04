---
title: 'Module: tree_sitter_analyzer/languages/_go_variable_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_go_variable_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._go_variable_helpers`/
symbols:
  _extract_one_field: _extract_one_field().
  _build_go_variable: _build_go_variable().
  extract_var_spec: extract_var_spec().
  extract_var_or_const: extract_var_or_const().
  extract_struct_fields: extract_struct_fields().
  _go_var_names_and_type: _go_var_names_and_type().
  _GO_VAR_TYPE_NODES: _GO_VAR_TYPE_NODES.
  _iter_var_const_specs: _iter_var_const_specs().
  _GO_FIELD_TYPE_NODES: _GO_FIELD_TYPE_NODES.
---
# Module: [`tree_sitter_analyzer/languages/_go_variable_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_variable_helpers.py)

## Functions
- `_build_go_variable(name: str, node: Any, raw_text: str, var_type: str, is_const: bool)` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_variable_helpers.py#L70)
- `_extract_one_field(field_node: Any, struct_name: str, get_node_text: Callable[..., str])` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_variable_helpers.py#L154) — Extract a single field_declaration into a Variable.
- `_go_var_names_and_type(node: Any, get_node_text: Callable[..., str])` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_variable_helpers.py#L53)
- `_iter_var_const_specs(node: Any)` — [`L108`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_variable_helpers.py#L108)
- `extract_struct_fields(type_declaration_node: Any, get_node_text: Callable[..., str])` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_variable_helpers.py#L114) — Extract field declarations from a Go struct type_declaration node.
- `extract_var_or_const(node: Any, is_const: bool, get_node_text: Callable[..., str])` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_variable_helpers.py#L90) — Extract var or const declaration.
- `extract_var_spec(node: Any, is_const: bool, get_node_text: Callable[..., str])` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_variable_helpers.py#L34) — Extract single var/const spec.

## Module values
- `_GO_FIELD_TYPE_NODES` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_variable_helpers.py#L10)
- `_GO_VAR_TYPE_NODES` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_variable_helpers.py#L23)

