---
title: 'Module: tests/unit/test_kotlin_method_resolution.py'
type: catalog
provenance: extracted
module: tests/unit/test_kotlin_method_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_kotlin_method_resolution`/
symbols:
  _ctx: _ctx().
  test_build_context_returns_none_when_no_kotlin_file: test_build_context_returns_none_when_no_kotlin_file().
  test_local_top_level_function_resolves_local: test_local_top_level_function_resolves_local().
  test_this_method_resolves_local_when_unique: test_this_method_resolves_local_when_unique().
  test_super_method_resolves_local_when_unique: test_super_method_resolves_local_when_unique().
  test_this_method_ambiguous_across_classes_stays_unknown: test_this_method_ambiguous_across_classes_stays_unknown().
  test_this_method_does_not_bind_to_top_level_function: test_this_method_does_not_bind_to_top_level_function().
  test_unknown_local_name_stays_unknown: test_unknown_local_name_stays_unknown().
  test_bare_call_does_not_guess_other_file_same_language: test_bare_call_does_not_guess_other_file_same_language().
  test_bare_listof_classifies_stdlib: test_bare_listof_classifies_stdlib().
  test_bare_println_classifies_stdlib: test_bare_println_classifies_stdlib().
  test_bare_require_classifies_stdlib: test_bare_require_classifies_stdlib().
  test_local_def_shadows_stdlib_bare_function: test_local_def_shadows_stdlib_bare_function().
  test_project_owns_stdlib_name_in_other_kotlin_file_suppresses_stdlib: test_project_owns_stdlib_name_in_other_kotlin_file_suppresses_stdlib().
  test_receiver_method_call_stays_unknown: test_receiver_method_call_stays_unknown().
  test_qualified_stdlib_name_on_receiver_stays_unknown: test_qualified_stdlib_name_on_receiver_stays_unknown().
  test_no_cross_language_mis_wire_to_java_symbol: test_no_cross_language_mis_wire_to_java_symbol().
  test_no_cross_language_mis_wire_to_python_symbol: test_no_cross_language_mis_wire_to_python_symbol().
  test_stdlib_name_collision_with_java_symbol_still_stdlib: test_stdlib_name_collision_with_java_symbol_still_stdlib().
  _thunk: _thunk().
  test_build_context_built_when_kotlin_file_present: test_build_context_built_when_kotlin_file_present().
  test_kotlin_is_registered: test_kotlin_is_registered().
  _thunk._inner: _thunk()._inner().
---
# Module: [`tests/unit/test_kotlin_method_resolution.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py)

## Functions
- `_ctx(*, file_symbols: dict[str, list[tuple[str, str, int]]], file_languages: dict[str, str], global_name_table: dict[str, list[tuple[str, int]]] | None = None, file_class_methods: dict[str, dict[str, dict[str, int]]] | None = None)` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L42) — Build a Kotlin resolver context the way the registry would.
- `_inner()` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L36)
- `_thunk(value: dict[str, dict[str, dict[str, int]]] | None = None)` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L33) — A zero-arg lazy file_class_methods thunk (the registry passes a callable).
- `test_bare_call_does_not_guess_other_file_same_language()` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L187) — A bare call whose name is defined only in ANOTHER Kotlin file -> unknown
- `test_bare_listof_classifies_stdlib()` — [`L208`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L208) — ``listOf()`` is an auto-imported stdlib builder -> stdlib.
- `test_bare_println_classifies_stdlib()` — [`L218`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L218)
- `test_bare_require_classifies_stdlib()` — [`L227`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L227)
- `test_build_context_built_when_kotlin_file_present()` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L78)
- `test_build_context_returns_none_when_no_kotlin_file()` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L67)
- `test_kotlin_is_registered()` — [`L369`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L369) — Importing the languages package registers 'kotlin' in the registry.
- `test_local_def_shadows_stdlib_bare_function()` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L236) — A project top-level ``fun println(...)`` in the caller file shadows the
- `test_local_top_level_function_resolves_local()` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L89) — A bare call to a top-level function defined in the same file -> local.
- `test_no_cross_language_mis_wire_to_java_symbol()` — [`L295`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L295) — CRITICAL: a Kotlin callee whose bare name also exists as a symbol in a
- `test_no_cross_language_mis_wire_to_python_symbol()` — [`L327`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L327) — A bare Kotlin call whose name exists ONLY in a Python file -> unknown,
- `test_project_owns_stdlib_name_in_other_kotlin_file_suppresses_stdlib()` — [`L248`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L248) — If the project defines ``listOf`` as a function in ANOTHER Kotlin file, the
- `test_qualified_stdlib_name_on_receiver_stays_unknown()` — [`L278`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L278) — A stdlib NAME used as a member call (``something.listOf``) is NOT the bare
- `test_receiver_method_call_stays_unknown()` — [`L267`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L267) — A receiver method call (``items.map`` — receiver type not inferable) -> unknown.
- `test_stdlib_name_collision_with_java_symbol_still_stdlib()` — [`L346`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L346) — A Kotlin bare ``listOf()`` must classify stdlib even though a Java file
- `test_super_method_resolves_local_when_unique()` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L117) — ``super.helper()`` is also a member call -> unique same-file method.
- `test_this_method_ambiguous_across_classes_stays_unknown()` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L130) — Codex P2: ``this.helper()`` must NOT bind when the SAME file defines
- `test_this_method_does_not_bind_to_top_level_function()` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L161) — A receiver-qualified ``this.helper()`` must NOT bind to a top-level FREE
- `test_this_method_resolves_local_when_unique()` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L103) — ``this.helper()`` -> the same-file ``helper`` method (local) when unique.
- `test_unknown_local_name_stays_unknown()` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_kotlin_method_resolution.py#L177) — A bare name with no same-file definition and no stdlib signature -> unknown.

