---
title: 'Module: tests/unit/test_resolver_registry.py'
type: catalog
provenance: extracted
module: tests/unit/test_resolver_registry.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_resolver_registry`/test_
symbols:
  test_resolve_callee_routes_to_registered_language: resolve_callee_routes_to_registered_language().
  test_resolve_callee_falls_back_when_no_registered_language: resolve_callee_falls_back_when_no_registered_language().
  test_java_is_registered_via_discovery: java_is_registered_via_discovery().
  test_every_language_module_registers_a_resolver: every_language_module_registers_a_resolver().
  test_resolve_callee_routes_to_registered_language.fake_resolve: resolve_callee_routes_to_registered_language().fake_resolve().
---
# Module: [`tests/unit/test_resolver_registry.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_resolver_registry.py)

## Functions
- `fake_resolve(bare, full, caller_file, lang_ctx)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_resolver_registry.py#L46)
- `test_every_language_module_registers_a_resolver()` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_resolver_registry.py#L27) — Discovery guard: every non-underscore module under languages/ must have
- `test_java_is_registered_via_discovery()` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_resolver_registry.py#L20) — The languages/ subpackage auto-registers Java (migrated from the inline
- `test_resolve_callee_falls_back_when_no_registered_language()` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_resolver_registry.py#L67) — A file whose language has no registered resolver falls through to the
- `test_resolve_callee_routes_to_registered_language()` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_resolver_registry.py#L41) — A file whose language has a registered resolver (and a built context) is

