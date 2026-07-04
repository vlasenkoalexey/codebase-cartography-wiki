---
title: 'Module: tests/unit/test_rust_method_resolution.py'
type: catalog
provenance: extracted
module: tests/unit/test_rust_method_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_rust_method_resolution`/
symbols:
  _ctx: _ctx().
  test_build_context_returns_none_when_no_rust_file: test_build_context_returns_none_when_no_rust_file().
  test_local_free_function_resolves_local: test_local_free_function_resolves_local().
  test_self_method_resolves_local: test_self_method_resolves_local().
  test_self_method_resolves_local_when_method_name_unique: test_self_method_resolves_local_when_method_name_unique().
  test_self_method_ambiguous_across_impls_stays_unknown: test_self_method_ambiguous_across_impls_stays_unknown().
  test_selfcap_method_ambiguous_across_impls_stays_unknown: test_selfcap_method_ambiguous_across_impls_stays_unknown().
  test_bare_free_fn_unaffected_by_method_duplicate: test_bare_free_fn_unaffected_by_method_duplicate().
  test_self_method_does_not_bind_to_free_function: test_self_method_does_not_bind_to_free_function().
  test_selfcap_assoc_does_not_bind_to_free_function: test_selfcap_assoc_does_not_bind_to_free_function().
  test_self_method_binds_method_even_when_free_fn_shares_name: test_self_method_binds_method_even_when_free_fn_shares_name().
  test_unknown_local_name_stays_unknown: test_unknown_local_name_stays_unknown().
  test_std_path_call_classifies_stdlib: test_std_path_call_classifies_stdlib().
  test_core_path_call_classifies_stdlib: test_core_path_call_classifies_stdlib().
  test_vec_new_associated_fn_classifies_stdlib: test_vec_new_associated_fn_classifies_stdlib().
  test_box_new_associated_fn_classifies_stdlib: test_box_new_associated_fn_classifies_stdlib().
  test_bare_new_stays_unknown: test_bare_new_stays_unknown().
  test_unknown_user_type_associated_fn_stays_unknown: test_unknown_user_type_associated_fn_stays_unknown().
  test_project_def_shadows_std_associated_fn: test_project_def_shadows_std_associated_fn().
  test_no_cross_language_mis_wire_to_other_language_symbol: test_no_cross_language_mis_wire_to_other_language_symbol().
  test_cross_language_bare_name_collision_python_only_owner: test_cross_language_bare_name_collision_python_only_owner().
  test_std_name_collision_with_python_symbol_still_stdlib: test_std_name_collision_with_python_symbol_still_stdlib().
  _thunk: _thunk().
  test_build_context_built_when_rust_file_present: test_build_context_built_when_rust_file_present().
  test_rust_is_registered: test_rust_is_registered().
  _thunk._inner: _thunk()._inner().
---
# Module: [`tests/unit/test_rust_method_resolution.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py)

## Functions
- `_ctx(*, file_symbols: dict[str, list[tuple[str, str, int]]], file_languages: dict[str, str], global_name_table: dict[str, list[tuple[str, int]]] | None = None)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L36) — Build a Rust resolver context the way the registry would.
- `_inner()` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L30)
- `_thunk(value: dict[str, dict[str, dict[str, int]]] | None = None)` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L27) — A zero-arg lazy file_class_methods thunk (the registry passes a callable).
- `test_bare_free_fn_unaffected_by_method_duplicate()` — [`L176`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L176) — A bare free-function call still resolves local even if an unrelated
- `test_bare_new_stays_unknown()` — [`L314`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L314) — A bare ``new`` with no std path (could be any project type) -> unknown.
- `test_box_new_associated_fn_classifies_stdlib()` — [`L305`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L305)
- `test_build_context_built_when_rust_file_present()` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L71)
- `test_build_context_returns_none_when_no_rust_file()` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L60)
- `test_core_path_call_classifies_stdlib()` — [`L283`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L283) — ``core::`` and ``alloc::`` paths are equally part of the std distribution.
- `test_cross_language_bare_name_collision_python_only_owner()` — [`L392`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L392) — A bare Rust call whose name exists ONLY in a Python file -> unknown, never
- `test_local_free_function_resolves_local()` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L82) — A bare call to a free function defined in the same file -> local.
- `test_no_cross_language_mis_wire_to_other_language_symbol()` — [`L360`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L360) — CRITICAL: a Rust callee whose bare name also exists as a symbol in a
- `test_project_def_shadows_std_associated_fn()` — [`L341`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L341) — If the project defines ``new`` and the call is ``Vec::new`` BUT a same-file
- `test_rust_is_registered()` — [`L433`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L433) — Importing the languages package registers 'rust' in the registry.
- `test_self_method_ambiguous_across_impls_stays_unknown()` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L130) — Codex P2: ``self.helper()`` must NOT bind when the SAME file defines
- `test_self_method_binds_method_even_when_free_fn_shares_name()` — [`L235`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L235) — When BOTH a free fn ``helper`` and exactly one impl METHOD ``helper`` exist in
- `test_self_method_does_not_bind_to_free_function()` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L195) — Codex P2 (#2): a receiver-qualified call ``self.helper()`` must NOT bind to a
- `test_self_method_resolves_local()` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L96) — ``self.helper()`` -> the same-file ``helper`` method (local).
- `test_self_method_resolves_local_when_method_name_unique()` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L110) — ``self.helper()`` resolves local only when exactly ONE method named
- `test_selfcap_assoc_does_not_bind_to_free_function()` — [`L222`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L222) — The ``Self::helper()`` form has the same hazard: a same-file FREE function
- `test_selfcap_method_ambiguous_across_impls_stays_unknown()` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L159) — The ``Self::helper()`` associated-call form has the same ambiguity hazard
- `test_std_name_collision_with_python_symbol_still_stdlib()` — [`L411`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L411) — A Rust ``std::mem::swap`` must classify stdlib even though a Python file
- `test_std_path_call_classifies_stdlib()` — [`L271`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L271) — A ``std::``-pathed associated call (``std::mem::swap``) -> stdlib.
- `test_unknown_local_name_stays_unknown()` — [`L258`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L258) — A bare name with no same-file definition and no std signature -> unknown.
- `test_unknown_user_type_associated_fn_stays_unknown()` — [`L329`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L329) — ``MyType::build`` (a project type's associated fn) -> unknown, never stdlib.
- `test_vec_new_associated_fn_classifies_stdlib()` — [`L295`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rust_method_resolution.py#L295) — ``Vec::new`` is a distinctively-std associated function -> stdlib.

