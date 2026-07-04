---
title: 'Module: tree_sitter_analyzer/formatters/_python_formatter_rows.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_python_formatter_rows.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._python_formatter_rows`/
symbols:
  format_python_class_method_row: format_python_class_method_row().
  format_python_method_row: format_python_method_row().
  _class_method_doc: _class_method_doc().
  get_python_visibility_symbol: get_python_visibility_symbol().
  _class_method_visibility_symbol: _class_method_visibility_symbol().
  _looks_like_other_method_doc: _looks_like_other_method_doc().
  _method_visibility: _method_visibility().
  _DOCSTRING_MISMATCH_WORDS: _DOCSTRING_MISMATCH_WORDS.
  _VISIBILITY_SYMBOLS: _VISIBILITY_SYMBOLS.
  _method_lines: _method_lines().
  _class_method_lines: _class_method_lines().
  _has_docstring_text: _has_docstring_text().
  _class_method_modifier: _class_method_modifier().
---
# Module: [`tree_sitter_analyzer/formatters/_python_formatter_rows.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_rows.py)

## Functions
- `_class_method_doc(formatter: Any, method: dict[str, Any])` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_rows.py#L76)
- `_class_method_lines(method: dict[str, Any])` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_rows.py#L69)
- `_class_method_modifier(method: dict[str, Any])` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_rows.py#L98)
- `_class_method_visibility_symbol(method: dict[str, Any], name: str)` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_rows.py#L64)
- `_has_docstring_text(docstring: Any)` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_rows.py#L88)
- `_looks_like_other_method_doc(docstring_text: str)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_rows.py#L94)
- `_method_lines(method: dict[str, Any])` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_rows.py#L40)
- `_method_visibility(method: dict[str, Any], name: str)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_rows.py#L32)
- `format_python_class_method_row(formatter: Any, method: dict[str, Any])` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_rows.py#L52) — Format a method table row for class-specific sections
- `format_python_method_row(formatter: Any, method: dict[str, Any])` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_rows.py#L14) — Format a method table row for Python
- `get_python_visibility_symbol(visibility: str)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_rows.py#L47) — Get Python visibility symbol

## Module values
- `_DOCSTRING_MISMATCH_WORDS` — [`L5`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_rows.py#L5)
- `_VISIBILITY_SYMBOLS` — [`L6`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_rows.py#L6)

