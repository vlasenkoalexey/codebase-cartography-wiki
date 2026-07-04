---
title: 'Module: tree_sitter_analyzer/_api_result_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_api_result_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._api_result_helpers`/
symbols:
  element_to_dict: element_to_dict().
  file_analysis_result: file_analysis_result().
  find_class_name: find_class_name().
  code_analysis_result: code_analysis_result().
  file_analysis_error: file_analysis_error().
  code_analysis_error: code_analysis_error().
  _with_success_sections: _with_success_sections().
  normalize_parameters: normalize_parameters().
  _OPTIONAL_ELEM_FIELDS: _OPTIONAL_ELEM_FIELDS.
  _contained_in_other_function: _contained_in_other_function().
---
# Module: [`tree_sitter_analyzer/_api_result_helpers.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_result_helpers.py)

## Functions
- `_contained_in_other_function(elem: Any, elements: Sequence[Any])` — [`L107`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_result_helpers.py#L107) — True when another function's span strictly contains ``elem``'s.
- `_with_success_sections(result: dict[str, Any], analysis_result: Any, *, include_elements: bool, include_queries: bool)` — [`L205`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_result_helpers.py#L205)
- `code_analysis_error(language: str, error: Exception)` — [`L251`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_result_helpers.py#L251) — Build the public API error response for source-string analysis.
- `code_analysis_result(analysis_result: Any, requested_language: str, *, include_elements: bool, include_queries: bool)` — [`L178`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_result_helpers.py#L178) — Build the public API response for source-string analysis.
- `element_to_dict(elem: Any, all_elements: Sequence[Any] | None = None, result_language: str | None = None)` — [`L53`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_result_helpers.py#L53) — Convert an analysis element to the stable API dict representation.
- `file_analysis_error(file_path: str | Path, language: str | None, error: Exception)` — [`L238`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_result_helpers.py#L238) — Build the public API error response for file analysis.
- `file_analysis_result(analysis_result: Any, file_path: str | Path, requested_language: str | None, *, include_elements: bool, include_queries: bool)` — [`L146`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_result_helpers.py#L146) — Build the public API response for file analysis.
- `find_class_name(elem: Any, elements: Sequence[Any])` — [`L123`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_result_helpers.py#L123) — Find the containing class name for a method element.
- `normalize_parameters(value: Any)` — [`L38`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_result_helpers.py#L38) — Convert a parameters value to a JSON-safe representation.

## Module values
- `_OPTIONAL_ELEM_FIELDS` — [`L8`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_api_result_helpers.py#L8)

