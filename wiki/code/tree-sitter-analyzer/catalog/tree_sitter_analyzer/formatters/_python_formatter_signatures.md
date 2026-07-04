---
title: 'Module: tree_sitter_analyzer/formatters/_python_formatter_signatures.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_python_formatter_signatures.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._python_formatter_signatures`/
symbols:
  create_compact_signature: create_compact_signature().
  shorten_type: shorten_type().
  format_python_signature: format_python_signature().
  format_python_signature_compact: format_python_signature_compact().
  _compact_param_types: _compact_param_types().
  _params_list: _params_list().
  _SHORT_TYPE_MAPPING: _SHORT_TYPE_MAPPING.
  _compact_param_type: _compact_param_type().
  _compact_return_type: _compact_return_type().
  _shorten_generic_type: _shorten_generic_type().
  _format_python_param: _format_python_param().
  _format_compact_python_param: _format_compact_python_param().
---
# Module: [`tree_sitter_analyzer/formatters/_python_formatter_signatures.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures.py)

## Functions
- `_compact_param_type(param: Any)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures.py#L38)
- `_compact_param_types(params: Any)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures.py#L30)
- `_compact_return_type(return_type: Any)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures.py#L48)
- `_format_compact_python_param(param: Any)` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures.py#L138)
- `_format_python_param(param: Any)` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures.py#L116)
- `_params_list(method: dict[str, Any])` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures.py#L109)
- `_shorten_generic_type(type_name: str)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures.py#L74)
- `create_compact_signature(method: dict[str, Any])` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures.py#L20) — Create compact method signature for Python
- `format_python_signature(method: dict[str, Any])` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures.py#L98) — Create Python method signature
- `format_python_signature_compact(method: dict[str, Any])` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures.py#L127) — Create compact Python method signature for class sections
- `shorten_type(type_name: Any)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures.py#L56) — Shorten type name for Python tables

## Module values
- `_SHORT_TYPE_MAPPING` — [`L5`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures.py#L5)

