---
title: 'Module: tests/unit/core/test_queries_ruby.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_queries_ruby.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_queries_ruby`/test_
symbols:
  test_ruby_queries_import: ruby_queries_import().
  test_get_all_queries: get_all_queries().
  test_list_queries: list_queries().
  test_ruby_class_query_structure: ruby_class_query_structure().
  test_ruby_method_query_structure: ruby_method_query_structure().
  test_ruby_constant_query_structure: ruby_constant_query_structure().
  test_all_queries_dict_structure: all_queries_dict_structure().
  test_all_queries_aliases: all_queries_aliases().
  test_get_query_existing: get_query_existing().
  test_get_query_alias: get_query_alias().
  test_get_query_not_found: get_query_not_found().
---
# Module: [`tests/unit/core/test_queries_ruby.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_ruby.py)

## Functions
- `test_all_queries_aliases()` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_ruby.py#L60) — Test cross-language aliases point to correct entries.
- `test_all_queries_dict_structure()` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_ruby.py#L46) — Test ALL_QUERIES contains expected keys and structure.
- `test_get_all_queries()` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_ruby.py#L71) — Test get_all_queries returns the full query registry.
- `test_get_query_alias()` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_ruby.py#L90) — Test get_query works with alias names.
- `test_get_query_existing()` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_ruby.py#L81) — Test get_query returns query string for known names.
- `test_get_query_not_found()` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_ruby.py#L99) — Test get_query raises ValueError for unknown names.
- `test_list_queries()` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_ruby.py#L109) — Test list_queries returns all query names including aliases.
- `test_ruby_class_query_structure()` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_ruby.py#L22) — Test Ruby class query contains expected patterns.
- `test_ruby_constant_query_structure()` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_ruby.py#L38) — Test Ruby constant query contains expected patterns.
- `test_ruby_method_query_structure()` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_ruby.py#L30) — Test Ruby method query contains expected patterns.
- `test_ruby_queries_import()` — [`L4`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_ruby.py#L4) — Test that Ruby queries can be imported.

