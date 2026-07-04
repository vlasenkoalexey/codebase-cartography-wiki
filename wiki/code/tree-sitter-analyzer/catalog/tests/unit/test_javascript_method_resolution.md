---
title: 'Module: tests/unit/test_javascript_method_resolution.py'
type: catalog
provenance: extracted
module: tests/unit/test_javascript_method_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_javascript_method_resolution`/
symbols:
  _ctx: _ctx().
  _index_js: _index_js().
  test_javascript_is_registered: test_javascript_is_registered().
  test_jsx_is_registered: test_jsx_is_registered().
  test_jsx_caller_bare_call_stays_unknown_not_python_builtin: test_jsx_caller_bare_call_stays_unknown_not_python_builtin().
  test_jsx_local_resolution_works: test_jsx_local_resolution_works().
  test_bare_call_to_same_file_function_is_local: test_bare_call_to_same_file_function_is_local().
  test_bare_call_does_not_bind_to_same_file_method: test_bare_call_does_not_bind_to_same_file_method().
  test_self_receiver_does_not_bind_to_same_file_helper: test_self_receiver_does_not_bind_to_same_file_helper().
  test_self_receiver_does_not_bind_to_same_file_method: test_self_receiver_does_not_bind_to_same_file_method().
  test_this_method_call_is_local_via_class_methods: test_this_method_call_is_local_via_class_methods().
  test_this_method_does_not_bind_across_sibling_classes: test_this_method_does_not_bind_across_sibling_classes().
  test_this_method_does_not_bind_sibling_via_file_symbols: test_this_method_does_not_bind_sibling_via_file_symbols().
  test_this_method_single_class_binds_even_with_flat_symbols: test_this_method_single_class_binds_even_with_flat_symbols().
  test_this_method_single_class_still_binds: test_this_method_single_class_still_binds().
  test_namespaced_builtin_classifies_as_builtin: test_namespaced_builtin_classifies_as_builtin().
  test_bare_builtin_method_name_is_not_builtin: test_bare_builtin_method_name_is_not_builtin().
  test_console_log_is_not_builtin: test_console_log_is_not_builtin().
  test_project_shadow_of_builtin_receiver_suppresses_builtin: test_project_shadow_of_builtin_receiver_suppresses_builtin().
  test_variable_shadow_of_builtin_receiver_suppresses_builtin: test_variable_shadow_of_builtin_receiver_suppresses_builtin().
  test_variable_shadow_only_blocks_the_shadowed_receiver: test_variable_shadow_only_blocks_the_shadowed_receiver().
  test_single_js_global_resolves_to_project: test_single_js_global_resolves_to_project().
  test_bare_call_does_not_bind_to_a_method_global: test_bare_call_does_not_bind_to_a_method_global().
  test_bare_call_does_not_bind_to_a_class_global: test_bare_call_does_not_bind_to_a_class_global().
  test_bare_call_binds_to_a_function_global: test_bare_call_binds_to_a_function_global().
  test_ts_family_global_is_resolvable_from_js_caller: test_ts_family_global_is_resolvable_from_js_caller().
  test_ambiguous_global_stays_unknown: test_ambiguous_global_stays_unknown().
  test_no_cross_language_mis_wire_global: test_no_cross_language_mis_wire_global().
  test_no_cross_language_mis_wire_prefers_js_same_name: test_no_cross_language_mis_wire_prefers_js_same_name().
  test_no_cross_language_builtin_suppression_ignores_foreign_owner: test_no_cross_language_builtin_suppression_ignores_foreign_owner().
  test_shadow_set_from_cache_is_module_scope_only: test_shadow_set_from_cache_is_module_scope_only().
  test_build_returns_none_when_no_js_file_indexed: test_build_returns_none_when_no_js_file_indexed().
  test_build_returns_context_when_js_file_indexed: test_build_returns_context_when_js_file_indexed().
  test_build_returns_context_when_only_jsx_file_indexed: test_build_returns_context_when_only_jsx_file_indexed().
  test_module_level_variable_shadow_still_suppresses_builtin: test_module_level_variable_shadow_still_suppresses_builtin().
  test_function_local_shadow_no_longer_suppresses_builtin: test_function_local_shadow_no_longer_suppresses_builtin().
---
# Module: [`tests/unit/test_javascript_method_resolution.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py)

## Functions
- `_ctx(*, file_symbols=None, file_class_methods=None, global_name_table=None, file_languages=None, shadowed_globals=None)` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L26) — Build a JS resolver context from explicit maps (thunk-style fcm).
- `_index_js(tmp_path, files: dict[str, str])` — [`L506`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L506) — Index *files* into a tmp project; return a row-factory sqlite conn.
- `test_ambiguous_global_stays_unknown()` — [`L428`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L428) — Two JS definitions of the same bare name → unknown (no guess).
- `test_bare_builtin_method_name_is_not_builtin()` — [`L285`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L285) — A bare ``parse`` / ``keys`` (no namespace) must NOT classify as builtin —
- `test_bare_call_binds_to_a_function_global()` — [`L402`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L402) — The complement of the above: a bare call whose lone JS-family owner is a
- `test_bare_call_does_not_bind_to_a_class_global()` — [`L386`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L386) — A bare ``Widget()`` whose only owner is a *class* is a construction, not a
- `test_bare_call_does_not_bind_to_a_method_global()` — [`L368`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L368) — Codex P2 #346: ``global_name_table`` holds every function/method/class,
- `test_bare_call_does_not_bind_to_same_file_method()` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L132) — A bare ``render()`` (no receiver) in a file whose only same-name symbol is
- `test_bare_call_to_same_file_function_is_local()` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L120)
- `test_build_returns_context_when_js_file_indexed()` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L80)
- `test_build_returns_context_when_only_jsx_file_indexed()` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L85) — Codex P2 #346: a project containing only ``.jsx`` files (tagged ``"jsx"``)
- `test_build_returns_none_when_no_js_file_indexed()` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L67)
- `test_console_log_is_not_builtin()` — [`L302`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L302) — ``console`` is a commonly shadowed domain logger name; deliberately not
- `test_function_local_shadow_no_longer_suppresses_builtin(tmp_path)` — [`L571`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L571) — FULL INDEX PATH (#626 precision gain): a function-local ``const Math``
- `test_javascript_is_registered()` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L48)
- `test_jsx_caller_bare_call_stays_unknown_not_python_builtin()` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L92) — Codex P2 #346: the canonical bug — a bare ``len()`` in a JSX file. With
- `test_jsx_is_registered()` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L53) — Codex P2 #346: ``.jsx`` files are tagged ``"jsx"`` by the detector, and
- `test_jsx_local_resolution_works()` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L104) — A same-file bare call inside a ``.jsx`` file resolves ``local``.
- `test_module_level_variable_shadow_still_suppresses_builtin(tmp_path)` — [`L547`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L547) — FULL INDEX PATH (#626 keep-side): module-scope ``const Math = {...}``
- `test_namespaced_builtin_classifies_as_builtin()` — [`L271`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L271)
- `test_no_cross_language_builtin_suppression_ignores_foreign_owner()` — [`L486`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L486) — A foreign-language symbol named ``Math`` must NOT suppress the JS builtin
- `test_no_cross_language_mis_wire_global()` — [`L448`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L448) — A bare callee whose ONLY project definition lives in a Python file must
- `test_no_cross_language_mis_wire_prefers_js_same_name()` — [`L464`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L464) — When the name exists in BOTH a JS file and a foreign file, only the JS
- `test_project_shadow_of_builtin_receiver_suppresses_builtin()` — [`L313`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L313) — If the project owns a JS object literally named ``Math``, ``Math.max``
- `test_self_receiver_does_not_bind_to_same_file_helper()` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L153) — Codex P2 #346: in browser/worker JS, ``self`` is the global scope
- `test_self_receiver_does_not_bind_to_same_file_method()` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L167) — ``self.render()`` must not bind a same-file class method ``render`` —
- `test_shadow_set_from_cache_is_module_scope_only(tmp_path)` — [`L524`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L524) — SET-CONSTRUCTION pin through the real cache (#626): a module-level
- `test_single_js_global_resolves_to_project()` — [`L355`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L355)
- `test_this_method_call_is_local_via_class_methods()` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L181)
- `test_this_method_does_not_bind_across_sibling_classes()` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L193) — Codex P2 #346: ``class A { run() { this.render(); } } class B { render(){} }``.
- `test_this_method_does_not_bind_sibling_via_file_symbols()` — [`L212`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L212) — Codex P2 #346 (line 235): real resolver contexts populate ``file_symbols``
- `test_this_method_single_class_binds_even_with_flat_symbols()` — [`L238`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L238) — The single-class case must still bind via ``file_class_methods`` even when
- `test_this_method_single_class_still_binds()` — [`L254`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L254) — Sanity: with exactly ONE class in the file, ``this.<method>`` is
- `test_ts_family_global_is_resolvable_from_js_caller()` — [`L417`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L417) — JS/TS are one interop family — a single ``.ts`` global is a valid bind.
- `test_variable_shadow_of_builtin_receiver_suppresses_builtin()` — [`L324`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L324) — Codex P2 #346: ``const Math = { max() {} }; Math.max()``. The shadow is a
- `test_variable_shadow_only_blocks_the_shadowed_receiver()` — [`L338`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_javascript_method_resolution.py#L338) — A variable shadow of ``Math`` must NOT suppress an unrelated builtin

