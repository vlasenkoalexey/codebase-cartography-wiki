---
title: 'Module: tests/unit/test_ruby_method_resolution.py'
type: catalog
provenance: extracted
module: tests/unit/test_ruby_method_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_ruby_method_resolution`/
symbols:
  _ctx: _ctx().
  test_ruby_is_registered: test_ruby_is_registered().
  test_bare_call_to_same_file_function_is_local: test_bare_call_to_same_file_function_is_local().
  test_bare_call_does_not_bind_to_same_file_method: test_bare_call_does_not_bind_to_same_file_method().
  test_unknown_bare_name_stays_unknown: test_unknown_bare_name_stays_unknown().
  test_self_method_call_is_local_via_class_methods: test_self_method_call_is_local_via_class_methods().
  test_self_method_does_not_bind_across_sibling_classes: test_self_method_does_not_bind_across_sibling_classes().
  test_self_method_does_not_bind_sibling_via_file_symbols: test_self_method_does_not_bind_sibling_via_file_symbols().
  test_self_method_single_class_binds_even_with_flat_symbols: test_self_method_single_class_binds_even_with_flat_symbols().
  test_namespaced_builtin_classifies_as_builtin: test_namespaced_builtin_classifies_as_builtin().
  test_bare_builtin_method_name_is_not_builtin: test_bare_builtin_method_name_is_not_builtin().
  test_puts_is_not_builtin: test_puts_is_not_builtin().
  test_project_shadow_of_builtin_receiver_suppresses_builtin: test_project_shadow_of_builtin_receiver_suppresses_builtin().
  test_single_ruby_global_resolves_to_project: test_single_ruby_global_resolves_to_project().
  test_bare_call_does_not_bind_to_a_method_global: test_bare_call_does_not_bind_to_a_method_global().
  test_bare_call_does_not_bind_to_a_class_global: test_bare_call_does_not_bind_to_a_class_global().
  test_bare_call_binds_to_a_function_global: test_bare_call_binds_to_a_function_global().
  test_ambiguous_global_stays_unknown: test_ambiguous_global_stays_unknown().
  test_no_cross_language_mis_wire_global: test_no_cross_language_mis_wire_global().
  test_no_cross_language_mis_wire_prefers_ruby_same_name: test_no_cross_language_mis_wire_prefers_ruby_same_name().
  test_no_cross_language_builtin_suppression_ignores_foreign_owner: test_no_cross_language_builtin_suppression_ignores_foreign_owner().
  test_build_returns_none_when_no_ruby_file_indexed: test_build_returns_none_when_no_ruby_file_indexed().
  test_build_returns_context_when_ruby_file_indexed: test_build_returns_context_when_ruby_file_indexed().
---
# Module: [`tests/unit/test_ruby_method_resolution.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py)

## Functions
- `_ctx(*, file_symbols=None, file_class_methods=None, global_name_table=None, file_languages=None)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L28) — Build a Ruby resolver context from explicit maps (thunk-style fcm).
- `test_ambiguous_global_stays_unknown()` — [`L313`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L313) — Two Ruby definitions of the same bare name → unknown (no guess).
- `test_bare_builtin_method_name_is_not_builtin()` — [`L210`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L210) — A bare ``sqrt`` (no namespace) must NOT classify as builtin — every domain
- `test_bare_call_binds_to_a_function_global()` — [`L298`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L298) — The complement: a bare call whose lone Ruby owner is a top-level
- `test_bare_call_does_not_bind_to_a_class_global()` — [`L282`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L282) — A bare ``Widget`` whose only owner is a *class* is a constant reference, not
- `test_bare_call_does_not_bind_to_a_method_global()` — [`L265`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L265) — A BARE ``render`` (no receiver) cannot call a class METHOD — methods need
- `test_bare_call_does_not_bind_to_same_file_method()` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L89) — A bare ``render`` (no receiver) in a file whose only same-name symbol is a
- `test_bare_call_to_same_file_function_is_local()` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L77)
- `test_build_returns_context_when_ruby_file_indexed()` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L69)
- `test_build_returns_none_when_no_ruby_file_indexed()` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L56)
- `test_namespaced_builtin_classifies_as_builtin()` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L196)
- `test_no_cross_language_builtin_suppression_ignores_foreign_owner()` — [`L372`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L372) — A foreign-language symbol named ``Math`` must NOT suppress the Ruby builtin
- `test_no_cross_language_mis_wire_global()` — [`L333`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L333) — A bare callee whose ONLY project definition lives in a Python file must
- `test_no_cross_language_mis_wire_prefers_ruby_same_name()` — [`L350`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L350) — When the name exists in BOTH a Ruby file and a foreign file, only the Ruby
- `test_project_shadow_of_builtin_receiver_suppresses_builtin()` — [`L238`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L238) — If the project owns a Ruby constant literally named ``Math``, ``Math.sqrt``
- `test_puts_is_not_builtin()` — [`L227`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L227) — ``puts`` is a ubiquitous bare ``Kernel`` name that every object/DSL can
- `test_ruby_is_registered()` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L48)
- `test_self_method_call_is_local_via_class_methods()` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L123) — In Ruby ``self`` is the current object, so ``self.render`` in a single-class
- `test_self_method_does_not_bind_across_sibling_classes()` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L137) — ``class A; def run; self.render; end; end; class B; def render; end; end``.
- `test_self_method_does_not_bind_sibling_via_file_symbols()` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L156) — Real resolver contexts populate ``file_symbols`` with EVERY method in the
- `test_self_method_single_class_binds_even_with_flat_symbols()` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L177) — The single-class case must still bind via ``file_class_methods`` even when
- `test_single_ruby_global_resolves_to_project()` — [`L252`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L252)
- `test_unknown_bare_name_stays_unknown()` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ruby_method_resolution.py#L109) — A bare call with no same-file def and no project owner stays ``unknown``

