---
title: 'Module: tree_sitter_analyzer/formatters/_typescript_formatter_signatures_table.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_typescript_formatter_signatures_table.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._typescript_formatter_signatures_table`/
symbols:
  format_typescript_signatures_table: format_typescript_signatures_table().
  _method_sig_line: _method_sig_line().
  _shorten_return_type: _shorten_return_type().
  _module_level_functions: _module_level_functions().
  _trim_trailing_blank_lines: _trim_trailing_blank_lines().
  _append_module_functions_block: _append_module_functions_block().
  _append_method_lines: _append_method_lines().
  _append_class_block: _append_class_block().
  _module_name: _module_name().
  _assign_methods_to_classes: _assign_methods_to_classes().
  _RETURN_ABBREVS._RETURN_ABBREVS: _RETURN_ABBREVS._RETURN_ABBREVS.
---
# Module: [`tree_sitter_analyzer/formatters/_typescript_formatter_signatures_table.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_signatures_table.py)

## Functions
- `_append_class_block(lines: list[str], cls: dict[str, Any], class_methods: list[dict[str, Any]])` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_signatures_table.py#L100) — Emit one class/interface block: header + method lines.
- `_append_method_lines(lines: list[str], methods: list[dict[str, Any]])` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_signatures_table.py#L131) — Emit one line per method: ``name →returnType(Np) start-end``.
- `_append_module_functions_block(lines: list[str], functions: list[dict[str, Any]])` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_signatures_table.py#L120) — Emit the module-level functions block.
- `_assign_methods_to_classes(methods: list[dict[str, Any]], classes: list[dict[str, Any]])` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_signatures_table.py#L180) — Assign each method to exactly ONE class — the innermost containing one.
- `_method_sig_line(method: dict[str, Any])` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_signatures_table.py#L140) — Format ``  methodName →returnType(Np) startLine-endLine``.
- `_module_level_functions(methods: list[dict[str, Any]], classes: list[dict[str, Any]])` — [`L211`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_signatures_table.py#L211) — Return methods that don't fall inside any class/interface range.
- `_module_name(file_path: str)` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_signatures_table.py#L88) — Extract a short module name from a file path (strips .ts/.tsx/.d.ts).
- `_shorten_return_type(ret: str)` — [`L169`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_signatures_table.py#L169) — Abbreviate common return types; strip generics to base name.
- `_trim_trailing_blank_lines(lines: list[str])` — [`L229`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_signatures_table.py#L229) — Remove trailing blank lines in-place.
- `format_typescript_signatures_table(data: dict[str, Any])` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_signatures_table.py#L28) — Render a lightweight method-directory for the given TypeScript structure data.

## Module values
- `_RETURN_ABBREVS` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_signatures_table.py#L153)

