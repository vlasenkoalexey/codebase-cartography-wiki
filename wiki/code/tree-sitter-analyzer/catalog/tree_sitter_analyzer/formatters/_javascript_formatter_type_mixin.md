---
title: 'Module: tree_sitter_analyzer/formatters/_javascript_formatter_type_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_javascript_formatter_type_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._javascript_formatter_type_mixin`/JavaScriptTableFormatterTypeMixin#
symbols:
  JavaScriptTableFormatterTypeMixin._get_function_type: _get_function_type().
  JavaScriptTableFormatterTypeMixin: ''
  JavaScriptTableFormatterTypeMixin._is_method: _is_method.
  JavaScriptTableFormatterTypeMixin._get_variable_kind: _get_variable_kind.
  JavaScriptTableFormatterTypeMixin._get_export_type: _get_export_type.
  JavaScriptTableFormatterTypeMixin._get_method_class: _get_method_class.
  JavaScriptTableFormatterTypeMixin._get_method_type: _get_method_type.
  JavaScriptTableFormatterTypeMixin._infer_js_type: _infer_js_type.
  JavaScriptTableFormatterTypeMixin._get_function_type_short: _get_function_type_short().
  JavaScriptTableFormatterTypeMixin._determine_scope: _determine_scope().
---
# Module: [`tree_sitter_analyzer/formatters/_javascript_formatter_type_mixin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_mixin.py)

## Classes
### `JavaScriptTableFormatterTypeMixin`
- def: [`tree_sitter_analyzer/formatters/_javascript_formatter_type_mixin.py:16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_mixin.py#L16)
- doc: Classification helpers for JavaScript analysis rows.
- signature: `class JavaScriptTableFormatterTypeMixin:`
- members:
  - `_determine_scope(self, var: dict[str, Any])` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_mixin.py#L51) — Determine variable scope
  - `_get_function_type(self, func: dict[str, Any])` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_mixin.py#L26) — Get full function type for JavaScript
  - `_get_function_type_short(self, func: dict[str, Any])` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_mixin.py#L39) — Get short function type for JavaScript
- protocol/private: `_get_export_type`[`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_mixin.py#L19), `_get_method_class`[`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_mixin.py#L20), `_get_method_type`[`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_mixin.py#L21), `_get_variable_kind`[`L22`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_mixin.py#L22), `_infer_js_type`[`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_mixin.py#L23), `_is_method`[`L24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_type_mixin.py#L24)
- uses (calls/refs, reference-scoped): [`JavaScriptTableFormatter`](javascript_formatter.md#JavaScriptTableFormatter), [`export_type`](_javascript_formatter_type_helpers.md#export_type), [`infer_js_type`](_javascript_formatter_type_helpers.md#infer_js_type), [`method_function_type`](_javascript_formatter_type_helpers.md#method_function_type), [`method_type`](_javascript_formatter_type_helpers.md#method_type), [`variable_kind`](_javascript_formatter_type_helpers.md#variable_kind), [`is_method`](_javascript_formatter_type_helpers.md#is_method), [`method_class`](_javascript_formatter_type_helpers.md#method_class)
- used by: [`JavaScriptTableFormatter`](javascript_formatter.md#JavaScriptTableFormatter)

