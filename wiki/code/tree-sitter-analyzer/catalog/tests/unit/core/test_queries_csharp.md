---
title: 'Module: tests/unit/core/test_queries_csharp.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_queries_csharp.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_queries_csharp`/test_csharp_
symbols:
  test_csharp_all_queries_registry: all_queries_registry().
  test_csharp_get_all_queries: get_all_queries().
  test_csharp_list_queries: list_queries().
  test_csharp_query_descriptions: query_descriptions().
  test_csharp_queries_import: queries_import().
  test_csharp_class_query_structure: class_query_structure().
  test_csharp_all_queries_aliases: all_queries_aliases().
  test_csharp_get_query: get_query().
  test_csharp_get_query_not_found: get_query_not_found().
---
# Module: [`tests/unit/core/test_queries_csharp.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_csharp.py)

## Functions
- `test_csharp_all_queries_aliases()` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_csharp.py#L33) — Test cross-language aliases are registered.
- `test_csharp_all_queries_registry()` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_csharp.py#L22) — Test ALL_QUERIES registry is built from CSHARP_QUERIES and CSHARP_QUERY_DESCRIPTIONS.
- `test_csharp_class_query_structure()` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_csharp.py#L13) — Test C# class query contains expected patterns.
- `test_csharp_get_all_queries()` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_csharp.py#L49) — Test get_all_queries returns the full registry.
- `test_csharp_get_query()` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_csharp.py#L57) — Test get_query returns query strings for known names.
- `test_csharp_get_query_not_found()` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_csharp.py#L68) — Test get_query raises ValueError for unknown name.
- `test_csharp_list_queries()` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_csharp.py#L78) — Test list_queries returns all available query names.
- `test_csharp_queries_import()` — [`L4`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_csharp.py#L4) — Test that C# queries can be imported.
- `test_csharp_query_descriptions()` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_csharp.py#L90) — Test every query has a corresponding description.

