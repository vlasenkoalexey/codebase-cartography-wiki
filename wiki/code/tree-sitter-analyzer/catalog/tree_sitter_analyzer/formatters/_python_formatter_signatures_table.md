---
title: 'Module: tree_sitter_analyzer/formatters/_python_formatter_signatures_table.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_python_formatter_signatures_table.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._python_formatter_signatures_table`/
symbols:
  format_python_signatures_table: format_python_signatures_table().
  _module_name: _module_name().
  _method_sig_line: _method_sig_line().
  _shorten_return_type: _shorten_return_type().
  _append_module_functions_block: _append_module_functions_block().
  _append_method_lines: _append_method_lines().
  _append_class_block: _append_class_block().
  _trim_trailing_blank_lines: _trim_trailing_blank_lines().
  _methods_in_range: _methods_in_range().
  _assign_methods_to_classes: _assign_methods_to_classes().
  _module_level_functions: _module_level_functions().
  _RETURN_ABBREVS._RETURN_ABBREVS: _RETURN_ABBREVS._RETURN_ABBREVS.
---
# Module: [`tree_sitter_analyzer/formatters/_python_formatter_signatures_table.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures_table.py)

## Functions
- `_append_class_block(lines: list[str], cls: dict[str, Any], all_methods: list[dict[str, Any]])` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures_table.py#L95) — Emit one class block: header + method lines (pre-assigned owners).
- `_append_method_lines(lines: list[str], methods: list[dict[str, Any]])` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures_table.py#L124) — Emit one line per method: ``name →returnType(Np) start-end``.
- `_append_module_functions_block(lines: list[str], functions: list[dict[str, Any]])` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures_table.py#L113) — Emit the module-level functions block.
- `_assign_methods_to_classes(methods: list[dict[str, Any]], classes: list[dict[str, Any]])` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures_table.py#L174) — Assign each method to exactly ONE class — the innermost containing one.
- `_method_sig_line(method: dict[str, Any])` — [`L133`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures_table.py#L133) — Format ``  methodName →returnType(Np) startLine-endLine``.
- `_methods_in_range(methods: list[dict[str, Any]], line_range: dict[str, Any])` — [`L205`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures_table.py#L205) — Return methods whose start line falls inside ``line_range``.
- `_module_level_functions(methods: list[dict[str, Any]], classes: list[dict[str, Any]])` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures_table.py#L221) — Return methods that don't fall inside any class range.
- `_module_name(file_path: str)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures_table.py#L83) — Extract a short module name from a file path.
- `_shorten_return_type(ret: str)` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures_table.py#L161) — Abbreviate common return types; leave complex generics short.
- `_trim_trailing_blank_lines(lines: list[str])` — [`L239`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures_table.py#L239) — Remove trailing blank lines in-place.
- `format_python_signatures_table(data: dict[str, Any])` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures_table.py#L20) — Render a lightweight method-directory for the given Python structure data.

## Module values
- `_RETURN_ABBREVS` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_signatures_table.py#L146)

