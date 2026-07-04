---
title: 'Module: tree_sitter_analyzer/formatters/_javascript_formatter_type_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_javascript_formatter_type_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._javascript_formatter_type_helpers`/
symbols:
  method_function_type: method_function_type().
  method_type: method_type().
  infer_js_type: infer_js_type().
  export_type: export_type().
  variable_kind: variable_kind().
  _variable_kind_from_text: _variable_kind_from_text().
  _first_truthy_flag: _first_truthy_flag().
  is_method: is_method().
  method_class: method_class().
  METHOD_FUNCTION_FLAGS: METHOD_FUNCTION_FLAGS.
  METHOD_TYPE_FLAGS: METHOD_TYPE_FLAGS.
  EXPORT_TYPE_FLAGS: EXPORT_TYPE_FLAGS.
  VARIABLE_KINDS: VARIABLE_KINDS.
  _literal_js_type: _literal_js_type().
  _is_function_like: _is_function_like().
---
# Module: [`tree_sitter_analyzer/formatters/_javascript_formatter_type_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_helpers.py)

## Functions
- `_first_truthy_flag(data: dict[str, Any], flags: tuple[tuple[str, str], ...], *, default: str)` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_helpers.py#L84)
- `_is_function_like(value_str: str)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_helpers.py#L109)
- `_literal_js_type(value_str: str)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_helpers.py#L93)
- `_variable_kind_from_text(raw_text: str)` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_helpers.py#L118)
- `export_type(export: Any)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_helpers.py#L77) — Return the export type label.
- `infer_js_type(value: Any)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_helpers.py#L49) — Infer JavaScript type from a literal-like value.
- `is_method(func: dict[str, Any])` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_helpers.py#L39) — Return whether a function mapping describes a class method.
- `method_class(method: dict[str, Any])` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_helpers.py#L44) — Return the class name for a method mapping.
- `method_function_type(func: dict[str, Any])` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_helpers.py#L29) — Return the full function type for a class method.
- `method_type(method: dict[str, Any])` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_helpers.py#L34) — Return the method type label.
- `variable_kind(var: dict[str, Any])` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_helpers.py#L68) — Return the JavaScript declaration kind for a variable mapping.

## Module values
- `EXPORT_TYPE_FLAGS` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_helpers.py#L20)
- `METHOD_FUNCTION_FLAGS` — [`L5`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_helpers.py#L5)
- `METHOD_TYPE_FLAGS` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_helpers.py#L12)
- `VARIABLE_KINDS` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_helpers.py#L26)

