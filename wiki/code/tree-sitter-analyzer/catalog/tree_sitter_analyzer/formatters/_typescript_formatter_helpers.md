---
title: 'Module: tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._typescript_formatter_helpers`/
symbols:
  format_method_row: format_method_row().
  doc_summary: doc_summary().
  line_range_text: line_range_text().
  get_class_methods: get_class_methods().
  get_class_fields: get_class_fields().
  create_full_signature: create_full_signature().
  create_csv_signature: create_csv_signature().
  typescript_title: typescript_title().
  field_type: field_type().
  format_typescript_modifiers: format_typescript_modifiers().
  create_compact_signature: create_compact_signature().
  trim_trailing_blank_lines: trim_trailing_blank_lines().
  grouped_class_methods: grouped_class_methods().
  _members_in_range: _members_in_range().
  _doc_summary: _doc_summary().
  _full_parameter_text: _full_parameter_text().
---
# Module: [`tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py)

## Functions
- `_doc_summary(formatter: Any, element: dict[str, Any])` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py#L163)
- `_full_parameter_text(param: Any)` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py#L151)
- `_members_in_range(members: list[dict[str, Any]], line_range: dict[str, int])` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py#L139)
- `create_compact_signature(method: dict[str, Any])` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py#L69) — Create compact TypeScript method signature.
- `create_csv_signature(method: dict[str, Any])` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py#L83) — Create CSV TypeScript method signature with full parameter details.
- `create_full_signature(method: dict[str, Any])` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py#L60) — Create full TypeScript method signature.
- `doc_summary(formatter: Any, element: dict[str, Any])` — [`L134`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py#L134) — Return a formatter-compatible documentation summary.
- `field_type(field: dict[str, Any])` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py#L39) — Return the best TypeScript field type text available.
- `format_method_row(formatter: Any, method: dict[str, Any])` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py#L88) — Format a TypeScript method table row.
- `format_typescript_modifiers(element: dict[str, Any])` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py#L48) — Format TypeScript element modifiers.
- `get_class_fields(fields: list[dict[str, Any]], line_range: dict[str, int])` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py#L32) — Get fields within a class range.
- `get_class_methods(methods: list[dict[str, Any]], line_range: dict[str, int])` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py#L25) — Get methods within a class range.
- `grouped_class_methods(methods: list[dict[str, Any]])` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py#L103) — Group methods into constructor, public, protected, and private buckets.
- `line_range_text(line_range: dict[str, int])` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py#L20) — Format a line-range mapping as start-end text.
- `trim_trailing_blank_lines(lines: list[str])` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py#L128) — Remove trailing blank lines in-place.
- `typescript_title(data: dict[str, Any], *, strip_declaration_suffix: bool)` — [`L6`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_typescript_formatter_helpers.py#L6) — Return the primary TypeScript title for a formatted result.

