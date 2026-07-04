---
title: 'Module: tree_sitter_analyzer/formatters/_java_formatter_signatures_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_java_formatter_signatures_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._java_formatter_signatures_mixin`/
symbols:
  JavaTableFormatterSignaturesMixin._format_signatures_table: JavaTableFormatterSignaturesMixin#_format_signatures_table().
  _append_class_block: _append_class_block().
  _append_method_lines: _append_method_lines().
  _method_sig_line: _method_sig_line().
  _shorten_return_type: _shorten_return_type().
  JavaTableFormatterSignaturesMixin: JavaTableFormatterSignaturesMixin#
  _RETURN_ABBREVS._RETURN_ABBREVS: _RETURN_ABBREVS._RETURN_ABBREVS.
---
# Module: [`tree_sitter_analyzer/formatters/_java_formatter_signatures_mixin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_signatures_mixin.py)

## Classes
### `JavaTableFormatterSignaturesMixin`
- def: [`tree_sitter_analyzer/formatters/_java_formatter_signatures_mixin.py:26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_signatures_mixin.py#L26)
- doc: Signatures-format rendering: name →returnType(Np) L-L per method.
- signature: `class JavaTableFormatterSignaturesMixin:`
- members:
  - `_format_signatures_table(self, data: dict[str, Any])` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_signatures_mixin.py#L29) — Render a lightweight method-directory for the given structure data.
- uses (calls/refs, reference-scoped): [`JavaTableFormatter`](java_formatter.md#JavaTableFormatter), [`trim_trailing_blank_lines`](../_legacy_table_formatter_common.md#trim_trailing_blank_lines), [`_append_class_block`](_java_formatter_signatures_mixin.md#_append_class_block), [`_java_title`](_java_formatter_full_mixin.md#_java_title), [`is_inner_class`](_java_formatter_class_mixin.md#is_inner_class), [`_append_method_lines`](_java_formatter_signatures_mixin.md#_append_method_lines)
- used by: [`JavaTableFormatter`](java_formatter.md#JavaTableFormatter)

## Functions
- `_append_class_block(lines: list[str], cls: dict[str, Any], data: dict[str, Any], all_classes: list[dict[str, Any]], all_methods: list[dict[str, Any]], all_fields: list[dict[str, Any]])` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_signatures_mixin.py#L84) — Emit one class block: header + method lines + optional field lines.
- `_append_method_lines(lines: list[str], methods: list[dict[str, Any]])` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_signatures_mixin.py#L122) — Emit one line per method: ``name →returnType(Np) start-end``.
- `_method_sig_line(method: dict[str, Any])` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_signatures_mixin.py#L131) — Format ``methodName →returnType(Np) startLine-endLine``.
- `_shorten_return_type(ret: str)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_signatures_mixin.py#L162) — Abbreviate common return types; leave complex generics intact.

## Module values
- `_RETURN_ABBREVS` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_signatures_mixin.py#L145)

