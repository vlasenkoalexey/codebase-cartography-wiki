---
title: 'Module: tree_sitter_analyzer/languages/_cpp_field_function_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_cpp_field_function_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._cpp_field_function_helpers`/
symbols:
  extract_function_from_field_declaration: extract_function_from_field_declaration().
  extract_function_declaration: extract_function_declaration().
  _field_function_context: _field_function_context().
  _apply_field_function_child: _apply_field_function_child().
  _merge_field_function_declarator: _merge_field_function_declarator().
  CppFieldFunctionExtractionContext: CppFieldFunctionExtractionContext#
  _FieldFunctionParts.modifiers: _FieldFunctionParts#modifiers.
  _field_function_parts: _field_function_parts().
  _FieldFunctionParts: _FieldFunctionParts#
  _FieldFunctionParts.name: _FieldFunctionParts#name.
  CppFieldFunctionExtractionContext.get_node_text: CppFieldFunctionExtractionContext#get_node_text.
  CppFieldFunctionExtractionContext.extract_parameters: CppFieldFunctionExtractionContext#extract_parameters.
  CppFieldFunctionExtractionContext.is_global_scope: CppFieldFunctionExtractionContext#is_global_scope.
  CppFieldFunctionExtractionContext.determine_visibility: CppFieldFunctionExtractionContext#determine_visibility.
  CppFieldFunctionExtractionContext.extract_comment_for_line: CppFieldFunctionExtractionContext#extract_comment_for_line.
  _append_unique: _append_unique().
  _FieldFunctionParts.return_type: _FieldFunctionParts#return_type.
  _FieldFunctionParts.parameters: _FieldFunctionParts#parameters.
  _FIELD_FUNCTION_NAME_NODES: _FIELD_FUNCTION_NAME_NODES.
  _append_text_modifier: _append_text_modifier().
  _function_declaration_parts: _function_declaration_parts().
---
# Module: [`tree_sitter_analyzer/languages/_cpp_field_function_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py)

## Classes
### `CppFieldFunctionExtractionContext`
- def: [`tree_sitter_analyzer/languages/_cpp_field_function_helpers.py:25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L25)
- signature: `class CppFieldFunctionExtractionContext:`
- members:
  - `determine_visibility` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L29)
  - `extract_comment_for_line` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L30)
  - `extract_parameters` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L27)
  - `get_node_text` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L26)
  - `is_global_scope` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L28)
- used by: [`extract_function_from_field_declaration`](_cpp_field_function_helpers.md#extract_function_from_field_declaration), [`_extract_function_from_field_declaration`](cpp_plugin.md#CppElementExtractor._extract_function_from_field_declaration), [`_field_function_context`](_cpp_field_function_helpers.md#_field_function_context)

### `_FieldFunctionParts`
- def: [`tree_sitter_analyzer/languages/_cpp_field_function_helpers.py:17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L17)
- signature: `class _FieldFunctionParts:`
- members:
  - `modifiers` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L21)
  - `name` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L18)
  - `parameters` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L20)
  - `return_type` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L19)
- used by: [`extract_function_from_field_declaration`](_cpp_field_function_helpers.md#extract_function_from_field_declaration), [`_apply_field_function_child`](_cpp_field_function_helpers.md#_apply_field_function_child), [`_merge_field_function_declarator`](_cpp_field_function_helpers.md#_merge_field_function_declarator), [`_field_function_parts`](_cpp_field_function_helpers.md#_field_function_parts)

## Functions
- `_append_text_modifier(modifiers: list[str], node: Any, get_node_text: Callable[..., str])` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L145)
- `_append_unique(modifiers: list[str], modifier: str)` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L153)
- `_apply_field_function_child(child: Any, parts: _FieldFunctionParts, get_node_text: Callable[..., str], extract_params_fn: Callable[[Any], list[str]])` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L105)
- `_field_function_context(context: CppFieldFunctionExtractionContext | Callable[..., str], *legacy_args: Any)` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L75)
- `_field_function_parts(node: Any, get_node_text: Callable[..., str], extract_params_fn: Callable[[Any], list[str]])` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L94)
- `_function_declaration_parts(node: Any, get_node_text: Callable[..., str], extract_params_fn: Callable[[Any], list[str]])` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L194)
- `_merge_field_function_declarator(parts: _FieldFunctionParts, declarator: Any, get_node_text: Callable[..., str], extract_params_fn: Callable[[Any], list[str]])` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L130)
- `extract_function_declaration(node: Any, get_node_text: Callable[..., str], extract_params_fn: Callable[[Any], list[str]])` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L158) — Extract a C++ function declaration or prototype.
- `extract_function_from_field_declaration(node: Any, context: CppFieldFunctionExtractionContext | Callable[..., str], *legacy_args: Any)` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L33) — Extract a C++ function from a field declaration.

## Module values
- `_FIELD_FUNCTION_NAME_NODES` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_field_function_helpers.py#L11)

