---
title: 'Module: tests/unit/languages/_test_sql_function_extraction_properties_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/languages/_test_sql_function_extraction_properties_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages._test_sql_function_extraction_properties_helpers`/
symbols:
  extract_sql_elements: extract_sql_elements().
  assert_regex_pattern_precision: assert_regex_pattern_precision().
  is_invalid_function_name: is_invalid_function_name().
  extract_function_names: extract_function_names().
  assert_sql_keywords_exclusion: assert_sql_keywords_exclusion().
  assert_function_boundary_detection: assert_function_boundary_detection().
  assert_valid_vs_invalid_identifier_extraction: assert_valid_vs_invalid_identifier_extraction().
  assert_extraction_count_consistency: assert_extraction_count_consistency().
  assert_output_ordering_preservation: assert_output_ordering_preservation().
  assert_deterministic_extraction: assert_deterministic_extraction().
  extract_functions: extract_functions().
  INVALID_FUNCTION_NAMES: INVALID_FUNCTION_NAMES.
  select_valid_function_names: select_valid_function_names().
  build_multiple_function_sql: build_multiple_function_sql().
  assert_function_body_content_exclusion: assert_function_body_content_exclusion().
  assert_invalid_identifier_rejected: assert_invalid_identifier_rejected().
  lower_names: lower_names().
  extract_function_tuples: extract_function_tuples().
  COMMON_COLUMN_NAMES: COMMON_COLUMN_NAMES.
  SQL_KEYWORDS: SQL_KEYWORDS.
  BODY_KEYWORDS: BODY_KEYWORDS.
  build_single_function_sql: build_single_function_sql().
  expected_function_lines: expected_function_lines().
---
# Module: [`tests/unit/languages/_test_sql_function_extraction_properties_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py)

## Functions
- `assert_deterministic_extraction(func_names: list[str], num_runs: int)` — [`L463`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L463)
- `assert_extraction_count_consistency(num_functions: int, func_names: list[str])` — [`L420`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L420)
- `assert_function_body_content_exclusion(func_name: str, column_name: str)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L210)
- `assert_function_boundary_detection(func_name: str, body_lines: int)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L303)
- `assert_invalid_identifier_rejected(invalid_name: str)` — [`L353`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L353)
- `assert_output_ordering_preservation(func_names: list[str])` — [`L442`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L442)
- `assert_regex_pattern_precision(func_name: str, line_content: str)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L274)
- `assert_sql_keywords_exclusion(func_name: str, keyword: str)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L242)
- `assert_valid_vs_invalid_identifier_extraction(valid_name: str, invalid_name: str)` — [`L380`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L380)
- `build_multiple_function_sql(names: list[str], body_template: str = " RETURN param * 2;")` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L198) — Build a SQL source containing CREATE FUNCTION declarations in order.
- `build_single_function_sql(func_name: str, body: str, parameter: str = "param INT")` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L183) — Build a MySQL-style CREATE FUNCTION block.
- `expected_function_lines(sql_code: str)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L341) — Return expected CREATE FUNCTION and END lines for generated SQL.
- `extract_function_names(sql_code: str)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L173) — Extract function names from source.
- `extract_function_tuples(sql_code: str)` — [`L491`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L491) — Create a deterministic representation of function extraction results.
- `extract_functions(sql_code: str)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L163) — Extract only SQL function elements from source.
- `extract_sql_elements(sql_code: str)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L146) — Parse SQL and return extracted elements using a fresh plugin instance.
- `is_invalid_function_name(name: str)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L133) — Return true when a candidate should be rejected as a function name.
- `lower_names(names: list[str])` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L178) — Return lower-cased function names for case-insensitive checks.
- `select_valid_function_names(names: list[str], limit: int | None = None)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L138) — Filter property-generated identifiers using the extractor's invalid-name set.

## Module values
- `BODY_KEYWORDS` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L121)
- `COMMON_COLUMN_NAMES` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L12)
- `INVALID_FUNCTION_NAMES` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L120)
- `SQL_KEYWORDS` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_function_extraction_properties_helpers.py#L34)

