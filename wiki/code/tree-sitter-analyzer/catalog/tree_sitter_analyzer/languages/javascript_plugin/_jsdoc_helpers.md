---
title: 'Module: tree_sitter_analyzer/languages/javascript_plugin/_jsdoc_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/javascript_plugin/_jsdoc_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.javascript_plugin._jsdoc_helpers`/
symbols:
  extract_jsdoc_for_line: extract_jsdoc_for_line().
  _extract_multiline_jsdoc: _extract_multiline_jsdoc().
  clean_jsdoc: clean_jsdoc().
  _cache_cleaned_jsdoc: _cache_cleaned_jsdoc().
  Cleaner.Cleaner: Cleaner.Cleaner.
  _previous_content_line: _previous_content_line().
  _strip_jsdoc_marker: _strip_jsdoc_marker().
---
# Module: [`tree_sitter_analyzer/languages/javascript_plugin/_jsdoc_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_jsdoc_helpers.py)

## Functions
- `_cache_cleaned_jsdoc(jsdoc_text: str, target_line: int, jsdoc_cache: dict[int, str], clean_jsdoc: Cleaner)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_jsdoc_helpers.py#L106)
- `_extract_multiline_jsdoc(content_lines: list[str], current_line: int, target_line: int, jsdoc_cache: dict[int, str], clean_jsdoc: Cleaner)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_jsdoc_helpers.py#L77)
- `_previous_content_line(content_lines: list[str], target_line: int)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_jsdoc_helpers.py#L65)
- `_strip_jsdoc_marker(line: str)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_jsdoc_helpers.py#L117)
- `clean_jsdoc(jsdoc_text: str)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_jsdoc_helpers.py#L51) — Clean JSDoc text by removing comment markers.
- `extract_jsdoc_for_line(content_lines: list[str], target_line: int, jsdoc_cache: dict[int, str], clean_jsdoc: Cleaner)` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_jsdoc_helpers.py#L13) — Extract JSDoc comment immediately before the specified line.

## Module values
- `Cleaner` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_jsdoc_helpers.py#L10)

