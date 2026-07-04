---
title: 'Module: tests/unit/test_php_method_resolution.py'
type: catalog
provenance: extracted
module: tests/unit/test_php_method_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_php_method_resolution`/
symbols:
  _ctx: _ctx().
  test_no_cross_language_mis_wire_end_to_end: test_no_cross_language_mis_wire_end_to_end().
  test_resolve_callee_routes_php_to_php_resolver: test_resolve_callee_routes_php_to_php_resolver().
  test_resolve_callee_php_builtin_through_registry: test_resolve_callee_php_builtin_through_registry().
  test_build_context_built_when_php_file_present: test_build_context_built_when_php_file_present().
  test_php_is_registered_via_discovery: test_php_is_registered_via_discovery().
  test_build_context_does_not_force_thunk_for_non_php: test_build_context_does_not_force_thunk_for_non_php().
  test_same_file_free_function_resolves_local: test_same_file_free_function_resolves_local().
  test_namespaced_free_call_resolves_local_on_last_segment: test_namespaced_free_call_resolves_local_on_last_segment().
  test_relative_namespaced_free_call_resolves_local: test_relative_namespaced_free_call_resolves_local().
  test_builtin_bare_function_classifies_builtin: test_builtin_bare_function_classifies_builtin().
  test_builtin_array_map_classifies_builtin: test_builtin_array_map_classifies_builtin().
  test_builtin_json_encode_classifies_builtin: test_builtin_json_encode_classifies_builtin().
  test_project_free_function_shadows_builtin: test_project_free_function_shadows_builtin().
  test_project_owns_builtin_name_in_other_php_file_suppresses_builtin: test_project_owns_builtin_name_in_other_php_file_suppresses_builtin().
  test_this_method_call_unique_class_resolves_local: test_this_method_call_unique_class_resolves_local().
  test_self_static_call_unique_class_resolves_local: test_self_static_call_unique_class_resolves_local().
  test_this_method_call_ambiguous_across_classes_stays_unknown: test_this_method_call_ambiguous_across_classes_stays_unknown().
  test_parent_call_resolves_unique_class_method: test_parent_call_resolves_unique_class_method().
  test_static_receiver_call_stays_unknown: test_static_receiver_call_stays_unknown().
  test_namespaced_static_receiver_call_stays_unknown: test_namespaced_static_receiver_call_stays_unknown().
  test_instance_receiver_call_stays_unknown: test_instance_receiver_call_stays_unknown().
  test_bare_name_not_in_file_and_not_builtin_stays_unknown: test_bare_name_not_in_file_and_not_builtin_stays_unknown().
  test_bare_call_does_not_bind_sibling_method: test_bare_call_does_not_bind_sibling_method().
  test_no_cross_language_mis_wire_direct: test_no_cross_language_mis_wire_direct().
  test_no_cross_language_builtin_name_not_suppressed_by_python: test_no_cross_language_builtin_name_not_suppressed_by_python().
  test_build_context_returns_none_without_php_files: test_build_context_returns_none_without_php_files().
  test_external_tier_is_empty: test_external_tier_is_empty().
  test_build_context_does_not_force_thunk_for_non_php._thunk: test_build_context_does_not_force_thunk_for_non_php()._thunk().
---
# Module: [`tests/unit/test_php_method_resolution.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py)

## Functions
- `_ctx(symbols: dict[str, list[tuple[str, str, int]]], *, class_methods: dict[str, dict[str, dict[str, int]]] | None = None, global_table: dict[str, list[tuple[str, int]]] | None = None, languages: dict[str, str] | None = None)` — [`L111`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L111) — Build a PHP context for unit tests.
- `_thunk()` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L93)
- `test_bare_call_does_not_bind_sibling_method()` — [`L309`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L309) — A bare ``render()`` must NOT bind to a same-file class ``method`` named
- `test_bare_name_not_in_file_and_not_builtin_stays_unknown()` — [`L301`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L301)
- `test_build_context_built_when_php_file_present()` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L77)
- `test_build_context_does_not_force_thunk_for_non_php()` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L89) — The lazy class-method thunk must NOT be forced when no PHP file exists.
- `test_build_context_returns_none_without_php_files()` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L66)
- `test_builtin_array_map_classifies_builtin()` — [`L176`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L176)
- `test_builtin_bare_function_classifies_builtin()` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L168)
- `test_builtin_json_encode_classifies_builtin()` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L184)
- `test_external_tier_is_empty()` — [`L319`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L319) — The PHP external tier is intentionally empty (RFC-0008 precision).
- `test_instance_receiver_call_stays_unknown()` — [`L288`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L288) — ``$obj->bar`` — receiver is a variable whose class type the edge does not
- `test_namespaced_free_call_resolves_local_on_last_segment()` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L150) — ``\App\helper`` (namespace ```` split) resolves to a same-file free
- `test_namespaced_static_receiver_call_stays_unknown()` — [`L275`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L275) — ``App\Util::run`` is a static RECEIVER call (last separator ``::``), NOT
- `test_no_cross_language_builtin_name_not_suppressed_by_python()` — [`L384`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L384) — A Python symbol named ``count`` must NOT suppress PHP's ``count`` built-in
- `test_no_cross_language_mis_wire_direct()` — [`L363`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L363) — A PHP caller's bare ``helper`` must NEVER resolve to a Python file that
- `test_no_cross_language_mis_wire_end_to_end(tmp_path: Path)` — [`L403`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L403) — Index a polyglot repo where ``helper`` exists as a Python def AND as a
- `test_parent_call_resolves_unique_class_method()` — [`L255`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L255)
- `test_php_is_registered_via_discovery()` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L51) — Dropping ``languages/php.py`` auto-registers the PHP resolver — no edit
- `test_project_free_function_shadows_builtin()` — [`L192`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L192) — A project free function named like a built-in (``count``) shadows it —
- `test_project_owns_builtin_name_in_other_php_file_suppresses_builtin()` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L200) — A project free function named ``count`` in ANOTHER php file shadows the
- `test_relative_namespaced_free_call_resolves_local()` — [`L160`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L160)
- `test_resolve_callee_php_builtin_through_registry()` — [`L348`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L348)
- `test_resolve_callee_routes_php_to_php_resolver()` — [`L331`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L331)
- `test_same_file_free_function_resolves_local()` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L142)
- `test_self_static_call_unique_class_resolves_local()` — [`L228`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L228)
- `test_static_receiver_call_stays_unknown()` — [`L264`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L264) — ``Foo::bar`` — ``Foo`` is a class whose definition the edge does not
- `test_this_method_call_ambiguous_across_classes_stays_unknown()` — [`L239`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L239) — Two classes in one file both define ``save`` — the caller's enclosing
- `test_this_method_call_unique_class_resolves_local()` — [`L216`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_php_method_resolution.py#L216) — ``$this->process`` binds to the single class defining ``process``.

