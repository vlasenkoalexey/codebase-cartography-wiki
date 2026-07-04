---
title: 'Module: tree_sitter_analyzer/languages/typescript_plugin/_tsdoc_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/typescript_plugin/_tsdoc_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.typescript_plugin._tsdoc_helpers`/
symbols:
  extract_tsdoc_for_line: extract_tsdoc_for_line().
  _extract_multiline_tsdoc: _extract_multiline_tsdoc().
  clean_tsdoc: clean_tsdoc().
  _cache_cleaned_tsdoc: _cache_cleaned_tsdoc().
  Cleaner.Cleaner: Cleaner.Cleaner.
  _previous_content_line: _previous_content_line().
  _strip_tsdoc_marker: _strip_tsdoc_marker().
---
# Module: [`tree_sitter_analyzer/languages/typescript_plugin/_tsdoc_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_tsdoc_helpers.py)

## Functions
- `_cache_cleaned_tsdoc(tsdoc_text: str, target_line: int, tsdoc_cache: dict[int, str], clean_tsdoc: Cleaner)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_tsdoc_helpers.py#L99)
- `_extract_multiline_tsdoc(content_lines: list[str], current_line: int, target_line: int, tsdoc_cache: dict[int, str], clean_tsdoc: Cleaner)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_tsdoc_helpers.py#L73)
- `_previous_content_line(content_lines: list[str], target_line: int)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_tsdoc_helpers.py#L61)
- `_strip_tsdoc_marker(line: str)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_tsdoc_helpers.py#L110)
- `clean_tsdoc(tsdoc_text: str)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_tsdoc_helpers.py#L47) — Clean TSDoc text by removing comment markers.
- `extract_tsdoc_for_line(content_lines: list[str], target_line: int, tsdoc_cache: dict[int, str], clean_tsdoc: Cleaner)` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_tsdoc_helpers.py#L13) — Extract TSDoc comment immediately before the specified line.

## Module values
- `Cleaner` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_tsdoc_helpers.py#L10)

