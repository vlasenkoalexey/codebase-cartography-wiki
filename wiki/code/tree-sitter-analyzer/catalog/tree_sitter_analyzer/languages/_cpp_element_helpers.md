---
title: 'Module: tree_sitter_analyzer/languages/_cpp_element_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_cpp_element_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._cpp_element_helpers`/
symbols:
  extract_cpp_function: extract_cpp_function().
  extract_cpp_class: extract_cpp_class().
  _function_context: _function_context().
  _class_context: _class_context().
  _cpp_direct_parent_class_name: _cpp_direct_parent_class_name().
  CppFunctionExtractionContext: CppFunctionExtractionContext#
  CppClassExtractionContext: CppClassExtractionContext#
  _is_cpp_constructor: _is_cpp_constructor().
  _cpp_containing_class_name: _cpp_containing_class_name().
  _cpp_enclosing_namespace: _cpp_enclosing_namespace().
  _cpp_receiver_type: _cpp_receiver_type().
  _cpp_namespace_name: _cpp_namespace_name().
  CppClassExtractionContext.current_namespace: CppClassExtractionContext#current_namespace.
  _is_cpp_field_type_reference: _is_cpp_field_type_reference().
  CppFunctionExtractionContext.content_lines: CppFunctionExtractionContext#content_lines.
  CppFunctionExtractionContext.parse_function_signature: CppFunctionExtractionContext#parse_function_signature.
  CppFunctionExtractionContext.calculate_complexity: CppFunctionExtractionContext#calculate_complexity.
  CppFunctionExtractionContext.is_global_scope: CppFunctionExtractionContext#is_global_scope.
  CppFunctionExtractionContext.determine_visibility: CppFunctionExtractionContext#determine_visibility.
  CppFunctionExtractionContext.extract_comment_for_line: CppFunctionExtractionContext#extract_comment_for_line.
  CppClassExtractionContext.get_node_text: CppClassExtractionContext#get_node_text.
  CppClassExtractionContext.content_lines: CppClassExtractionContext#content_lines.
  CppClassExtractionContext.extract_base_classes: CppClassExtractionContext#extract_base_classes.
  CppClassExtractionContext.extract_comment_for_line: CppClassExtractionContext#extract_comment_for_line.
  _CPP_CLASS_NODE_TYPES: _CPP_CLASS_NODE_TYPES.
  _CPP_CLASS_PARENT_WALK_LIMIT: _CPP_CLASS_PARENT_WALK_LIMIT.
  _source_slice: _source_slice().
  _CPP_NAMESPACE_PARENT_WALK_LIMIT: _CPP_NAMESPACE_PARENT_WALK_LIMIT.
  _CPP_NAMESPACE_NAME_NODE_TYPES: _CPP_NAMESPACE_NAME_NODE_TYPES.
  _cpp_split_qualified_name: _cpp_split_qualified_name().
  _cpp_type_name: _cpp_type_name().
  _cpp_has_definition_body: _cpp_has_definition_body().
  _class_parts: _class_parts().
---
# Module: [`tree_sitter_analyzer/languages/_cpp_element_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py)

## Classes
### `CppClassExtractionContext`
- def: [`tree_sitter_analyzer/languages/_cpp_element_helpers.py:24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L24)
- signature: `class CppClassExtractionContext:`
- members:
  - `content_lines` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L26)
  - `current_namespace` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L27)
  - `extract_base_classes` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L28)
  - `extract_comment_for_line` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L29)
  - `get_node_text` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L25)
- used by: [`extract_cpp_class`](_cpp_element_helpers.md#extract_cpp_class), [`_extract_class_optimized`](cpp_plugin.md#CppElementExtractor._extract_class_optimized), [`_class_context`](_cpp_element_helpers.md#_class_context)

### `CppFunctionExtractionContext`
- def: [`tree_sitter_analyzer/languages/_cpp_element_helpers.py:12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L12)
- signature: `class CppFunctionExtractionContext:`
- members:
  - `calculate_complexity` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L17)
  - `content_lines` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L13)
  - `determine_visibility` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L19)
  - `extract_comment_for_line` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L20)
  - `is_global_scope` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L18)
  - `parse_function_signature` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L14)
- used by: [`extract_cpp_function`](_cpp_element_helpers.md#extract_cpp_function), [`_extract_function_optimized`](cpp_plugin.md#CppElementExtractor._extract_function_optimized), [`_function_context`](_cpp_element_helpers.md#_function_context)

## Functions
- `_class_context(context: CppClassExtractionContext | Callable[..., str], *legacy_args: Any)` — [`L307`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L307)
- `_class_parts(node: Any, get_node_text: Callable[..., str], extract_base_classes: Callable)` — [`L324`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L324)
- `_cpp_containing_class_name(node: Any)` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L42) — Walk the parent chain (capped) to find the enclosing C++ class name.
- `_cpp_direct_parent_class_name(node: Any)` — [`L197`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L197) — Return the enclosing class/struct name when ``node`` is a nested type
- `_cpp_enclosing_namespace(node: Any)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L99) — Join enclosing namespace names outer→inner (``a::b``), or None.
- `_cpp_has_definition_body(node: Any)` — [`L229`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L229)
- `_cpp_namespace_name(ns_node: Any)` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L88) — Name of a ``namespace_definition`` node (None for anonymous namespaces).
- `_cpp_receiver_type(node: Any, qualifier: str | None)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L132) — Owner of a function: declarator qualifier + enclosing namespaces (#590).
- `_cpp_split_qualified_name(name: str)` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L120) — Split ``math::Foo::bar`` → (``math::Foo``, ``bar``).
- `_cpp_type_name(node: Any)` — [`L219`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L219)
- `_function_context(context: CppFunctionExtractionContext | Callable[..., str], *legacy_args: Any)` — [`L289`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L289)
- `_is_cpp_constructor(name: str, node: Any, qualifier: str | None = None)` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L66) — Return True when ``name`` matches the enclosing class name (constructor).
- `_is_cpp_field_type_reference(node: Any)` — [`L237`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L237)
- `_source_slice(content_lines: list[str], start_line: int, end_line: int)` — [`L339`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L339)
- `extract_cpp_class(node: Any, context: CppClassExtractionContext | Callable[..., str], *legacy_args: Any)` — [`L243`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L243) — Extract C++ class, struct, or union information. — documented in [tree_sitter_analyzer-utils-logging](../../../concepts/tree_sitter_analyzer-utils-logging.md)
- `extract_cpp_function(node: Any, context: CppFunctionExtractionContext | Callable[..., str], *legacy_args: Any)` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L147) — Extract a C++ function definition. — documented in [tree_sitter_analyzer-models-base](../../../concepts/tree_sitter_analyzer-models-base.md)

## Module values
- `_CPP_CLASS_NODE_TYPES` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L32)
- `_CPP_CLASS_PARENT_WALK_LIMIT` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L35)
- `_CPP_NAMESPACE_NAME_NODE_TYPES` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L37)
- `_CPP_NAMESPACE_PARENT_WALK_LIMIT` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_element_helpers.py#L36)

