---
title: 'Module: tests/unit/languages/_test_sql_plugin_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/languages/_test_sql_plugin_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages._test_sql_plugin_helpers`/
symbols:
  assert_end_to_end_sql_analysis_and_formatting: assert_end_to_end_sql_analysis_and_formatting().
  assert_e2e_sql_formatting: assert_e2e_sql_formatting().
  assert_sample_database_result: assert_sample_database_result().
  assert_analysis_with_tree_sitter_disabled: assert_analysis_with_tree_sitter_disabled().
  analyze_temp_sql: analyze_temp_sql().
  assert_analysis_with_missing_language: assert_analysis_with_missing_language().
  assert_specific_sql_constructs: assert_specific_sql_constructs().
  parse_sql: parse_sql().
  assert_sql_analysis_result_allows_fallback: assert_sql_analysis_result_allows_fallback().
  build_sql_parser: build_sql_parser().
  extract_sql_elements: extract_sql_elements().
  SAMPLE_DATABASE_EXPECTED_CLASSES: SAMPLE_DATABASE_EXPECTED_CLASSES.
  E2E_SQL_CONTENT: E2E_SQL_CONTENT.
  SIMPLE_SQL_CONTENT: SIMPLE_SQL_CONTENT.
  build_parser_for_language: build_parser_for_language().
  write_temp_sql_file: write_temp_sql_file().
  SAMPLE_DATABASE_EXPECTED_FUNCTIONS: SAMPLE_DATABASE_EXPECTED_FUNCTIONS.
  SAMPLE_DATABASE_EXPECTED_INDEXES: SAMPLE_DATABASE_EXPECTED_INDEXES.
  SQL_CONSTRUCT_CASES: SQL_CONSTRUCT_CASES.
  SQL_FALLBACK_ERROR_MESSAGES: SQL_FALLBACK_ERROR_MESSAGES.
  elements_grouped_by_model_type: elements_grouped_by_model_type().
  assert_table_metadata: assert_table_metadata().
  assert_product_columns: assert_product_columns().
  assert_view_dependencies: assert_view_dependencies().
---
# Module: [`tests/unit/languages/_test_sql_plugin_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py)

## Functions
- `analyze_temp_sql(plugin: Any, sql_content: str)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L292) — Analyze a temporary SQL file and remove it before returning.
- `assert_analysis_with_missing_language(plugin: Any)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L276) — Assert analyze_file handles a missing SQL parser language gracefully.
- `assert_analysis_with_tree_sitter_disabled(plugin: Any)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L259) — Assert analyze_file handles a disabled tree-sitter runtime gracefully.
- `assert_e2e_sql_formatting(plugin: Any, sql_content: str, file_path: str | Path)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L319) — Assert all SQL formatters can render extracted SQL elements.
- `assert_end_to_end_sql_analysis_and_formatting(plugin: Any)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L240) — Assert the SQL plugin can analyze and format one realistic SQL file.
- `assert_product_columns(sql_elements: list[Any])` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L214) — Assert products table column extraction covers known columns.
- `assert_sample_database_result(result: Any)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L134) — Assert broad sample_database.sql extraction expectations.
- `assert_specific_sql_constructs(plugin: Any)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L179) — Assert extraction for a table, view, index, and SQL function.
- `assert_sql_analysis_result_allows_fallback(result: Any)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L304) — Assert the SQL analysis result either succeeds by fallback or fails clearly.
- `assert_table_metadata(sql_elements: list[Any])` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L203) — Assert at least one SQL table element exposes metadata fields.
- `assert_view_dependencies(sql_elements: list[Any])` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L227) — Assert user_orders view exposes dependency metadata when extracted.
- `build_parser_for_language(language: Any)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L110) — Build a parser for an already-loaded tree-sitter language.
- `build_sql_parser()` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L101) — Build a tree-sitter SQL parser across supported tree-sitter APIs.
- `elements_grouped_by_model_type(elements: list[Any])` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L156) — Group generic analysis elements by their model class name.
- `extract_sql_elements(plugin: Any, sql_content: str)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L129) — Parse SQL content and return SQL-specific elements.
- `parse_sql(sql_content: str)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L124) — Parse SQL content using tree-sitter-sql.
- `write_temp_sql_file(sql_content: str)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L312) — Write SQL content to a temporary .sql file and return the path.

## Module values
- `E2E_SQL_CONTENT` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L75)
- `SAMPLE_DATABASE_EXPECTED_CLASSES` — [`L9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L9)
- `SAMPLE_DATABASE_EXPECTED_FUNCTIONS` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L16)
- `SAMPLE_DATABASE_EXPECTED_INDEXES` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L24)
- `SIMPLE_SQL_CONTENT` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L97)
- `SQL_CONSTRUCT_CASES` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L34)
- `SQL_FALLBACK_ERROR_MESSAGES` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_sql_plugin_helpers.py#L98)

