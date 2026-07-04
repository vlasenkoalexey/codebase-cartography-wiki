---
title: 'Module: tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.typescript_plugin._variable_helpers`/
symbols:
  extract_property: extract_property().
  parse_variable_declarator: parse_variable_declarator().
  extract_property_signature: extract_property_signature().
  _parse_property_parts: _parse_property_parts().
  _apply_property_child: _apply_property_child().
  _parse_variable_parts: _parse_variable_parts().
  extract_variables_from_declaration: extract_variables_from_declaration().
  is_exported_class: is_exported_class().
  _is_named_reexport: _is_named_reexport().
  TextExtractor.TextExtractor: TextExtractor.TextExtractor.
  is_framework_component: is_framework_component().
  _extract_direct_decorator_names: _extract_direct_decorator_names().
  _decorator_name: _decorator_name().
  _PropertyParts: _PropertyParts#
  _PropertyParts.name: _PropertyParts#name.
  _VariableParts.name: _VariableParts#name.
  _VariableParts.value: _VariableParts#value.
  _PropertyParts.type_name: _PropertyParts#type_name.
  _PropertyParts.value: _PropertyParts#value.
  _PropertyParts.is_static: _PropertyParts#is_static.
  _PropertyParts.visibility: _PropertyParts#visibility.
  _VariableParts: _VariableParts#
  _VariableParts.type_name: _VariableParts#type_name.
  infer_type_from_value: infer_type_from_value().
  _node_text: _node_text().
  TsdocExtractor.TsdocExtractor: TsdocExtractor.TsdocExtractor.
  _has_arrow_function_child: _has_arrow_function_child().
  _visibility_from_text: _visibility_from_text().
  TypeInferer.TypeInferer: TypeInferer.TypeInferer.
---
# Module: [`tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py)

## Classes
### `_PropertyParts`
- def: [`tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py:23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L23)
- signature: `class _PropertyParts:`
- members:
  - `is_static` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L27)
  - `name` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L24)
  - `type_name` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L25)
  - `value` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L26)
  - `visibility` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L28)
- used by: [`extract_property`](_variable_helpers.md#extract_property), [`_parse_property_parts`](_variable_helpers.md#_parse_property_parts), [`_apply_property_child`](_variable_helpers.md#_apply_property_child)

### `_VariableParts`
- def: [`tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py:32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L32)
- signature: `class _VariableParts:`
- members:
  - `name` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L33)
  - `type_name` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L34)
  - `value` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L35)
- used by: [`parse_variable_declarator`](_variable_helpers.md#parse_variable_declarator), [`_parse_variable_parts`](_variable_helpers.md#_parse_variable_parts)

## Functions
- `_apply_property_child(parts: _PropertyParts, child: tree_sitter.Node, get_node_text: TextExtractor)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L261)
- `_decorator_name(node: tree_sitter.Node)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L285)
- `_extract_direct_decorator_names(node: tree_sitter.Node)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L274)
- `_has_arrow_function_child(node: tree_sitter.Node)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L320)
- `_is_named_reexport(class_name: str, source_code: str)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L165) — Detect ``export { ... }`` re-export of ``class_name``.
- `_node_text(node: tree_sitter.Node)` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L296)
- `_parse_property_parts(node: tree_sitter.Node, get_node_text: TextExtractor)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L244)
- `_parse_variable_parts(node: tree_sitter.Node, get_node_text: TextExtractor)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L303)
- `_visibility_from_text(node_text: str)` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L324)
- `extract_property(node: tree_sitter.Node, get_node_text: TextExtractor)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L38) — Extract class property definition. — documented in [tree_sitter_analyzer-utils-logging](../../../../concepts/tree_sitter_analyzer-utils-logging.md)
- `extract_property_signature(node: tree_sitter.Node, get_node_text: TextExtractor)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L69) — Extract property signature from an interface.
- `extract_variables_from_declaration(node: tree_sitter.Node, kind: str, get_node_text: TextExtractor, parse_declarator: Callable, extract_tsdoc: TsdocExtractor)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L104) — Extract variables from a declaration node.
- `infer_type_from_value(value: str | None)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L185) — Infer TypeScript type from a value literal.
- `is_exported_class(class_name: str, source_code: str)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L146) — Check if a TypeScript type-like symbol is exported.
- `is_framework_component(framework_type: str, source_code: str, get_node_text: TextExtractor, node: tree_sitter.Node)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L127) — Check if class is a framework component.
- `parse_variable_declarator(node: tree_sitter.Node, kind: str, start_line: int, end_line: int, get_node_text: TextExtractor, infer_type_from_value: TypeInferer, extract_tsdoc: TsdocExtractor)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L211) — Parse an individual variable declarator with TypeScript type annotations. — documented in [tree_sitter_analyzer-utils-logging](../../../../concepts/tree_sitter_analyzer-utils-logging.md)

## Module values
- `TextExtractor` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L17)
- `TsdocExtractor` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L18)
- `TypeInferer` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_variable_helpers.py#L19)

