---
title: 'Module: tree_sitter_analyzer/languages/_cpp_signature_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_cpp_signature_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._cpp_signature_helpers`/
symbols:
  _apply_signature_child: _apply_signature_child().
  parse_function_signature: parse_function_signature().
  _merge_declarator: _merge_declarator().
  extract_parameters: extract_parameters().
  extract_comment_for_line: extract_comment_for_line().
  _SignatureParts.return_type: _SignatureParts#return_type.
  _merge_nested_declarator: _merge_nested_declarator().
  _SignatureParts.modifiers: _SignatureParts#modifiers.
  _TYPE_NODES_CPP: _TYPE_NODES_CPP.
  _SignatureParts: _SignatureParts#
  _SignatureParts.name: _SignatureParts#name.
  _SignatureParts.parameters: _SignatureParts#parameters.
  _append_declarator_symbol: _append_declarator_symbol().
  _append_unique: _append_unique().
  _FUNCTION_NAME_NODES: _FUNCTION_NAME_NODES.
  _collect_block_comment: _collect_block_comment().
  _append_text_modifier: _append_text_modifier().
---
# Module: [`tree_sitter_analyzer/languages/_cpp_signature_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_signature_helpers.py)

## Classes
### `_SignatureParts`
- def: [`tree_sitter_analyzer/languages/_cpp_signature_helpers.py:29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_signature_helpers.py#L29)
- signature: `class _SignatureParts:`
- members:
  - `modifiers` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_signature_helpers.py#L33)
  - `name` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_signature_helpers.py#L30)
  - `parameters` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_signature_helpers.py#L32)
  - `return_type` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_signature_helpers.py#L31)
- used by: [`_apply_signature_child`](_cpp_signature_helpers.md#_apply_signature_child), [`parse_function_signature`](_cpp_signature_helpers.md#parse_function_signature), [`_merge_declarator`](_cpp_signature_helpers.md#_merge_declarator), [`_merge_nested_declarator`](_cpp_signature_helpers.md#_merge_nested_declarator)

## Functions
- `_append_declarator_symbol(return_type: str, symbol: str)` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_signature_helpers.py#L149)
- `_append_text_modifier(modifiers: list[str], node: Any, get_node_text: Callable[..., str])` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_signature_helpers.py#L177)
- `_append_unique(modifiers: list[str], modifier: str)` — [`L185`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_signature_helpers.py#L185)
- `_apply_signature_child(child: Any, parts: _SignatureParts, get_node_text: Callable[..., str], extract_params_fn: Callable[[Any], list[str]])` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_signature_helpers.py#L105)
- `_collect_block_comment(start: int, end: int, content_lines: list[str])` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_signature_helpers.py#L52)
- `_merge_declarator(parts: _SignatureParts, declarator: Any, get_node_text: Callable[..., str], extract_params_fn: Callable[[Any], list[str]])` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_signature_helpers.py#L164)
- `_merge_nested_declarator(parts: _SignatureParts, declarator: Any, get_node_text: Callable[..., str], extract_params_fn: Callable[[Any], list[str]])` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_signature_helpers.py#L153)
- `extract_comment_for_line(line: int, content_lines: list[str])` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_signature_helpers.py#L36) — Extract comment documentation for a source line.
- `extract_parameters(params_node: Any, get_node_text: Callable[..., str])` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_signature_helpers.py#L62) — Extract function parameters.
- `parse_function_signature(node: Any, get_node_text: Callable[..., str], extract_params_fn: Callable[[Any], list[str]])` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_signature_helpers.py#L87) — Parse a C++ function signature.

## Module values
- `_FUNCTION_NAME_NODES` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_signature_helpers.py#L17)
- `_TYPE_NODES_CPP` — [`L9`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_signature_helpers.py#L9)

