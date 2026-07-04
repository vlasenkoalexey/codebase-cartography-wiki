---
title: 'Module: tests/unit/languages/test_typescript_namespace_extraction.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_typescript_namespace_extraction.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_typescript_namespace_extraction`/
symbols:
  _extract_classes: _extract_classes().
  _extract_function_names: _extract_function_names().
  test_nested_namespace_name: test_nested_namespace_name().
  test_ambient_string_module_name: test_ambient_string_module_name().
  test_symbols_inside_namespace_extracted: test_symbols_inside_namespace_extracted().
  test_top_level_kinds_unchanged: test_top_level_kinds_unchanged().
  _parse: _parse().
  TS_SRC: TS_SRC.
  test_namespace_itself_extracted: test_namespace_itself_extracted().
  test_module_itself_extracted: test_module_itself_extracted().
  test_nameless_namespace_node_returns_none: test_nameless_namespace_node_returns_none().
  test_namespace_extractor_exception_returns_none: test_namespace_extractor_exception_returns_none().
---
# Module: [`tests/unit/languages/test_typescript_namespace_extraction.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_namespace_extraction.py)

## Functions
- `_extract_classes()` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_namespace_extraction.py#L48)
- `_extract_function_names()` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_namespace_extraction.py#L54)
- `_parse()` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_namespace_extraction.py#L42)
- `test_ambient_string_module_name()` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_namespace_extraction.py#L97) — ``declare module "pkg" { }`` carries a string name — quotes stripped.
- `test_module_itself_extracted()` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_namespace_extraction.py#L64)
- `test_nameless_namespace_node_returns_none()` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_namespace_extraction.py#L108) — A namespace node with no name child must be skipped, not crash.
- `test_namespace_extractor_exception_returns_none()` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_namespace_extraction.py#L126) — An exploding node must be caught and yield None (error path).
- `test_namespace_itself_extracted()` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_namespace_extraction.py#L59)
- `test_nested_namespace_name()` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_namespace_extraction.py#L86) — ``namespace A.B { }`` carries a nested_identifier name.
- `test_symbols_inside_namespace_extracted()` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_namespace_extraction.py#L69) — The critical bug: everything inside a namespace was silently lost.
- `test_top_level_kinds_unchanged()` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_namespace_extraction.py#L78)

## Module values
- `TS_SRC` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_namespace_extraction.py#L20)

