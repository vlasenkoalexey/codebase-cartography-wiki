---
title: 'Module: tests/unit/core/test_queries_typescript_abstract_method.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_queries_typescript_abstract_method.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_queries_typescript_abstract_method`/
symbols:
  _run_query: _run_query().
  test_functions_query_captures_abstract_methods_exact_count: test_functions_query_captures_abstract_methods_exact_count().
  test_signatures_query_captures_abstract_methods_exact_count: test_signatures_query_captures_abstract_methods_exact_count().
  test_get_element_categories_method_includes_abstract_method_signature: test_get_element_categories_method_includes_abstract_method_signature().
  test_get_element_categories_signature_includes_abstract_method_signature: test_get_element_categories_signature_includes_abstract_method_signature().
  _parse: _parse().
  test_functions_query_contains_abstract_method_signature_pattern: test_functions_query_contains_abstract_method_signature_pattern().
  test_signatures_query_contains_abstract_method_signature_pattern: test_signatures_query_contains_abstract_method_signature_pattern().
  _ABSTRACT_SRC: _ABSTRACT_SRC.
  _lang: _lang().
---
# Module: [`tests/unit/core/test_queries_typescript_abstract_method.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_abstract_method.py)

## Functions
- `_lang()` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_abstract_method.py#L36)
- `_parse(src: str)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_abstract_method.py#L40)
- `_run_query(query_string: str, src: str)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_abstract_method.py#L46) — Execute a tree-sitter query string against *src* and return captures.
- `test_functions_query_captures_abstract_methods_exact_count()` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_abstract_method.py#L68) — Running FUNCTIONS against a 3-abstract-method snippet must yield exactly 3
- `test_functions_query_contains_abstract_method_signature_pattern()` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_abstract_method.py#L59) — FUNCTIONS string must reference abstract_method_signature so the query
- `test_get_element_categories_method_includes_abstract_method_signature()` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_abstract_method.py#L116) — TypeScriptPlugin.get_element_categories()['method'] must include
- `test_get_element_categories_signature_includes_abstract_method_signature()` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_abstract_method.py#L128) — TypeScriptPlugin.get_element_categories()['signature'] must include
- `test_signatures_query_captures_abstract_methods_exact_count()` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_abstract_method.py#L96) — Running SIGNATURES against the 3-abstract-method snippet must yield
- `test_signatures_query_contains_abstract_method_signature_pattern()` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_abstract_method.py#L89) — SIGNATURES string must reference abstract_method_signature.

## Module values
- `_ABSTRACT_SRC` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_abstract_method.py#L27)

