---
title: 'Module: tree_sitter_analyzer/languages/python_plugin/_signature_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/python_plugin/_signature_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.python_plugin._signature_helpers`/_
symbols:
  _extract_class_name_and_superclasses: extract_class_name_and_superclasses().
  _parse_function_signature_children: parse_function_signature_children().
  _extract_class_decorators: extract_class_decorators().
  _return_type_from_signature_text: return_type_from_signature_text().
  _extract_decorated_function_decorators: extract_decorated_function_decorators().
  _is_usable_return_type: is_usable_return_type().
  _extract_superclass_names: extract_superclass_names().
  _return_type_from_type_child: return_type_from_type_child().
  _PARAMETER_NODE_TYPES: PARAMETER_NODE_TYPES.
  _decode_optional_text: decode_optional_text().
  _strip_docstring_quotes: strip_docstring_quotes().
  _class_body_assignment_node: class_body_assignment_node().
  _normalize_decorator_text: normalize_decorator_text().
  _INVALID_RETURN_TYPE_MARKERS: INVALID_RETURN_TYPE_MARKERS.
---
# Module: [`tree_sitter_analyzer/languages/python_plugin/_signature_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_signature_helpers.py)

## Functions
- `_class_body_assignment_node(node: Any)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_signature_helpers.py#L41) — Return the assignment represented directly by a class-body child.
- `_decode_optional_text(node: Any)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_signature_helpers.py#L21)
- `_extract_class_decorators(parent: Any, get_node_text: Callable[[Any], str])` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_signature_helpers.py#L50)
- `_extract_class_name_and_superclasses(node: Any)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_signature_helpers.py#L66)
- `_extract_decorated_function_decorators(parent: Any, get_node_text: Callable[[Any], str])` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_signature_helpers.py#L130)
- `_extract_superclass_names(argument_list_node: Any)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_signature_helpers.py#L79)
- `_is_usable_return_type(return_type: str | None, *, reject_statement_fragments: bool)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_signature_helpers.py#L118)
- `_normalize_decorator_text(decorator_text: str)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_signature_helpers.py#L26)
- `_parse_function_signature_children(node: Any, get_node_text: Callable[[Any], str], extract_parameters: Callable[[Any], list[str]], return_type: str | None)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_signature_helpers.py#L142)
- `_return_type_from_signature_text(node_text: str)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_signature_helpers.py#L94) — Extract the return-type annotation from a Python function's text.
- `_return_type_from_type_child(child: Any, get_node_text: Callable[[Any], str], current_return_type: str | None)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_signature_helpers.py#L164)
- `_strip_docstring_quotes(docstring: str)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_signature_helpers.py#L32) — Remove Python string delimiters from a docstring literal.

## Module values
- `_INVALID_RETURN_TYPE_MARKERS` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_signature_helpers.py#L18)
- `_PARAMETER_NODE_TYPES` — [`L8`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_signature_helpers.py#L8)

