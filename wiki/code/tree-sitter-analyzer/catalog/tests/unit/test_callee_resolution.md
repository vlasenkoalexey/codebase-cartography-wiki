---
title: 'Module: tests/unit/test_callee_resolution.py'
type: catalog
provenance: extracted
module: tests/unit/test_callee_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_callee_resolution`/
symbols:
  Func: Func#
  test_resolver_supports_qualified_import_aliases_and_file_results: test_resolver_supports_qualified_import_aliases_and_file_results().
  test_resolver_first_match_helpers_avoid_collecting_all_candidates: test_resolver_first_match_helpers_avoid_collecting_all_candidates().
  test_resolver_prefers_same_file_then_import_then_global: test_resolver_prefers_same_file_then_import_then_global().
  test_resolver_can_return_import_file_without_matching_symbol: test_resolver_can_return_import_file_without_matching_symbol().
  test_resolver_can_limit_resolution_to_specific_phases: test_resolver_can_limit_resolution_to_specific_phases().
  test_global_fallback_gated_by_language_for_function_less_file: test_global_fallback_gated_by_language_for_function_less_file().
  test_global_fallback_allows_js_ts_family: test_global_fallback_allows_js_ts_family().
  test_global_fallback_demotes_test_shadow_for_source_caller: test_global_fallback_demotes_test_shadow_for_source_caller().
  test_global_fallback_keeps_test_target_for_test_caller: test_global_fallback_keeps_test_target_for_test_caller().
  Func.name: Func#name.
  Func.file: Func#file.
  Func.line: Func#line.
---
# Module: [`tests/unit/test_callee_resolution.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callee_resolution.py)

## Classes
### `Func`
- def: [`tests/unit/test_callee_resolution.py:11`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callee_resolution.py#L11)
- signature: `class Func:`
- members:
  - `file` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callee_resolution.py#L13)
  - `line` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callee_resolution.py#L14)
  - `name` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callee_resolution.py#L12)
- used by: (4 test-only callers)

## Functions
- `test_global_fallback_allows_js_ts_family()` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callee_resolution.py#L139) — Codex P2 #301: JavaScript and TypeScript are one interop family.
- `test_global_fallback_demotes_test_shadow_for_source_caller()` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callee_resolution.py#L154) — Codex/dogfood: a non-test caller must prefer the source def over a test mock.
- `test_global_fallback_gated_by_language_for_function_less_file()` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callee_resolution.py#L123) — Codex P2 #301: a caller file with no indexed functions is still gated.
- `test_global_fallback_keeps_test_target_for_test_caller()` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callee_resolution.py#L182) — A test caller may still resolve to a test helper (no demotion).
- `test_resolver_can_limit_resolution_to_specific_phases()` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callee_resolution.py#L67)
- `test_resolver_can_return_import_file_without_matching_symbol()` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callee_resolution.py#L52)
- `test_resolver_first_match_helpers_avoid_collecting_all_candidates()` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callee_resolution.py#L95)
- `test_resolver_prefers_same_file_then_import_then_global()` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callee_resolution.py#L17)
- `test_resolver_supports_qualified_import_aliases_and_file_results()` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callee_resolution.py#L40)

