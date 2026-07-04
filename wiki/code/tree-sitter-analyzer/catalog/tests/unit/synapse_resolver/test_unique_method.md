---
title: 'Module: tests/unit/synapse_resolver/test_unique_method.py'
type: catalog
provenance: extracted
module: tests/unit/synapse_resolver/test_unique_method.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.synapse_resolver.test_unique_method`/
symbols:
  _ctx: _ctx().
  test_unique_method_receiver_resolves_to_project: test_unique_method_receiver_resolves_to_project().
  test_class_method_disambiguates_non_unique: test_class_method_disambiguates_non_unique().
  test_self_method_via_callee_full_resolves_local: test_self_method_via_callee_full_resolves_local().
  test_unique_method_via_production_callee_full: test_unique_method_via_production_callee_full().
  test_self_method_resolves_within_enclosing_class: test_self_method_resolves_within_enclosing_class().
  test_ambiguous_method_stays_unknown: test_ambiguous_method_stays_unknown().
  test_self_method_not_hijacked: test_self_method_not_hijacked().
  test_bare_name_unaffected: test_bare_name_unaffected().
  test_bare_name_without_self_full_unaffected: test_bare_name_without_self_full_unaffected().
  test_self_method_no_cross_class_match: test_self_method_no_cross_class_match().
  test_class_method_unknown_class_with_ambiguous_method: test_class_method_unknown_class_with_ambiguous_method().
  test_class_method_duplicate_class_stays_unknown: test_class_method_duplicate_class_stays_unknown().
---
# Module: [`tests/unit/synapse_resolver/test_unique_method.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_unique_method.py)

## Functions
- `_ctx(**kw)` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_unique_method.py#L15)
- `test_ambiguous_method_stays_unknown()` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_unique_method.py#L36)
- `test_bare_name_unaffected()` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_unique_method.py#L55)
- `test_bare_name_without_self_full_unaffected()` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_unique_method.py#L76)
- `test_class_method_disambiguates_non_unique()` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_unique_method.py#L115) — execute defined on A and B; ClassName.execute (receiver type inferred)
- `test_class_method_duplicate_class_stays_unknown()` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_unique_method.py#L147) — P2 (Codex): Client defined in two modules → ambiguous, don't guess a file.
- `test_class_method_unknown_class_with_ambiguous_method()` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_unique_method.py#L134)
- `test_self_method_no_cross_class_match()` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_unique_method.py#L95) — P2#2: A.f calls self.helper(); only B defines helper → must NOT resolve to B.
- `test_self_method_not_hijacked()` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_unique_method.py#L48)
- `test_self_method_resolves_within_enclosing_class()` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_unique_method.py#L104) — P2#2: A.f calls self.g(); A defines g → resolve to A.g (not B's anything).
- `test_self_method_via_callee_full_resolves_local()` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_unique_method.py#L64) — self._x() arrives as callee_name='_x' + callee_full='self._x' — the bare
- `test_unique_method_receiver_resolves_to_project()` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_unique_method.py#L25)
- `test_unique_method_via_production_callee_full()` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_unique_method.py#L84) — P2#1: production rows are callee_name='all_edges' + callee_full='pg.all_edges'.

