---
title: 'Module: tree_sitter_analyzer/_legacy_table_formatter_common.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_legacy_table_formatter_common.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._legacy_table_formatter_common`/
symbols:
  trim_trailing_blank_lines: trim_trailing_blank_lines().
  get_visibility_symbol: get_visibility_symbol().
  convert_visibility: convert_visibility().
  extract_doc_summary: extract_doc_summary().
  get_platform_newline: get_platform_newline().
  create_full_signature: create_full_signature().
  shorten_type: shorten_type().
  clean_csv_text: clean_csv_text().
---
# Module: [`tree_sitter_analyzer/_legacy_table_formatter_common.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_common.py)

## Functions
- `clean_csv_text(text: str)` — [`L118`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_common.py#L118) — Clean text for legacy CSV-compatible table cells.
- `convert_visibility(visibility: str)` — [`L97`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_common.py#L97) — Convert visibility to a legacy full-table symbol.
- `create_full_signature(method: dict[str, Any])` — [`L26`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_common.py#L26) — Create a complete legacy method signature.
- `extract_doc_summary(javadoc: str)` — [`L103`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_common.py#L103) — Extract the first JavaDoc sentence using legacy rules.
- `get_platform_newline()` — [`L9`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_common.py#L9) — Get platform-specific newline character.
- `get_visibility_symbol(visibility: str)` — [`L14`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_common.py#L14) — Convert visibility to a legacy compact-table symbol.
- `shorten_type(type_name: Any)` — [`L56`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_common.py#L56) — Shorten a type name using the legacy full-table mapping.
- `trim_trailing_blank_lines(lines: list[str])` — [`L129`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_legacy_table_formatter_common.py#L129) — Remove trailing empty strings from a list of lines in-place.

