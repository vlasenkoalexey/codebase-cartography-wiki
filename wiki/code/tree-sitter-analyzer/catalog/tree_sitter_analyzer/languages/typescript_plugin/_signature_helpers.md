---
title: 'Module: tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.typescript_plugin._signature_helpers`/
symbols:
  parse_method_signature: parse_method_signature().
  _MethodSignatureParts.as_tuple: _MethodSignatureParts#as_tuple().
  _apply_method_child: _apply_method_child().
  parse_function_signature: parse_function_signature().
  _apply_function_child: _apply_function_child().
  _FunctionSignatureParts.as_tuple: _FunctionSignatureParts#as_tuple().
  _MethodSignatureParts.name: _MethodSignatureParts#name.
  FunctionSignature.FunctionSignature: FunctionSignature.FunctionSignature.
  MethodSignature.MethodSignature: MethodSignature.MethodSignature.
  TextExtractor.TextExtractor: TextExtractor.TextExtractor.
  ParameterExtractor.ParameterExtractor: ParameterExtractor.ParameterExtractor.
  GenericsExtractor.GenericsExtractor: GenericsExtractor.GenericsExtractor.
  _method_name_from_child: _method_name_from_child().
  _MethodSignatureParts.is_constructor: _MethodSignatureParts#is_constructor.
  _FunctionSignatureParts: _FunctionSignatureParts#
  _FunctionSignatureParts.name: _FunctionSignatureParts#name.
  _FunctionSignatureParts.parameters: _FunctionSignatureParts#parameters.
  _FunctionSignatureParts.is_async: _FunctionSignatureParts#is_async.
  _FunctionSignatureParts.is_generator: _FunctionSignatureParts#is_generator.
  _FunctionSignatureParts.return_type: _FunctionSignatureParts#return_type.
  _FunctionSignatureParts.generics: _FunctionSignatureParts#generics.
  _MethodSignatureParts: _MethodSignatureParts#
  _MethodSignatureParts.parameters: _MethodSignatureParts#parameters.
  _MethodSignatureParts.is_async: _MethodSignatureParts#is_async.
  _MethodSignatureParts.is_static: _MethodSignatureParts#is_static.
  _MethodSignatureParts.is_getter: _MethodSignatureParts#is_getter.
  _MethodSignatureParts.is_setter: _MethodSignatureParts#is_setter.
  _MethodSignatureParts.return_type: _MethodSignatureParts#return_type.
  _MethodSignatureParts.visibility: _MethodSignatureParts#visibility.
  _MethodSignatureParts.generics: _MethodSignatureParts#generics.
  _visibility_from_node: _visibility_from_node().
  _is_async_from_node: _is_async_from_node().
  _is_static_from_node: _is_static_from_node().
  _accessor_flags_from_text: _accessor_flags_from_text().
  _method_name_from_text: _method_name_from_text().
  _visibility_from_text: _visibility_from_text().
---
# Module: [`tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py)

## Classes
### `_FunctionSignatureParts`
- def: [`tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py:35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L35)
- signature: `class _FunctionSignatureParts:`
- members:
  - `as_tuple(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L43)
  - `generics` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L41)
  - `is_async` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L38)
  - `is_generator` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L39)
  - `name` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L36)
  - `parameters` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L37)
  - `return_type` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L40)
- uses (calls/refs, reference-scoped): [`FunctionSignature`](_signature_helpers.md#FunctionSignature.FunctionSignature)
- used by: [`parse_function_signature`](_signature_helpers.md#parse_function_signature), [`_apply_function_child`](_signature_helpers.md#_apply_function_child)

### `_MethodSignatureParts`
- def: [`tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py:55`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L55)
- signature: `class _MethodSignatureParts:`
- members:
  - `as_tuple(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L67)
  - `generics` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L65)
  - `is_async` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L58)
  - `is_constructor` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L62)
  - `is_getter` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L60)
  - `is_setter` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L61)
  - `is_static` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L59)
  - `name` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L56)
  - `parameters` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L57)
  - `return_type` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L63)
  - `visibility` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L64)
- uses (calls/refs, reference-scoped): [`MethodSignature`](_signature_helpers.md#MethodSignature.MethodSignature)
- used by: [`parse_method_signature`](_signature_helpers.md#parse_method_signature), [`_apply_method_child`](_signature_helpers.md#_apply_method_child)

## Functions
- `_accessor_flags_from_text(node_text: str)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L226)
- `_apply_function_child(parts: _FunctionSignatureParts, child: tree_sitter.Node, get_node_text: TextExtractor, extract_parameters: ParameterExtractor, extract_generics: GenericsExtractor)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L139)
- `_apply_method_child(parts: _MethodSignatureParts, child: tree_sitter.Node, get_node_text: TextExtractor, extract_parameters: ParameterExtractor, extract_generics: GenericsExtractor)` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L156)
- `_is_async_from_node(node: tree_sitter.Node)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L197) — Check for ``async`` keyword as a direct AST child of the method node.
- `_is_static_from_node(node: tree_sitter.Node)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L210) — Check for ``static`` keyword as a direct AST child of the method node.
- `_method_name_from_child(child: tree_sitter.Node, get_node_text: TextExtractor)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L234)
- `_method_name_from_text(node_text: str)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L249)
- `_visibility_from_node(node: tree_sitter.Node)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L174) — Read visibility from the ``accessibility_modifier`` AST child.
- `_visibility_from_text(node_text: str)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L218)
- `parse_function_signature(node: tree_sitter.Node, get_node_text: TextExtractor, extract_parameters: ParameterExtractor, extract_generics: GenericsExtractor)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L82) — Parse a TypeScript function signature.
- `parse_method_signature(node: tree_sitter.Node, get_node_text: TextExtractor, extract_parameters: ParameterExtractor, extract_generics: GenericsExtractor)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L106) — Parse a TypeScript class or interface method signature.

## Module values
- `FunctionSignature` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L17)
- `GenericsExtractor` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L16)
- `MethodSignature` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L20)
- `ParameterExtractor` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L15)
- `TextExtractor` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_signature_helpers.py#L14)

