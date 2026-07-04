---
title: 'Module: tests/fixtures/assertion_helpers.py'
type: catalog
provenance: extracted
module: tests/fixtures/assertion_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.fixtures.assertion_helpers`/
symbols:
  assert_analysis_result_valid: assert_analysis_result_valid().
  assert_file_output_valid: assert_file_output_valid().
  assert_has_keys: assert_has_keys().
  assert_dict_structure: assert_dict_structure().
  assert_element_has_required_fields: assert_element_has_required_fields().
  assert_list_contains_dicts_with_key: assert_list_contains_dicts_with_key().
  assert_query_result_valid: assert_query_result_valid().
  assert_no_duplicate_elements: assert_no_duplicate_elements().
  assert_error_message_contains: assert_error_message_contains().
  assert_performance_acceptable: assert_performance_acceptable().
  __all__: __all__.
---
# Module: [`tests/fixtures/assertion_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/assertion_helpers.py)

## Functions
- `assert_analysis_result_valid(result: dict[str, Any], expected_language: str | None = None, expected_file: str | None = None, require_success: bool = True)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/assertion_helpers.py#L74) — Assert that analysis result has valid structure.
- `assert_dict_structure(data: dict[str, Any], expected_structure: dict[str, type])` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/assertion_helpers.py#L46) — Assert that dictionary has expected structure with correct types.
- `assert_element_has_required_fields(element: dict[str, Any], element_type: str)` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/assertion_helpers.py#L119) — Assert that extracted element has required fields.
- `assert_error_message_contains(error_msg: str, expected_substrings: list[str])` — [`L295`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/assertion_helpers.py#L295) — Assert that error message contains expected substrings.
- `assert_file_output_valid(output: dict[str, Any], expected_format: str | None = None)` — [`L238`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/assertion_helpers.py#L238) — Assert that file output has valid structure.
- `assert_has_keys(data: dict[str, Any], required_keys: list[str], optional_keys: list[str] | None = None)` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/assertion_helpers.py#L14) — Assert that dictionary has required keys and only allowed keys.
- `assert_list_contains_dicts_with_key(items: list[dict[str, Any]], key: str, expected_values: set[Any] | None = None)` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/assertion_helpers.py#L155) — Assert that list contains dictionaries with specified key.
- `assert_no_duplicate_elements(elements: list[dict[str, Any]], key: str = "name")` — [`L269`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/assertion_helpers.py#L269) — Assert that list has no duplicate elements based on key.
- `assert_performance_acceptable(elapsed_time: float, max_time: float, operation: str = "operation")` — [`L321`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/assertion_helpers.py#L321) — Assert that operation completed within acceptable time.
- `assert_query_result_valid(result: list[dict[str, Any]], min_matches: int = 0, max_matches: int | None = None, require_node: bool = True, require_text: bool = True)` — [`L191`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/assertion_helpers.py#L191) — Assert that query result has valid structure.

## Module values
- `__all__` — [`L346`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/assertion_helpers.py#L346)

