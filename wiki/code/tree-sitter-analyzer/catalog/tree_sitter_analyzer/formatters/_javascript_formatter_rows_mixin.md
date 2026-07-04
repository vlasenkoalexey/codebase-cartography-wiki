---
title: 'Module: tree_sitter_analyzer/formatters/_javascript_formatter_rows_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_javascript_formatter_rows_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._javascript_formatter_rows_mixin`/
symbols:
  JavaScriptTableFormatterRowsMixin._create_full_params: JavaScriptTableFormatterRowsMixin#_create_full_params().
  JavaScriptTableFormatterRowsMixin: JavaScriptTableFormatterRowsMixin#
  JavaScriptTableFormatterRowsMixin._format_function_row: JavaScriptTableFormatterRowsMixin#_format_function_row().
  JavaScriptTableFormatterRowsMixin._format_method_row: JavaScriptTableFormatterRowsMixin#_format_method_row().
  JavaScriptTableFormatterRowsMixin._create_compact_params: JavaScriptTableFormatterRowsMixin#_create_compact_params().
  JavaScriptTableFormatterRowsMixin._get_function_signature: JavaScriptTableFormatterRowsMixin#_get_function_signature().
  _full_param_text: _full_param_text().
  _compact_param_name: _compact_param_name().
  JavaScriptTableFormatterRowsMixin._get_class_info: JavaScriptTableFormatterRowsMixin#_get_class_info().
---
# Module: [`tree_sitter_analyzer/formatters/_javascript_formatter_rows_mixin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_rows_mixin.py)

## Classes
### `JavaScriptTableFormatterRowsMixin`
- def: [`tree_sitter_analyzer/formatters/_javascript_formatter_rows_mixin.py:6`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_rows_mixin.py#L6)
- doc: Function, method, and metadata row helpers.
- signature: `class JavaScriptTableFormatterRowsMixin:`
- members:
  - `_create_compact_params(self, func: dict[str, Any])` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_rows_mixin.py#L55) — Create compact parameter list for JavaScript functions
  - `_create_full_params(self, func: dict[str, Any])` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_rows_mixin.py#L43) — Create full parameter list for JavaScript functions
  - `_format_function_row(self, func: dict[str, Any])` — [`L9`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_rows_mixin.py#L9) — Format a function table row for JavaScript
  - `_format_method_row(self, method: dict[str, Any])` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_rows_mixin.py#L25) — Format a method table row for JavaScript
  - `_get_class_info(self, cls: dict[str, Any])` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_rows_mixin.py#L77) — Get class information as formatted string
  - `_get_function_signature(self, func: dict[str, Any])` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_rows_mixin.py#L68) — Get function signature
- uses (calls/refs, reference-scoped): [`JavaScriptTableFormatter`](javascript_formatter.md#JavaScriptTableFormatter), [`_compact_param_name`](_javascript_formatter_rows_mixin.md#_compact_param_name), [`_full_param_text`](_javascript_formatter_rows_mixin.md#_full_param_text)
- used by: [`JavaScriptTableFormatter`](javascript_formatter.md#JavaScriptTableFormatter)

## Functions
- `_compact_param_name(param: Any)` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_rows_mixin.py#L103)
- `_full_param_text(param: Any)` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_javascript_formatter_rows_mixin.py#L92)

