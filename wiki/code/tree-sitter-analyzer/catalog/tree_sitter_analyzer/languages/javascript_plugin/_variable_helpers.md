---
title: 'Module: tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.javascript_plugin._variable_helpers`/
symbols:
  parse_variable_declarator: parse_variable_declarator().
  _apply_variable_child: _apply_variable_child().
  _parse_variable_parts: _parse_variable_parts().
  _VariableParts.value: _VariableParts#value.
  TextExtractor.TextExtractor: TextExtractor.TextExtractor.
  _value_after_assignment: _value_after_assignment().
  _variable_raw_text: _variable_raw_text().
  _VariableParts: _VariableParts#
  _VariableParts.name: _VariableParts#name.
  _VariableParts.is_destructuring: _VariableParts#is_destructuring.
  infer_type_from_value: infer_type_from_value().
  _VALUE_NODE_TYPES: _VALUE_NODE_TYPES.
  _DESTRUCTURING_PATTERN_TYPES: _DESTRUCTURING_PATTERN_TYPES.
  _has_arrow_function_child: _has_arrow_function_child().
  JsdocExtractor.JsdocExtractor: JsdocExtractor.JsdocExtractor.
  TypeInferer.TypeInferer: TypeInferer.TypeInferer.
---
# Module: [`tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py)

## Classes
### `_VariableParts`
- def: [`tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py:40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py#L40)
- signature: `class _VariableParts:`
- members:
  - `is_destructuring` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py#L43)
  - `name` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py#L41)
  - `value` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py#L42)
- used by: [`parse_variable_declarator`](_variable_helpers.md#parse_variable_declarator), [`_apply_variable_child`](_variable_helpers.md#_apply_variable_child), [`_parse_variable_parts`](_variable_helpers.md#_parse_variable_parts)

## Functions
- `_apply_variable_child(parts: _VariableParts, child: tree_sitter.Node, get_node_text: TextExtractor)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py#L125)
- `_has_arrow_function_child(node: tree_sitter.Node)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py#L157)
- `_parse_variable_parts(node: tree_sitter.Node, get_node_text: TextExtractor)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py#L111)
- `_value_after_assignment(node: tree_sitter.Node, get_node_text: TextExtractor)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py#L144)
- `_variable_raw_text(node: tree_sitter.Node, get_node_text: TextExtractor)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py#L161)
- `infer_type_from_value(value: str | None)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py#L86) — Infer JavaScript type from a literal-ish value.
- `parse_variable_declarator(node: tree_sitter.Node, kind: str, start_line: int, end_line: int, get_node_text: TextExtractor, infer_type: TypeInferer, extract_jsdoc: JsdocExtractor)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py#L46) — Parse an individual JavaScript variable declarator.

## Module values
- `JsdocExtractor` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py#L17)
- `TextExtractor` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py#L16)
- `TypeInferer` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py#L18)
- `_DESTRUCTURING_PATTERN_TYPES` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py#L36)
- `_VALUE_NODE_TYPES` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_variable_helpers.py#L20)

