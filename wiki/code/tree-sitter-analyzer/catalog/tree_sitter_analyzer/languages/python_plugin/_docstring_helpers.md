---
title: 'Module: tree_sitter_analyzer/languages/python_plugin/_docstring_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/python_plugin/_docstring_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.python_plugin._docstring_helpers`/
symbols:
  find_docstring_after_line: find_docstring_after_line().
  DocstringSearchResult: DocstringSearchResult#
  _extract_docstring_from_quoted_lines: _extract_docstring_from_quoted_lines().
  DocstringSearchResult.value: DocstringSearchResult#value.
  DocstringSearchResult.cache_value: DocstringSearchResult#cache_value.
  DocstringSearchResult.should_cache: DocstringSearchResult#should_cache.
  _docstring_quote_type: _docstring_quote_type().
  _format_multiline_docstring: _format_multiline_docstring().
---
# Module: [`tree_sitter_analyzer/languages/python_plugin/_docstring_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_docstring_helpers.py)

## Classes
### `DocstringSearchResult`
- def: [`tree_sitter_analyzer/languages/python_plugin/_docstring_helpers.py:9`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_docstring_helpers.py#L9)
- signature: `class DocstringSearchResult:`
- members:
  - `cache_value` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_docstring_helpers.py#L11)
  - `should_cache` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_docstring_helpers.py#L12)
  - `value` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_docstring_helpers.py#L10)
- used by: [`_extract_docstring_for_line`](_core_extractor_mixin.md#PythonExtractorCoreMixin._extract_docstring_for_line), [`find_docstring_after_line`](_docstring_helpers.md#find_docstring_after_line), [`_extract_docstring_from_quoted_lines`](_docstring_helpers.md#_extract_docstring_from_quoted_lines)

## Functions
- `_docstring_quote_type(line: str)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_docstring_helpers.py#L34)
- `_extract_docstring_from_quoted_lines(content_lines: list[str], line_index: int, quote_type: str)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_docstring_helpers.py#L42)
- `_format_multiline_docstring(docstring_lines: list[str])` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_docstring_helpers.py#L61)
- `find_docstring_after_line(content_lines: list[str], target_line: int)` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_docstring_helpers.py#L15)

